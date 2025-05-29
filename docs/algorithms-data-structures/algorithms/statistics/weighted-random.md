---
sidebar_position: 1
title: Взвешенная произвольная выборка
description: Взвешенная произвольная выборка
keywords: ['javascript', 'js', 'algorithms', 'алгоритмы']
tags: ['javascript', 'js', 'algorithms', 'алгоритмы']
---

# Взвешенная произвольная выборка

<img src="https://habrastorage.org/webt/e9/94/i2/e994i2o7uknxvrwxlxocf8amr9k.png" />
<br />

__Описание__

- [Что такое взвешенная случайная выборка?](https://ru.statisticseasily.com/glossario/what-is-weighted-random-sampling/)
- [GitHub](https://github.com/harryheman/algorithms-data-structures/blob/main/src/algorithms/statistics/weighted-random.js)

Допустим, у нас есть список элементов. Элемент может быть чем угодно. Например, у нас может быть список фруктов и овощей, которые мы любим кушать: `[ '🍌', '🍎', '🥕' ]`.

Список весов представляет вес (вероятность выбора, важность) каждого элемента. Веса - это числа. Например, веса `[3, 7, 1]` означают следующее:

- мы выбираем яблоко чаще всего (`7` из `3+7+1=11` раз)
- банан мы выбираем менее часто (`3` из `11` раз)
- морковку мы не любим, поэтому выбираем ее редко (`1` из `11` раз)

> Если говорить в терминах вероятности, то веса должны быть представлены числами с плавающей запятой, сумма которых дает `1` (например, `[0.1, 0.5, 0.2, 0.2]`).

Взвешенная произвольная выборка (weighted random) - это функция, которая возвращает произвольный элемент списка с учетом его веса, поэтому элементы с большим весом выбирается чаще.

Пример интерфейса функции:

```javascript
const items =   [ '🍌', '🍎', '🥕' ];
const weights = [  3,    7,    1  ];

function weightedRandom(items, weights) {
  // Реализация...
}

const nextSnackToEat = weightedRandom(items, weights); // вероятнее всего будет '🍎'
```

__Применение__

- в [генетической алгоритме](https://ru.wikipedia.org/wiki/%D0%93%D0%B5%D0%BD%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B0%D0%BB%D0%B3%D0%BE%D1%80%D0%B8%D1%82%D0%BC) взвешенная произвольная выборка используется на стадии выборки, когда нам нужно выбрать наиболее приспособленных/сильных особей на основе оценки их приспособленности для спаривания и создания следующего более сильного поколения. См. [Самопаркующийся авто за 500 строк кода](https://habr.com/ru/users/aio350/articles/page2/)
- в [рекуррентных нейронных сетях (RNN)](https://ru.wikipedia.org/wiki/%D0%A0%D0%B5%D0%BA%D1%83%D1%80%D1%80%D0%B5%D0%BD%D1%82%D0%BD%D0%B0%D1%8F_%D0%BD%D0%B5%D0%B9%D1%80%D0%BE%D0%BD%D0%BD%D0%B0%D1%8F_%D1%81%D0%B5%D1%82%D1%8C) при принятии решения о выборе следующей буквы (для формирования предложения) на основе вероятности следующей буквы. См. Jupyter Notebook [Recipe Generation using Recurrent Neural Network (RNN)](https://nbviewer.org/github/trekhleb/machine-learning-experiments/blob/master/experiments/recipe_generation_rnn/recipe_generation_rnn.ipynb)
- в [балансировщике нагрузки Nginx](https://docs.nginx.com/nginx/admin-guide/load-balancer/http-load-balancer/) для более частой отправки запросов на сервер с более высоким весом
- во многих других областях

__Алгоритм__

Самый простой подход состоит в следующем:

1. Дублируем каждый элемент в соответствии с его весом.
2. Выбираем произвольный элемент.

Например, для наших фруктов и овощей можно сгенерировать следующий список:

```javascript
const items =   [ '🍌', '🍎', '🥕' ];
const weights = [  3,    7,    1  ];

// Дублируем элементы на основе их весов
const weightedItems = [
  '🍌', '🍌', '🍌',
  '🍎', '🍎', '🍎', '🍎', '🍎', '🍎', '🍎',
  '🥕',
];

// Теперь просто извлекаем произвольный элемент из `weightedItems`
```

Однако, как вы можете видеть, такой подход требует большого количества памяти в случае, когда у нас много элементов для повторения. Например, повторение строки `"some-random-string"` 10 млн раз потребует выделения около `180 Мб` памяти только для массива `weightedItems`.

Более эффективный подход состоит в следующем:

1. Готовим список совокупных весов для каждого элемента (список `cumulativeWeights` будет иметь такую же длину, как исходный список `weights`). В нашем случае он будет выглядеть так: `cumulativeWeights = [3, 3 + 7, 3 + 7 + 1] = [3, 10, 11]`.
2. Выбираем произвольное число в диапазоне от `0` до наибольшего совокупного веса. В нашем случае таким диапазоном будет `[0...11]`. Допустим, мы получили `randomNumber = 8`.
3. Перебираем `cumulativeWeights` слева направо и берем первый элемент, который больше или равен `randomNumber`. Индекс такого элемента используется для выбора элемента из списка `items`.

Основная идея данного подхода состоит в том, что более высокие веса будут "занимать" больше числового пространства. Таким образом, более высока вероятность выбора произвольного числа из "числовой группы более высокого веса".

```javascript
const weights =           [3, 7,  1 ];
const cumulativeWeights = [3, 10, 11];

// `cumulativeWeights` можно представить так
const pseudoCumulativeWeights = [
  1, 2, 3,               // <-- 3 числа
  4, 5, 6, 7, 8, 9, 10,  // <-- 7 чисел
  11,                    // <-- 1 число
];
```

__Реализация__

```javascript
// algorithms/statistics/weighted-random.js
/**
 * Возвращает произвольный элемент на основе его веса.
 * Элементы с более высоким весом выбираются чаще (с большей вероятностью).
 *
 * Например:
 * - items = ['banana', 'orange', 'apple']
 * - weights = [0, 0.2, 0.8]
 * - weightedRandom(items, weights) в 80% случаев будет возвращать 'apple',
 * в 20% случаев - 'orange' и никогда - 'banana' (поскольку вероятность его выбора равна 0%)
 *
 * @param {any[]} items
 * @param {number[]} weights
 * @returns {{item: any, index: number}}
 */
export default function weightedRandom(items, weights) {
  if (!items.length || !weights.length) {
    throw new Error('Элементы/веса не должны быть пустыми')
  }
  if (items.length !== weights.length) {
    throw new Error('Массивы элементов и весов должны иметь одинаковую длину')
  }

  // Готовим массив совокупных весов.
  // Например:
  // - weights = [1, 4, 3]
  // - cumulativeWeights = [1, 5, 8]
  const cumulativeWeights = []
  for (let i = 0; i < weights.length; i++) {
    cumulativeWeights[i] = weights[i] + (cumulativeWeights[i - 1] || 0)
  }

  // Получаем произвольное число в диапазоне [0...sum(weights)].
  // Например:
  // - weights = [1, 4, 3]
  // - maxCumulativeWeight = 8
  // - диапазон произвольного числа - [0...8]
  const maxCumulativeWeight = cumulativeWeights.at(-1)
  const random = Math.random() * maxCumulativeWeight

  // Извлекаем произвольный элемент на основе его веса.
  // Элементы с более высоким весом выбираются чаще
  const index = cumulativeWeights.findIndex((cumulativeWeight) => {
    return cumulativeWeight >= random
  })
  const item = items[index]

  return {
    item,
    index,
  }
}
```

<spoiler title="Тесты:">

```javascript
import weightedRandom from '../weighted-random'

describe('weightedRandom', () => {
  it('при передаче пустого массива элементов или весов должно выбрасываться исключение', () => {
    const getWeightedRandomWithInvalidInputs = () => {
      weightedRandom([], [])
    }
    expect(getWeightedRandomWithInvalidInputs).toThrow(
      'Элементы/веса не должны быть пустыми',
    )
  })

  it('при несовпадении количества элементов и весов должно выбрасываться исключение', () => {
    const getWeightedRandomWithInvalidInputs = () => {
      weightedRandom(['a', 'b', 'c'], [10, 0])
    }
    expect(getWeightedRandomWithInvalidInputs).toThrow(
      'Массивы элементов и весов должны иметь одинаковую длину',
    )
  })

  it('должен правильно выполнять взвешенную произвольную выборку в простых случаях', () => {
    expect(weightedRandom(['a', 'b', 'c'], [1, 0, 0])).toEqual({
      index: 0,
      item: 'a',
    })
    expect(weightedRandom(['a', 'b', 'c'], [0, 1, 0])).toEqual({
      index: 1,
      item: 'b',
    })
    expect(weightedRandom(['a', 'b', 'c'], [0, 0, 1])).toEqual({
      index: 2,
      item: 'c',
    })
    expect(weightedRandom(['a', 'b', 'c'], [0, 1, 1])).not.toEqual({
      index: 0,
      item: 'a',
    })
    expect(weightedRandom(['a', 'b', 'c'], [1, 0, 1])).not.toEqual({
      index: 1,
      item: 'b',
    })
    expect(weightedRandom(['a', 'b', 'c'], [1, 1, 0])).not.toEqual({
      index: 2,
      item: 'c',
    })
  })

  it('должен правильно выполнять взвешенную произвольную выборку', () => {
    // Количество выборок
    const ATTEMPTS_NUM = 1000
    // Погрешность количества выборок элемента.
    // Например, если мы хотим, чтобы элемент 'a' выбирался 300 раз из 1000 (30%),
    // тогда 267 раз является приемлемым, поскольку это больше 250 (300 - 50)
    // и меньше 350 (300 + 50)
    const THRESHOLD = 50

    const items = ['a', 'b', 'c'] // значения элементов неважны
    const weights = [0.1, 0.3, 0.6]

    const counter = []
    for (let i = 0; i < ATTEMPTS_NUM; i += 1) {
      const randomItem = weightedRandom(items, weights)
      if (!counter[randomItem.index]) {
        counter[randomItem.index] = 1
      } else {
        counter[randomItem.index] += 1
      }
    }

    for (let itemIndex = 0; itemIndex < items.length; itemIndex += 1) {
      /*
        Элемент под индексом 0 должен выбираться 100 раз (в идеале)
        или, учитывая порог, [100 - 50, 100 + 50] раз.

        Элемент под индексом 1 должен выбираться 300 раз (в идеале)
        или, учитывая порог, [300 - 50, 300 + 50] раз.

        Элемент под индексом 2 должен выбираться 600 раз (в идеале)
        или, учитывая порог, [600 - 50, 600 + 50] раз
       */
      expect(counter[itemIndex]).toBeGreaterThan(
        ATTEMPTS_NUM * weights[itemIndex] - THRESHOLD,
      )
      expect(counter[itemIndex]).toBeLessThan(
        ATTEMPTS_NUM * weights[itemIndex] + THRESHOLD,
      )
    }
  })
})
```

</spoiler>

Запускаем тесты:

```bash
npm run test ./algorithms/statistics
```

<img src="https://habrastorage.org/webt/b4/vf/m-/b4vfm-aglfggwqjagfsl9g-uqsq.png" />
<br />
