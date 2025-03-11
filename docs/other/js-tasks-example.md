<a name="top"></a>

[На главную](../README.md)

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
|   | Общие вопросы |
|1 | [Tasks Minin](#1) |
|2 | [Задачи с собеседований на понимание основ](#2) |
|3 | [Codewars tasks 1](#3) |
|4 | [](#4) |
|5 | [](#5) |
|6 | [](#6) |
|7 | [](#7) |
|8 | [](#8) |
|9 | [](#9) |
|10 | [](#10) |
|11 | [](#11) |
|12 | [](#12) |
|13 | [](#13) |
|14 | [](#14) |
|15 | [](#15) |
|16 | [](#16) |
|17 | [](#17) |



<a name="questions"></a>

## Задачи по Javascript

  **[⬆ Наверх](#top)**
  

1. ### <a name="1"></a> Tasks Minin
	
- [Уникальность всех символов в строке()](#unique)
- [Плоский массив()](#flatten)
- [Удаление всех повторяющихся значений в строке()](#dupes)
- [Какая строка встречается чаще всего()](#frequency)
- [Повернута ли строка()](#rotate)
- [Является ли массив подмножеством другого массива()](#subset)
- [Анаграммы()](#anagrams)
- [Перевернуть матрицу 3х3()](#matrix)
- [Алгоритмы: Простой поиск()](#search)
- [Алгоритмы: Сбалансированные скобки()](#balanced)
- [Алгоритмы: Очередь с О(1) сложностью операций()](#queue)
- [Deep Equal()](#equal)
- [Последовательность Фибоначчи()](#fib)
- [Своя функция bind()](#bind)
- [Универсальная сумма()](#sum)
- [GroupBy()](#group)	

## Строки и массивы

### Уникальность всех символов в строке <a name="unique"></a>

Напишите функцию, которая определяет уникальны ли все символы в строке. Регистр должен учитываться: `‘a’` и `‘A’` разные символы.

**Input**: String

**Output**: Boolean
	
```js
function isUnique(str) {
  
  // Решение 1 =>

  for (let i = 0; i < str.length; i++) {
    if (str.lastIndexOf(str[i]) !== i) {
      return false;
    }
  }
  return true;

  // Решение 2 =>

  const chars = new Set()

  for (let i = 0; i < str.length; i++) {
    const current = str[i]

    if (chars.has(current)) {
      return false
    }

    chars.add(current)
  }
  return true


  // Решение 3 =>

  return new Set(str).size === str.length;
}

console.log(isUnique('abcdef'));
console.log(isUnique('1234567'));
console.log(isUnique('abcABC'));
console.log(isUnique('abcadef'));
```	
**[⬆ Наверх](#41)**
	
	
### Плоский массив <a name="flatten"></a>

Напишите функцию, принимающая массив с вложенными массивами и распакуйте в результирующий плоский массов. В результате должны получить новый одномерный массив.

**Input**: Array

**Output**: Array
	
```js
// Рекурсия =>

function flatten(array) {
  const res = []

  for (let i = 0; i < array.length; i++) {
    if (Array.isArray(array[i])) {
      const flat = flatten(array[i])
      
      for (let j = 0; j < flat.length; j++) {
        res.push(flat[j])
      }
    } else {
      res.push(array[i])
    }
  }

  return res
}

console.log(flatten([[1], [[2, 3]], [[[4]]]])) // -> [1, 2, 3, 4]	
```	
**[⬆ Наверх](#41)**
	
	
### Удаление всех повторяющихся значений в строке <a name="dupes"></a>

Напишите функцию, которая принимает строку и возвращает новую, в которой все дублирующиеся символы будут удалены.

**Input**: String

**Output**: String
	
```js
function removeDupes(str) {

  // Решение 1 =>

  const chars = {}
  const res = []

  for (let i = 0; i < str.length; i++) {
    if (!chars[str[i]]) {
      chars[str[i]] = true
      res.push(str[i])
    }
  }

  return res.join('')

  // Решение 1 =>

  return Array.from(new Set(str)).join('')
}	
	
console.log(removeDupes('abcd')) // -> 'abcd'
console.log(removeDupes('aabbccdd')) // -> 'abcd'
console.log(removeDupes('abcddbca')) // -> 'abcd'
console.log(removeDupes('abababcdcdcd')) // -> 'abcd'	
```	
**[⬆ Наверх](#41)**
	
	
### Какая строка встречается чаще всего <a name="frequenc"></a>

Напишите функцию, которая принимает массив строк и возвращает самую частовстречающуюся строку в этом массиве. Если таких строк несколько, то нужно вернуть первую, идя слева на право.

**Input**: String[]

**Output**: String
	
```js
function highestFrequency(array) {
  const map = {}
  let maxFreq = 0
  let maxFreqStr = array[0]

  for (let i = 0; i < array.length; i++) {
    const current = array[i]

    if (map[current]) {
      map[current]++
    } else {
      map[current] = 1
    }

    if (map[current] > maxFreq) {
      maxFreq = map[current]
      maxFreqStr = current
    }
  }

  return maxFreqStr
}
	
console.log(highestFrequency(['a', 'b', 'c', 'c', 'd', 'e'])) // -> c
console.log(highestFrequency(['abc', 'def', 'abc', 'def', 'abc'])) // -> abc
console.log(highestFrequency(['abc', 'def'])) // -> abc
console.log(highestFrequency(['abc', 'abc', 'def', 'def', 'def', 'ghi', 'ghi', 'ghi', 'ghi' ])) // -> ghi	
```	
**[⬆ Наверх](#41)**
	
	
### Повернута ли строка? <a name="rotate"></a>

Напишите функцию, которая принимает 2 строки. Верните `true` если строки являются перевернутым вариантом друг друга (см. пример). Иначе верните `false`.

**Input**: String, String

**Output**: Boolean
	
```js
function isStringRotated(source, test) {

  // Решение 1 =>

  if (source.length !== test.length) {
    return false
  }
  
  for (let i = 0; i < source.length; i++) {
    const rotate = source.slice(i, source.length) + source.slice(0, i)
  
    if (rotate === test) {
      return true
    }
  }
  
  return false

  // Решение 2 =>

  return source.length === test.length && (source + source).includes(test)
}

console.log(isStringRotated('javascript', 'scriptjava')) // -> true
console.log(isStringRotated('javascript', 'iptjavascr')) // -> true
console.log(isStringRotated('javascript', 'java')) // -> false	
```	
**[⬆ Наверх](#41)**
	
	
### Является ли массив подмножеством другого массива <a name="subset"></a>

Напишите функцию, которая проверяет, является ли второй массив подмножеством первого. То есть есть ли элементы второго массива в первом.

**Input**: Number[] & String[], Number[] & String[]

**Output**: Boolean
	
```js
function arraySubset(source, subset) {
  if (source.length < subset.length) {
    return false
  }

  for (let i = 0; i < subset.length; i++) {
    const index = source.indexOf(subset[i])

    if (index === -1) {
      return false
    }

    delete source[index]
  }
  
  return true
}

console.log(arraySubset([2, 1, 3], [1, 2, 3])) // -> true
console.log(arraySubset([2, 1, 1, 3], [1, 2, 3])) // -> true
console.log(arraySubset([1, 1, 1, 3], [1, 3, 3])) // -> false
console.log(arraySubset([1, 2], [1, 2, 3])) // -> false	
```	
**[⬆ Наверх](#41)**
	
	
### Анаграммы <a name="anagrams"></a>

Напишите функцию, которая проверяет, являются ли все элементы в массиве анаграммами друг друга.

**Input**: String[]

**Output**: Boolean
	
```js
function allAnagrams(array) {
  const sorted = array.map(str => str.split('').sort().join(''))

  for (let i = 1; i < sorted.length; i++) {
    if (sorted[i] !== sorted[0]) {
      return false
    }
  }
  return true
}

console.log(allAnagrams(['abcd', 'bdac', 'cabd'])) // true
console.log(allAnagrams(['abcd', 'bdXc', 'cabd'])) // false	
```	
**[⬆ Наверх](#41)**
				    
				    
### Перевернуть матрицу 3х3 <a name="matrix"></a>

Напишите функцию, которая принимает матрицу 3х3 и переворачивает на 90 градусов по часовой стрелке.

**Дополнительно**: Напишите еще 2 функции, которые переворачивают матрицу на 180 и 270 градусов.

```
[1, 2, 3]    [7, 4, 1]
[4, 5, 6] -> [8, 5, 2]  
[7, 8, 9]    [9, 6, 3]   
```

**Input**: Number[][]

**Output**: Number[][]
	
```js
const matrix = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9]
]

function rotate(source) {
  const newMatrix = source[0].map(() => [])

  for (let i = 0; i < source.length; i++) {
    for (let j = 0; j < source[0].length; j++) {
      newMatrix[j][source.length - 1 - i] = source[i][j]
    }
  }

  return newMatrix
}

function rotate180(source) {
  return rotate(rotate(source))
}

function rotate270(source) {
  return rotate180(rotate(source))
}

function rotate360(source) {
  return rotate270(rotate(source))
}

console.log(rotate(matrix))
console.log(rotate180(matrix))
console.log(rotate270(matrix))
console.log(rotate360(matrix))	
```	
**[⬆ Наверх](#41)**
	
	
## Алгоритмы

### Простой поиск <a name="search"></a>

Напишите функцию, которая принимает отсортированный массив с числами и число. Необходимо вернуть индекс числа, если оно есть в массиве. Иначе вернуть `-1`.

**Input**: Number[], Number

**Output**: Number
	
```js
// Решение 1 =>

// Time: O(n)
function search(array, target) {
  for (let i = 0; i < array.length; i++) {
    if (array[i] === target) {
      return i
    }
  }
  return -1
}

// Решение 2 =>

// Time: O(log(n))
function binary(array, target) {
  let start = 0
  let end = array.length - 1

  if (target < array[start] || target > array[end]) {
    return -1
  }

  while (true) {
    if (target === array[start]) {
      return start
    }

    if (target === array[end]) {
      return end
    }

    if (end - start <= 1) {
      return -1
    }

    const middle = Math.floor((start + end) / 2)

    if (target > array[middle]) {
      start = middle + 1
    } else if (target < array[middle]) {
      end = middle - 1
    } else {
      return middle
    }
  }
}

console.log(search([1, 3, 6, 13, 17], 13)) // -> 3
console.log(search([1, 3, 6, 13, 17], 12)) // -> -1	
```	
**[⬆ Наверх](#41)**
	
	
### Сбалансированные скобки <a name="balanced"></a>

Напишите функцию, которая проверит строку на сбалансированность скобок: `{}, (), []`. Вернуть `true` если они сбалансированы, иначе `false`.

**Input**: String

**Output**: Boolean
	
```js
function isBalanced(string) {
  const start = '({['
  const end = ']})'

  const map = {
    '}': '{',
    ')': '(',
    ']': '['
  }

  const queue = []

  for (let i = 0; i < string.length; i++) {
    const char = string[i]

    if (start.includes(char)) {
      queue.push(char)
    } else if (end.includes(char)) {
      const last = queue.pop()

      if (map[char] !== last) {
        return false
      }
    }
  }

  return !queue.length
}

console.log(isBalanced('(x + y) - (4)')) // -> true
console.log(isBalanced('(((10 ) ()) ((?)(:)))')) // -> true
console.log(isBalanced('[{()}]')) // -> true
console.log(isBalanced('(50)(')) // -> false
console.log(isBalanced('[{]}')) // -> false	
```	
**[⬆ Наверх](#41)**
	
	
### Очередь с О(1) сложностью операций <a name="queue"></a>

Создайте очередь, в которой буду реализованы операции на добавление элементов в конец очереди, удаление первого элемента и вычисление размера очереди с сложностью алгоритма `О(1)` .

```js	
class Queue {
    constructor() {
        // todo
    }
    
    enqueue(item) {
        // todo: добавить элемент в конец очереди
    }
  
    dequeue() {
        // todo: удалить первый элемент из очереди
    }
  
    get size() {
        // todo: возвращает размер списка
				// нельзя использовать геттер
    }
}	
```

// Решение 1 =>
	
### Решение - LinkedList	
```js
class LinkedList {
  #length = 0

  constructor() {
    this.head = null
    this.tail = null
  }

  addToTail(value) {
    const node = {
      value,
      next: null
    }

    if (this.#length === 0) {
      this.head = node
      this.tail = node
    } else {
      this.tail = node
    }

    this.#length++
  }

  removeFromHead() {
    if (this.#length === 0) {
      return
    }

    const value = this.head.value

    this.head = this.head.next
    this.#length--

    return value
  }

  size() {
    return this.#length
  }
}

class Queue extends LinkedList {
  constructor() {
    super()

    this.enqueue = this.addToTail
    this.dequeue = this.removeFromHead
  }

  get size() {
    return super.size()
  }
}
	
const queue = new Queue()
	
queue.enqueue(1)
queue.enqueue(2)	
queue.enqueue(3)
	
queue.dequeue()	
	
console.log(queue.size)		
```	

// Решение 2 =>

### Решение - HashTable	
```js	
class Queue {
  #storage = {}
  #last = 0
  #first = 0

  enqueue(item) {
    this.#storage[this.#last] = item
    this.#last++
  }

  dequeue() {
    if (this.size === 0) {
      return
    }

    const value = this.#storage[this.#first]
    delete this.#storage[this.#first]
    this.#first++
    return value
  }

  get size() {
    return this.#last = this.#first
  }
}
	
const table = new Queue()
	
table.enqueue(1)
table.enqueue(2)	
table.enqueue(3)
	
table.dequeue()	
	
console.log(table.size)	
```	
**[⬆ Наверх](#41)**
	
	
## JavaScript

### Deep Equal <a name="equal"></a>

Напишите функцию, которая будет проверять на “глубокое” равенство 2 входящих параметра

**Inputs**: Any, Any

**Output**: Boolean
	
```js
function deepEqual(a, b) {
  if (Number.isNaN(a) && Number.isNaN(b)) {
    return true
  }

  if (typeof a !== typeof b) {
    return false
  }

  if (typeof a !== 'object' || a === null || b === null) {
    return a === b
  }

  if (Object.keys(a).length !== Object.keys(b).length) {
    return false
  }

  for (const key of Object.keys(a)) {
    if (!deepEqual(a[key], b[key])) {
      return false
    }
  }

  return true
}
	
const source = {a: 1, b: {c: 1}}
const test1 = {a: 1, b: {c: 1}}
const test2 = {a: 1, b: {c: 2}}
console.log(deepEqual(source, test1)) // -> true
console.log(deepEqual(source, test2)) // -> false
console.log(deepEqual(NaN, NaN)) // -> true
console.log(deepEqual('test', 'test!')) // -> false
console.log(deepEqual()) // -> true	
```	
**[⬆ Наверх](#41)**
	
	
### Последовательность Фибоначчи <a name="fib"></a>

Напишите функцию, которая будет генерировать последовательность Фиббоначи длинны `n`, которую передали как аргумент.

**Input**: Number

**Output**: Number[]
	
```js
function fibonacci(n) {
  const sequence = [1, 1]

  if (n < 2) {
    return sequence.slice(0, n)
  }

  while (sequence.length < n) {
    const last = sequence[sequence.length - 1]
    const prev = sequence[sequence.length - 2]
    sequence.push(last + prev)
  }

  return sequence
}
	
console.log(fibonacci(8)) // -> [1, 1, 2, 3, 5, 8, 13, 21]	
```	

### fibinacci с рекурсией
```js
const fibinacci = (function () {
  const seq = [1, 1];

  return function (n) {
    console.log('Called with ', n);

    if (seq.length >= n) {
      console.log('No compute');
      return seq.slice(0, n);
    }

    while (seq.length < n) {
      const last = seq[seq.length - 1];
      const prev = seq[seq.length - 2];
      seq.push(last + prev);
      console.log('Pushed: ', seq[seq.length - 1]);
    }

    return seq;
  };
})();

console.log(fibinacci(10)) // -> [1, 1, 2, 3, 5, 8, 13, 21]
console.log(fibinacci(8)) // -> [1, 1, 2, 3, 5, 8, 13, 21]
console.log(fibinacci(12)) // -> [1, 1, 2, 3, 5, 8, 13, 21]
console.log(fibinacci(11)) // -> [1, 1, 2, 3, 5, 8, 13, 21]
```	
**[⬆ Наверх](#41)**
	
	
### Своя функция bind <a name="bind"></a>

Реализуйте функцию `bind`.

**Input**: Object, arguments

**Output**: Function

```js
Function.prototype.myBind = function(context, ...args) {
  return (...rest) => {
    return this.call(context, ...args.concat(rest))
  }
}

function log(...props) {
  console.log(this.name, this.age, ...props)
}

const obj = {name: 'Vladilen', age: 28}

log.myBind(obj, 1, 2)()	// -> Vladilen, 28, 1, 2
```	
**[⬆ Наверх](#41)**
	
	
### Универсальная сумма <a name="sum"></a>

Напишите функцию, которая складывает 2 числа. Работать функция должна как показано в примере ниже:

**Input**: Number, Number

**Output**: Number
	
```js
function add(a, b) {
  if (!a) {
    return add
  }
  if (!b) {
    return function calc(c) {
      if (!c) return calc
      return a + c
    }
  }

  return a + b
}
	
add(20, 22) // -> 42
add(20)(22) // -> 42
add(20)()(22) // -> 42
add(20)()()()(22) // -> 42
add(20)()()()()()()()()()()()(22) // -> 42
add()(20)(22) // -> 42
add()()()()(20)(22) // -> 42
add()(20)()(22) // -> 42
add()()()()()(20)()()()(22) // -> 42	
```	
**[⬆ Наверх](#41)**
	
	
### GroupBy <a name="group"></a>

Напишите функцию `groupBy`.

**Input**: Number[] & String[], Function & String

**Output**: Object
	
```js
function groupBy(array, fn) {
  return array.reduce((res, current) => {
    const key = typeof fn === 'function' ? fn(current) : current[fn]

    if (!res[key]) {
      res[key] = []
    }
    res[key].push(current)

    return res
  }, {})
}
	
groupBy([6.1, 4.2, 6.3], Math.floor) // -> { '4': [4.2], '6': [6.1, 6.3] }
groupBy(['one', 'two', 'three'], 'length') // -> { '3': ['one', 'two'], '5': ['three'] }	
```			
**[⬆ Наверх](#41)**
	
  **[⬆ Наверх](#top)**
	
2. ### <a name="2"></a> Задачи с собеседований на понимание основ

```js
// 1) Какое будет выведено значение: let x = 5; alert( x++ ); ?

let x = 5; 
alert( x++ ); 
// 5, постфиксная форма сначало ставит такой же результат, но в следующем выводе даст +1.
alert( ++x ); /* префиксная, увеличит сразу, будет 6 */

// 2) Чему равно такое выражение: [ ] + false - null + true ?

// [ ] + false - null + true

console.log([] + false - null + true); // 'NaN'
// [] + false = string

// 3) Что выведет этот код: let y = 1; let x = y = 2; alert(x); ?

let y = 1; 
let x = y = 2; 
alert(x); //2
alert(y); //2
// число это примитивный тип данных, он передаеться по значению, с права на лево

// 4) Чему равна сумма [] + 1 + 2?

// [] + 1 + 2

//[] по факту первращается в пустую сроку

console.log([] + 1 + 2); // '12' - string

// 5) Что выведет этот код: alert( "1"[0] )?

alert( "1"[0] ); //1

// 6) Чему равно 2 && 1 && null && 0 && undefined ?

// 2 && 1 && null && 0 && undefined

console.log(2 && 1 && null && 0 && undefined); // null

// && (И) - запинаеться на лжи!
// || (ИЛИ) - запинаеться на правде!

// 7) Есть ли разница между выражениями? !!( a && b ) и (a && b)?

console.log(!!( 1 && 2 ) === (1 && 2)); // false
// (!! - два восклицательных знака (знак НЕ) превращают следующее за ним выражение в Булиновое значение)

// 8)
// Что выведет этот код: alert( null || 2 && 3 || 4 ); ?

//         (2)3     (1)3    (3)3
// alert( null || 2 && 3 || 4 ); //3

// && - приоритет 6, (И) - запинаеться на лжи! когда у нас оба аргумента при логическом сравнении равны, 
//то оператор будет возвращать последнее значени, в нашем случае: 2 && 3 = 3;

// || - приоритет 5, (ИЛИ) запинается на первой правде, в нашем случа 3 || 4 = 3;


// 9) 
// a = [1, 2, 3]; b = [1, 2, 3]; Правда ли что a == b ?

const a = [1, 2, 3];
const b = [1, 2, 3];
console.log(a == b); //false


// 10)
// Что выведет этот код: alert( +"Infinity" ); ?

alert( +"Infinity" ); // Infinity; это будет number


// 11)
//Верно ли сравнение: "Ёжик" > "яблоко"?

// console.log("Ёжик" > "яблоко"); //false
// идет посимвольное сравнение, если первые знаки равны то сравнивается вторые знаки и тд.
// Таблица Unicode для русских букв

// 12)
//Чему равно 0 || "" || 2 || undefined || true || falsе ?

console.log(0 || "" || 2 || undefined || true || falsе); // 2

// && (И) - запинаеться на лжи!
// || (ИЛИ) - запинаеться на правде!	
	
// 13)
/* Сделайте так, чтобы этот код работал:
duplicate([1, 2, 3, 4, 5]); -> [1,2,3,4,5,1,2,3,4,5] */
		
function duplicate(arr) {
  return arr.concat(arr);
}

duplicate([1, 2, 3, 4, 5]); // [1,2,3,4,5,1,2,3,4,5]	
```



  **[⬆ Наверх](#top)**
	
3. ### <a name="3"></a> Codewars tasks 1

### 8 kyu
	
```js
// Завершите функцию квадратной суммы, чтобы она возводила в квадрат каждое переданное ей число, а затем суммировала результаты.

// Например, for [1, 2, 2]это должно возвращаться , 9потому что 1^2 + 2^2 + 2^2 = 9.

function squareSum(numbers) {
  let sum = 0;

  for (let i = 0; i < numbers.length; i++) {
    sum += numbers[i] ** 2;
  }

  return sum;
}

//

function squareSum(numbers) {
  return numbers.reduce((sum, n) => {
    return n * n + sum;
  }, 0);
}


// Find the smallest integer in the array

class SmallestIntegerFinder {
  findSmallestInt(args) {
    const min = Math.min(...args);
    return min;
  }
}

//

class SmallestIntegerFinder {
  findSmallestInt(args) {
    return Math.min(...args);
  }
}


// Return Negative

function makeNegative(num) {
  return num < 0 ? num : -num;
}

//

function makeNegative(num) {
  return -Math.abs(num);
}


// Fake Binary

function fakeBin(x) {
  return x
    .split('')
    .map((n) => (n < 5 ? 0 : 1))
    .join('');
}


// Capitalization and Mutability

function capitalizeWord(word) {
  return word[0].toUpperCase() + word.slice(1);
}

//

const capitalizeWord = (word) =>
  word.replace(word.charAt(0), word.charAt(0).toUpperCase());


// Wilson primes

function amIWilson(p) {
  if (p === 5 || p === 13 || p === 563) {
    return true;
  }
  return false;
}

//

function amIWilson(p) {
  return p === 5 || p === 13 || p === 563;
}


// Convert number to reversed array of digits

function digitize(n) {
  return String(n).split('').map(Number).reverse();
}

//

function digitize(n) {
  return n.toString().split('').reverse().map(Number);
}


// Task

setTimeout(function timeout() {
  console.log(' 1');
}, 0);

let createPromise = new Promise(function (resolve, reject) {
  console.log('2');
  resolve();
});

createPromise.then(function () {
  console.log(3);
});

console.log(4);

// 2431


// Quarter of the year

const quarterOf = (month) => {
  if (month <= 3) {
    return 1;
  } else if (month <= 6) {
    return 2;
  } else if (month <= 9) {
    return 3;
  } else {
    return 4;
  }
};

//

const quarterOf1 = (m) => Math.ceil(m / 3);


// If you can't sleep, just count sheep!!

var countSheep = function (num) {
  let sheep = '';

  for (i = 1; i <= num; i++) {
    sheep += i + ' sheep...';
  }

  return sheep;
};


// Beginner - Reduce but Grow

function grow(x) {
  return x.reduce((acc, current) => acc * current);
}


// Remove String Spaces

function noSpace(x) {
  return x.replace(/\s/g, '');
}

//

function noSpace(x) {
  return x.split(' ').join('');
}


// Beginner - Lost Without a Map

function maps(x) {
  return x.map((n) => n * 2);
}


// Well of Ideas - Easy Version

function well(x) {
  const good = x.filter((idea) => idea === 'good').length;

  return good === 0 ? 'Fail!' : good > 2 ? 'I smell a series!' : 'Publish!';
}


// Convert boolean values to strings 'Yes' or 'No'.

function boolToWord(bool) {
  return bool ? 'Yes' : 'No';
}

//

function boolToWord(bool) {
  if (bool === true) return 'Yes';
  if (bool === false) return 'No';
}


// Geometry Basics: Distance between points in 2D

function distanceBetweenPoints(a, b) {
  return Math.hypot(a.x - b.x, a.y - b.y);
}

//

return Math.sqrt(Math.abs(a.x - b.x) ** 2 + Math.abs(a.y - b.y) ** 2);


// Take the Derivative

function derive(coefficient, exponent) {
  return `${coefficient * exponent}x^${exponent - 1}`;
}

//

function derive(a, b) {
  return a * b + 'x^' + (b - 1);
}


// Count by X

function countBy(x, n) {
  let z = [];

  for (let i = 1; i <= n; i++) {
    z.push(x * i);
  }

  return z;
}


// Beginner Series #4 Cockroach

function cockroachSpeed(s) {
  return Math.floor(s * 27.7778);
}

//

const cockroachSpeed = (s) => Math.floor(s / 0.036);

//

function cockroachSpeed(s) {
  const secsInHour = 3600;
  const centimetersInKilometers = 100000;

  return Math.floor((s * centimetersInKilometers) / secsInHour);
}


// Find Nearest square number

function nearestSq(n) {
  return Math.pow(Math.round(Math.sqrt(n)), 2);
}


// Even or Odd

function even_or_odd(number) {
  if (number % 2 == 0) {
    return 'Even';
  } else {
    return 'Odd';
  }
}

//

function even_or_odd(number) {
  return number % 2 ? 'Odd' : 'Even';
}


// Do I get a bonus?

function bonusTime(salary, bonus) {
  if (bonus === true) return `£${salary * 10}`;
  if (bonus === false) return `£${salary}`;
}

//

function bonusTime(salary, bonus) {
  return bonus ? `£${10 * salary}` : `£${salary}`;
}


// Sum Mixed Array

function sumMix(x) {
  return x.reduce((acc, cur) => Number(acc) + Number(cur), 0);
}


// Jenny's secret message

function greet(name) {
  if (name === 'Johnny') return 'Hello, my love!';

  return 'Hello, ' + name + '!';
}


// Century From Year

function century(year) {
  return Math.floor(year / 100) + (year % 100 ? 1 : 0);
}

//

function century(year) {
  return Math.ceil(year / 100); //using ceiling method to round up to nearest century (100)
}


// Count of positives / sum of negatives

function countPositivesSumNegatives(input) {
  let positiveNums = 0;
  let negativeNums = 0;

  if (input === null || input.length === 0) {
    return [];
  } else {
    input.forEach((num) => (num > 0 ? positiveNums++ : (negativeNums += num)));
  }

  return [positiveNums, negativeNums];
}


// How much water do I need?

function howMuchWater(water, load, clothes) {
  return clothes < load
    ? 'Not enough clothes'
    : clothes > 2 * load
    ? 'Too much clothes'
    : +(water * 1.1 ** (clothes - load)).toFixed(2);
}

//

function howMuchWater(water, load, clothes) {
  if (clothes > 2 * load) return 'Too much clothes';
  if (clothes < load) return 'Not enough clothes';
  return +(water * 1.1 ** (clothes - load)).toFixed(2);
}


// Online RPG: player to qualifying stage?

function playerRankUp(points) {
  if (points >= 100) {
    return 'Well done! You have advanced to the qualifying stage. Win 2 out of your next 3 games to rank up.';
  } else {
    return false;
  }
}

//

function playerRankUp(points) {
  return points >= 100
    ? 'Well done! You have advanced to the qualifying stage. Win 2 out of your next 3 games to rank up.'
    : false;
}


// isReallyNaN

const isReallyNaN = (val) => Number.isNaN(val);

//

const isReallyNaN1 = Number.isNaN;


// Square(n) Sum

function squareSum(numbers) {
  return numbers.reduce(function (sum, n) {
    return n * n + sum;
  }, 0);
}

//

function squareSum(numbers) {
  return numbers.reduce((sum, n) => {
    return n * n + sum;
  }, 0);
}


// Sum of positive

function positiveSum(arr) {
  let res = 0;

  for (let i = 0; i < arr.length; i++) {
    if (arr[i] > 0) {
      res += arr[i];
    }
  }

  return res;
}


// How good are you really?

function betterThanAverage(classPoints, yourPoints) {
  const average = classPoints.reduce((x, y) => x + y, 0) / classPoints.length;

  return average > yourPoints ? false : true;
}

//

function betterThanAverage(classPoints, yourPoints) {
  return (
    yourPoints > classPoints.reduce((a, b) => a + b, 0) / classPoints.length
  );
}


// Convert a Number to a String!

function numberToString(num) {
  return num + '';
}

//

function numberToString(num) {
  return num.toString();
}


// Find Multiples of a Number

function findMultiples(integer, limit) {
  let multiples = [];

  for (let i = integer; i <= limit; i = i + integer) {
    multiples.push(i);
  }

  return multiples;
}


// Opposite number

function opposite(number) {
  return -number;
}


// Beginner Series #1 School Paperwork

function paperwork(n, m) {
  if (n < 0 || m < 0) return 0;
  return n * m;
}

//

function paperwork(n, m) {
  return n > 0 && m > 0 ? n * m : 0;
}


// FIXME: Replace all dots

let replaceDots = function (str) {
  return str.replace(/[.]/g, '-');
};

//

var replaceDots1 = function (str) {
  return str.replace(/\./g, '-');
};


// They say that only the name is long enough to attract attention. They also said that only a simple Kata will have someone to solve it. This is a sadly story #1: Are they opposite?

function isOpposite(s1, s2) {
  return !s1 || !s2
    ? false
    : s1 ===
        s2.replace(/[a-z]/gi, (c) =>
          c < 'a' ? c.toLowerCase() : c.toUpperCase()
        );
}

//

function isOpposite(s1, s2) {
  return (
    s1
      .split('')
      .map((c) => (c === c.toUpperCase() ? c.toLowerCase() : c.toUpperCase()))
      .join('') === s2 && s1 !== ''
  );
}


// N-th Power

function index(array, n) {
  if (array.length <= n || 0 > n) {
    return -1;
  } else {
    return Math.pow(array[n], n);
  }
}

//

const index = (array, n) => (array.length > n ? Math.pow(array[n], n) : -1);


// Convert a Boolean to a String

function booleanToString(b) {
  return b.toString();
}

//

function booleanToString(b) {
  return b ? 'true' : 'false';
}


// Find the position!

function position(letter) {
  return 'Position of alphabet: ' + (letter.charCodeAt(0) - 97 + 1);
}

//

function position(letter) {
  const alphabet = 'abcdefghijklmnopqrstuvwxyz';
  return 'Position of alphabet: ' + (alphabet.indexOf(letter) + 1);
}


// Sum without highest and lowest number

function sumArray(array) {
  if (array && array.length > 1) {
    const sortedArray = array.sort((a, b) => a - b).slice(1, -1);
    return sortedArray.reduce((acc, cur) => acc + cur, 0);
  }

  return 0;
}


// Is he gonna survive?

function hero(bullets, dragons) {
  return bullets >= 2 * dragons;
}

//

function hero(bullets, dragons) {
  return bullets >= dragons * 2;
}


// Hex to Decimal

function hexToDec(hexString) {
  return parseInt(hexString, 16);
}


// Is n divisible by x and y?

function isDivisible(n, x, y) {
  if (n % x == 0 && n % y == 0) {
    return true;
  } else {
    return false;
  }
}

//

function isDivisible(n, x, y) {
  return n % x === 0 && n % y === 0;
}


// Sum Arrays

function sum(numbers) {
  'use strict';

  return numbers.reduce((acc, cur) => acc + cur, 0);
}


// Will there be enough space?

function enough(cap, on, wait) {
  if (cap <= on + wait) {
    return on + wait - cap;
  } else {
    return 0;
  }
}

//

function enough(cap, on, wait) {
  return Math.max(wait + on - cap, 0);
}

//

function enough(cap, on, wait) {
  return on + wait > cap ? on + wait - cap : 0;
}


// Playing with cubes II

class Cube {
  constructor(side) {
    this.setSide(side);
  }

  getSide() {
    return this.side;
  }

  setSide(side = 0) {
    this.side = Math.abs(side);
  }
}


// Counting sheep...

function countSheeps(arrayOfSheep) {
  return arrayOfSheep.filter((sheep) => sheep === true).length;
}

//

function countSheeps(arrayOfSheeps) {
  return arrayOfSheeps.filter(Boolean).length;
}


// Powers of 2

function powersOfTwo(n) {
  let res = [];

  for (let i = 0; i <= n; i++) {
    res.push(2 ** i);
  }

  return res;
}


// Rock Paper Scissors!

function rockPaperScissors(p1, p2) {
  if (p1 === p2) {
    return `Draw!`;
  }

  if (p1 === 'rock' && p2 === 'scissors') {
    return `Player 1 won!`;
  } else if (p1 === 'paper' && p2 === 'rock') {
    return `Player 1 won!`;
  } else if (p1 === 'scissors' && p2 === 'paper') {
    return `Player 1 won!`;
  } else {
    return `Player 2 won!`;
  }
}


// CSV representation of array

function toCsvText(array) {
  return array.join('\n');
}


// Is this my tail?

function correctTail(body, tail) {
  let sub = body.substr(body.length - tail.length);

  if (sub == tail) {
    return true;
  } else {
    return false;
  }
}

//

function correctTail(bod, tail) {
  return bod[bod.length - 1] === tail;
}


// Reverse List Order

function reverseList(list) {
  return list.reverse();
}


// L1: Set Alarm

function setAlarm(employed, vacation) {
  if (employed && !vacation) {
    return true;
  } else {
    return false;
  }
}

//

function setAlarm(employed, vacation) {
  return employed && !vacation;
}


// Regexp Basics - is it a digit?

String.prototype.digit = function () {
  return /^\d$/.test(this);
};

//

String.prototype.digit = function () {
  return /^[0-9]$/.test(this);
};


// Compare within margin

const closeCompare = (a, b, margin) =>
  Math.abs(a - b) <= margin ? 0 : Math.sign(a - b);

//

function closeCompare(a, b, m = 0) {
  return Math.abs(a - b) <= m ? 0 : Math.sign(a - b);
}


// Total amount of points

function points(games) {
  return games
    .map((str) => str.split(':').map(Number))
    .map(([x, y]) => (x > y ? 3 : x == y ? 1 : 0))
    .reduce((acc, cur) => acc + cur, 0);
}


// A wolf in sheep's clothing

function warnTheSheep(queue) {
  if (queue[queue.length - 1] === 'wolf') {
    return 'Pls go away and stop eating my sheep';
  } else {
    let index = queue.findIndex((x) => x == 'wolf');
    return `Oi! Sheep number ${
      queue.length - index - 1
    }! You are about to be eaten by a wolf!`;
  }
}

//

function warnTheSheep(queue) {
  const position = queue.reverse().indexOf('wolf');
  return position === 0
    ? 'Pls go away and stop eating my sheep'
    : `Oi! Sheep number ${position}! You are about to be eaten by a wolf!`;
}


// Pillars

function pillars(numPill, dist, width) {
  return numPill > 1 ? (numPill - 1) * dist * 100 + (numPill - 2) * width : 0;
}

//

function pillars(numPill, dist, width) {
  return numPill <= 1 ? 0 : (numPill - 1) * dist * 100 + (numPill - 2) * width;
}


// Convert a String to a Number!

const stringToNumber = (str) => {
  return +str;
};

//

const stringToNumber1 = (str) => {
  return parseInt(str);
};

//

const stringToNumber2 = (str) => {
  return Number(str);
};


// Correct the mistakes of the character recognition software

function correct(string) {
  return string.replace(/5/g, 'S').replace(/0/g, 'O').replace(/1/g, 'I');
}


// Function 3 - multiplying two numbers

const multiply = (a, b) => a * b;

//

function multiply(a, b) {
  if (typeof a == 'number' && typeof b == 'number') return a * b;
}


// String Templates - Bug Fixing #5

function buildString(...template) {
  return `I like ${template.join(', ')}!`;
}


// Find Maximum and Minimum Values of a List

const min = function (list) {
  return Math.min(...list);
};

const max = function (list) {
  return Math.max(...list);
};

//

const min1 = (list) => Math.min(...list);
const max1 = (list) => Math.max(...list);


// Is the string uppercase?

String.prototype.isUpperCase = function () {
  return this == this.toUpperCase();
};

//

String.prototype.isUpperCase = function () {
  return this.toUpperCase() === this.toString();
};


// Expressions Matter

function expressionMatter(a, b, c) {
  return Math.max(a + b + c, a * b * c, (a + b) * c, a * (b + c));
}

//

function expressionMatter(a, b, c) {
  return Math.max(
    ...[
      `${a * (b + c)}`,
      `${a * b * c}`,
      `${a + b * c}`,
      `${(a + b) * c}`,
      `${a + b + c}`,
    ]
  );
}


// Will you make it?

const zeroFuel = (distanceToPump, mpg, fuelLeft) => {
  return mpg * fuelLeft >= distanceToPump ? true : false;
};

//

const zeroFuel1 = (distanceToPump, mpg, fuelLeft) => {
  return distanceToPump / mpg <= fuelLeft;
};


// Object Oriented Piracy

function Ship(draft, crew) {
  this.draft = draft;
  this.crew = crew;
  this.isWorthIt = function () {
    return this.draft - this.crew * 1.5 > 20;
  };
}

//

function Ship2(draft, crew) {
  this.draft = draft;
  this.crew = crew;
}

Ship2.prototype.isWorthIt = function () {
  return this.draft - this.crew * 1.5 > 20;
};


// String repeat

function repeatStr (n, s) {
  return s.repeat(n);
}


// Holiday VI - Shark Pontoon

function shark(pontoonDistance, sharkDistance, youSpeed, sharkSpeed, dolphin) {
  return sharkDistance / (dolphin ? sharkSpeed / 2 : sharkSpeed) > pontoonDistance / youSpeed ? 'Alive!' : 'Shark Bait!'
}

// 

function shark(pontoonDistance, sharkDistance, youSpeed, sharkSpeed, dolphin){
  if(dolphin){
    sharkSpeed /= 2;
  }
  return pontoonDistance/youSpeed < sharkDistance/sharkSpeed ? "Alive!" : "Shark Bait!";
}


// Exclusive "or" (xor) Logical Operator

function xor(a, b) {
  if (a && b) {
    return false
  } else if ((!a && b) || (a && !b)) {
    return true
  } {
    return false
  }
}

//

function xor(a, b) {
  return a != b;
}

// 

function xor(a, b) {
  return (a || b) && !(a && b);
}


// Simple validation of a username with regex

function validateUsr(username) {
  return /^[a-z0-9_]{4,16}$/.test(username)
}

// 

function validateUsr(username) {
  return (/^[a-z0-9_]{4,16}$/.test(username));
}


// Count Odd Numbers below n

function oddCount(n){
  return Math.floor(n / 2)
}



// Opposites Attract

function lovefunc(flower1, flower2){
  if (flower1 % 2 == 0 && flower2 % 2 == 1) {
    return true
  }
  
  if (flower1 % 2 === 1 && flower2 % 2 === 0) {
    return true
  } else {
    return false
  }
}

// 

function lovefunc(flower1, flower2){
  return flower1 % 2 !== flower2 % 2;
}

// 

function lovefunc(flower1, flower2){
  return (flower1 + flower2) % 2 === 1
}


// Bin to Decimal

function binToDec(bin) {
  return parseInt(bin, 2)
}


// Simple multiplication

function simpleMultiplication(number) {
  return number % 2 === 0 ? number * 8 : number * 9
}


// Welcome to the City

function sayHello( name, city, state ) {
  return `Hello, ${name.join(' ')}! Welcome to ${city}, ${state}!`
}


// 

function sayHello( name, city, state ) {
  return 'Hello, ' + name.join(' ') + '! Welcome to ' + city + ', ' + state + '!';
}


// Grasshopper - Debug sayHello

function sayHello(name) {
  return `Hello, ${name}`
}


// 

function sayHello (name) {
  return 'Hello, ' +  name;
}


// To square(root) or not to square(root)

function squareOrSquareRoot(array) {
  return array.map(x => Math.sqrt(x) % 1 ? x * x : Math.sqrt(x))  
}


// 

function squareOrSquareRoot(array) {
  return array.map(x => {
    const r = Math.sqrt(x);
    return (r % 1 == 0) ? r : (x*x);
  });  
}


// Name Shuffler

function nameShuffler(str){
  return str.split(" ").reverse().join(' ')
}


// Double Char

function doubleChar(str) {
  return str.split('').map(x => x + x).join('')
}


// Convert a string to an array

function stringToArray(string){
  return string.split(' ')
}


// Removing Elements

function removeEveryOther(arr){
  return arr.filter((_, index) => index % 2 === 0)
}


// Area of a Square

function squareArea(A){
  return +Math.pow(2 * A / Math.PI, 2).toFixed(2)
}


// 

function squareArea(A){
  // Calculate the circumference of A 
  const circumference = A * 4;
  
  // Calculate the radius of A
  const radius = circumference / (Math.PI * 2);
  
  // Calculate the area of the square, rounded to 2 decimal places
  const area = Number((radius**2).toFixed(2));
  
  // Return the result
  return area;
}


// Plural

function plural(n) {
  return n == 1 ? false : true
}

// 

function plural(n) {
  return n != 1;
}


// Determine offspring sex based on genes XX and XY chromosomes

function chromosomeCheck(sperm) {
  if (sperm === 'XX') {
    return "Congratulations! You're going to have a daughter."
  } else if (sperm === 'XY') {
    return "Congratulations! You're going to have a son."
  } else if (sperm === 'YX') {
    return "Congratulations! You're going to have a son."
  } else {
    return 'I dont understand anything, what is it?'
  }
}

// 

function chromosomeCheck(sperm) {
  return `Congratulations! You're going to have a ${sperm === 'XY' ? 'son' : 'daughter'}.`
}


// Function 2 - squaring an argument

const square = (x) => x ** 2

// 

const square2 = (n) => n * n;


// 101 Dalmatians - squash the bugs, not the dogs!

function howManyDalmatians(number) {
  let dogs = ["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIANS!!!"];
  
  return number <= 10 ? dogs[0] : number <= 50 ? dogs[1] : number == 101 ?  dogs[3] : dogs[2]
}

// 

function howManyDalmatians(number){
  if (number <= 10) {
    return "Hardly any"
  } else if (number <= 50) {
    return "More than a handful!"
  } else if (number === 101) {
    return "101 DALMATIANS!!!"
  } else {
    return "Woah that's a lot of dogs!" 
  }
}


// Define a card suit

function defineSuit(card) {
  if (card.includes('♣')) return 'clubs'
  if (card.includes('♦')) return 'diamonds'
  if (card.includes('♥')) return 'hearts'
  if (card.includes('♠')) return 'spades'  
}


// Freudian translator

let toFreud=s=>s.replace(/[^ ]+/g,'sex')

// 

const toFreud = str => str === '' ? '' : str.split(' ').map(e => 'sex').join(' ')

//

function toFreud(string) {
  return string.replace(/\S+/g, 'sex');
}


// You Can't Code Under Pressure #1

function doubleInteger(i) {
  return i * 2;
}


// Name on billboard

function billboard(name, price = 30) {
  let totalCost = 0;

  for (let i = 0; i < name.length; i++) {
    totalCost += price;
  }

  return totalCost;
}


// Sum of differences in array

function sumOfDifferences(arr) {
  return arr.length > 1 ? Math.max(...arr) - Math.min(...arr) : 0
}


// What is between?

function between(a, b) {
  return Array.from(new Array(b - a + 1), x => a++)
}


// Training JS #1: create your first JS function and print "Hello World!"

function helloWorld() {
  const str = "Hello World!"
  
  console.log(str)
}


// Cat years, Dog years


var humanYearsCatYearsDogYears = function(y) {
  if (y == 1) return [1, 15, 15]
  if (y == 2) return [2, 24, 24]
  return [y, (y-2) * 4 + 24, (y-2) * 5 + 24]
}

//

const humanYearsCatYearsDogYears = (humanYears) => {
  let catYears = 0;
  let dogYears = 0;
  
  for (let i = 1; i <= humanYears; i++) {
    if (i === 1) {
      catYears += 15;
      dogYears += 15;
    }
    else if (i === 2) {
      catYears += 9;
      dogYears += 9;
    }
    else {
      catYears += 4;
      dogYears += 5;
    }
  }
  return [humanYears,catYears,dogYears];
}

//

const humanYearsCatYearsDogYears = humanYears => [
  humanYears,
  ( humanYears - 1 ? 16 : 11 ) + 4 * humanYears,
  ( humanYears - 1 ? 14 : 10 ) + 5 * humanYears,
];

//

function humanYearsCatYearsDogYears(humanYears) {
  switch (humanYears) {
    case 1:
      return [1, 15, 15]
    case 2:
      return [2, 24, 24];
    default:
      return [humanYears, (humanYears - 2) * 4 + 24, (humanYears - 2) * 5 + 24 ];
  }
  
}


// Check same case

const sameCase = (a, b) => /[a-z]/i.test(a) && /[a-z]/i.test(b) ? Number(/[a-z]/.test(a) == /[a-z]/.test(b)) : -1

//

function sameCase(a, b){
  if(a.toUpperCase() === a.toLowerCase() || b.toLowerCase() === b.toUpperCase()){
     return -1
   }else if(a === a.toLowerCase() && b === b.toLowerCase() || a === a.toUpperCase() && b === b.toUpperCase()){
       return 1
   }else{
     return 0
   }
}


// Fundamentals: Return

function add(a,b){
  return a + b
}

function divide(a,b){
  return a / b
}

function multiply(a,b){
  return a * b
}

function mod(a,b){
  return a % b
}
 
function exponent(a,b){
  return a ** b
}
  
function subt(a,b){
  return a - b
}


// Short Long Short

function solution(a, b){
  let short = a.length < b.length ? a : b
  let long = a.length > b.length ? a : b
  
  return short + long + short
}

//

function solution(a, b) {
  return a.length < b.length ? a + b + a : b + a + b
}

//

function solution(a, b){
  return (a.length > b.length) ? b + a + b : a + b + a;
}


// Цикл в цикле, делаеи елочку со *

let result = '';
const length = 7;

for (let i = 1; i < length; i++) {

  for (let j = 0; j < i; j++) {
    result += '*';
  }

  result += '\n';
}

console.log(result);

//*
//**
//***
//****
//*****
//******


// Цикл в цикле, тройная глубина + break & continie

first: for (let i = 0; i < 3; i++) {
  console.log(`First level: ${i}`)

  for (let j = 0; j < 3; j++) {
    console.log(`Second level: ${j}`)

    for (let k = 0; k < 5; k++) {
      if (k === 2) continue first;
      // if (k === 2) break first;

      console.log(`Third level: ${k
      }`)
    }
  } 
}

			  
// Abbreviate a Two Word Name

function abbrevName(name){
  return name.split(' ').map(x => x[0].toUpperCase()).join('.')
}

//

function abbrevName(name){
  const newArray = name.split(" ")
  return (newArray[0][0] + "." + newArray[1][0]).toUpperCase()
}

//

function abbrevName(name){
  return name.match(/\b(\w)/g).toString().toUpperCase().replace(',', '.');
}

	
// Beginner Series #2 Clock

function past(h, m, s){
  return h * 3600000 + m * 60000 + s * 1000;
}

	
// Invert values

function invert(array) {
  return array.map(num => num * -1);
}

//

const invert = array => array.map(num => -num);

	
// Reversed sequence

const reverseSeq = n => {
  let arr = [];
  
  for (let i = n; i > 0; i--) {
    arr.push(i)
  }
  
  return arr;
};

	
// MakeUpperCase

function makeUpperCase(str) {
  return str.toUpperCase()
}

	
// Remove First and Last Character

function removeChar(str){
  return str.slice(1, -1)
};

	
// You only need one - Beginner

function check(a, x) {
  return a.includes(x) || a.includes('x')
}

// 

function check(a,x){
  return a.includes(x);
};

	
// I love you, a little , a lot, passionately ... not at all

function howMuchILoveYou(nbPetals) {
  const arr = ['I love you', 'a little', 'a lot', 'passionately', 'madly', 'not at all'];
  
  for (let i = 0; i <= nbPetals; i++) {
    arr.push(arr[i])
  }
  
  return arr[nbPetals - 1]
}

// 

const phrases = [
  'I love you',
  'a little',
  'a lot',
  'passionately',
  'madly',
  'not at all',
]

function howMuchILoveYou(n) {
   return phrases[(n - 1) % phrases.length] 
}

			       
// Beginner - Lost Without a Map

function maps(x){
  return x.map(y => y * 2)
}

	
// Is the string uppercase?

String.prototype.isUpperCase = function() {
  return this.toUpperCase() === this.toString()
}

	
// Return Negative

function makeNegative(num) {
  return -Math.abs(num)
}

// 

function makeNegative(num) {
  return num < 0 ? num : -num;
}

		
// Returning Strings

function greet(name){
  return `Hello, ${name} how are you doing today?`
}

		
// Get Nth Even Number

function nthEven(n){
  return n * 2 - 2
}

		
// Reversed Strings

function solution(str){
  let res = '';
  
  for (let i of str) {
    res = i + res
  }
  
  return res;
}

// 

function solution(str){
  return str.split('').reverse().join('');  
}

		
// Simple validation of a username with regex


/**
  - `^`        Start from the beginning of the string.
  - `[]`       Allow any character specified, including...
  - `a-z`      anything from a to z,
  - `0-9`      anything from 0 to 9,
  - `_`        and underscore.
  - `{4,16}`   Accept 4 to 16 of allowed characters, both numbers included.
  - `$`        End the string right after specified amount of allowed characters is given.
*/

function validateUsr(username) {
  return /^[0-9a-z_]{4,16}$/.test(username)
}

// get character from ASCII Value

function getChar(c){
  return String.fromCharCode(c)
}

		
// For Twins: 1. Types

function typeValidation(variable, type) {
  return typeof variable == type
}

		
// Safen User Input Part I - htmlspecialchars

function htmlspecialchars(formData) {
  let arr = [];
  
  for (let i = 0; i < formData.length; i++){
    if (formData[i] == '<'){
      arr.push('&lt;');
      
    } else if(formData[i] == '>'){
      arr.push('&gt;');
      
    } else if(formData[i] == '"'){
      arr.push('&quot;');
      
    } else if(formData[i] == '&'){
      arr.push('&amp;');
      
    } else {
      arr.push(formData[i]);
    }
  }
  return arr.join('');
}

// 

function htmlspecialchars(formData) {
  return formData.replace(/&/g, "&amp;")
                .replace(/"/g, "&quot;")
                .replace(/</g, "&lt;")
                .replace(/>/g, "&gt;");
}

	
// Twice as old

function twiceAsOld(dadYearsOld, sonYearsOld) {
  let twice = dadYearsOld - sonYearsOld * 2;
  
  return twice < 0 ? twice * (-1) : twice
}

// 

function twiceAsOld(dadYearsOld, sonYearsOld) {
  return Math.abs(dadYearsOld - 2 * sonYearsOld);
}

	
// Filling an array (part 1)

const arr = N => Array.from({length: N}, (_, index) => index);

// 

function arr(n){
  var newArr = [];
  for(var i = 0; i < n; i++){
    newArr.push(i);
  }
  return newArr;
}

		       
// Closure

function createCounter() {
  let counter = 0;

  const myFunction = function() {
    counter = counter + 1;
    return counter;
  }

  return myFunction;
}

const increment = createCounter();
const c1 = increment();
const c2 = increment();
const c3 = increment();

console.log(c1, c2, c3) // -> 1, 2, 3

	
// Simple and Recursion 

function pow(x, n) {
  let result = 1;

  for (let i = 0; i < n; i++) {
    result *= x;
  }

  return result;
}

function pow(x, n) {
  if (n === 1) {
    return x;
  } else {
    return x * pow(x, n - 1);
  }
}

pow(2, 1); // 2
pow(2, 2); // 4
pow(2, 3); // 8
pow(2, 4); // 16		
```

  **[⬆ Наверх](#top)**
