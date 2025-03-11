<a name="top"></a>

[На главную](../README.md)

## Вопросы

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
|     | Core |
|250 | [Рекурсия для дочерних компонентов](#250) |
|251 | [Что такое предохранители (error boundaries)?](#251) |
|252 | [keys в React. Метод жизненного цикла shouldComponentUpdate](#252) |
|253 | [react-router v5](#253) |
|254 | [Route, Switch, Link v5](#254) |
|255 | [react-router v6](#255) |
|256 | [](#256) |
|257 | [React / redux Dev Tools](#257) |
|258 | [HOC - Компонент высшего порядка](#258) |
|259 | [React Transition Group](#259) |
|260 | [Formik, Yup - работа с формами](#260) |
|261 | [](#261) |
|     | Хуки |
|300 | [Хуки в React](#300) |
|301 | [Методы жизненного цикла может заменить Хуки](#301) |
|302 | [Хуки](#302) |
|303 | [Хуки практика](#303) |
|304 | [Создание собственных хуков](#304) |
|305 | [Практика создание собственных хуков](#305) |
|306 | [](#306) |
|307 | [](#307) |
|308 | [](#308) |
|309 | [](#309) |
|310 | [](#310) |
|320 | [](#320) |
|321 | [](#321) |
|322 | [](#322) |
|323 | [](#323) |
|324 | [](#324) |
|325 | [configureStore(), createReducer(), createAction(), createSlice(), createAsyncThunk(), createEntityAdapter()](#325) |
|326 | [](#326) |
|327 | [](#327) |
|328 | [](#328) |
|329 | [](#329) |
|     | Redux Toolkit |
|330 | [Redux Toolkit: configureStore()](#330) |
|331 | [Redux Toolkit: createAction()](#331) |
|332 | [Redux Toolkit: createReducer()](#332) |
|333 | [Redux Toolkit: createSlice()](#333) |
|334 | [Redux Toolkit: createAsyncThunk()](#334) |
|335 | [Redux Toolkit: createEntityAdapter()](#335) |
|336 | [Redux Toolkit: RTK Query](#336) |
|337 | [](#337) |
|338 | [Redux Toolkit пример](#338) |
|339 | [Redux Toolkit пример 2](#339) |
|340 | [Redux Toolkit createAsyncThunk](#340) |
|341 | [RTK Query](#341) |
|342 | [](#342) |
|343 | [](#343) |
|344 | [](#344) |
|345 | [](#345) |
|346 | [](#346) |
|347 | [](#347) |
|     | Redux |
|350 | [Redux](#350) |
|351 | [connect. HOC](#351) |
|352 | [actions](#352) |
|353 | [reducer](#353) |
|354 | [middleware](#354) |
|355 | [Redux, Actions, Reducer, Store - примеры](#355) |
|356 | [redux-forms в экосистеме React + Redux](#356) |
|357 | [Redux пример](#357) |
|358 | [Соединяем React и Redux при помощи connect и хуков](#358) |
|359 | [combineReducers и reducers](#359) |
|360 | [createSelector from 'reselect'](#360) |
|361 | [enhancer](#361) |
|362 | [applyMiddleware](#362) |
|363 | [ReduxThunk](#363) |
|364 | [](#364) |
|365 | [](#365) |
|377 | [](#377) |
|378 | [](#378) |
|379 | [](#379) |
|380 | [](#380) |
|381 | [](#381) |



<a name="questions"></a>

250. ### <a name="250"></a> Рекурсия для дочерних компонентов

 Рекурсия по дочерним элементам
По умолчанию при рекурсивном обходе дочерних элементов DOM-узла React проходит по обоим спискам потомков одновременно и создаёт мутацию, когда находит отличие.

Например, при добавлении элемента в конец дочерних элементов, преобразование между этими деревьями работает отлично:
```jsx harmony
<ul>
  <li>первый</li>
  <li>второй</li>
</ul>

<ul>
  <li>первый</li>
  <li>второй</li>
  <li>третий</li>
</ul>
```
React сравнит два дерева <li первый</li, сравнит два дерева <li второй</li, а затем вставит дерево <li третий</li.

Если попробовать реализовать это наивно, вставив элемент в начало, то пострадает производительность. Например, преобразование между этими деревьями работает плохо:
```jsx harmony
<ul>
  <li>Санкт-Петербург</li>
  <li>Москва</li>
</ul>

<ul>
  <li>Ростов-на-Дону</li>
  <li>Санкт-Петербург</li>
  <li>Москва</li>
</ul>
```
React будет мутировать каждого потомка, вместо того чтобы оставить <li Санкт-Петербург</li>  и <li Москва</li> нетронутыми. Эта неэффективность может стать проблемой.

### Ключи

Для решения этой проблемы React поддерживает атрибут key. Когда у дочерних элементов есть ключи, React использует их, чтобы сопоставить потомков исходного дерева с потомками последующего дерева. Например, если добавить key к неэффективному примеру выше, преобразование дерева станет эффективным:
```jsx harmony
<ul>
  <li key="2015">Санкт-Петербург</li>
  <li key="2016">Москва</li>
</ul>

<ul>
  <li key="2014">Ростов-на-Дону</li>
  <li key="2015">Санкт-Петербург</li>
  <li key="2016">Москва</li>
</ul>
```
Теперь React знает, что элемент с ключом '2014' — новый, а элементы с ключами '2015' и '2016' только что переместились.

На практике найти ключ обычно несложно. Элемент, который вы хотите отобразить, уже может иметь уникальный идентификатор, и ключ может быть взят из ваших данных:
```jsx harmony
<li key={item.id}>{item.name}</li>
```
Когда уникальное значение отсутствует, вы можете добавить новое свойство идентификатора в вашу модель или прохешировать данные, чтобы сгенерировать ключ. Ключ должен быть уникальным только среди его соседей, а не глобально.
    
  **[⬆ Наверх](#top)**
  
251. ### <a name="251"></a> Что такое предохранители (error boundaries)

 `Error boundaries` - это React-компоненты, которые перехватывают любые ошибки, возникающие в дереве потомков, выводят сообщения об ошибках в консоль и отображают резервный UI вместо "сломанного". Предохранители перехватывают ошибки во время рендеринга, в методах жизненного цикла и в конструкторах любых дочерних компонентов.

Классовый компонент становится предохранителем, когда в нем определяются методы жизненного цикла `static getDerivedStateFromError()` или `componentDidCatch()` (один или оба). `static getDerivedStateFromError()` используется для рендеринга запасного UI после возникновения ошибки. `componentDidCatch()` используется для вывода сообщения об ошибке в консоль.

*Пример*

```js
import React, { Component } from 'react'

class ErrorBoundary extends Component {
   state = {
      isErrorOccured: false,
      errorMessage: ''
   }
   componentDidCatch = (error, info) => {
      this.setState({
        isErrorOccured: true,
        errorMessage: error
      })
   }
   render() {
      if(this.state.isErrorOccured) {
         return <p>Что-то пошло не так</p>
      } else {
         return <div>{this.props.children}</div>
      }
   }
}

export default ErrorBoundary
```

Здесь у нас имеется объект состояния с двумя свойствами - `isErrorOccured` и `errorMessage`, которые будут обновлены при возникновении ошибки. Для обновления состояния мы используем метод `componentDidCatch()`, принимающий два аргумента - `error` и `info`.

**Как использовать предохранитель?**

```js
<ErrorBoundary>
   <User/>
</ErrorBoundary>
```

**Предохранители не перехватывают ошибки в:**

* Обработчиках событий
* Асинхронном коде (например, в `setTimeout()`)
* При серверном рендеринге
* При выбрасывании исключения в самом предохранителе
    
  **[⬆ Наверх](#top)**
  
252. ### <a name="252"></a> keys в React. Метод жизненного цикла shouldComponentUpdate

 ### Ключи

Ключи помогают React определять, какие элементы были изменены, добавлены или удалены. Их необходимо указывать, чтобы React мог сопоставлять элементы массива с течением времени:
```jsx harmony
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```
Лучший способ выбрать ключ — это использовать строку, которая будет явно отличать элемент списка от его соседей. Чаще всего вы будете использовать ID из ваших данных как ключи:
```jsx harmony
const todoItems = todos.map((todo) =>
  <li key={todo.id}>
    {todo.text}
  </li>
);
```
Когда у вас нет заданных ID для списка, то в крайнем случае можно использовать индекс элемента как ключ:
```jsx harmony
const todoItems = todos.map((todo, index) =>
  // Делайте так, только если у элементов массива нет заданного ID
  <li key={index}>
    {todo.text}
  </li>
);
```
Мы не рекомендуем использовать индексы как ключи, если порядок элементов может поменяться. Это негативно скажется на производительности и может вызвать проблемы с состоянием компонента. Почитайте статью Робина Покорни (Robin Pokorny), которая объясняет, почему индексы-ключи приводят к проблемам. Если вы опустите ключ для элемента в списке, то React по умолчанию будет использовать индексы как ключи.

### shouldComponentUpdate

shouldComponentUpdate(nextProps, nextState)

Используйте shouldComponentUpdate(), чтобы указать необходимость следующего рендера на основе изменений состояния и пропсов. По умолчанию происходит повторный рендер при любом изменении состояния. В большинстве случаев вы должны полагаться на это поведение.

shouldComponentUpdate() вызывается перед рендером, когда получает новые пропсы или состояние. Значение по умолчанию равно true. Этот метод не вызывается при первом рендере или когда используется forceUpdate().

Этот метод нужен только для повышения производительности. Но не опирайтесь на его возможность «предотвратить» рендер, это может привести к багам. Вместо этого используйте PureComponent, который позволяет не описывать поведение shouldComponentUpdate() вручную. PureComponent поверхностно сравнивает пропсы и состояние и позволяет не пропустить необходимое обновление.

Если вы уверены, что хотите написать его вручную, вы можете сравнить this.props с nextProps, а this.state с nextState. Верните false чтобы пропустить обновление React. Возврат false не предотвращает повторный рендер дочерних компонентов при изменении их состояния.

Мы не рекомендуем делать глубокое сравнение или использовать JSON.stringify() в shouldComponentUpdate(). Это неэффективно и плохо влияет на производительность.

В настоящее время, если shouldComponentUpdate() возвращает false, то UNSAFE_componentWillUpdate(), render() и componentDidUpdate() не будут вызваны. В будущем React может рассматривать shouldComponentUpdate() как подсказку, а не строгое указание. В таком случае возврат false сможет привести к повторному рендеру компонента.
    
  **[⬆ Наверх](#top)**
  
253. ### <a name="253"></a> react-router v5

 React Router это стандартная библиотека маршрутизации (routing) в React. Он хранит интерфейс приложения синхронизированным с URL на браузере. React Router позволяет вам маршрутизировать "поток данных" (data flow) в вашем приложении понятным способом.

### 1. Основная маршрутизация

В приведенном ниже примере у нас имеется 3 страницы, обрабатываемые роутером: главная (home), контакты (about) и страница с пользователями (users). При клике по <Link> (ссылке) роутер рендерит соответствующий <Route> (маршрут, путь).

Обратите внимание: за сценой <Link> рендерит <a> с настоящим href, так что люди, использующие клавиатуру для навигации или экранные считываюющие устройства (screen readers), смогут без проблем пользоваться приложением.
```jsx harmony
import React from 'react'
import {
  BrowserRouter as Router,
  Switch,
  Route,
  Link
} from 'react-router-dom'

export const App = () => (
  <Router>
      <header>
        <nav>
          <ul>
            <li>
              <Link to="/">Главная</Link>
            </li>
            <li>
              <Link to="/about">Контакты</Link>
            </li>
            <li>
              <Link to="/users">Пользователи</Link>
            </li>
          </ul>
        </nav>
      </header>

      <main>
        {/* <Switch> рендерит первый <Route>, совпавший с URL */}
        <Switch>
          <Route path="/about">
            <About />
          </Route>
          <Route path="/users">
            <Users />
          </Route>
          <Route path="/">
            <Home />
          </Route>
        </Switch>
      </main>
  </Router>
)

const Home = () => <h2>Главная</h2>

const About = () => <h2>Контакты</h2>

const Users = () => <h2>Пользователи</h2>
```	      
	      
### 2. Вложенный роутинг
	      
Ниже приводится пример вложенного роутинга. Маршрут /topics загружает компонент Topics, который, в свою очередь, рендерит дальнейшие <Route> на основе значения :id.
```jsx harmony
import React from "react"
import {
  BrowserRouter as Router,
  Switch,
  Route,
  Link,
  useRouteMatch,
  useParams
} from "react-router-dom"

export const App = () => (
  <Router>
    <header>
      <nav>
        <ul>
          <li>
            <Link to="/">Главная</Link>
          </li>
          <li>
            <Link to="/about">Контакты</Link>
          </li>
          <li>
            <Link to="/topics">Темы</Link>
          </li>
        </ul>
      </nav>
    </header>

    <main>
      <Switch>
        <Route path="/about">
          <About />
        </Route>
        <Route path="/topics">
          <Topics />
        </Route>
        <Route path="/">
          <Home />
        </Route>
      </Switch>
    </main>
  </Router>
)

const Home = () => <h2>Главная</h2>

const About = () => <h2>Контакты</h2>

function Topics() {
  const match = useRouteMatch()

  return (
    <>
      <h2>Темы</h2>

      <nav>
        <ul>
          <li>
            <Link to={`${match.url}/components`}>Компоненты</Link>
          </li>
          <li>
            <Link to={`${match.url}/props-vs-state`}>Пропы против состояния</Link>
          </li>
        </ul>
      </nav>

      {/* Страница Topics имеет собственный <Switch> с маршрутами,
          основанными на URL /topics. Вы можете думать о втором
          <Route> как о странице для остальных тем
          или как о странице, отображаемой,
          когда ни одна из тем не выбрана */}
      <div>
        <Switch>
          <Route path={`${match.path}/:topicId`}>
            <Topic />
          </Route>
          <Route path={match.path}>
            <h3>Пожалуйста, выберите тему.</h3>
          </Route>
        </Switch>
      </div>
    </>
  )
}

function Topic() {
  const { topicId } = useParams()
  return <h3>Идентификатор выбранной темы: {topicId}</h3>
}
```
	      
### Основные компоненты
	      
В React Router существует 3 категории компонентов:

- роутеры (routers), например, <BrowserRouter> или <HashRouter>
- маршруты (route matchers), например, <Route> или <Switch>
- и навигация (navigation), например, <Link>, <NavLink> или <Redirect>
	      
Все компоненты, используемые в веб-приложении, должны быть импортированы из react-router-dom.

### Роутеры
	      
Любая маршрутизация начинается с роутера. Для веб-проектов react-router-dom предоставляет <BrowserRouter> и <HashRouter>. Основное отличие между ними состоит в способе хранения URL и взаимодействия с сервером.

<BrowserRouter> использует обычные URL. В этом случае URL выглядят как обычно, но требуется определенная настройка сервера. В частности, сервер должен обслуживать все страницы, используемые на клиенте. Create React App поддерживает это из коробки в режиме разработки и содержит инструкции для правильной настройки сервера.
<HashRouter> хранить текущую локацию в хэш-части URL (после символа "#"), поэтому URL выглядит примерно так: http://example.com/#/your/page. Поскольку хэш не отправляется серверу, его специальная настройка не требуется.
	
Для использования роутера необходимо обернуть в него компонент верхнего уровня:
	
```jsx harmony
import React from "react"
import ReactDOM from "react-dom"
import { BrowserRouter } from "react-router-dom"

const App = () => <h1>Привет, React Router</h1>

ReactDOM.render(
  <BrowserRouter>
    <App />
  </BrowserRouter>,
  document.getElementById("root")
)	      
```	      

### Маршруты
	
Существует 2 вида компонентов для поиска совпадений с URL: Switch и Route. При рендеринге <Switch> определяет <Route>, соответствующий текущему URL. При обнаружении такого маршрута, он рендерится, остальные маршруты игнорируются. Это означает, что вы должны помещать более специфические маршруты перед менее специфическими.

Если совпадения не найдено, <Switch> ничего не рендерит (точнее, рендерит null).
```jsx harmony
import React from "react"
import ReactDOM from "react-dom"
import {
  BrowserRouter as Router,
  Switch,
  Route
} from "react-router-dom"

const App = () => (
  <main>
    <Switch>
      {/* Если текущим URL является /about, рандерится данный маршрут,
          остальные игнорируются */}
      <Route path="/about">
        <About />
      </Route>

      {/* Обратите внимание на порядок расположения этих двух маршрутов.
          Более специфический path="/contact/:id" находится перед path="/contact" */}
      <Route path="/contact/:id">
        <Contact />
      </Route>
      <Route path="/contact">
        <AllContacts />
      </Route>

      {/* Если ни один из предыдущих роутеров не совпал,
          рендерится данный маршрут (он является резервным).

          Важно: маршрут с path="/" всегда будет совпадать с
          URL, поскольку все URL начинаются с /. Поэтому
          мы поместили его последним */}
      <Route path="/">
        <Home />
      </Route>
    </Switch>
  </main>
)

ReactDOM.render(
  <Router>
    <App />
  </Router>,
  document.getElementById("root")
)
```	
	
Обратите внимание, что <Route path> ищет совпадение с началом, а не со всем URL. Поэтому <Route path="/"> всегда будет совпадать с URL. Поэтому в <Switch> мы, обычно, помещаем его последним. Другим возможным решением является использование атрибута exact: <Route exact path="/">, который заставляет роутер искать полное совпадение.

### Навигация
	
React Router предоставляет компонент <Link> для создания ссылок в приложении. При использовании <Link> в HTML рендерится <a>.
	
```jsx harmony
<Link to="/">Главная</Link>
// <a href="/">Главная</a>
```	
	
<NavLink> - это специальный тип <Link>, позволяющий определять стили для активного состояния ссылки.
```jsx harmony
<NavLink to="/react" activeClassName="hurray">
  React
</NavLink>

// Когда URL является /react, рендерится это:
// <a href="/react" className="hurray">React</a>

// Когда URL является другим:
// <a href="/react">React</a>
```	
Для принудительной навигации используется <Redirect>. При рендеринге <Redirect> выполняется перенаправление.
```jsx harmony
<Redirect to="/login">	
```	

## Пример с проекта
	
### App.js	
```jsx harmony
import {BrowserRouter as Router, Route, Switch} from 'react-router-dom';

import {MainPage, ComicsPage} from '../pages';
import AppHeader from "../appHeader/AppHeader";

const App = () => {
    
    return (
        <Router>
            <div className="app">
                <AppHeader/>
                <main>
                    <Switch>
                        <Route exact path="/">
                            <MainPage/>
                        </Route>
                        <Route exact path="/comics">
                            <ComicsPage/>
                        </Route>
                    </Switch>
                </main>
            </div>
        </Router>
    )
}

export default App;	
```	
### MainPage.js
```jsx harmony
import { useState } from "react";

import RandomChar from "../randomChar/RandomChar";
import CharList from "../charList/CharList";
import CharInfo from "../charInfo/CharInfo";
import ErrorBoundary from "../errorBoundary/ErrorBoundary";

import decoration from '../../resources/img/vision.png';

const MainPage = () => {

    const [selectedChar, setChar] = useState(null);

    const onCharSelected = (id) => {
        setChar(id);
    }

    return (
        <>
            <ErrorBoundary>
                <RandomChar/>
            </ErrorBoundary>
            <div className="char__content">
                <ErrorBoundary>
                    <CharList onCharSelected={onCharSelected}/>
                </ErrorBoundary>
                <ErrorBoundary>
                    <CharInfo charId={selectedChar}/>
                </ErrorBoundary>
            </div>
            <img className="bg-decoration" src={decoration} alt="vision"/>
        </>
    )
}

export default MainPage;	
```
### ComicsPage.js
```jsx harmony
import ComicsList from "../comicsList/ComicsList";
import AppBanner from "../appBanner/AppBanner";

const ComicsPage = () => {
    return (
        <>
            <AppBanner/>
            <ComicsList/>
        </>
    )
}

export default ComicsPage;	
```	
	
https://github.com/harryheman/React-Total/blob/main/md/react-router.md#%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B0%D0%BD%D0%B8%D0%B5
    
  **[⬆ Наверх](#top)**
  
254. ### <a name="254"></a> Route, Switch, Link v6

 ### <a name="router"></a> `<Router>`

Общий низкоуровневый интерфейс для компонентов роутера. Обычно, используется один из следующих роутеров:

- [&lt;BrowserRouter>](#browser)
- [&lt;HashRouter>](#hash)
- [&lt;MemoryRouter>](#memory)
- [&lt;StaticRouter>](#static)
- `<NativeRouter>`

- [Route](#route)		
- [Switch](#switch)	
- [Link](#link)	
- [NavLink](#nav)
- [Redirect](#redirect)
	
	
Одним из случаев использования низкоуровневого `<Router>` является синхронизация пользовательской истории с такими библиотеками для управления состоянием приложения, как `Redux` или `MobX`. *Обратите внимание*, что делать этого не рекомендуется.

#### Пропы

- `history`: object - атрибут, используемый для навигации
- `children`: node - дочерний элемент

	
### <a name="browser"></a> `<BrowserRouter>`

`<Router>`, использующий `HTML5 history API` (события "pushState", "replaceState" и "popState") для синхронизации UI с URL.

```js
<BrowserRouter
  basename={optionalString}
  forceRefresh={optionalBool}
  getUserConfirmation={optionalFunc}
  keyLength={optionalNumber}
>
  <App />
</BrowserRouter>
```

#### Пропы

- `basename`: string - базовый URL для всех локаций. Если приложение обслуживается из поддиректории на сервере, базовый URL должен иметь значение данной поддиректории

```js
<BrowserRouter basename="/calendar">
    <Link to="/today"/> // рендерится как <a href="/calendar/today">
    <Link to="/tomorrow"/> // рендерится как <a href="/calendar/tomorrow">
    ...
</BrowserRouter>
```

- `getUserConfirmation`: func - функция для подтверждения перехода на другую страницу (по умолчанию используется `window.confirm`)

```js
<BrowserRouter
  getUserConfirmation={(message, callback) => {
    // поведение по умолчанию
    const allowTransition = window.confirm(message)
    callback(allowTransition)
  }}
/>
```

- `forceRefresh`: bool - если `true`, выполняется полное обновление страницы. Используется для имитации поведения сервера при переключении страниц
- `keyLength`: number - длина `location.key` (по умолчанию равняется 6)
- `children`: node - дочерние элементы

**[⬆ 254](#254)**	

	
### <a name="hash"></a> `<HashRouter>`

`<Router>`, использующий хэш-часть URL (т.е. `window.location.hash`) для синхронизации UI с URL.

*Обратите внимание*, что хэш-история не поддерживает `location.key` или `location.state`.

```js
<HashRouter
  basename={optionalString}
  getUserConfirmation={optionalFunc}
  hashType={optionalString}
>
  <App />
</HashRouter>
```

#### Пропы

- `basename`: string - базовый URL для всех локаций

```js
<HashRouter basename="/calendar"/>
<Link to="/today"/> // рендерится как <a href="#/calendar/today">
```

- `getUserConfirmation`: func - функция для подтверждения перехода на другую страницу (по умолчанию используется `window.confirm`)
- `hashType`: string - тип кодировки для `window.location.hash`. Доступные значения:
  - `slash` - `#/` и `#/sunshine/lollipops` (значение по умолчанию)
  - `noslash` - `#` и `#sunshine/lollipops`
  - `hashbang` - `#!/` и `#!/sunshine/lollipops` (признан устаревшим в Chrome)
- `children`: node - дочерний элемент

**[⬆ 254](#254)**
	
	
### <a name="memory"></a> `<MemoryRouter>`

`<Router>`, хранящий историю URL в памяти (не читает и не пишет в адресную строку). Используется для тестирования и вне браузера (например, в `React Native`).

```js
<MemoryRouter
  initialEntries={optionalArray}
  initialIndex={optionalNumber}
  getUserConfirmation={optionalFunc}
  keyLength={optionalNumber}
>
  <App />
</MemoryRouter>
```

#### Пропы

- `initialEntries`: array - массив локаций в стеке истории. Локации могут быть полноценными объектами с `{ pathname, search, hash, state }` или строками

```js
<MemoryRouter
  initialEntries={["/one", "/two", { pathname: "/three" }]}
  initialIndex={1}
>
  <App />
</MemoryRouter>
```

- `initialIndex`: number - индекс начальной локации в массиве `initialEntries`
- `getUserConfirmation`: func - функция для подтверждения перехода на другую страницу (по умолчанию используется `window.confirm`)
- `keyLength`: number - длина `location.key` (по умолчанию - 6)
- `children`: node - дочерние элементы

**[⬆ 254](#254)**
	
	
### <a name="static"></a> `<StaticRouter>`

`<Router>`, не изменяющий локацию. Используется в сценариях рендеринга на стороне сервера и для тестирования результатов рендеринга при подключении определенной локации.

Пример node-сервера, отправляющего статус-код 302 для `<Redirect>` и обычный HTML в ответ на другие запросы:

```js
import http from "http"
import React from "react"
import ReactDOMServer from "react-dom/server"
import { StaticRouter } from "react-router"

http
  .createServer((req, res) => {
    // Данный объект контекста содержит результаты рендеринга
    const context = {}

    const html = ReactDOMServer.renderToString(
      <StaticRouter location={req.url} context={context}>
        <App />
      </StaticRouter>
    )

    // context.url будет содержать URL для перенаправления при использовании <Redirect>
    if (context.url) {
      res.writeHead(302, {
        Location: context.url
      })
      res.end()
    } else {
      res.write(html)
      res.end()
    }
  })
  .listen(3000)
```

#### Пропы

- `basename`: string - базовый URL для всех локаций
- `location`: string - URL, принимаемый сервером (`req.url`)
- `location`: object - объект локации вида `{ pathname, search, hash, state }`
- `context`: object - обычный JS-объект. В процессе рендеринга компоненты могут добавлять свойства к этому объекту для хранения информации о рендеринге

```js
const context = {}
<StaticRouter context={context}>
  <App />
</StaticRouter>
```

При совпадении, `<Route>` передает компоненту, подлежащему рендерингу, объект контекста как проп `staticContext`. После рендеринга, эти свойства могут использоваться для настройки ответа сервера:

```js
if (context.status === "404") {
  // ...
}
```

- `children`: node - дочерние элементы


**[⬆ 254](#254)**

	
### Route <a name="route"></a>			

Данный компонент является ключевым в `React Router`. Поэтому важно хорошо знать, как он работает. В основном, он отвечает за рендеринг определенного UI при совпадении значения его пропа `path` с текущим URL.

Рассмотрим следующий код:

```js
import React from "react"
import ReactDOM from "react-dom"
import { BrowserRouter as Router, Route } from "react-router-dom"

ReactDOM.render(
  <Router>
    <div>
      <Route exact path="/">
        <Home />
      </Route>
      <Route path="/news">
        <NewsFeed />
      </Route>
    </div>
  </Router>,
  node
)
```

Если локацией приложения будет `/`, то иерархия UI будет выглядеть так:

```js
<div>
  <Home />
  <!-- react-empty: 2 -->
</div>
```

А для локации `/news` так:

```js
<div>
  <!-- react-empty: 1 -->
  <NewsFeed />
</div>
```

Комментарии "react-empty" - это детали реализации нулевого рендеринга. Технически, маршрут рендерится всегда: при совпадении с текущей локацией рендерится компонент, при несовпадении - `null`. Если один и тот же компонент является потомком нескольких `<Route>`, `React` будет рассматривать его как один и тот же экземпляр и состояние компонента будет автономным, т.е. компонент не будет перерисовываться при изменении локации. Во избежание этого к каждому `<Route>` добавляется проп `key` с уникальным значением.

#### Методы рендеринга маршрута

Рекомендуемым способом рендеринга является использование дочерних элементов как в приведенном выше примере. Тем не менее, существует и другие способы:

- `<Route component>`
- `<Route render>`
- `<Route children>`

Следует придерживаться одного стиля.

#### Пропы маршрута

Все 3 метода рендеринга принимают следующие пропы:

- `match`
- `location`
- `history`

#### component

Компонент, подлежащий рендерингу при совпадении с локацией. Данному компоненту доступны все пропы маршрута:

```js
import React from "react"
import ReactDOM from "react-dom"
import { BrowserRouter as Router, Route } from "react-router-dom"

// Все пропы маршрута (match, location и history) доступны для User
const User = (props) => <h1>Привет, {props.match.params.username}!</h1>

ReactDOM.render(
  <Router>
    <Route path="/user/:username" component={User} />
  </Router>,
  node
)
```

При использовании `component` (вместо `render` или `children`), маршрут использует `React.createElement` для создания нового React-элемента. Это означает, что при передаче встроенной функции в качестве пропа компонента, при каждом рендеринге будет создаваться новый компонент. Это приводит к размонтированию/монтированию нового компонента вместо обновления существующего. Поэтому при необходимости передачи встроенной функции следует использовать `render` или `children`.

#### render: func

Это позволяет реализовать встроенный рендеринг без нежелательного перемонтирования.

Вместо создания нового элемента с помощью пропа `component`, можно передать функцию, вызываемую при совпадении с локацией. Данная функция имеет доступ ко всем пропам маршрута:

```js
import React from "react"
import ReactDOM from "react-dom"
import { BrowserRouter as Router, Route } from "react-router-dom"

// встроенный рендеринг
ReactDOM.render(
  <Router>
    <Route path="/home" render={() => <div>Главная</div>} />
  </Router>,
  node
)

// композиция
// Вы можете распаковать routeProps, чтобы сделать их доступными для Component
const FadingRoute = ({ component: Component, ...rest }) => (
  <Route
    {...rest}
    render={routeProps => (
      <FadeIn>
        <Component {...routeProps} />
      </FadeIn>
    )}
  />
)

ReactDOM.render(
  <Router>
    <FadingRoute path="/cool" component={Something} />
  </Router>,
  node
)
```

#### children: func

Порой нам требуется условный рендеринг. В этом случае можно использовать функцию в качестве значения пропа `children`. Она работает как `render`, за исключением того, что вызывается в зависимости от совпадения с локацией.

Данный проп принимает те же пропы маршрута. При несовпадении маршрута, проп `match` будет иметь значение `null`. Это позволяет динамически обновлять UI. В приведенном ниже примере мы динамически добавляем класс `active`:

```js
import React from "react"
import ReactDOM from "react-dom"
import {
  BrowserRouter as Router,
  Link,
  Route
} from "react-router-dom"

const ListItemLink = ({ to, ...rest }) => (
  <Route
    path={to}
    children={({ match }) => (
      <li className={match ? "active" : ""}>
        <Link to={to} {...rest} />
      </li>
    )}
  />
)

ReactDOM.render(
  <Router>
    <ul>
      <ListItemLink to="/somewhere" />
      <ListItemLink to="/somewhere-else" />
    </ul>
  </Router>,
  node
)
```

Это также может использоваться для анимации:

```js
<Route
  children={({ match, ...rest }) => (
    {/* Animate будет рендерится всегда, поэтому можно использовать жизненный цикл
        для анимации монтирования/размонтирования его потомков */}
    <Animate>
      {match && <Something {...rest}/>}
    </Animate>
  )}
/>
```

#### Пропы

- `path`: string, string[] - любой валидный URL или массив таких URL (маршрут без `path` совпадает с любой локацией)

```js
<Route path="/users/:id">
  <User />
</Route>
<Route path={["/users/:id", "/profile/:id"]}>
  <User />
</Route>
```

- `exact`: bool - если `true`, осуществляется поиск точного совпадения с `location.pathname`

```js
<Route exact path="/one">
  <About />
</Route>
```

- `strict`: bool - если `true`, при поиске совпадения учитывается замыкающий слэш
- `location`: object - используется для поиска совпадения с указанной локацией вместо текущей
- `sensitive`: bool - если `true`, при поиске совпадения учитывается регистр

**[⬆ 254](#254)**	
	
	
### Switch <a name="switch"></a>		

Рендерит первый дочерний `<Route>` или `<Redirect>` при совпадении с текущей локацией (URL).

**В чем состоит особенность `<Switch>`?**

Особенность `<Switch>` состоит в том, что он рендерит только один маршрут из набора. Без `<Switch>` рендерится каждый маршрут, совпавший с локацией.

```js
import { Route } from "react-router"

const routes = (
  <div>
    <Route path="/about">
      <About />
    </Route>
    <Route path="/:user">
      <User />
    </Route>
    <Route>
      <NoMatch />
    </Route>
  </div>
)
```

В приведенном примере при значении URL, равном `/about`, все 3 компонента будут совпадать с локацией и отрендерятся. Это позволяет выстраивать композицию компонентов ("сайдбары" - sidebars, "хлебные крошки" - breadcrumbs, "табы" - tabs и т.д.).

Тем не менее, обычно, мы хотим рендерить только один `<Route>`. Если мы находимся в `/about`, то едва ли мы хотим рендерить компонент `<User />` или страницу ошибки 404. Вот как добиться этого с помощью `<Switch>`:

```js
import { Route, Switch } from "react-router"

const routes = (
  <Switch>
    <Route exact path="/">
      <Home />
    </Route>
    <Route path="/about">
      <About />
    </Route>
    <Route path="/:user">
      <User />
    </Route>
    <Route>
      <NoMatch />
    </Route>
  </Switch>
)
```

Это также может быть полезным для выполнения анимированных переходов, поскольку новый маршрут рендерится на той же позиции, что и предыдущий.

#### Пропы

- `location`: object - используется для поиска совпадения вместо текущего объекта локации (текущего браузерного URL)
- `children`: node - потомки `<Switch>` должны быть элементами `<Route>` или `<Redirect>`. `<Route>` совпадает по пропу `path`, `<Redirect>` - по пропу `from`. Указанные элементы без соответствующих пропов всегда совпадают. При включении `<Redirect>` в `<Switch>`, в последнем могут использоваться все пропы `<Route>` (`path`, `exact` и `strict`). Проп `from` - это синоним пропа `path`. Если в `<Switch>` передан проп `location`, значение `location` совпавшего потомка будет перезаписано.

```js
import { Redirect, Route, Switch } from "react-router"

let routes = (
  <Switch>
    <Route exact path="/">
      <Home />
    </Route>

    <Route path="/users">
      <Users />
    </Route>
    <Redirect from="/accounts" to="/users" />

    <Route>
      <NoMatch />
    </Route>
  </Switch>
)
```
	
**[⬆ 254](#254)**

	
### Link <a name="link"></a>	

- [&lt;NavLink>](#nav)

Обеспечивает декларативный и доступный способ навигации в приложении.

```js
<Link to="/about">Контакты</Link>
```

#### Пропы

- `to`: string - строковое представление локации, создаваемое посредством объединения свойств "pathname", "search" и "hash"

```js
<Link to="/courses?sort=name" />
```
- `to`: object - объект, который может иметь следующие свойства:
  - `pathname`: string - название пути
  - `search`: string - параметры строки запроса
  - `hash`: string - хэш-часть URL
  - `state`: object - состояние локации

```js
<Link
  to={{
    pathname: "/courses",
    search: "?sort=name",
    hash: "#the-hash",
    state: { fromDashboard: true }
  }}
/>
```

- `to`: func - функция, которой в качестве аргумента передается текущая локация и которая должна вернуть представление локации в виде строки или объекта

```js
<Link to={location => ({ ...location, pathname: "/courses" })} />
<Link to={location => `${location.pathname}?sort=name`} />
```

- `replace`: bool - если `true`, тогда новая локация заменяет текущую в стеке истории, а не добавляется к ней

```js
<Link to="/courses" replace />
```

- `component`: React.Component - для реализации собственного компонента навигации достаточно передать данный проп

```js
const FancyLink = React.forwardRef((props, ref) => (
  <a ref={ref} {...props}>💅 {props.children}</a>
))

<Link to="/" component={FancyLink} />
```

- другие - `title`, `id`, `className` и т.д.

**[⬆ 254](#254)**	
	
	
### NavLink <a name="nav"></a>		

Специальная версия `<Link>`, предназначенная для добавления стилей к элементу, совпадающему с текущим URL (активному элементу).

```js
<NavLink to="/about">About</NavLink>
```

#### Пропы

- `activeClassName`: string - класс активного элемента. Значением по умолчанию является `active`. Объединяется с пропом `className`

```js
<NavLink to="/faq" activeClassName="selected">
  Часто задаваемые вопросы
</NavLink>
```

- `activeStyle`: object - стили, применяемые к активному элементу

```js
<NavLink
  to="/faq"
  activeStyle={{
    fontWeight: "bold",
    color: "red"
  }}
>
  Часто задаваемые вопросы
</NavLink>
```

- `exact`: bool - если `true`, тогда активный класс/стили применяются только при точном совпадении
- `strict`: bool - если `true`, тогда при определении совпадения учитывается замыкающий (последний) слэш
- `isActive`: func - дополнительная логика для определения активности ссылки

```js
<NavLink
  to="/events/123"
  isActive={(match, location) => {
    if (!match) {
      return false
    }

    // событие считается активным только при условии, что его идентификатор является нечетным числом
    const eventID = parseInt(match.params.eventID)
    return !isNaN(eventID) && eventID % 2 === 1
  }}
>
  Событие 123
</NavLink>
```

- `location`: object - используется для сравнения с другой локацией
- `aria-current`: string - значение атрибута `aria-current` активной ссылки. Возможные значения: `page` (значение по умолчанию), `step`, `location`, `date`, `time`, `true`, `false`.

**[⬆ 254](#254)**	
	

### Redirect <a name="redirect"></a>	

Рендеринг `<Redirect>` приводит к перемещению в новую локацию. Новая локация перезаписывает текущую в стеке истории, как при серверном перенаправлении (HTTP 3xx).

```js
<Route exact path="/">
  {loggedIn ? <Redirect to="/dashboard" /> : <PublicHomePage />}
</Route>
```

#### Пропы

- `to`: string - любой валидный URL
- `to`: object - объект локации для перенаправления

```js
<Redirect
  to={{
    pathname: "/login",
    search: "?utm=your+face",
    state: { referrer: currentLocation }
  }}
/>
```

В компоненте `Login` объект `state` доступен через `props.location.state`, а ключ `referrer` - через `props.state.referrer`.

- `push`: bool - если `true`, новая локация добавляется в стек истории, а не заменяет текущую
- `from`: string - любой валидный URL. Может использоваться только при включении в `<Switch>`

```js
<Switch>
  <Redirect from="/old-path" to="/new-path" />
  <Route path="/new-path">
    <Place />
  </Route>
</Switch>

// Перенаправление с совпавшими параметрами
<Switch>
  <Redirect from="/users/:id" to="/users/profile/:id" />
  <Route path="/users/profile/:id">
    <Profile />
  </Route>
</Switch>
```

- `exact`: bool - точное совпадение, аналог `Route.exact`. Может использоваться только совместно с `from`
- `strict`: bool - учет замыкающего слэша, аналог `Route.strict`. Может использоваться только совместно с `from`
- `sensitive`: bool - учет регистра, аналог `Route.sensitive`

**[⬆ 254](#254)**
    
  **[⬆ Наверх](#top)**
  
255. ### <a name="255"></a> react-router v6

```jsx harmony
import * as React from "react";
import { Routes, Route, Outlet, Link } from "react-router-dom";

export default function App() {
  return (
    <div>
      <h1>Basic Example</h1>

      <p>
        This example demonstrates some of the core features of React Router
        including nested <code>&lt;Route&gt;</code>s,{" "}
        <code>&lt;Outlet&gt;</code>s, <code>&lt;Link&gt;</code>s, and using a
        "*" route (aka "splat route") to render a "not found" page when someone
        visits an unrecognized URL.
      </p>

      {/* Routes nest inside one another. Nested route paths build upon
            parent route paths, and nested route elements render inside
            parent route elements. See the note about <Outlet> below. */}
      <Routes>
        <Route path="/" element={<Layout />}>
          <Route index element={<Home />} />
          <Route path="about" element={<About />} />
          <Route path="dashboard" element={<Dashboard />} />

          {/* Using path="*"" means "match anything", so this route
                acts like a catch-all for URLs that we don't have explicit
                routes for. */}
          <Route path="*" element={<NoMatch />} />
        </Route>
      </Routes>
    </div>
  );
}

function Layout() {
  return (
    <div>
      {/* A "layout route" is a good place to put markup you want to
          share across all the pages on your site, like navigation. */}
      <nav>
        <ul>
          <li>
            <Link to="/">Home</Link>
          </li>
          <li>
            <Link to="/about">About</Link>
          </li>
          <li>
            <Link to="/dashboard">Dashboard</Link>
          </li>
          <li>
            <Link to="/nothing-here">Nothing Here</Link>
          </li>
        </ul>
      </nav>

      <hr />

      {/* An <Outlet> renders whatever child route is currently active,
          so you can think about this <Outlet> as a placeholder for
          the child routes we defined above. */}
      <Outlet />
    </div>
  );
}

function Home() {
  return (
    <div>
      <h2>Home</h2>
    </div>
  );
}

function About() {
  return (
    <div>
      <h2>About</h2>
    </div>
  );
}

function Dashboard() {
  return (
    <div>
      <h2>Dashboard</h2>
    </div>
  );
}

function NoMatch() {
  return (
    <div>
      <h2>Nothing to see here!</h2>
      <p>
        <Link to="/">Go to the home page</Link>
      </p>
    </div>
  );
}  
```  
  
https://github.com/remix-run/react-router/blob/main/docs/upgrading/v5.md#upgrade-to-react-router-v6      
      
  **[⬆ Наверх](#top)**
  
256. ### <a name="256"></a> 

 
    
  **[⬆ Наверх](#top)**
  
257. ### <a name="257"></a> React / redux Dev Tools

React Developer Tools позволяют инспектировать иерархию компонентов, включая их состояние и пропы. Они существуют как в виде расширения для браузера (Chrome и Firefox), так и в виде самостоятельного приложения (работают с другими окружениями, такими как Safari, IE и React Native).

Вот некоторые из основных возможностей Redux DevTools:
	
1. Позволяют инспектировать каждое состояние и полезную нагрузку операции
2. Позволяют возвращаться назад, "отменяя" выполнение операций
3. При изменении кода редуктора осуществляется повторное вычисление каждой "зафиксированной" операции
4. Если редуктор выбросил исключение, вы сможете увидеть, в процессе выполнения какой операции это произошло, и в чем заключается ошибка
5. С помощью метода `persistState()` можно сохранить сессию отладки между перезагрузками страницы
    
  **[⬆ Наверх](#top)**
  
258. ### <a name="258"></a> HOC - Компонент высшего порядка

`Компонент высшего порядка` (Higher-Order Component, HOC) — это один из продвинутых способов для повторного использования логики. HOC не являются частью API React, но часто применяются из-за композиционной природы компонентов.

## Как создать компонент высшего порядка?

![Higher Order Components](./assets/img2/Higher-Order-Components.jpg)

Компонент высшего порядка (Higher Order Component, HOC) - это функция, принимающая компонент и возвращающая новый компонент. Это продвинутая техника, позволяющая повторно использовать логику компонента. `HOC` не являются частью `React API`. `HOC` является паттерном, производным от композиционной природы `React`. Компонент преобразует пропы в `UI`, а `HOC` трансформирует один компонент в другой. Примерами популярных `HOC` являются методы `connect` в `Redux` и `createContainer` в `Relay`.

```jsx
// HOC.js
import React, { Component } from 'react'

export default function Hoc(WrappedComponent) {
  return class extends Component {
    render() {
      return (
        <div>
          <WrappedComponent></WrappedComponent>
        </div>
      )
    }
  }
}
```

```jsx
// App.js
import React, { Component } from 'react'
import Hoc from './HOC'

class App extends Component {
  render() {
    return (
      <div>
        Компонента высшего порядка
      </div>
    )
  }
}

App = Hoc(App)

export default App
```

_Обратите внимание:_

- Мы не модифицируем компоненты, а создаем новые.
- `HOC` используются для композиции компонентов в целях обеспечения возможности повторного использования кода.
- `HOC` являются "чистыми" (pure) функциями. Они не имеют побочных эффектов (side effects) и всегда возвращают одинаковые результаты для одних и тех же аргументов.	    

	    
`Компонент высшего порядка` — это функция, которая принимает компонент и возвращает новый компонент.	    
	    
```jsx harmony
import {useState, useEffect} from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

const withSlider = (BaseComponent, getData) => {
    return (props) => {
        const [slide, setSlide] = useState(0);
        const [autoplay, setAutoplay] = useState(false)

        useEffect(() => {
            setSlide(getData);
        }, [])

        function changeSlide(i) {
            setSlide(slide => slide + i);
        }

        return <BaseComponent
                            {...props}
                            slide={slide}
                            autoplay={autoplay}
                            changeSlide={changeSlide}
                            setAutoplay={setAutoplay} />
    }
}

const getDataFromFirstFetch = () => {return 10};
const getDataFromSecondFetch = () => {return 20};

const SliderFirst = (props) => {

    return (
        <Container>
            <div className="slider w-50 m-auto">
                <img className="d-block w-100" src="https://www.planetware.com/wpimages/2020/02/france-in-pictures-beautiful-places-to-photograph-eiffel-tower.jpg" alt="slide" />
                <div className="text-center mt-5">Active slide {props.slide}</div>
                <div className="buttons mt-3">
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => props.changeSlide(-1)}>-1</button>
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => props.changeSlide(1)}>+1</button>
                </div>
            </div>
        </Container>
    )
}

const SliderSecond = (props) => {

    return (
        <Container>
            <div className="slider w-50 m-auto">
                <img className="d-block w-100" src="https://www.planetware.com/wpimages/2020/02/france-in-pictures-beautiful-places-to-photograph-eiffel-tower.jpg" alt="slide" />
                <div className="text-center mt-5">Active slide {props.slide} <br/>{props.autoplay ? 'auto' : null} </div>
                <div className="buttons mt-3">
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => props.changeSlide(-1)}>-1</button>
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => props.changeSlide(1)}>+1</button>
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => props.setAutoplay(autoplay => !props.autoplay)}>toggle autoplay</button>
                </div>
            </div>
        </Container>
    )
}

const SliderWithFirstFetch = withSlider(SliderFirst, getDataFromFirstFetch());
const SliderWithSecondFetch = withSlider(SliderSecond, getDataFromSecondFetch());

const withLogger = WrappedComponent => props => {
    useEffect(() => {
        console.log('first render!')
    }, [])

    return <WrappedComponent {...props} />
}

const Hello = () => {
    return (
      <h1>Hello!</h1>
    )
}

const HelloWithLogger = withLogger(Hello);

function App() {
    return (
        <>
            <HelloWithLogger />
            <SliderWithFirstFetch />
            <SliderWithSecondFetch />
        </>
    );
}

export default App;	    
```	    
 
### Пример с  документации
	    
```jsx harmony
class CommentList extends React.Component {
  constructor(props) {
    super(props);
    this.handleChange = this.handleChange.bind(this);
    this.state = {
      // "DataSource" -- произвольный глобальный источник данных
      comments: DataSource.getComments()
    };
  }

  componentDidMount() {
    // Подписаться на оповещения
    DataSource.addChangeListener(this.handleChange);
  }

  componentWillUnmount() {
    // Отписаться от оповещений
    DataSource.removeChangeListener(this.handleChange);
  }

  handleChange() {
    // Сохранить комментарии из внешнего источника в локальном состоянии
    this.setState({
      comments: DataSource.getComments()
    });
  }

  render() {
    return (
      <div>
        {this.state.comments.map((comment) => (
          <Comment comment={comment} key={comment.id} />
        ))}
      </div>
    );
  }
}
```	
	
Теперь мы решили реализовать новый компонент, который отслеживает изменения конкретной публикации и повторяет уже знакомый нам шаблон:
	
```jsx harmony
class BlogPost extends React.Component {
  constructor(props) {
    super(props);
    this.handleChange = this.handleChange.bind(this);
    this.state = {
      blogPost: DataSource.getBlogPost(props.id)
    };
  }

  componentDidMount() {
    DataSource.addChangeListener(this.handleChange);
  }

  componentWillUnmount() {
    DataSource.removeChangeListener(this.handleChange);
  }

  handleChange() {
    this.setState({
      blogPost: DataSource.getBlogPost(this.props.id)
    });
  }

  render() {
    return <TextBlock text={this.state.blogPost} />;
  }
}
```	
	
Разница между CommentList и BlogPost в том, что они вызывают разные методы DataSource и рендерят разный вывод. Однако в большинстве своём они похожи:

- Оба компонента подписываются на оповещения от DataSource при монтировании.
- Оба меняют внутреннее состояние при изменении DataSource.
- Оба отписываются от DataSource при размонтировании.
	
Можете представить, что в больших приложениях связка «подписаться на DataSource, затем вызвать setState» повторяется очень часто. Было бы здорово абстрагировать эту функциональность и использовать её в других компонентах.

Давайте реализуем функцию withSubscription — она будет создавать компоненты и подписывать их на обновления DataSource (наподобие CommentList и BlogPost). Функция будет принимать оборачиваемый компонент и через пропсы передавать ему новые данные:

```jsx harmony	
const CommentListWithSubscription = withSubscription(
  CommentList,
  (DataSource) => DataSource.getComments()
);

const BlogPostWithSubscription = withSubscription(
  BlogPost,
  (DataSource, props) => DataSource.getBlogPost(props.id)
);
```
	
Первый параметр — это оборачиваемый компонент. Второй — функция, которая извлекает нужные нам данные, она получает DataSource и текущие пропсы.

Когда CommentListWithSubscription и BlogPostWithSubscription рендерятся, они передают в CommentList и BlogPost обновлённые данные DataSource через проп data:

```jsx harmony	
// Эта функция принимает компонент...
function withSubscription(WrappedComponent, selectData) {
  // ...и возвращает другой компонент...
  return class extends React.Component {
    constructor(props) {
      super(props);
      this.handleChange = this.handleChange.bind(this);
      this.state = {
        data: selectData(DataSource, props)
      };
    }

    componentDidMount() {
      // ...который подписывается на оповещения...
      DataSource.addChangeListener(this.handleChange);
    }

    componentWillUnmount() {
      DataSource.removeChangeListener(this.handleChange);
    }

    handleChange() {
      this.setState({
        data: selectData(DataSource, this.props)
      });
    }

    render() {
      // ... и рендерит оборачиваемый компонент со свежими данными!
      // Обратите внимание, что мы передаём остальные пропсы
      return <WrappedComponent data={this.state.data} {...this.props} />;
    }
  };
}	    
```	    
	    
  **[⬆ Наверх](#top)**
  
259. ### <a name="259"></a> React Transition Group

https://github.com/harryheman/my-js/blob/master/docs/guide/react-transition-group.md	
	
http://reactcommunity.org/react-transition-group/	
	
```jsx harmony
import { useState } from 'react';
import { Container } from 'react-bootstrap';
import { CSSTransition } from 'react-transition-group';
import './App.css';

const Modal = (props) => {
  const duration = 300;

  // const defaultStyle = {
  //     transition: `all ${duration}ms ease-in-out`,
  //     opacity: 0,
  //     visibility: 'hidden'
  // }
  //
  // const transitionStyles = {
  //     entering: { opacity: 1, visibility: 'visible' },
  //     entered:  { opacity: 1, visibility: 'visible' },
  //     exiting:  { opacity: 0, visibility: 'hidden' },
  //     exited:  { opacity: 0, visibility: 'hidden' },
  // };

  return (
    <CSSTransition
      in={props.show}
      timeout={duration}
      onEnter={() => props.setShowTrigger(false)}
      onExited={() => props.setShowTrigger(true)}
      classNames='modal'
      mountOnEnter
      unmountOnExit
    >
      <div className='modal mt-5 d-block'>
        <div className='modal-dialog'>
          <div className='modal-content'>
            <div className='modal-header'>
              <h5 className='modal-title'>Typical modal window</h5>
              <button
                onClick={() => props.onClose(false)}
                type='button'
                className='btn-close'
                aria-label='Close'
              ></button>
            </div>
            <div className='modal-body'>
              <p>Modal body content</p>
            </div>
            <div className='modal-footer'>
              <button
                onClick={() => props.onClose(false)}
                type='button'
                className='btn btn-secondary'
              >
                Close
              </button>
              <button
                onClick={() => props.onClose(false)}
                type='button'
                className='btn btn-primary'
              >
                Save changes
              </button>
            </div>
          </div>
        </div>
      </div>
    </CSSTransition>
  );
};

function App() {
  const [showModal, setShowModal] = useState(false);
  const [showTrigger, setShowTrigger] = useState(true);

  return (
    <Container>
      <Modal
        show={showModal}
        onClose={setShowModal}
        setShowTrigger={setShowTrigger}
      />
      {showTrigger ? (
        <button
          type='button'
          className='btn btn-warning mt-5'
          onClick={() => setShowModal(true)}
        >
          Open Modal
        </button>
      ) : null}
    </Container>
  );
}

export default App;	
```	
    
  **[⬆ Наверх](#top)**
	
260. ### <a name="260"></a> Formik, Yup - работа с формами

### хук useFormik	
```jsx harmony
import {useFormik} from 'formik';
import * as Yup from 'yup';

const Form = () => {

	const formik = useFormik({
		initialValues: {
			name: '',
			email: '',
			amount: 0,
			currency: '',
			text: '',
			terms: false
		},
		validationSchema: Yup.object({
			name: Yup.string()
				.min(2, 'Минимум 2 символа')
				.required('Обязательное поле'),
			email: Yup.string()
				.email('Неправильный email адрес')
				.required('Обязательное поле'),
			amount: Yup.number()
				.min(5, 'Не менее 5')
				.required('Обязательное поле'),
			currency: Yup.string().required('Выберите валюту'),
			text: Yup.string()
				.min(10, 'Не менее 10 символов'),
			terms: Yup.boolean()
				.required('Необходимо согласие!')
				.oneOf([true], 'Необходимо согласие!')
		}),
		onSubmit: values => console.log(JSON.stringify(values, null, 2))
	})

	return (
		<form className="form" onSubmit={formik.handleSubmit}>
			<h2>Отправить пожертвование</h2>
			<label htmlFor="name">Ваше имя</label>
			<input
				id="name"
				name="name"
				type="text"
				value={formik.values.name}
				onChange={formik.handleChange}
				onBlur={formik.handleBlur}
			/>
			{formik.errors.name && formik.touched.name ? <div className='error'>{formik.errors.name}</div> : null}
			<label htmlFor="email">Ваша почта</label>
			<input
				id="email"
				name="email"
				type="email"
				value={formik.values.email}
				onChange={formik.handleChange}
				onBlur={formik.handleBlur}
			/>
			{formik.errors.email && formik.touched.email ? <div className='error'>{formik.errors.email}</div> : null}
			<label htmlFor="amount">Количество</label>
			<input
				id="amount"
				name="amount"
				type="number"
				value={formik.values.amount}
				onChange={formik.handleChange}
				onBlur={formik.handleBlur}
			/>
			{formik.errors.amount && formik.touched.amount ? <div className='error'>{formik.errors.amount}</div> : null}
			<label htmlFor="currency">Валюта</label>
			<select
				id="currency"
				name="currency"
				value={formik.values.currency}
				onChange={formik.handleChange}
				onBlur={formik.handleBlur}>
				<option value="">Выберите валюту</option>
				<option value="USD">USD</option>
				<option value="UAH">UAH</option>
				<option value="RUB">RUB</option>
			</select>
			{formik.errors.currency && formik.touched.currency ? <div className='error'>{formik.errors.currency}</div> : null}
			<label htmlFor="text">Ваше сообщение</label>
			<textarea
				id="text"
				name="text"
				value={formik.values.text}
				onChange={formik.handleChange}
				onBlur={formik.handleBlur}
			/>
			{formik.errors.text && formik.touched.text ? <div className='error'>{formik.errors.text}</div> : null}
			<label className="checkbox">
				<input
					name="terms"
					type="checkbox"
					value={formik.values.terms}
					onChange={formik.handleChange}
					onBlur={formik.handleBlur}
				/>
				Соглашаетесь с политикой конфиденциальности?
			</label>
			{formik.errors.terms && formik.touched.terms ? <div className='error'>{formik.errors.terms}</div> : null}
			<button type="submit">Отправить</button>
		</form>
	)
}

export default Form;	
```	

### Formik, Form, Field, ErrorMessage
```jsx harmony
import { Formik, Form, Field, ErrorMessage } from 'formik';
import * as Yup from 'yup';

const CustomForm = () => {

	return (
		<Formik
			initialValues = {{
				name: '',
				email: '',
				amount: 0,
				currency: '',
				text: '',
				terms: false
			}}
			validationSchema = {Yup.object({
				name: Yup.string()
					.min(2, 'Минимум 2 символа')
					.required('Обязательное поле'),
				email: Yup.string()
					.email('Неправильный email адрес')
					.required('Обязательное поле'),
				amount: Yup.number()
					.min(5, 'Не менее 5')
					.required('Обязательное поле'),
				currency: Yup.string().required('Выберите валюту'),
				text: Yup.string()
					.min(10, 'Не менее 10 символов'),
				terms: Yup.boolean()
					.required('Необходимо согласие!')
					.oneOf([true], 'Необходимо согласие!')
			})}
			onSubmit = {values => console.log(JSON.stringify(values, null, 2))}
		>
			<Form className="form">
				<h2>Отправить пожертвование</h2>
				<label htmlFor="name">Ваше имя</label>
				<Field
					id="name"
					name="name"
					type="text"
				/>
				<ErrorMessage className='error' name='name' component='div' />
				<label htmlFor="email">Ваша почта</label>
				<Field
					id="email"
					name="email"
					type="email"
				/>
				<ErrorMessage className='error' name='email' component='div' />
				<label htmlFor="amount">Количество</label>
				<Field
					id="amount"
					name="amount"
					type="number"
				/>
				<ErrorMessage className='error' name='amount' component='div' />
				<label htmlFor="currency">Валюта</label>
				<Field
					id="currency"
					name="currency"
					as='select'>
					<option value="">Выберите валюту</option>
					<option value="USD">USD</option>
					<option value="UAH">UAH</option>
					<option value="RUB">RUB</option>
				</Field>
				<ErrorMessage className='error' name='currency' component='div' />
				<label htmlFor="text">Ваше сообщение</label>
				<Field
					id="text"
					name="text"
					as='textarea'
				/>
				<ErrorMessage className='error' name='text' component='div' />
				<label className="checkbox">
					<Field
						name="terms"
						type="checkbox"
					/>
					Соглашаетесь с политикой конфиденциальности?
				</label>
				<ErrorMessage className='error' name='terms' component='div' />
				<button type="submit">Отправить</button>
			</Form>
		</Formik>
	)
}

export default CustomForm;	
```	

### useField
```jsx harmony
import { Formik, Form, Field, ErrorMessage, useField } from 'formik';
import * as Yup from 'yup';

const MyTextInput = ({label, ...props}) => {
	const [field, meta] = useField(props);

	return (
		<>
			<label htmlFor={props.name}>{label}</label>
			<input {...props} {...field} />
			{meta.touched && meta.error ? (
				<div className='error'>{meta.error}</div>
			) : null}
		</>
	)
};

const MyCheckbox = ({children, ...props}) => {
	const [field, meta] = useField({...props, type: 'checkbox'});

	return (
		<>
			<label className='checkbox'>
				<input type='checkbox' {...props} {...field} />
				{children}
			</label>

			{meta.touched && meta.error ? (
				<div className='error'>{meta.error}</div>
			) : null}
		</>
	)
};

const CustomForm = () => {

	return (
		<Formik
			initialValues = {{
				name: '',
				email: '',
				amount: 0,
				currency: '',
				text: '',
				terms: false
			}}
			validationSchema = {Yup.object({
		name: Yup.string()
			.min(2, 'Минимум 2 символа')
			.required('Обязательное поле'),
			email: Yup.string()
			.email('Неправильный email адрес')
			.required('Обязательное поле'),
			amount: Yup.number()
			.min(5, 'Не менее 5')
			.required('Обязательное поле'),
			currency: Yup.string().required('Выберите валюту'),
			text: Yup.string()
			.min(10, 'Не менее 10 символов'),
			terms: Yup.boolean()
			.required('Необходимо согласие!')
			.oneOf([true], 'Необходимо согласие!')
	})}
			onSubmit = {values => console.log(JSON.stringify(values, null, 2))}
		>
			<Form className="form">
				<h2>Отправить пожертвование</h2>				
				<MyTextInput
					label='Ваше имя'
					id="name"
					name="name"
					type="text"
				/>
				<MyTextInput
					label='Ваша почта'
					id="email"
					name="email"
					type="email"
				/>
				<label htmlFor="amount">Количество</label>
				<Field
					id="amount"
					name="amount"
					type="number"
				/>
				<ErrorMessage className='error' name='amount' component='div' />
				<label htmlFor="currency">Валюта</label>
				<Field
					id="currency"
					name="currency"
					as='select'>
					<option value="">Выберите валюту</option>
					<option value="USD">USD</option>
					<option value="UAH">UAH</option>
					<option value="RUB">RUB</option>
				</Field>
				<ErrorMessage className='error' name='currency' component='div' />
				<label htmlFor="text">Ваше сообщение</label>
				<Field
					id="text"
					name="text"
					as='textarea'
				/>
				<ErrorMessage className='error' name='text' component='div' />
				<MyCheckbox
					name='terms'>
					Соглашаетесь с политикой конфиденциальности?
				</MyCheckbox>
				<button type="submit">Отправить</button>
			</Form>
		</Formik>
	)
}

export default CustomForm;	
```	

### Валидация без Yup
```jsx harmony
const validate = values => {
	const errors = {};

	if (!values.name) {
		errors.name = 'Обязательное поле!';
	} else if (values.name.length < 2) {
		errors.name = 'Миниммум 2 символа';
	}

	if (values.email) {
		errors.email = 'Обязательное поле!';
	} else if (!/^[A-Z0-9._%+-]+@[A-Z0-9.-]+\.[A-Z]{2,}$/i.test(values.email)
	) {
		errors.email = 'Неправильный email адрес'
	}

	return errors;
}	
```	
	
  **[⬆ Наверх](#top)**
	
261. ### <a name="261"></a> 

 
    
  **[⬆ Наверх](#top)**	
  
300. ### <a name="300"></a> Хуки в React

 `Хуки` — это функции, с помощью которых вы можете «подцепиться» к состоянию и методам жизненного цикла React из функциональных компонентов. Хуки не работают внутри классов — они дают вам возможность использовать React без классов.
	
```jsx harmony
import React, { useState } from 'react';

function Example() {
  // Объявление переменной состояния, которую мы назовём "count"
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>Вы кликнули {count} раз</p>
      <button onClick={() => setCount(count + 1)}>
        Нажми на меня
      </button>
    </div>
  );
}
```	

### Преимущества хуков	
- Хуки дают новый мощный способ повторного использования кода в компонентах.	
- Хуки позволяют нам организовать логику внутри компонента в многоразовые изолированные блоки
- С помощью хуков написание кода намного проще, и я считаю, что чтение функциональных компонентов с помощью хуков требует меньшего переключения контекста, поскольку ты не прыгаешь по файлу, чтобы определить, в каком методе жизненного цикла, по твоему мнению, что-то произошло.
- Хуки позволяют вам повторно использовать логику состояния, не затрагивая дерево компонентов
- Хуки позволяют разбить один компонент на маленькие функции по их назначению (например, подписке или загрузке данных)	
- Хуки позволяют использовать больше возможностей React без написания классов
    
  **[⬆ Наверх](#top)**
	
301. ### <a name="301"></a> Методы жизненного цикла может заменить Хуки

 ### Как методы жизненного цикла соответствуют хукам?	
- constructor: Функциональному компоненту не нужен конструктор. Вы можете инициализировать состояние, используя вызов useState. Если вычисления состояния затратны, вы можете передать функцию в useState.
- getDerivedStateFromProps: Запланировать обновление при рендере.
- shouldComponentUpdate: Смотрите объяснение React.memo ниже.
- render: Это тело функционального компонента.
- componentDidMount, componentDidUpdate, componentWillUnmount: Хук useEffect заменяет все их комбинации (включая более редкие случаи).
- getSnapshotBeforeUpdate, componentDidCatch и getDerivedStateFromError: В данный момент не существует хуков-аналогов для этих методов, но они будут скоро добавлены.
    
  **[⬆ Наверх](#top)**
	
302. ### <a name="302"></a> Хуки

 `Хуки` — это функции, с помощью которых вы можете «подцепиться» к состоянию и методам жизненного цикла React из функциональных компонентов. Хуки не работают внутри классов — они дают вам возможность использовать React без классов.	
	
`Хуки` — нововведение в React 16.8, которое позволяет использовать состояние и другие возможности React без написания классов.	
	
- [useState](#useState)
- [useEffect](#useEffect)	
- [useContext](#useContext)	
- [useReducer](#useReducer)	
- [useCallback](#useCallback)	
- [useMemo](#useMemo)	
- [useRef](#useRef)
- [useImperativeHandle](#useImperativeHandle)
- [useLayoutEffect](#useLayoutEffect)
- [useDebugValue](#useDebugValue)
- [useDeferredValue](#useDeferredValue)
- [useTransition](#useTransition)	
- [useId](#useId)	
	
### useState <a name="useState"></a>
	
```jsx harmony	
const [state, setState] = useState(initialState);
```	
Возвращает значение с состоянием и функцию для его обновления.

Во время первоначального рендеринга возвращаемое состояние (state) совпадает со значением, переданным в качестве первого аргумента (initialState).

Функция setState используется для обновления состояния. Она принимает новое значение состояния и ставит в очередь повторный рендер компонента.
```jsx harmony
setState(newState);
```	
Во время последующих повторных рендеров первое значение, возвращаемое useState, всегда будет самым последним состоянием после применения обновлений.

`Функциональные обновления`
	
Если новое состояние вычисляется с использованием предыдущего состояния, вы можете передать функцию в setState. Функция получит предыдущее значение и вернёт обновлённое значение. Вот пример компонента счётчик, который использует обе формы setState:
```jsx harmony
function Counter({initialCount}) {
  const [count, setCount] = useState(initialCount);
  return (
    <>
      Счёт: {count}
      <button onClick={() => setCount(initialCount)}>Сбросить</button>
      <button onClick={() => setCount(prevCount => prevCount - 1)}>-</button>
      <button onClick={() => setCount(prevCount => prevCount + 1)}>+</button>
    </>
  );
}
```	
Кнопки «+» и «-» используют функциональную форму, потому что обновлённое значение основано на предыдущем значении. Но кнопка «Сбросить» использует обычную форму, потому что она всегда устанавливает счётчик обратно в 0.

	
### Пример
	
```jsx harmony
import React, {useState} from 'react'

function computeInitialCounter() {
  console.log('Some calculations...')
  return Math.trunc(Math.random() * 20)
}

function App() {
  // const [counter, setCounter] = useState(0)
  // const [counter, setCounter] = useState(computeInitialCounter())
  const [counter, setCounter] = useState(() => {
    return computeInitialCounter()
  })

  const [state, setState] = useState({
    title: 'Счетчик',
    date: Date.now()
  })

  function increment() {
    // setCounter(counter + 1)
    // setCounter(counter + 1)
    setCounter((prevCounter) => {
      return prevCounter + 1
    })
    // setCounter(prev => prev + 1)
  }

  function decrement() {
    setCounter(counter - 1)
  }

  function updateTitle() {
    setState(prev => {
      return {
        ...prev,
        title: 'Новое название'
      }
    })
  }

  return (
    <div>
      <h1>Счетчик: {counter}</h1>
      <button onClick={increment} className="btn btn-success">Добавить</button>
      <button onClick={decrement} className="btn btn-danger">Убрать</button>
      <button onClick={updateTitle} className="btn btn-default">Изменить название</button>

      <pre>{JSON.stringify(state, null, 2)}</pre>
    </div>
  )
}

export default App	
```	
	
	
**[⬆ 302](#302)**
	
	
### useEffect <a name="useEffect"></a>	
	
```jsx harmony	
useEffect(didUpdate);
```	
Принимает функцию, которая содержит императивный код, возможно, с эффектами.

Мутации, подписки, таймеры, логирование и другие побочные эффекты не допускаются внутри основного тела функционального компонента (называемого этапом рендеринга React). Это приведёт к запутанным ошибкам и несоответствиям в пользовательском интерфейсе.

Вместо этого используйте useEffect. Функция, переданная в useEffect, будет запущена после того, как рендер будет зафиксирован на экране. Думайте об эффектах как о лазейке из чисто функционального мира React в мир императивов.

По умолчанию эффекты запускаются после каждого завершённого рендеринга, но вы можете решить запускать их только при изменении определённых значений.

`Очистка эффекта`
	
Часто эффекты создают ресурсы, которые необходимо очистить (или сбросить) перед тем, как компонент покидает экран, например подписку или идентификатор таймера. Чтобы сделать это, функция переданная в useEffect, может вернуть функцию очистки. Например, чтобы создать подписку:
```jsx harmony
useEffect(() => {
  const subscription = props.source.subscribe();
  return () => {
    // Очистить подписку
    subscription.unsubscribe();
  };
});
```	
Функция очистки запускается до удаления компонента из пользовательского интерфейса, чтобы предотвратить утечки памяти. Кроме того, если компонент рендерится несколько раз (как обычно происходит), предыдущий эффект очищается перед выполнением следующего эффекта. В нашем примере это означает, что новая подписка создаётся при каждом обновлении. Чтобы избежать воздействия на каждое обновление, обратитесь к следующему разделу.

`Порядок срабатывания эффектов`
	
В отличие от componentDidMount и componentDidUpdate, функция, переданная в useEffect, запускается во время отложенного события после разметки и отрисовки. Это делает хук подходящим для многих распространённых побочных эффектов, таких как настройка подписок и обработчиков событий, потому что большинство типов работы не должны блокировать обновление экрана браузером.

Однако не все эффекты могут быть отложены. Например, изменение DOM, которое видно пользователю, должно запускаться синхронно до следующей отрисовки, чтобы пользователь не замечал визуального несоответствия. (Различие концептуально схоже с пассивным и активным слушателями событий.) Для этих типов эффектов React предоставляет один дополнительный хук, называемый useLayoutEffect. Он имеет ту же сигнатуру, что и useEffect, и отличается только в его запуске.

Хотя useEffect откладывается до тех пор, пока браузер не выполнит отрисовку, он гарантированно срабатывает перед любыми новыми рендерами. React всегда полностью применяет эффекты предыдущего рендера перед началом нового обновления.

`Условное срабатывание эффекта`
	
По умолчанию эффекты запускаются после каждого завершённого рендера. Таким образом, эффект всегда пересоздаётся, если значение какой-то из зависимости изменилось.

Однако в некоторых случаях это может быть излишним, например, в примере подписки из предыдущего раздела. Нам не нужно создавать новую подписку на каждое обновление, а только если изменился проп source.

Чтобы реализовать это, передайте второй аргумент в useEffect, который является массивом значений, от которых зависит эффект. Наш обновлённый пример теперь выглядит так:
```jsx harmony
useEffect(
  () => {
    const subscription = props.source.subscribe();
    return () => {
      subscription.unsubscribe();
    };
  },
  [props.source],
);	
```

```jsx harmony
import React, { useState, useEffect } from 'react';

function FriendStatus(props) {
  const [isOnline, setIsOnline] = useState(null);

  useEffect(() => {
    function handleStatusChange(status) {
      setIsOnline(status.isOnline);
    }
    ChatAPI.subscribeToFriendStatus(props.friend.id, handleStatusChange);
    // Указываем, как сбросить этот эффект:
    return function cleanup() {
      ChatAPI.unsubscribeFromFriendStatus(props.friend.id, handleStatusChange);
    };
  });

  if (isOnline === null) {
    return 'Загрузка...';
  }
  return isOnline ? 'В сети' : 'Не в сети';
}	
```
	
### Пример
	
```jsx harmony
import React, {useState, useEffect} from 'react'

function App() {
  const [type, setType] = useState('users')
  const [data, setData] = useState([])
  const [pos, setPos] = useState({
    x: 0, y: 0
  })

  // useEffect(() => {
  //   console.log('render')
  // })

  useEffect(() => {
    fetch(`https://jsonplaceholder.typicode.com/${type}`)
      .then(response => response.json())
      .then(json => setData(json))

    return () => {
      console.log('clean type')
    }
  }, [type])

  const mouseMoveHandler = event => {
    setPos({
      x: event.clientX,
      y: event.clientY
    })
  }

  useEffect(() => {
    console.log('ComponentDidMount')

    window.addEventListener('mousemove', mouseMoveHandler)

    return () => {
      window.removeEventListener('mousemove', mouseMoveHandler)
    }
  }, [])

  return (
    <div>
      <h1>Ресурс: {type}</h1>

      <button onClick={() => setType('users')}>Пользователи</button>
      <button onClick={() => setType('todos')}>Todos</button>
      <button onClick={() => setType('posts')}>Посты</button>

      {/*<pre>{JSON.stringify(data, null, 2)}</pre>*/}
      <pre>{JSON.stringify(pos, null, 2)}</pre>
    </div>
  )
}

export default App	
```	
	
	
**[⬆ 302](#302)**
	
	
### useContext <a name="useContext"></a>	
	
```jsx harmony	
const value = useContext(MyContext);
```	
Принимает объект контекста (значение, возвращённое из React.createContext) и возвращает текущее значение контекста для этого контекста. Текущее значение контекста определяется пропом value ближайшего <MyContext.Provider> над вызывающим компонентом в дереве.

Когда ближайший <MyContext.Provider> над компонентом обновляется, этот хук вызовет повторный рендер с последним значением контекста, переданным этому провайдеру MyContext. Даже если родительский компонент использует React.memo или реализует shouldComponentUpdate, то повторный рендер будет выполняться, начиная c компонента, использующего useContext.

Запомните, аргументом для useContext должен быть непосредственно сам объект контекста:

- Правильно: useContext(MyContext)
- Неправильно: useContext(MyContext.Consumer)
- Неправильно: useContext(MyContext.Provider)
	
Компонент, вызывающий useContext, всегда будет перерендериваться при изменении значения контекста. Если повторный рендер компонента затратен, вы можете оптимизировать его с помощью мемоизации.

useContext(MyContext) позволяет только читать контекст и подписываться на его изменения. Вам всё ещё нужен <MyContext.Provider> выше в дереве, чтобы предоставить значение для этого контекста.

`Соединим все вместе с Context.Provider`
```jsx harmony
const themes = {
  light: {
    foreground: "#000000",
    background: "#eeeeee"
  },
  dark: {
    foreground: "#ffffff",
    background: "#222222"
  }
};

const ThemeContext = React.createContext(themes.light);

function App() {
  return (
    <ThemeContext.Provider value={themes.dark}>
      <Toolbar />
    </ThemeContext.Provider>
  );
}

function Toolbar(props) {
  return (
    <div>
      <ThemedButton />
    </div>
  );
}

function ThemedButton() {
  const theme = useContext(ThemeContext);
  return (
    <button style={{ background: theme.background, color: theme.foreground }}>
      Я стилизован темой из контекста!
    </button>
  );
}	
```

**[⬆ 302](#302)**
	
	
### useReducer <a name="useReducer"></a>	
	
```jsx harmony	
const [state, dispatch] = useReducer(reducer, initialArg, init);
```	
Альтернатива для useState. Принимает редюсер типа (state, action) => newState и возвращает текущее состояние в паре с методом dispatch. (Если вы знакомы с Redux, вы уже знаете, как это работает.)

Хук useReducer обычно предпочтительнее useState, когда у вас сложная логика состояния, которая включает в себя несколько значений, или когда следующее состояние зависит от предыдущего. useReducer также позволяет оптимизировать производительность компонентов, которые запускают глубокие обновления, поскольку вы можете передавать dispatch вместо колбэков.

Вот пример счётчика из раздела useState, переписанный для использования редюсера:
```jsx harmony
const initialState = {count: 0};

function reducer(state, action) {
  switch (action.type) {
    case 'increment':
      return {count: state.count + 1};
    case 'decrement':
      return {count: state.count - 1};
    default:
      throw new Error();
  }
}

function Counter() {
  const [state, dispatch] = useReducer(reducer, initialState);
  return (
    <>
      Count: {state.count}
      <button onClick={() => dispatch({type: 'decrement'})}>-</button>
      <button onClick={() => dispatch({type: 'increment'})}>+</button>
    </>
  );
}
```	

`Указание начального состояния`
	
Существует два разных способа инициализации состояния useReducer. Вы можете выбрать любой из них в зависимости от ситуации. Самый простой способ — передать начальное состояние в качестве второго аргумента:
```jsx harmony
  const [state, dispatch] = useReducer(
    reducer,
    {count: initialCount}
  );
```	

`Ленивая инициализация`
Вы также можете создать начальное состояние лениво. Для этого вы можете передать функцию init в качестве третьего аргумента. Начальное состояние будет установлено равным результату вызова init(initialArg).

Это позволяет извлечь логику для расчёта начального состояния за пределы редюсера. Это также удобно для сброса состояния позже в ответ на действие:
```jsx harmony
function init(initialCount) {
  return {count: initialCount};
}

function reducer(state, action) {
  switch (action.type) {
    case 'increment':
      return {count: state.count + 1};
    case 'decrement':
      return {count: state.count - 1};
    case 'reset':
      return init(action.payload);
    default:
      throw new Error();
  }
}

function Counter({initialCount}) {
  const [state, dispatch] = useReducer(reducer, initialCount, init);
  return (
    <>
      Count: {state.count}
      <button
        onClick={() => dispatch({type: 'reset', payload: initialCount})}>
        Reset
      </button>
      <button onClick={() => dispatch({type: 'decrement'})}>-</button>
      <button onClick={() => dispatch({type: 'increment'})}>+</button>
    </>
  );
}
```	

**[⬆ 302](#302)**
	
	
### useCallback <a name="useCallback"></a>	
	
```jsx harmony	
const memoizedCallback = useCallback(
  () => {
    doSomething(a, b);
  },
  [a, b],
);
```	
Возвращает мемоизированный колбэк.

Передайте встроенный колбэк и массив зависимостей. Хук useCallback вернёт мемоизированную версию колбэка, который изменяется только, если изменяются значения одной из зависимостей. Это полезно при передаче колбэков оптимизированным дочерним компонентам, которые полагаются на равенство ссылок для предотвращения ненужных рендеров (например, shouldComponentUpdate).

useCallback(fn, deps) — это эквивалент useMemo(() => fn, deps).

### Пример
	
```jsx harmony
import React, {useState, useCallback} from 'react'
import ItemsList from './ItemsList'

function App() {
  const [colored, setColored] = useState(false)
  const [count, setCount] = useState(1)

  const styles = {
    color: colored ? 'darkred' : 'black'
  }

  const generateItemsFromAPI = useCallback((indexNumber) => {
    return new Array(count).fill('').map((_, i) => `Элемент ${i + indexNumber}`)
  }, [count])

  return (
    <>
      <h1 style={styles}>Количество элементов: {count}</h1>
      <button className={'btn btn-success'} onClick={() => setCount(prev => prev + 1)}>Добавить</button>
      <button className={'btn btn-warning'} onClick={() => setColored(prev => !prev)}>Изменить</button>

      <ItemsList getItems={generateItemsFromAPI} />
    </>
  )
}

export default App	
```	
	
	
**[⬆ 302](#302)**
	
	
### useMemo <a name="useMemo"></a>	

```jsx harmony	
const memoizedValue = useMemo(() => computeExpensiveValue(a, b), [a, b]);
```	
Возвращает мемоизированное значение.

Передайте «создающую» функцию и массив зависимостей. useMemo будет повторно вычислять мемоизированное значение только тогда, когда значение какой-либо из зависимостей изменилось. Эта оптимизация помогает избежать дорогостоящих вычислений при каждом рендере.

Помните, что функция, переданная useMemo, запускается во время рендеринга. Не делайте там ничего, что вы обычно не делаете во время рендеринга. Например, побочные эффекты принадлежат useEffect, а не useMemo.

Если массив не был передан, новое значение будет вычисляться при каждом рендере.

Вы можете использовать useMemo как оптимизацию производительности, а не как семантическую гарантию. В будущем React может решить «забыть» некоторые ранее мемоизированные значения и пересчитать их при следующем рендере, например, чтобы освободить память для компонентов вне области видимости экрана. Напишите свой код, чтобы он по-прежнему работал без useMemo, а затем добавьте его для оптимизации производительности.	

### Пример
	
```jsx harmony
import React, {useState, useMemo, useEffect} from 'react'

function complexCompute(num) {
  console.log('complexCompute')
  let i = 0
  while (i < 1000000000) i++
  return num * 2
}

function App() {
  const [number, setNumber] = useState(42)
  const [colored, setColored] = useState(false)

  const styles = useMemo(() => ({
    color: colored ? 'darkred' : 'black'
  }), [colored])

  const computed = useMemo(() => {
    return complexCompute(number)
  }, [number])

  useEffect(() => {
    console.log('Styles changed')
  }, [styles])

  return (
    <>
      <h1 style={styles}>Вычисляемое свойство: {computed}</h1>
      <button className={'btn btn-success'} onClick={() => setNumber(prev => prev + 1)}>Добавить</button>
      <button className={'btn btn-danger'} onClick={() => setNumber(prev => prev - 1)}>Убрать</button>
      <button className={'btn btn-warning'} onClick={() => setColored(prev => !prev)}>Изменить</button>
    </>
  )
}

export default App	
```		
	
**[⬆ 302](#302)**
	
	
### useRef <a name="useRef"></a>
	
```jsx harmony	
const refContainer = useRef(initialValue);
```	
useRef возвращает изменяемый ref-объект, свойство .current которого инициализируется переданным аргументом (initialValue). Возвращённый объект будет сохраняться в течение всего времени жизни компонента.

Обычный случай использования — это доступ к потомку в императивном стиле:
```jsx harmony
function TextInputWithFocusButton() {
  const inputEl = useRef(null);
  const onButtonClick = () => {
    // `current` указывает на смонтированный элемент `input`
    inputEl.current.focus();
  };
  return (
    <>
      <input ref={inputEl} type="text" />
      <button onClick={onButtonClick}>Установить фокус на поле ввода</button>
    </>
  );
}
```	
По сути, useRef похож на «коробку», которая может содержать изменяемое значение в своём свойстве .current.

Возможно, вы знакомы с рефами в основном как со способом получить доступ к DOM. Если вы передадите React объект рефа с помощью подобного выражения <div ref={myRef}/>, React установит собственное свойство .current на соответствующий DOM-узел при каждом его изменении.

Но хук useRef() полезен не только установкой атрибута с рефом. Он удобен для сохранения любого мутируемого значения, по аналогии с тем, как вы используете поля экземпляра в классах.

Это возможно, поскольку useRef() создаёт обычный JavaScript-объект. Единственная разница между useRef() и просто созданием самого объекта {current: ...} — это то, что хук useRef даст один и тот же объект с рефом при каждом рендере.

Имейте в виду, что useRef не уведомляет вас, когда изменяется его содержимое. Мутирование свойства .current не вызывает повторный рендер. Если вы хотите запустить некоторый код, когда React присоединяет или отсоединяет реф к узлу DOM, вы можете использовать колбэк-реф вместо этого.

	
### Пример
	
```jsx harmony
import React, {useState, useEffect, useRef} from 'react'

function App() {
  // const [renderCount, setRenderCount] = useState(1)
  const [value, setValue] = useState('initial')
  const renderCount = useRef(1)
  const inputRef = useRef(null)
  const prevValue = useRef('')

  useEffect(() => {
    renderCount.current++
  })

  useEffect(() => {
    prevValue.current = value
  }, [value])

  const focus = () => inputRef.current.focus()

  return (
    <div>
      <h1>Количество рендеров: {renderCount.current}</h1>
      <h2>Прошлое состояние: {prevValue.current}</h2>
      <input ref={inputRef} type="text" onChange={e => setValue(e.target.value)} value={value} />
      <button className="btn btn-success" onClick={focus}>Фокус</button>
    </div>
  )
}

export default App	
```	
	
	
**[⬆ 302](#302)**
	

### useImperativeHandle <a name="useImperativeHandle"></a>
	
```jsx harmony	
useImperativeHandle(ref, createHandle, [deps])
```	
useImperativeHandle настраивает значение экземпляра, которое предоставляется родительским компонентам при использовании ref. Как всегда, в большинстве случаев следует избегать императивного кода, использующего ссылки. useImperativeHandle должен использоваться с forwardRef:
```jsx harmony
function FancyInput(props, ref) {
  const inputRef = useRef();
  useImperativeHandle(ref, () => ({
    focus: () => {
      inputRef.current.focus();
    }
  }));
  return <input ref={inputRef} ... />;
}
FancyInput = forwardRef(FancyInput);
```	
В этом примере родительский компонент, который отображает <FancyInput ref={inputRef} />, сможет вызывать inputRef.current.focus().

**[⬆ 302](#302)**
	
	
### useLayoutEffect <a name="useLayoutEffect"></a>
	
Сигнатура идентична useEffect, но этот хук запускается синхронно после всех изменений DOM. Используйте его для чтения макета из DOM и синхронного повторного рендеринга. Обновления, запланированные внутри useLayoutEffect, будут полностью применены синхронно перед тем, как браузер получит шанс осуществить отрисовку.

Предпочитайте стандартный useEffect, когда это возможно, чтобы избежать блокировки визуальных обновлений.	

**[⬆ 302](#302)**
	

### useDebugValue <a name="useDebugValue"></a>	
```jsx harmony	
useDebugValue(value)
```	
useDebugValue может использоваться для отображения метки для пользовательских хуков в React DevTools.

Например, рассмотрим пользовательский хук useFriendStatus, описанный в разделе «Создание собственных хуков»:
```jsx harmony
function useFriendStatus(friendID) {
  const [isOnline, setIsOnline] = useState(null);

  // ...

  // Показывать ярлык в DevTools рядом с этим хуком
  // например, «Статус друга: В сети»
  useDebugValue(isOnline ? 'В сети' : 'Не в сети');

  return isOnline;
}	
```
**[⬆ 302](#302)**
	
	
### useDeferredValue <a name="useDeferredValue"></a>
	
```jsx harmony	
const deferredValue = useDeferredValue(value);
```	
useDeferredValue accepts a value and returns a new copy of the value that will defer to more urgent updates. If the current render is the result of an urgent update, like user input, React will return the previous value and then render the new value after the urgent render has completed.

This hook is similar to user-space hooks which use debouncing or throttling to defer updates. The benefits to using useDeferredValue is that React will work on the update as soon as other work finishes (instead of waiting for an arbitrary amount of time), and like startTransition, deferred values can suspend without triggering an unexpected fallback for existing content.

Memoizing deferred children
useDeferredValue only defers the value that you pass to it. If you want to prevent a child component from re-rendering during an urgent update, you must also memoize that component with React.memo or React.useMemo:

```jsx harmony	
function Typeahead() {
  const query = useSearchQuery('');
  const deferredQuery = useDeferredValue(query);

  // Memoizing tells React to only re-render when deferredQuery changes,
  // not when query changes.
  const suggestions = useMemo(() =>
    <SearchSuggestions query={deferredQuery} />,
    [deferredQuery]
  );

  return (
    <>
      <SearchInput query={query} />
      <Suspense fallback="Loading results...">
        {suggestions}
      </Suspense>
    </>
  );
}
```	
**[⬆ 302](#302)**
	
	
### useTransition <a name="useTransition"></a>
	
```jsx harmony	
const [isPending, startTransition] = useTransition();
```	
Returns a stateful value for the pending state of the transition, and a function to start it.

startTransition lets you mark updates in the provided callback as transitions:

```jsx harmony	
startTransition(() => {
  setCount(count + 1);
})
```
	
isPending indicates when a transition is active to show a pending state:
```jsx harmony	
function App() {
  const [isPending, startTransition] = useTransition();
  const [count, setCount] = useState(0);
  
  function handleClick() {
    startTransition(() => {
      setCount(c => c + 1);
    })
  }

  return (
    <div>
      {isPending && <Spinner />}
      <button onClick={handleClick}>{count}</button>
    </div>
  );
}
```	
**[⬆ 302](#302)**
	
	
### useId
	
```jsx harmony	
const id = useId();
```	
useId is a hook for generating unique IDs that are stable across the server and client, while avoiding hydration mismatches.

useId is not for generating keys in a list. Keys should be generated from your data.

For a basic example, pass the id directly to the elements that need it:
```jsx harmony
function Checkbox() {
  const id = useId();
  return (
    <>
      <label htmlFor={id}>Do you like React?</label>
      <input id={id} type="checkbox" name="react"/>
    </>
  );
};
```	
	
For multiple IDs in the same component, append a suffix using the same id:
```jsx harmony
function NameFields() {
  const id = useId();
  return (
    <div>
      <label htmlFor={id + '-firstName'}>First Name</label>
      <div>
        <input id={id + '-firstName'} type="text" />
      </div>
      <label htmlFor={id + '-lastName'}>Last Name</label>
      <div>
        <input id={id + '-lastName'} type="text" />
      </div>
    </div>
  );
}
```	
	
**[⬆ 302](#302)**
    
  **[⬆ Наверх](#top)**

	
	
303. ### <a name="303"></a> Хуки пример

### useState	
```jsx harmony
import { useState } from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

const Slider = (props) => {

	const [slide, setSlide] = useState(0);
	const [autoplay, setAutoplay] = useState(false);

	function changeSlide(i) {
		setSlide(slide => slide + i)
	}

	const toggleAutoplay = () => {
		setAutoplay(autoplay => !autoplay)
	}

	return (
		<Container>
			<div className="slider w-50 m-auto">
				<div className="text-center mt-5">Active slide {slide}
					<br/>{autoplay ? 'auto' : null}
				</div>
				<div className="buttons mt-3">
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(-1)}>-1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(1)}>+1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={toggleAutoplay}>toggle autoplay
					</button>
				</div>
			</div>
		</Container>
	)
}

function App() {
	const [slider, setSlider] = useState(true);

	return (
		<>
			<button onClick={() => setSlider(false)}>Click</button>
			{slider ? <Slider/> : null}
		</>
	);
}

export default App;	
```	
	
	
### useEffect	
```jsx harmony
import { useState, useEffect } from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

const Slider = (props) => {

	const [slide, setSlide] = useState(0);
	const [autoplay, setAutoplay] = useState(false);

	function logging() {
		console.log('log!')
	}

	useEffect(() => {
		console.log('effect')
		document.title = `Slide: ${slide}`;

		window.addEventListener('click', logging);
		
		return () => {
			window.removeEventListener('click', logging);
		}

	}, [slide]);

	useEffect(() => {
		console.log('autoplay');
	}, [autoplay])

	function changeSlide(i) {
		setSlide(slide => slide + i)
	}

	const toggleAutoplay = () => {
		setAutoplay(autoplay => !autoplay)
	}

	return (
		<Container>
			<div className="slider w-50 m-auto">

				<Slide getSomeImages={getSomeImages} />

				<div className="text-center mt-5">Active slide {slide}
					<br/>{autoplay ? 'auto' : null}
				</div>
				<div className="buttons mt-3">
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(-1)}>-1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(1)}>+1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={toggleAutoplay}>toggle autoplay
					</button>
				</div>
			</div>
		</Container>
	)
}

function App() {
	const [slider, setSlider] = useState(true);

	return (
		<>
			<button onClick={() => setSlider(false)}>Click</button>
			{slider ? <Slider/> : null}
		</>
	);
}

export default App;	
```	
 
### useCallback	
```jsx harmony
import { useState, useEffect, useCallback } from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

const Slider = (props) => {

	const [slide, setSlide] = useState(0);
	const [autoplay, setAutoplay] = useState(false);

	const getSomeImages = useCallback(() => {
		console.log('fetching');
		return [
			'https://data.pixiz.com/output/user/frame/preview/400x400/0/8/1/5/3445180_4e787.jpg',
			'http://anekdotov.net/pic/photo/0221155646p.jpg'
		]
	}, [slide]);


	function logging() {
		console.log('log!')
	}

	useEffect(() => {
		console.log('effect')
		document.title = `Slide: ${slide}`;

		window.addEventListener('click', logging);
		
		return () => {
			window.removeEventListener('click', logging);
		}

	}, [slide]);

	useEffect(() => {
		console.log('autoplay');
	}, [autoplay])

	function changeSlide(i) {
		setSlide(slide => slide + i)
	}

	const toggleAutoplay = () => {
		setAutoplay(autoplay => !autoplay)
	}

	return (
		<Container>
			<div className="slider w-50 m-auto">
				
				<Slide getSomeImages={getSomeImages} />
				
				<div className="text-center mt-5">Active slide {slide}
					<br/>{autoplay ? 'auto' : null}
				</div>
				<div className="buttons mt-3">
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(-1)}>-1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(1)}>+1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={toggleAutoplay}>toggle autoplay
					</button>
				</div>
			</div>
		</Container>
	)
}

const Slide = ({getSomeImages}) => {
	const [images, setImages] = useState([]);

	useEffect(() => {
		setImages(getSomeImages())
	}, [getSomeImages])

	return (
		<>
			{images.map((url, i) => <img key={i} className="d-block w-100"
																	 src={url}
																	 alt="slide"/>)}
		</>
	)
}

function App() {
	const [slider, setSlider] = useState(true);
	
	return (
		<>
			<button onClick={() => setSlider(false)}>Click</button>
			{slider ? <Slider/> : null}
		</>
	);
}

export default App;	
```	

### useMemo	
```jsx harmony
import { useState, useEffect, useCallback, useMemo} from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

const countTotal = (num) => {
	console.log('counting...')
	return num + 10
}

const Slider = (props) => {

	const [slide, setSlide] = useState(0);
	const [autoplay, setAutoplay] = useState(false);

	const getSomeImages = useCallback(() => {
		console.log('fetching');
		return [
			'https://data.pixiz.com/output/user/frame/preview/400x400/0/8/1/5/3445180_4e787.jpg',
			'http://anekdotov.net/pic/photo/0221155646p.jpg'
		]
	}, [slide]);

	
	function logging() {
		console.log('log!')
	}

	useEffect(() => {
		console.log('effect')
		document.title = `Slide: ${slide}`;

		window.addEventListener('click', logging);
		
		return () => {
		 	window.removeEventListener('click', logging);
		}

	}, [slide]);

	useEffect(() => {
		console.log('autoplay');
	}, [autoplay])

	function changeSlide(i) {
		setSlide(slide => slide + i)
	}

	const toggleAutoplay = () => {
		setAutoplay(autoplay => !autoplay)
	}

	const total = useMemo(() => {
		return countTotal(slide)
	}, [slide]);

	const style = useMemo(() => ({
		color: slide > 4 ? 'red' : 'black'
	}), [slide])

	useEffect(() => {
		console.log('styles!')
	}, [style]);

	return (
		<Container>
			<div className="slider w-50 m-auto">

				<Slide getSomeImages={getSomeImages} />

				<div className="text-center mt-5">Active slide {slide}
					<br/>{autoplay ? 'auto' : null}
				</div>
				<div style={style} className="text-center mt-5">Total slides: {total}</div>
				<div className="buttons mt-3">
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(-1)}>-1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={() => changeSlide(1)}>+1
					</button>
					<button
						className="btn btn-primary me-2"
						onClick={toggleAutoplay}>toggle autoplay
					</button>
				</div>
			</div>
		</Container>
	)
}

const Slide = ({getSomeImages}) => {
	const [images, setImages] = useState([]);

	useEffect(() => {
		setImages(getSomeImages())
	}, [getSomeImages])

	return (
		<>
			{images.map((url, i) => <img key={i} className="d-block w-100"
																	 src={url}
																	 alt="slide"/>)}
		</>
	)
}

function App() {
	const [slider, setSlider] = useState(true);


	return (
		<>
			<button onClick={() => setSlider(false)}>Click</button>
			{slider ? <Slider/> : null}
		</>
	);
}

export default App;	
```
	
### useRef	
```jsx harmony
import {useRef, useState} from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

const Form = () => {
    const [text, setTetx] = useState('');

    const myRef = useRef(1);

    return (
        <Container>
            <form className="w-50 border mt-5 p-3 m-auto">
                <div className="mb-3">
                    <label htmlFor="exampleFormControlInput1" className="form-label">Email address</label>
                    <input onChange={(e) => setTetx(e.target.value)} type="email" className="form-control" id="exampleFormControlInput1" placeholder="name@example.com"/>
                    </div>
                    <div className="mb-3">
                    <label htmlFor="exampleFormControlTextarea1" className="form-label">Example textarea</label>
                    <textarea onClick={() => myRef.current++} className="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
                </div>
            </form>
        </Container>
    )
}

function App() {
    return (
        <Form/>
    );
}

export default App;	
```		

### useContextt

Content	
```jsx harmony
import {createContext} from 'react';

const dataContext = createContext({
	mail: "name@example.com",
	text: 'some text',
	forceChangeMail: () => {}
});

export default dataContext;	
```	

Input	
```jsx harmony
import {useContext} from 'react';
import dataContext from './ConContext';

const InputComponent = () => {

	const context = useContext(dataContext);

	return (
		<input
			value={context.mail}
			type="email"
			className='form-control'
			placeholder='name@example.com'
			onFocus={context.forceChangeMail}
		/>
	)
}

export default InputComponent;	
```
	
Form
```jsx harmony
import {Container} from 'react-bootstrap';
import InputComponent from './ConInput';

const Form = (props) => {

	console.log('update')

	return (
		<Container>
			<form className="w-50 border mt-5 p-3 m-auto">
				<div className="mb-3">
					<label htmlFor="exampleFormControlInput1" className="form-label mt-3">Email address</label>
					<InputComponent />
				</div>
				<div className="mb-3">
					<label htmlFor="exampleFormControlTextarea1" className="form-label">Example textarea</label>
					<textarea value={props.text} className="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
				</div>
			</form>
		</Container>
	)
}

export default Form;	
```	

App	
```jsx harmony
import { useState } from 'react';
import './App.css';
import Form from './ConForm';
import dataContext from './ConContext';

const {Provider} = dataContext;


function App() {
    const [data, setData] = useState({
        mail: "name@example.com",
        text: 'some text',
        forceChangeMail: forceChangeMail
    });

    function forceChangeMail() {
      setData({...data, mail: 'test@gmail.com'})
    }

    return (
        <Provider value={data}>
            <Form text={data.text}/>
            <button 
                onClick={() => setData({
                    mail: "second@example.com",
                    text: 'another text',
                    forceChangeMail: forceChangeMail
                })}>
                Click me
            </button>
        </Provider>
    );
}

export default App;	
```
	
### useReducer
```jsx harmony
import {useState, useReducer} from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

function reducer (state, action) {
    switch (action.type) {
        case 'toggle':
          return {autoplay: !state.autoplay}
        case 'slow':
            return {autoplay: 300}
        case 'fast':
            return {autoplay: 700}
        case 'custom':
            return {autoplay: action.payload}
        default:
            throw new Error();
    }
}

function init(initial) {
    return {autoplay: initial}
}

const Slider = ({initial}) => {
    const [slide, setSlide] = useState(0);
    const [autoplay, dispatch] = useReducer(reducer, initial, init);
    // const [autoplay, dispatch] = useReducer(reducer, {autoplay: false});

    function changeSlide(i) {
        setSlide(slide => slide + i);
    }

    return (
        <Container>
            <div className="slider w-50 m-auto">
                <img className="d-block w-100" src="https://www.planetware.com/wpimages/2020/02/france-in-pictures-beautiful-places-to-photograph-eiffel-tower.jpg" alt="slide" />
                <div className="text-center mt-5">Active slide {slide} <br/>{autoplay.autoplay ? 'auto' : null} </div>
                <div className="buttons mt-3">
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => changeSlide(-1)}>-1</button>
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => changeSlide(1)}>+1</button>
                    <button 
                        className="btn btn-primary me-2"
                        onClick={() => dispatch({type: 'toggle'})}>toggle autoplay</button>
                    <button
                      className="btn btn-primary me-2"
                      onClick={() => dispatch({type: 'slow'})}>slow autoplay</button>
                    <button
                      className="btn btn-primary me-2"
                      onClick={() => dispatch({type: 'fast'})}>fast autoplay</button>
                    <button
                      className="btn btn-primary me-2"
                      onClick={(e) => dispatch({type: 'custom', payload: +e.target.textContent})}>1000</button>
                </div>
            </div>
        </Container>
    )
}

function App() {
    return (
        <Slider initial={false}/>
    );
}

export default App;	
```	

### useDeferredValue

useDeferredValue оптимизирует работу приложения, если у вас большой список или сложная верстка или когда есть динамический списко данных, подсказок, табов. Стоит применять там где можно выполнить рендер отложенно.	
	
```jsx harmony
import data from './data';
import { useState, useMemo, useDeferredValue } from 'react';

function App() {
  const [text, setText] = useState('');
  const [posts, setPosts] = useState(data);
  const deferedValue = useDeferredValue(text);

  const filteredPosts = useMemo(() => {
    return posts.filter((item) =>
      item.name.toLowerCase().includes(deferedValue)
    );
  }, [deferedValue]);

  const onValueChange = (e) => {
    setText(e.target.value);
  };

  return (
    <>
      <input value={text} type='text' onChange={onValueChange} />

      <hr />

      <div>
        {filteredPosts.map((post) => (
          <div key={post._id}>
            <h4>{post.name}</h4>
          </div>
        ))}
      </div>
    </>
  );
}

export default App;	
```
	
### useTransition
	
useTransition оптимизирует работу приложения, если у вас большой список или сложная верстка или когда есть динамический списко данных, подсказок, табов. Стоит применять там где можно выполнить рендер отложенно.	
	
```jsx harmony
import data from './data';
import { useState, useMemo, useTransition } from 'react';

function App() {
  const [text, setText] = useState('');
  const [posts, setPosts] = useState(data);
  const [isPending, startTransition] = useTransition();

  const filteredPosts = useMemo(() => {
    return posts.filter((item) =>
      item.name.toLowerCase().includes(text)
    );
  }, [text]);

  const onValueChange = (e) => {
    startTransition(() => {
      setText(e.target.value);
    });
  };

  return (
    <>
      <input value={text} type='text' onChange={onValueChange} />

      <hr />

      <div>
        {isPending ? (
          <h3>Loading</h3>
        ) : (
          filteredPosts.map((post) => (
            <div key={post._id}>
              <h4>{post.name}</h4>
            </div>
          ))
        )}
      </div>
    </>
  );
}

export default App;	
```	

### useId
	  
```jsx harmony	  
const id = useId();
```	  
useId is a hook for generating unique IDs that are stable across the server and client, while avoiding hydration mismatches.

useId is not for generating keys in a list. Keys should be generated from your data.

For a basic example, pass the id directly to the elements that need it:
```jsx harmony
function Checkbox() {
  const id = useId();
  return (
    <>
      <label htmlFor={id}>Do you like React?</label>
      <input id={id} type="checkbox" name="react"/>
    </>
  );
};
```	  
	  
For multiple IDs in the same component, append a suffix using the same id:
```jsx harmony
function NameFields() {
  const id = useId();
  return (
    <div>
      <label htmlFor={id + '-firstName'}>First Name</label>
      <div>
        <input id={id + '-firstName'} type="text" />
      </div>
      <label htmlFor={id + '-lastName'}>Last Name</label>
      <div>
        <input id={id + '-lastName'} type="text" />
      </div>
    </div>
  );
}
```	
	  
  **[⬆ Наверх](#top)**
	
304. ### <a name="304"></a> Создание собственных хуков

Создание пользовательских хуков позволяет вам перенести логику компонентов в функции, которые можно повторно использовать.		
	
```jsx harmony
 function useCounter(initial) {
    const [counter, setCounter] = React.useState(initial);
  
    // Это вариант с запросом, чтобы он нормально работал после активации - уберите все props,
    // которые приходят в компонент + аргумент initial поменяйте на 0 или null
  
    // React.useEffect(() => {
    //     fetch('https://www.random.org/integers/?num=1&min=-50&max=50&col=1&base=10&format=plain&rnd=new')
    //         .then(res => res.text())
    //         .then(res => setCounter(res))
    //         .catch(err => console.log(err))
    // }, [])
  
    const incCounter = () => {
      if (counter < 50) {
        setCounter(counter => counter + 1)
      }
    } 

    const decCounter = () => {
      if (counter > -50) {
        setCounter(counter => counter - 1)
      }
    }

    const rndCounter = () => {
      setCounter(+(Math.random() * (50 - -50) + -50).toFixed(0))
    }

    const resetCounter = () => {
      setCounter(initial)
    }
    
    return {
      counter,
      incCounter,
      decCounter,
      rndCounter,
      resetCounter
    }
}

const Counter = (props) => {
    const {counter, incCounter, decCounter, rndCounter, resetCounter} = useCounter(props.counter);

    return (
      <div className="component">
        <div className="counter">{counter}</div>
        <div className="controls">
          <button onClick={incCounter}>INC</button>
          <button onClick={decCounter}>DEC</button>
          <button onClick={rndCounter}>RND</button>
          <button onClick={resetCounter}>RESET</button>
        </div>
      </div>
    )
}

const RndCounter = (props) => {
    const {counter, rndCounter, resetCounter} = useCounter(props.counter);

    return (
      <div className="component">
        <div className="counter">{counter}</div>
        <div className="controls">
          <button onClick={rndCounter}>RND</button>
          <button onClick={resetCounter}>RESET</button>
        </div>
      </div>
    )
}

const App = () => {
    return (
        <>
            <Counter counter={0}/>
            <RndCounter counter={5}/>
        </>
    )
}

ReactDOM.render(<App />, document.getElementById('app')); 
``` 
 
```jsx harmony
import {useState, useEffect} from 'react';
import {Container} from 'react-bootstrap';
import './App.css';

function useInputWithValidate(initialValue) {
	const [value, setValue] = useState(initialValue);

	const onChange = event => {
		setValue(event.target.value);
	}

	const validateInput = () => {
		return value.search(/\d/) >= 0
	}

	return {value, onChange, validateInput}
}

const Form = () => {

	const input = useInputWithValidate('');
	const textArea = useInputWithValidate('');

	const color = input.validateInput() ? 'text-danger' : null;

	return (
		<Container>
			<form className="w-50 border mt-5 p-3 m-auto">
				<div className="mb-3">
					<input value={`${input.value} / ${textArea.value}`} type="text" className="form-control" readOnly/>
					<label htmlFor="exampleFormControlInput1" className="form-label mt-3">Email address</label>
					<input onChange={input.onChange} type="email" value={input.value} className={`form-control ${color}`}
								 id="exampleFormControlInput1" placeholder="name@example.com"/>
				</div>
				<div className="mb-3">
					<label htmlFor="exampleFormControlTextarea1" className="form-label">Example textarea</label>
					<textarea onChange={textArea.onChange} value={textArea.value} className="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
				</div>
			</form>
		</Container>
	)
}

function App() {
	return (
		<Form/>
	);
}

export default App;	
```	
	
  **[⬆ Наверх](#top)**
	
305. ### <a name="305"></a> Практика создание собственных хуков

### http.hook.js	  
```jsx harmony
import { useState, useCallback } from "react";

export const useHttp = () => {
    const [loading, setLoading] = useState(false);
    const [error, setError] = useState(null);

    const request = useCallback(async (url, method = 'GET', body = null, headers = {'Content-Type': 'application/json'}) => {

        setLoading(true);

        try {
            const response = await fetch(url, {method, body, headers});

            if (!response.ok) {
                throw new Error(`Could not fetch ${url}, status: ${response.status}`);
            }

            const data = await response.json();

            setLoading(false);
            return data;
        } catch(e) {
            setLoading(false);
            setError(e.message);
            throw e;
        }
    }, []);

    const clearError = useCallback(() => setError(null), []);

    return {loading, request, error, clearError}
}	  
```
	  
### MarvelService.js 
```jsx harmony
import {useHttp} from '../hooks/http.hook';

const useMarvelService = () => {
    const {loading, request, error, clearError} = useHttp();

    const _apiBase = 'https://gateway.marvel.com:443/v1/public/';
    // ЗДЕСЬ БУДЕТ ВАШ КЛЮЧ, ЭТОТ КЛЮЧ МОЖЕТ НЕ РАБОТАТЬ
    const _apiKey = 'apikey=c5d6fc8b83116d92ed468ce36bac6c62';
    const _baseOffset = 210;

    const getAllCharacters = async (offset = _baseOffset) => {
        const res = await request(`${_apiBase}characters?limit=9&offset=${offset}&${_apiKey}`);
        return res.data.results.map(_transformCharacter);
    }

    const getCharacter = async (id) => {
        const res = await request(`${_apiBase}characters/${id}?${_apiKey}`);
        return _transformCharacter(res.data.results[0]);
    }

    const getAllComics = async (offset = 0) => {
        const res = await request(`${_apiBase}comics?orderBy=issueNumber&limit=8&offset=${offset}&${_apiKey}`);
        return res.data.results.map(_transformComics);
    }

    const getComics = async (id) => {
        const res = await request(`${_apiBase}comics/${id}?${_apiKey}`);
        return _transformComics(res.data.results[0]);
    }

    const _transformCharacter = (char) => {
        return {
            id: char.id,
            name: char.name,
            description: char.description ? `${char.description.slice(0, 210)}...` : 'There is no description for this character',
            thumbnail: char.thumbnail.path + '.' + char.thumbnail.extension,
            homepage: char.urls[0].url,
            wiki: char.urls[1].url,
            comics: char.comics.items
        }
    }

    const _transformComics = (comics) => {
        return {
            id: comics.id,
            title: comics.title,
            description: comics.description || 'There is no description',
            pageCount: comics.pageCount ? `${comics.pageCount} p.` : 'No information about the number of pages',
            thumbnail: comics.thumbnail.path + '.' + comics.thumbnail.extension,
            language: comics.textObjects.language || 'en-us',
            price: comics.prices.price ? `${comics.prices.price}$` : 'not available'
        }
    }

    return {loading, error, clearError, getAllCharacters, getCharacter, getAllComics, getComics}
}

export default useMarvelService;	  
```
	  
### RandomChar.js
```jsx harmony
import {useState, useEffect} from 'react';
import Spinner from '../spinner/Spinner';
import ErrorMessage from '../errorMessage/ErrorMessage';
import useMarvelService from '../../services/MarvelService';

import './randomChar.scss';
import mjolnir from '../../resources/img/mjolnir.png';

const RandomChar = () => {

    const [char, setChar] = useState(null);
    const {loading, error, getCharacter, clearError} = useMarvelService();

    useEffect(() => {
        updateChar();
        const timerId = setInterval(updateChar, 60000);

        return () => {
            clearInterval(timerId)
        }
    }, [])

    const onCharLoaded = (char) => {
        setChar(char);
    }

    const updateChar = () => {
        clearError();
        const id = Math.floor(Math.random() * (1011400 - 1011000)) + 1011000;
        getCharacter(id)
            .then(onCharLoaded);
    }

    const errorMessage = error ? <ErrorMessage/> : null;
    const spinner = loading ? <Spinner/> : null;
    const content = !(loading || error || !char) ? <View char={char} /> : null;

    return (
        <div className="randomchar">
            {errorMessage}
            {spinner}
            {content}
            <div className="randomchar__static">
                <p className="randomchar__title">
                    Random character for today!<br/>
                    Do you want to get to know him better?
                </p>
                <p className="randomchar__title">
                    Or choose another one
                </p>
                <button onClick={updateChar} className="button button__main">
                    <div className="inner">try it</div>
                </button>
                <img src={mjolnir} alt="mjolnir" className="randomchar__decoration"/>
            </div>
        </div>
    )
}

const View = ({char}) => {
    const {name, description, thumbnail, homepage, wiki} = char;
    let imgStyle = {'objectFit' : 'cover'};
    if (thumbnail === 'http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available.jpg') {
        imgStyle = {'objectFit' : 'contain'};
    }

    return (
        <div className="randomchar__block">
            <img src={thumbnail} alt="Random character" className="randomchar__img" style={imgStyle}/>
            <div className="randomchar__info">
                <p className="randomchar__name">{name}</p>
                <p className="randomchar__descr">
                    {description}
                </p>
                <div className="randomchar__btns">
                    <a href={homepage} className="button button__main">
                        <div className="inner">homepage</div>
                    </a>
                    <a href={wiki} className="button button__secondary">
                        <div className="inner">Wiki</div>
                    </a>
                </div>
            </div>
        </div>
    )
}

export default RandomChar;	  
```
	  
### CharList.js
```jsx harmony
import {useState, useEffect, useRef} from 'react';
import PropTypes from 'prop-types';

import Spinner from '../spinner/Spinner';
import ErrorMessage from '../errorMessage/ErrorMessage';
import useMarvelService from '../../services/MarvelService';
import './charList.scss';

const CharList = (props) => {

    const [charList, setCharList] = useState([]);
    const [newItemLoading, setNewItemLoading] = useState(false);
    const [offset, setOffset] = useState(210);
    const [charEnded, setCharEnded] = useState(false);

    const {loading, error, getAllCharacters} = useMarvelService();

    useEffect(() => {
        onRequest(offset, true);
    }, [])

    const onRequest = (offset, initial) => {
        initial ? setNewItemLoading(false) : setNewItemLoading(true);
        getAllCharacters(offset)
            .then(onCharListLoaded)
    }

    const onCharListLoaded = (newCharList) => {
        let ended = false;
        if (newCharList.length < 9) {
            ended = true;
        }

        setCharList(charList => [...charList, ...newCharList]);
        setNewItemLoading(newItemLoading => false);
        setOffset(offset => offset + 9);
        setCharEnded(charEnded => ended);
    }

    const itemRefs = useRef([]);

    const focusOnItem = (id) => {
        // Я реализовал вариант чуть сложнее, и с классом и с фокусом
        // Но в теории можно оставить только фокус, и его в стилях использовать вместо класса
        // На самом деле, решение с css-классом можно сделать, вынеся персонажа
        // в отдельный компонент. Но кода будет больше, появится новое состояние
        // и не факт, что мы выиграем по оптимизации за счет бОльшего кол-ва элементов

        // По возможности, не злоупотребляйте рефами, только в крайних случаях
        itemRefs.current.forEach(item => item.classList.remove('char__item_selected'));
        itemRefs.current[id].classList.add('char__item_selected');
        itemRefs.current[id].focus();
    }

    // Этот метод создан для оптимизации, 
    // чтобы не помещать такую конструкцию в метод render
    function renderItems(arr) {
        const items =  arr.map((item, i) => {
            let imgStyle = {'objectFit' : 'cover'};
            if (item.thumbnail === 'http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available.jpg') {
                imgStyle = {'objectFit' : 'unset'};
            }
            
            return (
                <li 
                    className="char__item"
                    tabIndex={0}
                    ref={el => itemRefs.current[i] = el}
                    key={item.id}
                    onClick={() => {
                        props.onCharSelected(item.id);
                        focusOnItem(i);
                    }}
                    onKeyPress={(e) => {
                        if (e.key === ' ' || e.key === "Enter") {
                            props.onCharSelected(item.id);
                            focusOnItem(i);
                        }
                    }}>
                        <img src={item.thumbnail} alt={item.name} style={imgStyle}/>
                        <div className="char__name">{item.name}</div>
                </li>
            )
        });
        // А эта конструкция вынесена для центровки спиннера/ошибки
        return (
            <ul className="char__grid">
                {items}
            </ul>
        )
    }
    
    const items = renderItems(charList);

    const errorMessage = error ? <ErrorMessage/> : null;
    const spinner = loading && !newItemLoading ? <Spinner/> : null;

    return (
        <div className="char__list">
            {errorMessage}
            {spinner}
            {items}
            <button 
                className="button button__main button__long"
                disabled={newItemLoading}
                style={{'display': charEnded ? 'none' : 'block'}}
                onClick={() => onRequest(offset)}>
                <div className="inner">load more</div>
            </button>
        </div>
    )
}

CharList.propTypes = {
    onCharSelected: PropTypes.func.isRequired
}

export default CharList;	  
```
	  
### CharInfo.js
```jsx harmony
import { useState, useEffect } from 'react';
import PropTypes from 'prop-types';

import useMarvelService from '../../services/MarvelService';
import Spinner from '../spinner/Spinner';
import ErrorMessage from '../errorMessage/ErrorMessage';
import Skeleton from '../skeleton/Skeleton';

import './charInfo.scss';

const CharInfo = (props) => {

    const [char, setChar] = useState(null);

    const {loading, error, getCharacter, clearError} = useMarvelService();

    useEffect(() => {
        updateChar()
    }, [props.charId])

    const updateChar = () => {
        const {charId} = props;
        if (!charId) {
            return;
        }

        clearError();
        getCharacter(charId)
            .then(onCharLoaded)
    }

    const onCharLoaded = (char) => {
        setChar(char);
    }

    const skeleton = char || loading || error ? null : <Skeleton/>;
    const errorMessage = error ? <ErrorMessage/> : null;
    const spinner = loading ? <Spinner/> : null;
    const content = !(loading || error || !char) ? <View char={char}/> : null;

    return (
        <div className="char__info">
            {skeleton}
            {errorMessage}
            {spinner}
            {content}
        </div>
    )
}

const View = ({char}) => {
    const {name, description, thumbnail, homepage, wiki, comics} = char;

    let imgStyle = {'objectFit' : 'cover'};
    if (thumbnail === 'http://i.annihil.us/u/prod/marvel/i/mg/b/40/image_not_available.jpg') {
        imgStyle = {'objectFit' : 'contain'};
    }

    return (
        <>
            <div className="char__basics">
                <img src={thumbnail} alt={name} style={imgStyle}/>
                <div>
                    <div className="char__info-name">{name}</div>
                    <div className="char__btns">
                        <a href={homepage} className="button button__main">
                            <div className="inner">homepage</div>
                        </a>
                        <a href={wiki} className="button button__secondary">
                            <div className="inner">Wiki</div>
                        </a>
                    </div>
                </div>
            </div>
            <div className="char__descr">
                {description}
            </div>
            <div className="char__comics">Comics:</div>
            <ul className="char__comics-list">
                {comics.length > 0 ? null : 'There is no comics with this character'}
                {
                    comics.map((item, i) => {
                        // eslint-disable-next-line
                        if (i > 9) return;
                        return (
                            <li key={i} className="char__comics-item">
                                {item.name}
                            </li>
                        )
                    })
                }                
            </ul>
        </>
    )
}

CharInfo.propTypes = {
    charId: PropTypes.number
}

export default CharInfo;	  
```
	  
### ComicsList.js
```jsx harmone
import {useState, useEffect} from 'react';
import useMarvelService from '../../services/MarvelService';
import Spinner from '../spinner/Spinner';
import ErrorMessage from '../errorMessage/ErrorMessage';

import './comicsList.scss';

const ComicsList = () => {

    const [comicsList, setComicsList] = useState([]);
    const [newItemLoading, setnewItemLoading] = useState(false);
    const [offset, setOffset] = useState(0);
    const [comicsEnded, setComicsEnded] = useState(false);

    const {loading, error, getAllComics} = useMarvelService();

    useEffect(() => {
        onRequest(offset, true);
    }, [])

    const onRequest = (offset, initial) => {
        initial ? setnewItemLoading(false) : setnewItemLoading(true);
        getAllComics(offset)
            .then(onComicsListLoaded)
    }

    const onComicsListLoaded = (newComicsList) => {
        let ended = false;
        if (newComicsList.length < 8) {
            ended = true;
        }
        setComicsList([...comicsList, ...newComicsList]);
        setnewItemLoading(false);
        setOffset(offset + 8);
        setComicsEnded(ended);
    }

    function renderItems (arr) {
        const items = arr.map((item, i) => {
            return (
                <li className="comics__item" key={i}>
                    <a href="#">
                        <img src={item.thumbnail} alt={item.title} className="comics__item-img"/>
                        <div className="comics__item-name">{item.title}</div>
                        <div className="comics__item-price">{item.price}</div>
                    </a>
                </li>
            )
        })

        return (
            <ul className="comics__grid">
                {items}
            </ul>
        )
    }

    const items = renderItems(comicsList);

    const errorMessage = error ? <ErrorMessage/> : null;
    const spinner = loading && !newItemLoading ? <Spinner/> : null;

    return (
        <div className="comics__list">
            {errorMessage}
            {spinner}
            {items}
            <button 
                disabled={newItemLoading} 
                style={{'display' : comicsEnded ? 'none' : 'block'}}
                className="button button__main button__long"
                onClick={() => onRequest(offset)}>
                <div className="inner">load more</div>
            </button>
        </div>
    )
}

export default ComicsList;	  
```	  	  
	  
  **[⬆ Наверх](#top)**
	
306. ### <a name="306"></a> 

 
    
  **[⬆ Наверх](#top)**
	
307. ### <a name="307"></a> 

 
    
  **[⬆ Наверх](#top)**
	
308. ### <a name="308"></a> 

 
    
  **[⬆ Наверх](#top)**
	
309. ### <a name="309"></a> 

 
    
  **[⬆ Наверх](#top)**
	
310. ### <a name="310"></a> 

 
    
  **[⬆ Наверх](#top)**

325. ### <a name="325"></a> configureStore(), createReducer(), createAction(), createSlice(), createAsyncThunk(), createEntityAdapter()

- [configureStore()](#configureStore)
- [createReducer()](#createReducer)
- [createAction()](#createAction)
- [createSlice()](#createSlice)
- [createAsyncThunk()](#createAsyncThunk)
- [createEntityAdapter()](#createEntityAdapter)	

	
`Redux Toolkit` предоставляет инструменты для настройки хранилища и выполнения наиболее распространенных операций, а также содержит полезные утилиты, позволяющие упростить код.	
	
### configureStore() <a name="configureStore"></a>

`configureStore()` помогает решить названные проблемы следующим образом:
- Принимает объект с "именованными" параметрами, что облегчает изучение кода
- Позволяет передавать массив middlewares и enhancers, автоматически вызывая applyMiddleware() и compose()
- автоматически включает расширение Redux DevTools
	
Кроме того, configureStore() автоматически добавляет следующих посредников:
- redux-thunk - наиболее часто используемый промежуточный слой для работы с синхронной и асинхронной логикой за пределами компонентов
- в режиме разработки, промежуточный слой для обнаружения распространенных ошибок, вроде мутирования состояния или использования несериализуемых значений
	
Простейшим способом создания и настройки хранилища является передача в configureStore() корневого редуктора в качестве аргумента reducer:
	
```jsx harmony
import { configureStore } from '@reduxjs/toolkit'
import rootReducer from './reducers'

const store = configureStore({
  reducer: rootReducer
})

export default store
```	
	
Также допускается передавать объект с частичными редукторами, в этом случае configureStore() автоматически вызывает combineReducers():
	
```jsx harmony
import usersReducer from './usersReducer'
import postsReducer from './postsReducer'

const store = configureStore({
  reducer: {
    users: usersReducer,
    posts: postsReducer
  }
})
```
	
Обратите внимание, что это работает только для одного уровня вложенности. Если требуются вложенные редукторы, придется вызывать combineReducers() самостоятельно.	
	
**[⬆ 325](#325)**

	
### createReducer() <a name="createReducer"></a>

Функция `createReducer()` похожа на функцию создания поисковой таблицы из документации по Redux. В ней используется библиотека immer, что позволяет писать "мутирующий" код, обновляющий состояние иммутабельно. Это защищает от непреднамеренного мутирования состояния в редукторе.	

```jsx harmony
const todosReducer = createReducer([], builder => {
  builder
    .addCase('ADD_TODO', (state, action) => {
      // "мутируем" массив, вызывая push()
      state.push(action.payload)
    })
    .addCase('TOGGLE_TODO', (state, action) => {
      const todo = state[action.payload.index]
      // "мутируем" объект, перезаписывая его поле `completed`
      todo.completed = !todo.completed
    })
    .addCase('REMOVE_TODO', (state,action) => {
      // мы по-прежнему можем использовать иммутабельную логику обновления состояния
      return state.filter((todo,i) => i !== action.payload.index)
    })
})	
```	

Функция createReducer() может быть очень полезной, но следует помнить о том, что:

"Мутирующий" код правильно работает только внутри createReducer()
Immer не позволяет смешивать "мутирование" черновика (draft) состояния и возвращение нового состояния	
	
	
**[⬆ 325](#325)**

	
### createAction() <a name="createAction"></a>
	
Написание создателей операции вручную может быть утомительным. Redux Toolkit предоставляет функцию createAction(), которая генерирует создателя операции с указанным типом операции и преобразует переданные аргументы в поле payload:

```jsx harmony	
const addTodo = createAction('ADD_TODO')
addTodo({ text: 'Buy milk' })
// { type : "ADD_TODO", payload : {text : "Buy milk"}} )
```
	
createAction() также принимает аргумент-колбек prepare, позволяющий кастомизировать результирующее поле payload и добавлять поле meta, при необходимости.
	
```jsx harmony
const actionCreator = createAction('SOME_ACTION_TYPE')

console.log(actionCreator.toString())
// SOME_ACTION_TYPE

console.log(actionCreator.type)
// SOME_ACTION_TYPE

const reducer = createReducer({}, builder => {
  // Здесь будет автоматически вызван `actionCreator.toString()`
  // Кроме того, при использовании TypeScript, будет правильно предложен (предположен) тип операции
  builder.addCase(actionCreator, (state, action) => {})

  // Или вы можете указать поле `type`
  // В этому случае, при использовании TypeScript, тип операции предложен не будет
  builder.addCase(actionCreator.type, (state, action) => {})
})	
```	
	
**[⬆ 325](#325)**
	
	
### createSlice() <a name="createSlice"></a>
	
`createSlice()` автоматически генерирует типы и создателей операции на основе переданного названия редуктора:

```jsx harmony	
const postsSlice = createSlice({
  name: 'posts',
  initialState: [],
  reducers: {
    createPost(state, action) {},
    updatePost(state, action) {},
    deletePost(state, action) {}
  }
})

console.log(postsSlice)
/*
{
  name: 'posts',
  actions : {
      createPost,
      updatePost,
      deletePost,
  },
  reducer
}
*/

const { createPost } = postsSlice.actions

console.log(createPost({ id: 123, title: 'Привет, народ!' }))
// { type : 'posts/createPost', payload : { id : 123, title : 'Привет, народ!' } }
```
	
`createSlice()` анализирует функции, определенные в поле reducers, создает редуктор для каждого случая и генерирует создателя, использующего название редуктора в качестве типа операции. Таким образом, редуктор createPost становится типом операции posts/createPost, а создатель createPost() возвращает операцию с этим типом.

Экспорт и использование частей состояния
	
Обычно, мы определяем часть и экспортируем создателей и редукторы:

```jsx harmony	
const postsSlice = createSlice({
  name: 'posts',
  initialState: [],
  reducers: {
    createPost(state, action) {},
    updatePost(state, action) {},
    deletePost(state, action) {}
  }
})

// Извлекаем объект с создателями и редуктор
const { actions, reducer } = postsSlice
// Извлекаем и экспортируем каждого создателя по названию
export const { createPost, updatePost, deletePost } = actions
// Экпортируем редуктор по умолчанию или по названию
export default reducer
```	
	
**[⬆ 325](#325)**

	
### createAsyncThunk() <a name="createAsyncThunk"></a>
	
`createAsyncThunk()` упрощает процесс выполнения асинхронных запросов - мы передаем ему строку для префикса типа операции и колбек создателя полезной нагрузки (payload), выполняющего реальную асинхронную логику и возвращающего промис с результатом. `createAsyncThunk()` возвращает преобразователя, который заботится об отправке правильных операций на основе возвращенного промиса, и типы операции, которые можно обработать в редукторах:

```jsx harmony	
import { createAsyncThunk, createSlice } from '@redux/toolkit'
import { userAPI } from './userAPI'

// Создаем преобразователя
const fetchUserById = createAsyncThunk(
  'user/fetchByIdStatus',
  async (userId, thunkAPI) => {
    const response = await userAPI.fetchById(userId)
    return response.data
  }
)

// Обрабатываем операции в редукторах
const usersSlice = createSlice({
  name: 'users',
  initialState: {entries: [], loading: 'idle'},
  reducers: {
    // стандартная логика редуктора с авто-генерируемыми типами операции для каждого редуктора
  },
  extraReducers: {
    [fetchUserById.fullfilled]: (state, action) => {
      // Добавляем пользователя в массив состояния
      state.entries.push(action.payload)
    }
  }
})

// Позже, отправляем `thunk`
dispatch(fetchUserById(123))
```	
	
**[⬆ 325](#325)**
	
	
### createEntityAdapter() <a name="createEntityAdapter"></a>
	
`createEntityAdapter()` предоставляет стандартизированный способ хранения данных путем преобразования коллекции в форму { ids: [], entities: {} }. Кроме предопределения формы состояния, эта функция генерирует набор редукторов и селекторов, которые знают, как работать с такими данными.
	
```jsx harmony
import {
  createSlice,
  createAsyncThunk,
  createEntityAdapter
} from '@reduxjs/toolkit'
import userAPI from './userAPI'

export const fetchUsers = createAsyncThunk('users/fetchAll', async () => {
  const response = await userAPI.fetchAll()
  // В данном случае `response.data` будет выглядеть так:
  // [{id: 1, first_name: 'Example', last_name: 'User'}]
  return response.data
})

export const updateUser = createAsyncThunk('users/updateOne', async arg => {
  const response = await userAPI.updateUser(arg)
  // В данном случае `response.data` будет выглядеть так:
  // { id: 1, first_name: 'Example', last_name: 'UpdatedLastName'}
  return response.data
})

export const usersAdapter = createEntityAdapter()

// По умолчанию `createEntityAdapter()` возвращает `{ ids: [], entities: {} }`
// Для отслеживания 'loading' или других ключей, их необходимо инициализировать:
// `getInitialState({ loading: false, activeRequestId: null })`
const initialState = usersAdapter.getInitialState()

export const slice = createSlice({
  name: 'users',
  initialState,
  reducers: {
    removeUser: usersAdapter.removeOne
  },
  extraReducers: builder => {
    builder.addCase(fetchUsers.fulfilled, usersAdapter.upsertMany)
    builder.addCase(updateUser.fulfilled, (state, { payload }) => {
      const { id, ...changes } = payload
      usersAdapter.updateOne(state, { id, changes })
    })
  }
})

const reducer = slice.reducer
export default reducer

export const { removeUser } = slice.actions
```	
	
**[⬆ 325](#325)**
    
  **[⬆ Наверх](#top)**
		

326. ### <a name="326"></a> 

 
    
  **[⬆ Наверх](#top)**
	
327. ### <a name="327"></a> 

 
    
  **[⬆ Наверх](#top)**
	
328. ### <a name="328"></a> 

 
    
  **[⬆ Наверх](#top)**
	
329. ### <a name="329"></a> 

 
    
  **[⬆ Наверх](#top)**	
	
330. ### <a name="330"></a> Redux Toolkit: configureStore()

```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import heroes from '../reducers/heroes';
import filters from '../reducers/filters';

const stringMiddleware = () => (next) => (action) => {
    if (typeof action === 'string') {
        return next({
            type: action
        })
    }
    return next(action)
};

const store = configureStore({
    reducer: {heroes, filters},
    middleware: getDefaultMiddleware => getDefaultMiddleware().concat(stringMiddleware),
    devTools: process.env.NODE_ENV !== 'production',
})

export default store;			
```			
    
  **[⬆ Наверх](#top)**
	  
331. ### <a name="331"></a> Redux Toolkit: createAction()

```jsx harmony
import { createAction } from "@reduxjs/toolkit";

export const fetchHeroes = (request) => (dispatch) => {
    dispatch(heroesFetching());
    request("http://localhost:3001/heroes")
        .then(data => dispatch(heroesFetched(data)))
        .catch(() => dispatch(heroesFetchingError()))
}

export const fetchFilters = (request) => (dispatch) => {
    dispatch(filtersFetching());
    request("http://localhost:3001/filters")
        .then(data => dispatch(filtersFetched(data)))
        .catch(() => dispatch(filtersFetchingError()))
}

// export const heroesFetching = () => {
//     return {
//         type: 'HEROES_FETCHING'
//     }
// }

export const heroesFetching = createAction('HEROES_FETCHING');

// export const heroesFetched = (heroes) => {
//     return {
//         type: 'HEROES_FETCHED',
//         payload: heroes
//     }
// }

export const heroesFetched = createAction('HEROES_FETCHED');

// export const heroesFetchingError = () => {
//     return {
//         type: 'HEROES_FETCHING_ERROR'
//     }
// }

export const heroesFetchingError = createAction('HEROES_FETCHING_ERROR');

export const filtersFetching = () => {
    return {
        type: 'FILTERS_FETCHING'
    }
}

export const filtersFetched = (filters) => {
    return {
        type: 'FILTERS_FETCHED',
        payload: filters
    }
}

export const filtersFetchingError = () => {
    return {
        type: 'FILTERS_FETCHING_ERROR'
    }
}

export const activeFilterChanged = (filter) => {
    return {
        type: 'ACTIVE_FILTER_CHANGED',
        payload: filter
    }
}

// export const heroCreated = (hero) => {
//     return {
//         type: 'HERO_CREATED',
//         payload: hero
//     }
// }

export const heroCreated = createAction('HERO_CREATED');

// export const heroDeleted = (id) => {
//     return {
//         type: 'HERO_DELETED',
//         payload: id
//     }
// }

export const heroDeleted = createAction('HERO_DELETED');			
```			
    
  **[⬆ Наверх](#top)**	  

332. ### <a name="332"></a> Redux Toolkit: createReducer()

```jsx harmony
import { createReducer } from "@reduxjs/toolkit";

import {
    heroesFetching,
    heroesFetched,
    heroesFetchingError,
    heroCreated,
    heroDeleted
} from '../actions';

const initialState = {
    heroes: [],
    heroesLoadingStatus: 'idle'
}

const heroes = createReducer(initialState, {
    [heroesFetching]: state => {state.heroesLoadingStatus = 'loading'},
    [heroesFetched]: (state, action) => {
                    state.heroesLoadingStatus = 'idle';
                    state.heroes = action.payload;
                },
    [heroesFetchingError]: state => {
                    state.heroesLoadingStatus = 'error';
                },
    [heroCreated]: (state, action) => {
                    state.heroes.push(action.payload);
                },
    [heroDeleted]: (state, action) => {
                    state.heroes = state.heroes.filter(item => item.id !== action.payload);
                }
        },
    [],
    state => state
)

// или вот так ->			
			
const heroes = createReducer(initialState, builder => {
     builder
         .addCase(heroesFetching, state => {
             state.heroesLoadingStatus = 'loading';
         })
         .addCase(heroesFetched, (state, action) => {
             state.heroesLoadingStatus = 'idle';
             state.heroes = action.payload;
         })
         .addCase(heroesFetchingError, state => {
             state.heroesLoadingStatus = 'error';
         })
         .addCase(heroCreated, (state, action) => {
             state.heroes.push(action.payload);
         })
         .addCase(heroDeleted, (state, action) => {
             state.heroes = state.heroes.filter(item => item.id !== action.payload);
         })
         .addDefaultCase(() => {});
})

export default heroes;			
```			
    
  **[⬆ Наверх](#top)**
			
333. ### <a name="333"></a> Redux Toolkit: createSlice()

### heroesSlice			
```jsx harmony
import { createSlice } from "@reduxjs/toolkit";

const initialState = {
    heroes: [],
    heroesLoadingStatus: 'idle'
}

const heroesSlice = createSlice({
    name: 'heroes',
    initialState,
    reducers: {
        heroesFetching: state => {state.heroesLoadingStatus = 'loading'},
        heroesFetched: (state, action) => {
            state.heroesLoadingStatus = 'idle';
            state.heroes = action.payload;
        },
        heroesFetchingError: state => {
            state.heroesLoadingStatus = 'error';
        },
        heroCreated: (state, action) => {
            state.heroes.push(action.payload);
        },
        heroDeleted: (state, action) => {
            state.heroes = state.heroes.filter(item => item.id !== action.payload);
        }
    }
});

const {actions, reducer} = heroesSlice;

export default reducer;
export const {
    heroesFetching,
    heroesFetched,
    heroesFetchingError,
    heroCreated,
    heroDeleted
} = actions;			
```			

### filtersSlice
```jsx harmony
import { createSlice } from "@reduxjs/toolkit";

const initialState = {
    filters: [],
    filtersLoadingStatus: 'idle',
    activeFilter: 'all'
}

const filtersSlice = createSlice({
    name: 'filters',
    initialState,
    reducers: {
        filtersFetching: state => {state.filtersLoadingStatus = 'loading'},
        filtersFetched: (state, action) => {
            state.filtersLoadingStatus = 'idle';
            state.filters = action.payload;
        },
        filtersFetchingError: state => {
            state.filtersLoadingStatus = 'error';
        },
        filtersChanged: (state, action) => {
            state.activeFilter = action.payload;
        }
    }
});

const {actions, reducer} = filtersSlice;

export default reducer;
export const {
    filtersFetching,
    filtersFetched,
    filtersFetchingError,
    filtersChanged
} = actions;			
```						
			
  **[⬆ Наверх](#top)**			

334. ### <a name="334"></a> Redux Toolkit: createAsyncThunk()

### heroesSlice.js
```jsx harmony
import { createSlice, createAsyncThunk } from "@reduxjs/toolkit";
import {useHttp} from '../../hooks/http.hook';

const initialState = {
    heroes: [],
    heroesLoadingStatus: 'idle'
}

export const fetchHeroes = createAsyncThunk(
    'heroes/fetchHeroes',
    async () => {
        const {request} = useHttp();
        return await request("http://localhost:3001/heroes");
    }
);

const heroesSlice = createSlice({
    name: 'heroes',
    initialState,
    reducers: {
        heroCreated: (state, action) => {
            state.heroes.push(action.payload);
        },
        heroDeleted: (state, action) => {
            state.heroes = state.heroes.filter(item => item.id !== action.payload);
        }
    },
    extraReducers: (builder) => {
        builder
            .addCase(fetchHeroes.pending, state => {state.heroesLoadingStatus = 'loading'})
            .addCase(fetchHeroes.fulfilled, (state, action) => {
                state.heroesLoadingStatus = 'idle';
                state.heroes = action.payload;
            })
            .addCase(fetchHeroes.rejected, state => {
                state.heroesLoadingStatus = 'error';
            })
            .addDefaultCase(() => {})
    }
});

const {actions, reducer} = heroesSlice;

export default reducer;
export const {
    heroesFetching,
    heroesFetched,
    heroesFetchingError,
    heroCreated,
    heroDeleted
} = actions;			
```			

### filtersSlice.js
```jsx harmony
import { createSlice, createAsyncThunk } from "@reduxjs/toolkit";
import {useHttp} from '../../hooks/http.hook';

const initialState = {
    filters: [],
    filtersLoadingStatus: 'idle',
    activeFilter: 'all'
}

export const fetchFilters = createAsyncThunk(
    'filters/fetchFilters',
    async () => {
        const {request} = useHttp();
        return await request("http://localhost:3001/filters");
    }
);

const filtersSlice = createSlice({
    name: 'filters',
    initialState,
    reducers: {
        filtersChanged: (state, action) => {
            state.activeFilter = action.payload;
        }
    },
    extraReducers: (builder) => {
        builder
            .addCase(fetchFilters.pending, state => {state.filtersLoadingStatus = 'loading'})
            .addCase(fetchFilters.fulfilled, (state, action) => {
                state.filtersLoadingStatus = 'idle';
                state.filters = action.payload;
            })
            .addCase(fetchFilters.rejected, state => {
                state.filtersLoadingStatus = 'error';
            })
            .addDefaultCase(() => {})
    }
});

const {actions, reducer} = filtersSlice;

export default reducer;
export const {
    filtersFetching,
    filtersFetched,
    filtersFetchingError,
    filtersChanged
} = actions;			
```			

### http.hook.js
```jsx harmony
export const useHttp = () => {

    const request = async (url, method = 'GET', body = null, headers = {'Content-Type': 'application/json'}) => {

        try {
            const response = await fetch(url, {method, body, headers});

            if (!response.ok) {
                throw new Error(`Could not fetch ${url}, status: ${response.status}`);
            }

            const data = await response.json();

            return data;
        } catch(e) {
            throw e;
        }
    };

    return {request}
}			
```			

### HeroesList.js
```jsx harmony
import {useHttp} from '../../hooks/http.hook';
import { useEffect, useCallback } from 'react';
import { useDispatch, useSelector } from 'react-redux';
import { CSSTransition, TransitionGroup} from 'react-transition-group';
import { createSelector } from '@reduxjs/toolkit';

import { heroDeleted, fetchHeroes } from './heroesSlice';

import HeroesListItem from "../heroesListItem/HeroesListItem";
import Spinner from '../spinner/Spinner';

import './heroesList.scss';

const HeroesList = () => {

    const filteredHeroesSelector = createSelector(
        (state) => state.filters.activeFilter,
        (state) => state.heroes.heroes,
        (filter, heroes) => {
            if (filter === 'all') {
                return heroes;
            } else {
                return heroes.filter(item => item.element === filter);
            }
        }
    );

    const filteredHeroes = useSelector(filteredHeroesSelector);
    const heroesLoadingStatus = useSelector(state => state.heroes.heroesLoadingStatus);
    const dispatch = useDispatch();
    const {request} = useHttp();

    useEffect(() => {
        dispatch(fetchHeroes());
        // eslint-disable-next-line
    }, []);

    const onDelete = useCallback((id) => {
        request(`http://localhost:3001/heroes/${id}`, "DELETE")
            .then(data => console.log(data, 'Deleted'))
            .then(dispatch(heroDeleted(id)))
            .catch(err => console.log(err));
        // eslint-disable-next-line  
    }, [request]);

    if (heroesLoadingStatus === "loading") {
        return <Spinner/>;
    } else if (heroesLoadingStatus === "error") {
        return <h5 className="text-center mt-5">Ошибка загрузки</h5>
    }

    const renderHeroesList = (arr) => {
        if (arr.length === 0) {
            return (
                <CSSTransition
                    timeout={0}
                    classNames="hero">
                    <h5 className="text-center mt-5">Героев пока нет</h5>
                </CSSTransition>
            )
        }

        return arr.map(({id, ...props}) => {
            return (
                <CSSTransition 
                    key={id}
                    timeout={500}
                    classNames="hero">
                    <HeroesListItem  {...props} onDelete={() => onDelete(id)}/>
                </CSSTransition>
            )
        })
    }

    const elements = renderHeroesList(filteredHeroes);
    return (
        <TransitionGroup component="ul">
            {elements}
        </TransitionGroup>
    )
}

export default HeroesList;			
```			

### HeroesFilters.js
```jsx harmony
import {useHttp} from '../../hooks/http.hook';
import { useEffect } from 'react';
import { useDispatch, useSelector } from 'react-redux';
import classNames from 'classnames';

import { filtersChanged, fetchFilters } from './filtersSlice';
import Spinner from '../spinner/Spinner';

const HeroesFilters = () => {

    const {filters, filtersLoadingStatus, activeFilter} = useSelector(state => state.filters);
    const dispatch = useDispatch();
    const {request} = useHttp();

    useEffect(() => {
        dispatch(fetchFilters(request));

        // eslint-disable-next-line
    }, []);

    if (filtersLoadingStatus === "loading") {
        return <Spinner/>;
    } else if (filtersLoadingStatus === "error") {
        return <h5 className="text-center mt-5">Ошибка загрузки</h5>
    }

    const renderFilters = (arr) => {
        if (arr.length === 0) {
            return <h5 className="text-center mt-5">Фильтры не найдены</h5>
        }

        return arr.map(({name, className, label}) => {

            const btnClass = classNames('btn', className, {
                'active': name === activeFilter
            });
            
            return <button 
                        key={name} 
                        id={name} 
                        className={btnClass}
                        onClick={() => dispatch(filtersChanged(name))}
                        >{label}</button>
        })
    }

    const elements = renderFilters(filters);

    return (
        <div className="card shadow-lg mt-4">
            <div className="card-body">
                <p className="card-text">Отфильтруйте героев по элементам</p>
                <div className="btn-group">
                    {elements}
                </div>
            </div>
        </div>
    )
}

export default HeroesFilters;
```			
			
  **[⬆ Наверх](#top)**			

335. ### <a name="335"></a> Redux Toolkit: createEntityAdapter()

### heroesSlice.js
```jsx harmony
import { createSlice, createAsyncThunk, createEntityAdapter, createSelector } from "@reduxjs/toolkit";
import {useHttp} from '../../hooks/http.hook';

const heroesAdapter = createEntityAdapter();

const initialState = heroesAdapter.getInitialState({
    heroesLoadingStatus: 'idle'
});

export const fetchHeroes = createAsyncThunk(
    'heroes/fetchHeroes',
    async () => {
        const {request} = useHttp();
        return await request("http://localhost:3001/heroes");
    }
);

const heroesSlice = createSlice({
    name: 'heroes',
    initialState,
    reducers: {
        heroCreated: (state, action) => {
            heroesAdapter.addOne(state, action.payload);
        },
        heroDeleted: (state, action) => {
            heroesAdapter.removeOne(state, action.payload);
        }
    },
    extraReducers: (builder) => {
        builder
            .addCase(fetchHeroes.pending, state => {state.heroesLoadingStatus = 'loading'})
            .addCase(fetchHeroes.fulfilled, (state, action) => {
                state.heroesLoadingStatus = 'idle';
                heroesAdapter.setAll(state, action.payload);
            })
            .addCase(fetchHeroes.rejected, state => {
                state.heroesLoadingStatus = 'error';
            })
            .addDefaultCase(() => {})
    }
});

const {actions, reducer} = heroesSlice;

export default reducer;

const {selectAll} = heroesAdapter.getSelectors(state => state.heroes);

export const filteredHeroesSelector = createSelector(
    (state) => state.filters.activeFilter,
    selectAll,
    (filter, heroes) => {
        if (filter === 'all') {
            return heroes;
        } else {
            return heroes.filter(item => item.element === filter);
        }
    }
);

export const {
    heroesFetching,
    heroesFetched,
    heroesFetchingError,
    heroCreated,
    heroDeleted
} = actions;			
```			

### filtersSlice.js
```jsx harmony
import { createSlice, createAsyncThunk, createEntityAdapter } from "@reduxjs/toolkit";
import {useHttp} from '../../hooks/http.hook';

const filtersAdapter = createEntityAdapter();

const initialState = filtersAdapter.getInitialState({
    filtersLoadingStatus: 'idle',
    activeFilter: 'all'
});

export const fetchFilters = createAsyncThunk(
    'filters/fetchFilters',
    async () => {
        const {request} = useHttp();
        return await request("http://localhost:3001/filters");
    }
);

const filtersSlice = createSlice({
    name: 'filters',
    initialState,
    reducers: {
        filtersChanged: (state, action) => {
            state.activeFilter = action.payload;
        }
    },
    extraReducers: (builder) => {
        builder
            .addCase(fetchFilters.pending, state => {state.filtersLoadingStatus = 'loading'})
            .addCase(fetchFilters.fulfilled, (state, action) => {
                state.filtersLoadingStatus = 'idle';
                filtersAdapter.setAll(state, action.payload);
            })
            .addCase(fetchFilters.rejected, state => {
                state.filtersLoadingStatus = 'error';
            })
            .addDefaultCase(() => {})
    }
});

const {actions, reducer} = filtersSlice;

export default reducer;

export const {selectAll} = filtersAdapter.getSelectors(state => state.filters);

export const {
    filtersFetching,
    filtersFetched,
    filtersFetchingError,
    filtersChanged
} = actions;			
```			
		
### HeroesList.js
```jsx harmony
import {useHttp} from '../../hooks/http.hook';
import { useEffect, useCallback } from 'react';
import { useDispatch, useSelector } from 'react-redux';
import { CSSTransition, TransitionGroup} from 'react-transition-group';

import { heroDeleted, fetchHeroes, filteredHeroesSelector } from './heroesSlice';

import HeroesListItem from "../heroesListItem/HeroesListItem";
import Spinner from '../spinner/Spinner';

import './heroesList.scss';

const HeroesList = () => {
    const filteredHeroes = useSelector(filteredHeroesSelector);
    const heroesLoadingStatus = useSelector(state => state.heroes.heroesLoadingStatus);
    const dispatch = useDispatch();
    const {request} = useHttp();

    useEffect(() => {
        dispatch(fetchHeroes());
        // eslint-disable-next-line
    }, []);

    const onDelete = useCallback((id) => {
        request(`http://localhost:3001/heroes/${id}`, "DELETE")
            .then(data => console.log(data, 'Deleted'))
            .then(dispatch(heroDeleted(id)))
            .catch(err => console.log(err));
        // eslint-disable-next-line  
    }, [request]);

    if (heroesLoadingStatus === "loading") {
        return <Spinner/>;
    } else if (heroesLoadingStatus === "error") {
        return <h5 className="text-center mt-5">Ошибка загрузки</h5>
    }

    const renderHeroesList = (arr) => {
        if (arr.length === 0) {
            return (
                <CSSTransition
                    timeout={0}
                    classNames="hero">
                    <h5 className="text-center mt-5">Героев пока нет</h5>
                </CSSTransition>
            )
        }

        return arr.map(({id, ...props}) => {
            return (
                <CSSTransition 
                    key={id}
                    timeout={500}
                    classNames="hero">
                    <HeroesListItem  {...props} onDelete={() => onDelete(id)}/>
                </CSSTransition>
            )
        })
    }

    const elements = renderHeroesList(filteredHeroes);
    return (
        <TransitionGroup component="ul">
            {elements}
        </TransitionGroup>
    )
}

export default HeroesList;			
```			
			
### HeroesFilters.js
```jsx harmony
import {useHttp} from '../../hooks/http.hook';
import { useEffect } from 'react';
import { useDispatch, useSelector } from 'react-redux';
import classNames from 'classnames';
import store from '../../store';

import { filtersChanged, fetchFilters, selectAll } from './filtersSlice';
import Spinner from '../spinner/Spinner';

const HeroesFilters = () => {

    const {filtersLoadingStatus, activeFilter} = useSelector(state => state.filters);
    const filters = selectAll(store.getState());
    const dispatch = useDispatch();
    const {request} = useHttp();

    useEffect(() => {
        dispatch(fetchFilters(request));

        // eslint-disable-next-line
    }, []);

    if (filtersLoadingStatus === "loading") {
        return <Spinner/>;
    } else if (filtersLoadingStatus === "error") {
        return <h5 className="text-center mt-5">Ошибка загрузки</h5>
    }

    const renderFilters = (arr) => {
        if (arr.length === 0) {
            return <h5 className="text-center mt-5">Фильтры не найдены</h5>
        }

        return arr.map(({name, className, label}) => {

            const btnClass = classNames('btn', className, {
                'active': name === activeFilter
            });
            
            return <button 
                        key={name} 
                        id={name} 
                        className={btnClass}
                        onClick={() => dispatch(filtersChanged(name))}
                        >{label}</button>
        })
    }

    const elements = renderFilters(filters);

    return (
        <div className="card shadow-lg mt-4">
            <div className="card-body">
                <p className="card-text">Отфильтруйте героев по элементам</p>
                <div className="btn-group">
                    {elements}
                </div>
            </div>
        </div>
    )
}

export default HeroesFilters;			
```						

### HeroesAddForm.js
```jsx harmony
import {useHttp} from '../../hooks/http.hook';
import { useState } from 'react';
import { useDispatch, useSelector } from 'react-redux';
import { v4 as uuidv4 } from 'uuid';
import store from '../../store';

import { selectAll } from '../heroesFilters/filtersSlice';
import { heroCreated } from '../heroesList/heroesSlice';

const HeroesAddForm = () => {
    const [heroName, setHeroName] = useState('');
    const [heroDescr, setHeroDescr] = useState('');
    const [heroElement, setHeroElement] = useState('');

    const {filtersLoadingStatus} = useSelector(state => state.filters);
    const filters = selectAll(store.getState());
    const dispatch = useDispatch();
    const {request} = useHttp();

    const onSubmitHandler = (e) => {
        e.preventDefault();
        const newHero = {
            id: uuidv4(),
            name: heroName,
            description: heroDescr,
            element: heroElement
        }

        request("http://localhost:3001/heroes", "POST", JSON.stringify(newHero))
            .then(res => console.log(res, 'Отправка успешна'))
            .then(dispatch(heroCreated(newHero)))
            .catch(err => console.log(err));

        setHeroName('');
        setHeroDescr('');
        setHeroElement('');
    }

    const renderFilters = (filters, status) => {
        if (status === "loading") {
            return <option>Загрузка элементов</option>
        } else if (status === "error") {
            return <option>Ошибка загрузки</option>
        }
        
        if (filters && filters.length > 0 ) {
            return filters.map(({name, label}) => {
                // eslint-disable-next-line
                if (name === 'all')  return;

                return <option key={name} value={name}>{label}</option>
            })
        }
    }

    return (
        <form className="border p-4 shadow-lg rounded" onSubmit={onSubmitHandler}>
            <div className="mb-3">
                <label htmlFor="name" className="form-label fs-4">Имя нового героя</label>
                <input 
                    required
                    type="text" 
                    name="name" 
                    className="form-control" 
                    id="name" 
                    placeholder="Как меня зовут?"
                    value={heroName}
                    onChange={(e) => setHeroName(e.target.value)}/>
            </div>

            <div className="mb-3">
                <label htmlFor="text" className="form-label fs-4">Описание</label>
                <textarea
                    required
                    name="text" 
                    className="form-control" 
                    id="text" 
                    placeholder="Что я умею?"
                    style={{"height": '130px'}}
                    value={heroDescr}
                    onChange={(e) => setHeroDescr(e.target.value)}/>
            </div>

            <div className="mb-3">
                <label htmlFor="element" className="form-label">Выбрать элемент героя</label>
                <select 
                    required
                    className="form-select" 
                    id="element" 
                    name="element"
                    value={heroElement}
                    onChange={(e) => setHeroElement(e.target.value)}>
                    <option value="">Я владею элементом...</option>
                    {renderFilters(filters, filtersLoadingStatus)}
                </select>
            </div>

            <button type="submit" className="btn btn-primary">Создать</button>
        </form>
    )
}

export default HeroesAddForm;			
```						
			
  **[⬆ Наверх](#top)**			

336. ### <a name="336"></a> Redux Toolkit: RTK Query

apiSlice.js		
```jsx harmony
import {createApi, fetchBaseQuery} from '@reduxjs/toolkit/query/react';

export const apiSlice = createApi({
    reducerPath: 'api',
    baseQuery: fetchBaseQuery({baseUrl: 'http://localhost:3001'}),
    tagTypes: ['Heroes'],
    endpoints: builder => ({
        getHeroes: builder.query({
            query: () => '/heroes',
            providesTags: ['Heroes']
        }),
        createHero: builder.mutation({
            query: hero => ({
                url: '/heroes',
                method: 'POST',
                body: hero
            }),
            invalidatesTags: ['Heroes']
        }),
        deleteHero: builder.mutation({
            query: id => ({
                url: `/heroes/${id}`,
                method: 'DELETE'
            }),
            invalidatesTags: ['Heroes']
        })
    })
});

export const {useGetHeroesQuery, useCreateHeroMutation, useDeleteHeroMutation} = apiSlice;		
```		

store/index.js		
```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import filters from '../components/heroesFilters/filtersSlice';
import { apiSlice } from '../api/apiSlice'; 

const stringMiddleware = () => (next) => (action) => {
    if (typeof action === 'string') {
        return next({
            type: action
        })
    }
    return next(action)
};

const store = configureStore({
    reducer: {  filters, 
                [apiSlice.reducerPath]: apiSlice.reducer},
    middleware: getDefaultMiddleware => getDefaultMiddleware().concat(stringMiddleware, apiSlice.middleware),
    devTools: process.env.NODE_ENV !== 'production'
})

export default store;		
```		

HeroesList.js
```jsx harmony
import { useCallback, useMemo } from 'react';
import { useSelector } from 'react-redux';
import { CSSTransition, TransitionGroup} from 'react-transition-group';

import { useGetHeroesQuery, useDeleteHeroMutation } from '../../api/apiSlice';

import HeroesListItem from "../heroesListItem/HeroesListItem";
import Spinner from '../spinner/Spinner';

import './heroesList.scss';

const HeroesList = () => {
    const {
        data: heroes = [],
        isLoading,
        isError,
    } = useGetHeroesQuery();

    const [deleteHero] = useDeleteHeroMutation();

    const activeFilter = useSelector(state => state.filters.activeFilter);

    const filteredHeroes = useMemo(() => {
        const filteredHeroes = heroes.slice();

        if (activeFilter === 'all') {
            return filteredHeroes;
        } else {
            return filteredHeroes.filter(item => item.element === activeFilter);
        }
    }, [heroes, activeFilter]);

    const onDelete = useCallback((id) => {
        deleteHero(id);
        // eslint-disable-next-line  
    }, []);

    if (isLoading) {
        return <Spinner/>;
    } else if (isError) {
        return <h5 className="text-center mt-5">Ошибка загрузки</h5>
    }

    const renderHeroesList = (arr) => {
        if (arr.length === 0) {
            return (
                <CSSTransition
                    timeout={0}
                    classNames="hero">
                    <h5 className="text-center mt-5">Героев пока нет</h5>
                </CSSTransition>
            )
        }

        return arr.map(({id, ...props}) => {
            return (
                <CSSTransition 
                    key={id}
                    timeout={500}
                    classNames="hero">
                    <HeroesListItem  {...props} onDelete={() => onDelete(id)}/>
                </CSSTransition>
            )
        })
    }

    const elements = renderHeroesList(filteredHeroes);
    return (
        <TransitionGroup component="ul">
            {elements}
        </TransitionGroup>
    )
}

export default HeroesList;		
```		

HeroesAddForm.js
```jsx harmony
import { useState } from 'react';
import { useSelector } from 'react-redux';
import { v4 as uuidv4 } from 'uuid';
import store from '../../store';

import { selectAll } from '../heroesFilters/filtersSlice';
import { useCreateHeroMutation } from '../../api/apiSlice';

const HeroesAddForm = () => {
    const [heroName, setHeroName] = useState('');
    const [heroDescr, setHeroDescr] = useState('');
    const [heroElement, setHeroElement] = useState('');

    const [createHero] = useCreateHeroMutation();

    const {filtersLoadingStatus} = useSelector(state => state.filters);
    const filters = selectAll(store.getState());

    const onSubmitHandler = (e) => {
        e.preventDefault();
        const newHero = {
            id: uuidv4(),
            name: heroName,
            description: heroDescr,
            element: heroElement
        }

        createHero(newHero).unwrap();

        setHeroName('');
        setHeroDescr('');
        setHeroElement('');
    }

    const renderFilters = (filters, status) => {
        if (status === "loading") {
            return <option>Загрузка элементов</option>
        } else if (status === "error") {
            return <option>Ошибка загрузки</option>
        }
        
        if (filters && filters.length > 0 ) {
            return filters.map(({name, label}) => {
                // eslint-disable-next-line
                if (name === 'all')  return;

                return <option key={name} value={name}>{label}</option>
            })
        }
    }

    return (
        <form className="border p-4 shadow-lg rounded" onSubmit={onSubmitHandler}>
            <div className="mb-3">
                <label htmlFor="name" className="form-label fs-4">Имя нового героя</label>
                <input 
                    required
                    type="text" 
                    name="name" 
                    className="form-control" 
                    id="name" 
                    placeholder="Как меня зовут?"
                    value={heroName}
                    onChange={(e) => setHeroName(e.target.value)}/>
            </div>

            <div className="mb-3">
                <label htmlFor="text" className="form-label fs-4">Описание</label>
                <textarea
                    required
                    name="text" 
                    className="form-control" 
                    id="text" 
                    placeholder="Что я умею?"
                    style={{"height": '130px'}}
                    value={heroDescr}
                    onChange={(e) => setHeroDescr(e.target.value)}/>
            </div>

            <div className="mb-3">
                <label htmlFor="element" className="form-label">Выбрать элемент героя</label>
                <select 
                    required
                    className="form-select" 
                    id="element" 
                    name="element"
                    value={heroElement}
                    onChange={(e) => setHeroElement(e.target.value)}>
                    <option value="">Я владею элементом...</option>
                    {renderFilters(filters, filtersLoadingStatus)}
                </select>
            </div>

            <button type="submit" className="btn btn-primary">Создать</button>
        </form>
    )
}

export default HeroesAddForm;			
```						
		
  **[⬆ Наверх](#top)**			

337. ### <a name="337"></a> 

 
    
  **[⬆ Наверх](#top)**			

338. ### <a name="338"></a> Redux Toolkit пример приложения

### index.js		
```jsx harmony
import React from 'react';
import ReactDOM from 'react-dom';
import { Provider } from 'react-redux';
import store from './store';
import './index.css';
import App from './App';

ReactDOM.render(
  <React.StrictMode>
    <Provider store={store}>
      <App />
    </Provider>
  </React.StrictMode>,
  document.getElementById('root')
);		
```
		
### store/index.js
```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import todoReducer from './todoSlice';

export default configureStore({
  reducer: {
    todos: todoReducer,
  },
});		
```
		
### todoSlice.js
```jsx harmony
import { createSlice } from '@reduxjs/toolkit';

const todoSlice = createSlice({
    name: 'todos',
    initialState: {
        todos: [],
    },
    reducers: {
        addTodo(state, action) {
            state.todos.push({
              id: new Date().toISOString(),
              text: action.payload.text,
              completed: false,
            });
        },
        toggleComplete(state, action) {
            const toggledTodo = state.todos.find(todo => todo.id === action.payload.id);
            toggledTodo.completed = !toggledTodo.completed;
        },
        removeTodo(state, action) {
            state.todos = state.todos.filter(todo => todo.id !== action.payload.id);
        }
    },
});

export const {addTodo, toggleComplete, removeTodo} = todoSlice.actions;

export default todoSlice.reducer;		
```		

### App.jsx
```jsx harmony
import {useState} from 'react';
import { useDispatch } from 'react-redux';

import { addTodo } from './store/todoSlice';
import NewTodoForm from './components/NewTodoForm';
import TodoList from './components/TodoList';

import './App.css';


function App() {
  const [text, setText] = useState('');
  const dispatch = useDispatch();

  const handleAction = () => {
    if(text.trim().length) {
      dispatch(addTodo({text}));
      setText('');
    }
  }

  return (
    <div className='App'>
      <NewTodoForm
        value={text}
        updateText={setText}
        handleAction={handleAction}
      />
      <TodoList />
    </div>
  );
}

export default App;		
```		

### TodoList.jsx
```jsx harmony
import { useSelector } from 'react-redux';
import TodoItem from './TodoItem';

const TodoList = () => {
    const todos = useSelector(state => state.todos.todos);

  return (
    <ul>
      {todos.map((todo) => (
        <TodoItem
          key={todo.id}
          {...todo}
        />
      ))}
    </ul>
  );
};

export default TodoList;		
```		

### TodoItem.jsx
```jsx harmony
import { useDispatch } from 'react-redux';
import {toggleComplete, removeTodo} from '../store/todoSlice';

const TodoItem = ({ id, text, completed }) => {
  const dispatch = useDispatch();

  return (
    <li>
      <input
        type='checkbox'
        checked={completed}
        onChange={() => dispatch(toggleComplete({ id }))}
      />
      <span>{text}</span>
      <span onClick={() => dispatch(removeTodo({id}))}>&times;</span>
    </li>
  );
};

export default TodoItem;		
```		

### NewTodoForm.jsx
```jsx harmony
const NewTodoForm = ({ value, updateText, handleAction }) => {
  return (
    <label>
      <input
        placeholer='new todo'
        value={value}
        onChange={(e) => updateText(e.target.value)}
      />
      <button onClick={handleAction}>Add todo</button>
    </label>
  );
};

export default NewTodoForm;		
```			

## Typescript + Redux Toolkit
		
### index.tsx
```jsx harmony
import ReactDOM from 'react-dom/client';
import {Provider} from 'react-redux';
import store from './store';
import './index.css';
import App from './App';

const root = ReactDOM.createRoot(
  document.getElementById('root') as HTMLElement
);
root.render(
  <Provider store={store}>
    <App />
  </Provider>
);		
```		

### store/index.ts
```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import todoReducer from './todoSlice';

const store = configureStore({
  reducer: {
    todos: todoReducer,
  },
});

export default store;

export type RootState = ReturnType<typeof store.getState>;
export type AppDispatch = typeof store.dispatch;		
```		

### hooks.ts
```jsx harmony
import {useDispatch, useSelector, TypedUseSelectorHook} from 'react-redux';
import type {RootState, AppDispatch} from './store';

export const useAppDispatch = () => useDispatch<AppDispatch>();
export const useAppSelector: TypedUseSelectorHook<RootState> = useSelector;		
```		

### todoSlice.ts
```jsx harmony
import { createSlice, PayloadAction } from '@reduxjs/toolkit';

type Todo = {
  id: string;
  title: string;
  completed: boolean;
}

type TodosState = {
  list: Todo[];
}

const initialState: TodosState = {
  list: [],
}

const todoSlice = createSlice({
  name: 'todos',
  initialState,
  reducers: {
    addTodo(state, action: PayloadAction<string>) {
      state.list.push({
        id: new Date().toISOString(),
        title: action.payload,
        completed: false,
      });
    },
    toggleComplete(state, action: PayloadAction<string>) {
      const toggledTodo = state.list.find(todo => todo.id === action.payload);
      if (toggledTodo) {
        toggledTodo.completed = !toggledTodo.completed;
      }
    },
    removeTodo(state, action: PayloadAction<string>) {
      state.list = state.list.filter(todo => todo.id !== action.payload);
    }
  },
});

export const { addTodo, toggleComplete, removeTodo } = todoSlice.actions;

export default todoSlice.reducer;		
```		

### App.tsx
```jsx harmony
import { useState } from 'react';
import { useAppDispatch } from './hook';
import { addTodo } from './store/todoSlice';
import NewTodoForm from './components/NewTodoForm';
import TodoList from './components/TodoList';

import './App.css';


function App() {
  const [text, setText] = useState('');
  const dispatch = useAppDispatch();

  const handleAction = () => {
    if (text.trim().length) {
      dispatch(addTodo(text));
      setText('');
    }
  }

  return (
    <div className='App'>
      <NewTodoForm
        value={text}
        updateText={setText}
        handleAction={handleAction}
      />
      <TodoList />
    </div>
  );
}

export default App;		
```		

### TodoList.tsx
```jsx harmony
import { useAppSelector } from '../hook';
import TodoItem from './TodoItem';

const TodoList: React.FC = () => {
  const todos = useAppSelector(state => state.todos.list);

  return (
    <ul>
      {todos.map((todo) => (
        <TodoItem
          key={todo.id}
          {...todo}
        />
      ))}
    </ul>
  );
};

export default TodoList;		
```		

### TodoItem.tsx
```jsx harmony
import { useAppDispatch } from '../hook';
import { toggleComplete, removeTodo } from '../store/todoSlice';

interface TodoItemProps {
  id: string,
  title: string,
  completed: boolean,
}

const TodoItem: React.FC<TodoItemProps> = ({ id, title, completed }) => {
  const dispatch = useAppDispatch();

  return (
    <li>
      <input
        type='checkbox'
        checked={completed}
        onChange={() => dispatch(toggleComplete(id))}
      />
      <span>{title}</span>
      <span onClick={() => dispatch(removeTodo(id))}>&times;</span>
    </li>
  );
};

export default TodoItem;		
```
		
### NewTodoForm.tsx
```jsx harmony
interface NewTodoFormProps {
  value: string,
  updateText: (str: string) => void,
  handleAction: () => void,
}

const NewTodoForm: React.FC<NewTodoFormProps> = ({ value, updateText, handleAction }) => {
  return (
    <label>
      <input
        placeholder='new todo'
        value={value}
        onChange={(e) => updateText(e.target.value)}
      />
      <button onClick={handleAction}>Add todo</button>
    </label>
  );
};

export default NewTodoForm;		
```				
		
  **[⬆ Наверх](#top)**			

339. ### <a name="339"></a> Redux Toolkit пример 2

### index.js
```jsx harmony
import React from 'react';
import ReactDOM from 'react-dom';
import { store } from './store/store';
import { Provider } from 'react-redux';
import './index.css';
import App from './App';

ReactDOM.render(
  <React.StrictMode>
    <Provider store={store}>
      <App />
    </Provider>
  </React.StrictMode>,
  document.getElementById('root')
);		
```		

### store.js
```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import userSlice from '../features/user/userSlice';
import todoSlice from '../features/todo/todoSlice';
import postSlice from '../features/post/postSlice';

export const store = configureStore({
  reducer: {
    user: userSlice,
    todo: todoSlice,
    post: postSlice,
  },
});		
```		

### App.js
```jsx harmony
import React from 'react';
import Form from './components/Form';
import TodoItem from './components/TodoItem';
import User from './components/User';
import Posts from './components/Posts';
import { useSelector } from 'react-redux';

function App() {
  return (
    <div className='min-h-screen h-full w-screen bg-indigo-400'>
      <div className='container mx-auto px-4'>
        <header className='flex gap-20 '>
          <div className='w-1/3'>
            <h1 className='font-bold my-5'>Redux Toolkit State Change</h1>
            <User />
          </div>
          <div className='w-1/3'>
            <h1 className='font-bold my-5'>Redux Toolkit Todo App</h1>
            <Form />

            {todos.map((todo) => (
              <TodoItem key={todo.id} todo={todo} />
            ))}
          </div>
          <div className='w-1/3'>
            <h1 className='font-bold my-5'>Redux Toolkit Async Thunk</h1>
            <Posts />
          </div>
        </header>
      </div>
    </div>
  );
}

export default App;		
```

## Приложение 1	
		
### userSlice.js		
```jsx harmony
import { createSlice } from '@reduxjs/toolkit';

const initialState = {
  firstName: '',
  lastName: '',
};

export const userSlice = createSlice({
  name: 'user',
  initialState,
  reducers: {
    setFirstName: (state, action) => {
      state.firstName = action.payload;
    },
    setLastName: (state, action) => {
      state.lastName = action.payload;
    },
  },
});

export const { setFirstName, setLastName } = userSlice.actions;

export default userSlice.reducer;		
```		

### User.js
```jsx harmony
import React from 'react';
import FirstName from './FirstName';
import LastName from './LastName';
import { useDispatch } from 'react-redux';
import { setFirstName, setLastName } from '../features/user/userSlice';

const User = () => {
  const dispatch = useDispatch();

  return (
    <div className='flex flex-col'>
      <input
        type='text'
        placeholder='First Name'
        onChange={(e) => {
          dispatch(setFirstName(e.target.value));
        }}
        className='w-full p-1 mb-2 focus:outline-none focus:border-lime-500 focus: border-2 placeholder:text-sm'
      />
      <input
        type='text'
        placeholder='Second Name'
        onChange={(e) => {
          dispatch(setLastName(e.target.value));
        }}
        className='w-full p-1 mb-2 focus:outline-none focus:border-lime-500 focus: border-2 placeholder:text-sm'
      />
      <div className='flex gap-20 py-5'>
        <div className='flex flex-col'>
          <div className='flex font-light'>First Name:</div>
          <div className='flex'>
            <FirstName />
          </div>
        </div>

        <div className='flex flex-col'>
          <div className='flex font-light'>Last Name:</div>
          <div className='flex'>
            <LastName />
          </div>
        </div>
      </div>
    </div>
  );
};

export default User;		
```		

### FirstName.js
```jsx harmony
import React from 'react';
import { useSelector } from 'react-redux';

const FirstName = () => {
  const name = useSelector((state) => state.user.firstName);

  return <div className='font-bold'>{name}</div>;
};

export default FirstName;		
```

### LastName
```jsx harmony
import React from 'react';
import { useSelector } from 'react-redux';

const LastName = () => {
  const lastname = useSelector((state) => state.user.lastName);

  return <div className='font-bold'>{lastname}</div>;
};

export default LastName;		
```					

## Приложение 2

### App.js
```jsx harmony
import React from 'react';
import Form from './components/Form';
import TodoItem from './components/TodoItem';
import User from './components/User';
import Posts from './components/Posts';
import { useSelector } from 'react-redux';

function App() {
  const todos = useSelector((state) => state.todo.todos);
		
  return (
    <div className='min-h-screen h-full w-screen bg-indigo-400'>
      <div className='container mx-auto px-4'>
        <header className='flex gap-20 '>
          <div className='w-1/3'>
            <h1 className='font-bold my-5'>Redux Toolkit State Change</h1>
            <User />
          </div>
          <div className='w-1/3'>
            <h1 className='font-bold my-5'>Redux Toolkit Todo App</h1>
            <Form />

            {todos?.map((todo) => (
              <TodoItem key={todo.id} todo={todo} />
            ))}
          </div>
          <div className='w-1/3'>
            <h1 className='font-bold my-5'>Redux Toolkit Async Thunk</h1>
            <Posts />
          </div>
        </header>
      </div>
    </div>
  );
}

export default App;		
```		
		
### todoSlice.js
```jsx harmony
import { createSlice } from '@reduxjs/toolkit';

const initialState = {
  todos: [],
};

export const todoSlice = createSlice({
  name: 'todos',
  initialState,
  reducers: {
    addTodo: (state, action) => {
      state.todos.push(action.payload);
    },
    toggleCompletedTodo: (state, action) => {
      const toggleTodo = state.todos.find((todo) => todo.id === action.payload);
      toggleTodo.completed = !toggleTodo.completed;
    },
    removeTodo: (state, action) => {
      state.todos = state.todos.filter((todo) => todo.id !== action.payload);
    },
  },
});

export const { addTodo, toggleCompletedTodo, removeTodo } = todoSlice.actions;
export default todoSlice.reducer;		
```		

### Form.js
```jsx harmony
import React from 'react';
import { useDispatch } from 'react-redux';
import { addTodo } from '../features/todo/todoSlice';
import { v4 } from 'uuid';

const Form = () => {
  const dispatch = useDispatch();
  const [todoValue, setTodoValue] = React.useState('');

  const addTodoHandler = () => {
    const todo = {
      id: v4(),
      text: todoValue,
      completed: false,
    };

    dispatch(addTodo(todo))
    setTodoValue('')
  };

  return (
    <form className='w-full flex' onSubmit={(e) => e.preventDefault()}>
      <input
        type='text'
        value={todoValue}
        placeholder='Type something...'
        onChange={(e) => setTodoValue(e.target.value)}
        className='w-full p-1 focus:outline-none focus:border-lime-500 focus: border-2 placeholder:text-sm'
      />
      <button
        type='submit'
        className='shrink-0 bg-lime-300  hover:bg-lime-400 transition-all px-3 text-sm'
        onClick={() => addTodoHandler()}
      >
        Submit
      </button>
    </form>
  );
};

export default Form;		
```		

### TodoItem.js
```jsx harmony
import React from 'react';
import { useDispatch } from 'react-redux';
import { toggleCompletedTodo, removeTodo } from '../features/todo/todoSlice';

const TodoItem = ({ todo }) => {
  const dispatch = useDispatch();

  const toggleTodoHandler = (id) => {
    dispatch(toggleCompletedTodo(id));
  };

  const removeTodoHandler = (id) => {
    dispatch(removeTodo(id));
  };

  return (
    <div className='flex justify-between items-center my-2'>
      <div
        onClick={() => toggleTodoHandler(todo.id)}
        className='text-sm px-4 py-2 cursor-pointer bg-lime-300 hover:bg-lime-400'
      >
        Complete
      </div>
      <div
        className={`text-sm ${
          todo.completed ? 'line-through font-medium text-lime-400' : ''
        }`}
      >
        {todo.text}
      </div>
      <div
        onClick={() => removeTodoHandler(todo.id)}
        className='text-sm px-4 py-2 flex bg-red-400 hover:bg-red-500 transition-all text-white cursor-pointer'
      >
        Delete
      </div>
    </div>
  );
};

export default TodoItem;		
```		

## Приложение 3

### postSlice.js
```jsx harmony
import { createSlice, createAsyncThunk } from '@reduxjs/toolkit';
import axios from 'axios';

const initialState = {
  posts: [],
};

export const getPosts = createAsyncThunk(
  'posts/getPosts',
  async (_, { rejectWithValue, dispatch }) => {
    const res = await axios.get('https://jsonplaceholder.typicode.com/posts');
    dispatch(setPosts(res.data));
  }
);

export const deletePostById = createAsyncThunk(
  'posts/deletePostById',
  async (id, { rejectWithValue, dispatch }) => {
    await axios.delete(`https://jsonplaceholder.typicode.com/posts/${id}`);
    dispatch(deletePost(id));
  }
);

export const postSlice = createSlice({
  name: 'posts',
  initialState,
  reducers: {
    setPosts: (state, action) => {
      state.posts = action.payload;
    },
    deletePost: (state, action) => {
      state.posts = state.posts.filter((post) => post.id !== action.payload);
    },
  },
  extraReducers: {
    [getPosts.fulfilled]: () => console.log('getPosts: fullfiled'),
    [getPosts.pending]: () => console.log('getPosts: pending'),
    [getPosts.rejected]: () => console.log('getPosts: rejected'),
    [deletePostById.fulfilled]: () => console.log('deletePostById: fullfiled'),
    [deletePostById.pending]: () => console.log('deletePostById: pending'),
    [deletePostById.rejected]: () => console.log('deletePostById: rejected'),
  },
});

export const { setPosts, deletePost } = postSlice.actions;

export default postSlice.reducer;		
```		

### Posts.js
```jsx harmony
import React from 'react';
import PostItem from './PostItem';
import { useDispatch, useSelector } from 'react-redux';
import { getPosts } from '../features/post/postSlice';

const Posts = () => {
  const dispatch = useDispatch();
  const posts = useSelector((state) => state.post.posts);

  return (
    <div>
      <button
        onClick={() => dispatch(getPosts())}
        type='submit'
        className='bg-lime-300  hover:bg-lime-400 transition-all p-2 text-sm'
      >
        Get posts
      </button>

      {posts?.map((post) => (
        <PostItem key={post.title} post={post} />
      ))}
    </div>
  );
};

export default Posts;		
```		

### PostItem.js
```jsx harmony
import React from 'react';
import { deletePostById } from '../features/post/postSlice';
import { useDispatch } from 'react-redux';

const PostItem = ({ post }) => {
  const dispatch = useDispatch();

  return (
    <div
      onClick={() => dispatch(deletePostById(post.id))}
      className='flex w-full bg-indigo-500 hover:bg-indigo-300 transition-all py-1 px-2 text-white rounded-sm cursor-pointer mt-4'
    >
      {post.title}
    </div>
  );
};

export default PostItem;		
```					
		
  **[⬆ Наверх](#top)**			

340. ### <a name="340"></a> Redux Toolkit createAsyncThunk

### index.js
```jsx harmony
import React from 'react';
import ReactDOM from 'react-dom';
import { Provider } from 'react-redux';
import store from './store';
import './index.css';
import App from './App';

ReactDOM.render(
  <React.StrictMode>
    <Provider store={store}>
      <App />
    </Provider>
  </React.StrictMode>,
  document.getElementById('root')
);		
```		
 
### store/index.js
```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import todoReducer from './todoSlice';

export default configureStore({
  reducer: {
    todos: todoReducer,
  },
});		
```		

### todoSlice.js
```jsx harmony
import { createSlice, createAsyncThunk } from '@reduxjs/toolkit';

export const fetchTodos = createAsyncThunk(
    'todos/fetchTodos',
    async function(_, {rejectWithValue}) {
        try {
            const response = await fetch('https://jsonplaceholder.typicode.com/todos?_limit=10');
            
            if (!response.ok) {
                throw new Error('Server Error!');
            }
    
            const data = await response.json();
    
            return data;
        } catch (error) {
            return rejectWithValue(error.message);
        }
    }
);

export const deleteTodo = createAsyncThunk(
    'todos/deleteTodo',
    async function(id, {rejectWithValue, dispatch}) {
        try {
            const response = await fetch(`https://jsonplaceholder.typicode.com/todos/${id}`, {
                method: 'DELETE',
            })

            if (!response.ok) {
                throw new Error('Can\'t delete task. Server error.');
            }

            dispatch(removeTodo({id}));

        } catch (error) {
            return rejectWithValue(error.message);
        }
    }
);

export const toggleStatus = createAsyncThunk(
    'todos/toggleStatus',
    async function (id, {rejectWithValue, dispatch, getState}) {
        const todo = getState().todos.todos.find(todo => todo.id === id);

        try {
            const response = await fetch(`https://jsonplaceholder.typicode.com/todos/${id}`, {
                method: 'PATCH',
                headers: {
                    'Content-Type': 'application/json',
                },
                body: JSON.stringify({
                    completed: !todo.completed,
                })
            });

            if (!response.ok) {
                throw new Error('Can\'t toggle status. Server error.');
            }

            dispatch(toggleComplete({id}));

        } catch (error) {
            return rejectWithValue(error.message)
        }
    }
);

export const addNewTodo = createAsyncThunk(
    'todos/addNewTodo',
    async function (text, {rejectWithValue, dispatch}) {
        try {
            const todo = {
                title: text,
                userId: 1,
                completed: false,
            };

            const response = await fetch('https://jsonplaceholder.typicode.com/todos', {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify(todo)
            });

            if (!response.ok) {
                throw new Error('Can\'t add task. Server error.');
            }

            const data = await response.json();
            dispatch(addTodo(data));

        } catch (error) {
            return rejectWithValue(error.message);
        }
    }
);

const setError = (state, action) => {
    state.status = 'rejected';
    state.error = action.payload;
}

const todoSlice = createSlice({
    name: 'todos',
    initialState: {
        todos: [],
        status: null,
        error: null,
    },
    reducers: {
        addTodo(state, action) {
            state.todos.push(action.payload);
        },
        toggleComplete(state, action) {
            const toggledTodo = state.todos.find(todo => todo.id === action.payload.id);
            toggledTodo.completed = !toggledTodo.completed;
        },
        removeTodo(state, action) {
            state.todos = state.todos.filter(todo => todo.id !== action.payload.id);
        }
    },
    extraReducers: {
        [fetchTodos.pending]: (state) => {
            state.status = 'loading';
            state.error = null;
        },
        [fetchTodos.fulfilled]: (state, action) => {
            state.status = 'resolved';
            state.todos = action.payload;
        },
        [fetchTodos.rejected]: setError,
        [deleteTodo.rejected]: setError,
        [toggleStatus.rejected]: setError,
    },
});

const {addTodo, toggleComplete, removeTodo} = todoSlice.actions;

export default todoSlice.reducer;		
```		

### App.js
```jsx harmony
import {useState, useEffect} from 'react';
import { useDispatch, useSelector } from 'react-redux';

import { addNewTodo, fetchTodos } from './store/todoSlice';
import NewTodoForm from './components/NewTodoForm';
import TodoList from './components/TodoList';

import './App.css';


function App() {
  const [text, setText] = useState('');
  const {status, error} = useSelector(state => state.todos);
  const dispatch = useDispatch();

  const handleAction = () => {
    if(text.trim().length) {
      dispatch(addNewTodo(text));
      setText('');
    }
  }

  useEffect(() => {
    dispatch(fetchTodos());
  }, [dispatch]);

  return (
    <div className='App'>
      <NewTodoForm
        value={text}
        updateText={setText}
        handleAction={handleAction}
      />

      {status === 'loading' && <h2>Loading...</h2>}
      {error &&  <h2>An error occured: {error}</h2>}

      <TodoList />
    </div>
  );
}

export default App;		
```		

### TodoList.js
```jsx harmony
import { useSelector } from 'react-redux';
import TodoItem from './TodoItem';

const TodoList = () => {
    const todos = useSelector(state => state.todos.todos);

  return (
    <ul>
      {todos.map((todo) => (
        <TodoItem
          key={todo.id}
          {...todo}
        />
      ))}
    </ul>
  );
};

export default TodoList;		
```		

### TodoItem.js
```jsx harmony
import { useDispatch } from 'react-redux';
import {toggleStatus, deleteTodo} from '../store/todoSlice';

const TodoItem = ({ id, title, completed }) => {
  const dispatch = useDispatch();

  return (
    <li>
      <input
        type='checkbox'
        checked={completed}
        onChange={() => dispatch(toggleStatus(id))}
      />
      <span>{title}</span>
      <span onClick={() => dispatch(deleteTodo(id))}>&times;</span>
    </li>
  );
};

export default TodoItem;		
```

### NewTodoForm.js
```jsx harmony
const NewTodoForm = ({ value, updateText, handleAction }) => {
  return (
    <label>
      <input
        placeholer='new todo'
        value={value}
        onChange={(e) => updateText(e.target.value)}
      />
      <button onClick={handleAction}>Add todo</button>
    </label>
  );
};

export default NewTodoForm;		
```		

## Typescript + Redux Toolkit
		
### index.tsx
```jsx harmony
import ReactDOM from 'react-dom/client';
import {Provider} from 'react-redux';
import store from './store';
import './index.css';
import App from './App';
import reportWebVitals from './reportWebVitals';

const root = ReactDOM.createRoot(
  document.getElementById('root') as HTMLElement
);
root.render(
  <Provider store={store}>
    <App />
  </Provider>
);		
```		

### store/index.ts
```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import todoReducer from './todoSlice';

const store = configureStore({
  reducer: {
    todos: todoReducer,
  },
});

export default store;

export type RootState = ReturnType<typeof store.getState>;
export type AppDispatch = typeof store.dispatch;		
```		

### hooks.ts
```jsx harmony
import {useDispatch, useSelector, TypedUseSelectorHook} from 'react-redux';
import type {RootState, AppDispatch} from './store';

export const useAppDispatch = () => useDispatch<AppDispatch>();
export const useAppSelector: TypedUseSelectorHook<RootState> = useSelector;		
```		

### todoSlice.ts
```jsx harmony
import { createSlice, PayloadAction, createAsyncThunk, AnyAction } from '@reduxjs/toolkit';

type Todo = {
  id: string;
  title: string;
  completed: boolean;
}

type TodosState = {
  list: Todo[];
  loading: boolean;
  error: string | null;
}
export const fetchTodos = createAsyncThunk<Todo[], undefined, {rejectValue: string}>(
    'todos/fetchTodos',
    async function (_, { rejectWithValue }) {
      const response = await fetch('https://jsonplaceholder.typicode.com/todos?_limit=10');

      if (!response.ok) {
        return rejectWithValue('Server Error!');
      }

      const data = await response.json();

      return data;
    }
);

export const addNewTodo = createAsyncThunk<Todo, string, { rejectValue: string }>(
  'todos/addNewTodo',
  async function (text, { rejectWithValue }) {
      const todo = {
        title: text,
        userId: 1,
        completed: false,
      };

      const response = await fetch('https://jsonplaceholder.typicode.com/todos', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json'
        },
        body: JSON.stringify(todo)
      });

      if (!response.ok) {
        return rejectWithValue('Can\'t add task. Server error.');
      }

      return (await response.json()) as Todo;
  }
);

export const toggleStatus = createAsyncThunk<Todo, string, { rejectValue: string, state: { todos: TodosState} }>(
  'todos/toggleStatus',
  async function (id, { rejectWithValue, getState }) {
    const todo = getState().todos.list.find(todo => todo.id === id);

    if (todo) {
      const response = await fetch(`https://jsonplaceholder.typicode.com/todos/${id}`, {
        method: 'PATCH',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify({
          completed: !todo.completed,
        })
      });
  
      if (!response.ok) {
        return rejectWithValue('Can\'t toggle status. Server error.');
      }
  
      return (await response.json()) as Todo; 
    }

    return rejectWithValue('No such todo in the list!')
  }
);

export const deleteTodo = createAsyncThunk<string, string, { rejectValue: string }>(
  'todos/deleteTodo',
  async function (id, { rejectWithValue }) {
    const response = await fetch(`https://jsonplaceholder.typicode.com/todos/${id}`, {
      method: 'DELETE',
    })

    if (!response.ok) {
      return rejectWithValue('Can\'t delete task. Server error.');
    }

    return id;
  }
);

const initialState: TodosState = {
  list: [],
  loading: false,
  error: null,
}

const todoSlice = createSlice({
  name: 'todos',
  initialState,
  reducers: {},
  extraReducers: (builder) => {
    builder
      .addCase(fetchTodos.pending, (state) => {
        state.loading = true;
        state.error = null;
      })
      .addCase(fetchTodos.fulfilled, (state, action) => {
        state.list = action.payload;
        state.loading = false;
      })
      .addCase(addNewTodo.pending, (state) => {
        state.error = null;
      })
      .addCase(addNewTodo.fulfilled, (state, action) => {
        state.list.push(action.payload);
      })
      .addCase(toggleStatus.fulfilled, (state, action) => {
        const toggledTodo = state.list.find(todo => todo.id === action.payload.id);
        if (toggledTodo) {
          toggledTodo.completed = !toggledTodo.completed;
        }
      })
      .addCase(deleteTodo.fulfilled, (state, action) => {
        state.list = state.list.filter(todo => todo.id !== action.payload);
      })
      .addMatcher(isError, (state, action: PayloadAction<string>) => {
        state.error = action.payload;
        state.loading = false;
      });
  }
});

// export const { addTodo, toggleComplete, removeTodo } = todoSlice.actions;

export default todoSlice.reducer;

function isError(action: AnyAction) {
  return action.type.endsWith('rejected');
}		
```		

### App.tsx
```jsx harmony
import { useState, useEffect } from 'react';
import { useAppDispatch, useAppSelector } from './hook';
import { fetchTodos, addNewTodo } from './store/todoSlice';
import NewTodoForm from './components/NewTodoForm';
import TodoList from './components/TodoList';

import './App.css';


function App() {
  const [text, setText] = useState('')
  const { loading, error } = useAppSelector(state => state.todos);;
  const dispatch = useAppDispatch();

  const handleAction = () => {
    if (text.trim().length) {
      dispatch(addNewTodo(text));
      setText('');
    }
  }

  useEffect(() => {
    dispatch(fetchTodos());
  }, [dispatch]);

  return (
    <div className='App'>
      <NewTodoForm
        value={text}
        updateText={setText}
        handleAction={handleAction}
      />

      {loading && <h2>Loading...</h2>}
      {error && <h2>An error occured: {error}</h2>}
      <TodoList />
    </div>
  );
}

export default App;		
```		

### TodoList.tsx
```jsx harmony
import { useAppSelector } from '../hook';
import TodoItem from './TodoItem';

const TodoList: React.FC = () => {
  const todos = useAppSelector(state => state.todos.list);

  return (
    <ul>
      {todos.map((todo) => (
        <TodoItem
          key={todo.id}
          {...todo}
        />
      ))}
    </ul>
  );
};

export default TodoList;		
```		

### TodoItem.tsx
```jsx harmony
import { useAppDispatch } from '../hook';
import { toggleStatus, deleteTodo } from '../store/todoSlice';

interface TodoItemProps {
  id: string,
  title: string,
  completed: boolean,
}

const TodoItem: React.FC<TodoItemProps> = ({ id, title, completed }) => {
  const dispatch = useAppDispatch();

  return (
    <li>
      <input
        type='checkbox'
        checked={completed}
        onChange={() => dispatch(toggleStatus(id))}
      />
      <span>{title}</span>
      <span onClick={() => dispatch(deleteTodo(id))}>&times;</span>
    </li>
  );
};

export default TodoItem;		
```		

### NewTodoForm.tsx
```jsx harmony
interface NewTodoFormProps {
  value: string,
  updateText: (str: string) => void,
  handleAction: () => void,
}

const NewTodoForm: React.FC<NewTodoFormProps> = ({ value, updateText, handleAction }) => {
  return (
    <label>
      <input
        placeholder='new todo'
        value={value}
        onChange={(e) => updateText(e.target.value)}
      />
      <button onClick={handleAction}>Add todo</button>
    </label>
  );
};

export default NewTodoForm;		
```				
		
  **[⬆ Наверх](#top)**			

341. ### <a name="341"></a> RTK Query

### index.js
```jsx harmony
import React from 'react';
import ReactDOM from 'react-dom';
import { Provider } from 'react-redux';
import './index.css';
import App from './App';
import { store } from './redux';

ReactDOM.render(
  <Provider store={store}>
    <App />
  </Provider>,
  document.getElementById('root')
);		
```		

### db.json
```jsx harmony
{
  "goods": [
    {
      "id": 1,
      "name": "Milk"
    },
    {
      "id": 2,
      "name": "bananas"
    },
    {
      "id": 3,
      "name": "icecream"
    }
  ]
}		
```		

### redux/index.js
```jsx harmony
export * from './store';
export * from './goodsApi';		
```		

### redux/goodsApi.js
```jsx harmony
import { createApi, fetchBaseQuery } from '@reduxjs/toolkit/query/react';

export const goodsApi = createApi({
    reducerPath: 'goodsApi',
    tagTypes: ['Products'],
    baseQuery: fetchBaseQuery({baseUrl: 'http://localhost:3001/'}),
    endpoints: (build) => ({
        getGoods: build.query({
            query: (limit = '') => `goods?${limit && `_limit=${limit}`}`,
            providesTags: (result) => result
              ? [
                  ...result.map(({ id }) => ({ type: 'Products', id })),
                  { type: 'Products', id: 'LIST' },
                ]
              : [{ type: 'Products', id: 'LIST' }],
        }),
        addProduct: build.mutation({
            query: (body) => ({
                url: 'goods',
                method: 'POST',
                body,
            }),
            invalidatesTags: [{type: 'Products', id: 'LIST'}]
        }),
        deleteProduct: build.mutation({
            query: (id) => ({
                url: `goods/${id}`,
                method: 'DELETE',
            }),
            invalidatesTags: [{type: 'Products', id: 'LIST'}]
        })
    })
});

export const {useGetGoodsQuery, useAddProductMutation, useDeleteProductMutation} = goodsApi;		
```		
		
### redux/store.js
```jsx harmony
import { configureStore } from '@reduxjs/toolkit';
import { goodsApi } from './goodsApi';

export const store = configureStore({
    reducer: {
        [goodsApi.reducerPath]: goodsApi.reducer,
    },
    middleware: (getDefaultMiddlware) => getDefaultMiddlware().concat(goodsApi.middleware)
});		
```		

### App.js
```jsx harmony
import { useState } from 'react';
import { useGetGoodsQuery, useAddProductMutation, useDeleteProductMutation } from './redux';

function App() {
  const [count, setCount] = useState('');
  const [newProduct, setNewProduct] = useState('');
  const {data = [], isLoading} = useGetGoodsQuery(count);
  const [addProduct, {isError}] = useAddProductMutation();
  const [deleteProduct] = useDeleteProductMutation();

  const handleAddProduct = async () => {
    if(newProduct) {
      await addProduct({name: newProduct}).unwrap();
      setNewProduct('');
    }
  }

  const handleDeleteProduct = async (id) => {
    await deleteProduct(id).unwrap();
  }

  if (isLoading) return <h1>Loading...</h1>

  return (
    <div>
      <div>
        <input
          type="text"
          value={newProduct}
          onChange={(e) => setNewProduct(e.target.value)}
        />
        <button onClick={handleAddProduct}>Add product</button>
      </div>
      <div>
        <select value={count} onChange={(e) => setCount(e.target.value)}>
          <option value="">all</option>
          <option value="1">1</option>
          <option value="2">2</option>
          <option value="3">3</option>
        </select>
      </div>
      <ul>
        {data.map(item => (
          <li key={item.id} onClick={() => handleDeleteProduct(item.id)}>
            {item.name}
          </li>
        ))}
      </ul>
    </div>
  );
}

export default App;		
```		
		
  **[⬆ Наверх](#top)**		

342. ### <a name="342"></a> 
		
		
  **[⬆ Наверх](#top)**		
		
343. ### <a name="343"></a> 
		
		
  **[⬆ Наверх](#top)**	
		
344. ### <a name="344"></a> 
		
		
  **[⬆ Наверх](#top)**	
		
345. ### <a name="345"></a> 
		
		
  **[⬆ Наверх](#top)**	
		
346. ### <a name="346"></a> 
		
		
  **[⬆ Наверх](#top)**	
		
347. ### <a name="347"></a> 
		
		
  **[⬆ Наверх](#top)**			
		
350. ### <a name="350"></a> Redux

 Redux - это ценный инструмент для управления вашим состоянием, но вы также должны учитывать, подходит ли он для вашей ситуации. Не используйте Redux только потому, что кто-то сказал, что вам нужно - потратьте некоторое время, чтобы понять потенциальные выгоды и компромиссы с его использованием.
	
*Redux* - это стабильный (предсказуемый) контейнер для хранения состояния JavaScript-приложений, основанный на паттерне проектирования Flux. Redux может использоваться с React и любой другой библиотекой. Он легкий (около 2 Кб) и не имеет зависимостей.	

![2](https://user-images.githubusercontent.com/80325645/152787114-911ae428-304e-49c9-bafd-63a93d54466a.jpg)  
	  
### Redux следует трем фундаментальным принципам:

1. Единственный источник истины: состояние всего приложения хранится в древовидном объекта - в одном хранилище. Единственное состояние-дерево облегчает наблюдение за изменениями и отладку или инспектирование приложения
2. Состояние доступно только для чтения: единственный способ изменить состояние заключается в запуске операции - объекте, описывающем произошедшее. Это позволяет гарантировать, что ни представления, ни сетевые коллбеки не буду иметь возможности изменять состояние напрямую
3. Изменения производятся с помощью "чистых" функций: для определения того, как изменяется состояние в зависимости от операции, создаются редукторы (reducers). Редукторы - это "чистые" функции, принимающие предыдущее состояние в качестве аргумента и возвращающие новое


### В чем заключаются преимущества и недостатки Redux?***

**Преимущества**

* Хранилище позволяет любому компоненту получать состояние без передачи пропов
* Состояние сохраняется даже при размонтировании компонента
* Предотвращает ненужные повторные рендеринги благодаря поверхностному сравнению нового и старого состояния
* Разделение UI и управления данными облегчает тестирование
* Сохраняется история изменения состояния, что позволяет легко повторять или отменять операции

**Недостатки**

* Отсутствует инкапсуляция. Любой компонент имеет доступ к данным, что может привести к проблемам с безопасностью
* Много шаблонного кода. Ограниченный дизайн
* Поскольку состояние является иммутабельным, редуктор обновляет его, каждый раз возвращая новое состояние, что влечет дополнительные расходы памяти	
	
	
*Redux может быть описан тремя фундаментальными принципами:*

### Единственный источник правды
	
Состояние всего вашего приложения сохранено в дереве объектов внутри одного стора.

Это облегчает создание универсальных приложений. Состояние на сервере может быть сериализировано и отправлено на клиент без дополнительных усилий. Это упрощает отладку приложения, когда мы имеем дело с единственным деревом состояния. Вы также можете сохранять состояние вашего приложения для ускорения процесса разработки. И с единственным деревом состояния вы получаете функциональность типа Undo/Redo из коробки.
```jsx harmony
console.log(store.getState())

{
  visibilityFilter: 'SHOW_ALL',
  todos: [
    {
      text: 'Consider using Redux',
      completed: true,
    },
    {
      text: 'Keep all state in a single tree',
      completed: false
    }
  ]
}
```
	
### Состояние только для чтения
	
Единственный способ изменить состояние — это применить экшен — объект, который описывает, что случится.

Это гарантирует, что представления или функции, реагирующие на события сети (network callbacks), никогда не изменят состояние напрямую. Поскольку все изменения централизованы и применяются последовательно в строгом порядке, поэтому нет необходимости следить за "гонкой состояний". Экшены — это всего лишь простые объекты, поэтому они могут быть залогированы, сериализированы, сохранены и затем воспроизведены для отладки или тестирования.
```jsx harmony
store.dispatch({
  type: 'COMPLETE_TODO',
  index: 1
})

store.dispatch({
  type: 'SET_VISIBILITY_FILTER',
  filter: 'SHOW_COMPLETED'
})
```
	
### Мутации написаны, как чистые функции
	
Для определения того, как дерево состояния будет трансформировано экшенами, вы пишете чистые редьюсеры.

Редьюсеры — это просто чистые функции, которые берут предыдущее состояние и экшен и возвращают новое состояние. Не забывайте возвращать новый объект состояния вместо того, чтобы изменять предыдущее. Вы можете начать с одного редьюсера, но в дальнейшем, когда ваше приложение разрастется, вы можете разделить его на более маленькие редьюсеры, которые управляют отдельными частями дерева состояния. Поскольку редьюсеры — это просто функции, вы можете контролировать порядок, в котором они вызываются, отправлять дополнительные данные или даже писать переиспользуемые редьюсеры для общих задач, например, для пагинации.
```jsx harmony
function visibilityFilter(state = 'SHOW_ALL', action) {
  switch (action.type) {
    case 'SET_VISIBILITY_FILTER':
      return action.filter
    default:
      return state
  }
}

function todos(state = [], action) {
  switch (action.type) {
    case 'ADD_TODO':
      return [
        ...state,
        {
          text: action.text,
          completed: false
        }
      ]
    case 'COMPLETE_TODO':
      return state.map((todo, index) => {
        if (index === action.index) {
          return Object.assign({}, todo, {
            completed: true
          })
        }
        return todo
      })
    default:
      return state
  }
}

import { combineReducers, createStore } from 'redux'
let reducer = combineReducers({ visibilityFilter, todos })
let store = createStore(reducer)	
```

	
### Сущности в React:
- Actions
- Reducers
- Store
- Dispatch	
	
	
	
*Flux* - это *парадигма проектирования приложений*, являющаяся альтернативой более традиционному паттерну MVC. Это не фреймворк или библиотека, а новый вид архитектуры, разработанный специально для React с учетом концепции однонаправленного потока данных. Facebook использует данный паттерн в своих внутренних проектах.	
	
### Отличия между Redux и Flux можно свести к следующему:

1. Недопустимость мутаций: во Flux состояние может быть изменяемым, а Redux требует, чтобы состояние было иммутабельным, и многие библиотеки для Redux исходят из предположения, что вы никогда не будете менять состояние напрямую. Вы можете обеспечить иммутабельность состояния с помощью таких пакетов, как `redux-immutable-state-invariant`, `Immutable.js` или условившись с другими членами команды о написании иммутабельного кода
2. Осторожность в выборе библиотек: Flux не пытается решать такие проблемы, как повторное выполнение/отмена выполнения, стабильность (постоянство) кода или проблемы, связанные с обработкой форм, явно, а Redux имеет возможность к расширению с помощью промежуточного программного обеспечения (middleware) и предохранителей хранилища, что породило богатую экосистему
3. Отсутствие интеграции с Flow: Flux позволяет осуществлять очень выразительную статическую проверку типов, а Redux пока не поддерживает такой возможности
    
  **[⬆ Наверх](#top)**
	
351. ### <a name="351"></a> connect. HOC

 ### Понимание того, что такое connect.
	
Для того, чтобы иметь возможность использовать хранилище в контейнере, необходимо выполнить следующие шаги:

1. **Использовать метод `mapStateToProps()`:** он передает переменные состояния из хранилища в определенные вами пропы
2. **Подключить пропы к контейнеру:** объект, возвращенный `mapStateToProps()` подключается к контейнеру. Вы можете импортировать `connect()` из `react-redux`:

 ```jsx harmony
 import React from 'react'
 import { connect } from 'react-redux'

 class App extends React.Component {
   render() {
     return <div>{this.props.containerData}</div>
   }
 }

 function mapStateToProps(state) {
   return { containerData: state.data }
 }

 export default connect(mapStateToProps)(App)
 ```	

Лучшим способом получить хранилище в компоненте является использование функции `connect()`, которая создает новый компонент, оборачивающий существующий. Этот паттерн называется *компоненты высшего порядка*, он является предпочтительным способом расширения функциональности компонента в React. Это позволяет передавать в компонент состояние и "создателей операций" (action creators), в том числе, при обновлении хранилища.

Создадим компонент `FilterLink` с помощью `connect()`:

```javascript
import { connect } from 'react-redux'
import { setVisibilityFilter } from '../actions'
import Link from '../components/Link'

const mapStateToProps = (state, ownProps) => ({
active: ownProps.filter === state.visibilityFilter
})

const mapDispatchToProps = (dispatch, ownProps) => ({
onClick: () => dispatch(setVisibilityFilter(ownProps.filter))
})

const FilterLink = connect(
mapStateToProps,
mapDispatchToProps
)(Link)

export default FilterLink
```

Поскольку такой вариант имеет несколько оптимизаций производительности и, как правило, меньше подвержен "багам", разработчики Redux почти всегда рекомендуют использовать `connect()` вместо прямого доступа к хранилищу (с помощью API контекста).

```javascript
     class MyComponent {
       someMethod() {
         doSomethingWith(this.context.store)
       }
     }
```	
	
	
### HOC
	
Higher-order component (HOC) - это функция, принимающая компонент и возвращающая новый компонент. Это паттерн, производный от композиционной природы React.

Мы называем такие компоненты *чистыми*, поскольку они могут принимать и динамически предоставлять дочерние компоненты, но не меняют и не копируют их поведение.

```javascript
const EnhancedComponent = higherOrderComponent(WrappedComponent)
```

HOC, обычно, используются для:

1. Обеспечения возможности переиспользования кода, логики, а также для абстрагирования шаблонов
2. Отложенного рендеринга
3. Абстрагирования и манипулирования состоянием
4. Манипулирования пропами	

	
HOC не являются частью React API. HOC является паттерном, производным от композиционной природы React. Компонент преобразует пропы в UI, а HOC трансформирует один компонент в другой. Примерами популярных HOC являются методы `connect()` в Redux и `createContainer()` в Relay.

```js
// HOC.js
import React, { Component } from 'react'

export default function Hoc(HocComponent){
    return class extends Component{
        render(){
            return (
                <div>
                  <HocComponent></HocComponent>
                </div>

            )
        }
    }
}
```

```js
// App.js
import React, { Component } from 'react'
import Hoc from './HOC'

class App extends Component {
  render() {
    return (
      <div>
        Пример компонента высшего порядка!
      </div>
    )
  }
}
App = Hoc(App)
export default App
```

**Обратите внимание:**

* Мы не модифицируем компоненты, а создаем новые
* HOC используются для композиции компонентов для обеспечения возможности повторного использования кода
* HOC являются "чистыми" функциями. Они не имеют побочных эффектов (side effects) и всегда возвращают одинаковые результаты для одних и тех же аргументов
    
  **[⬆ Наверх](#top)**
	
352. ### <a name="352"></a> actions

 *Actions* - это обычные JavaScript-объекты, содержащие данные приложения, которые отправляются в хранилище. Операции должны иметь свойство `type`, указывающее какой тип операции необходимо выполнить. Операции также могут содержать полезную нагрузку (payload) - данные для обновления состояния.

Вот как может выглядеть операция по добавлению новой задачи в список:

```jsx harmony
// здесь используется константа
{
type: ADD_TODO,
text: 'Добавление задачи в список'
}
```
	
Экшены — это структуры, которые передают данные из вашего приложения в стор. Они являются единственными источниками информации для стора. Вы отправляете их в стор, используя метод store.dispatch().

Например, вот экшен, которое представляет добавление нового пункта в список дел:
```jsx harmony
const ADD_TODO = 'ADD_TODO'
```
```jsx harmony	
{
  type: ADD_TODO,
  text: 'Build my first Redux app'
}
```	
Экшены — это обычные JavaScript-объекты. Экшены должны иметь поле type, которое указывает на тип исполняемого экшена. Типы должны быть, как правило, заданы, как строковые константы. После того, как ваше приложение разрастется, вы можете захотеть переместить их в отдельный модуль.
```jsx harmony
import { ADD_TODO, REMOVE_TODO } from '../actionTypes'
```	

Мы добавим еще один тип экшена, который будет отмечать задачу, как выполненную. Мы обращаемся к конкретному todo по index, потому что мы храним их в виде массива. В реальном приложении разумнее генерировать уникальный ID каждый раз, когда что-то новое создается.
```jsx harmony
{
  type: TOGGLE_TODO,
  index: 5
}
```	
Это хорошая идея, передавать как можно меньше данных в каждом экшене. Например, лучше отправить index, чем весь объект todo.

Наконец, мы добавим еще один тип экшена для изменения видимых, в данный момент, задач.
```jsx harmony
{
  type: SET_VISIBILITY_FILTER,
  filter: SHOW_COMPLETED
}
```
	
### Генераторы экшенов (Action Creators)
	
Генераторы экшенов (Action Creators) — не что иное, как функции, которые создают экшены. Довольно просто путать термины “action” и “action creator,” поэтому постарайтесь использовать правильный термин.

В Redux генераторы экшенов (action creators) просто возвращают action:
```jsx harmony
function addTodo(text) {
  return {
    type: ADD_TODO,
    text
  }
}
```	
Это делает их более переносимыми и легкими для тестирования.

В традиционной реализации Flux, генераторы экшенов (action creators) при выполнении часто вызывают dispatch, примерно так:
```jsx harmony
function addTodoWithDispatch(text) {
  const action = {
    type: ADD_TODO,
    text
  }
  dispatch(action)
}
```	
В Redux это не так. Вместо того чтобы на самом деле начать отправку, передайте результат в функцию dispatch():
```jsx harmony
dispatch(addTodo(text))
dispatch(completeTodo(index))
```	
Кроме того, вы можете создать связанный генератор экшена (bound action creator), который автоматически запускает отправку экшена:
```jsx harmony
const boundAddTodo = (text) => dispatch(addTodo(text))
const boundCompleteTodo = (index) => dispatch(completeTodo(index))
```	
Теперь вы можете вызвать его напрямую:
```jsx harmony
boundAddTodo(text)
boundCompleteTodo(index)
```	
Доступ к функции dispatch() может быть получен непосредственно из стора (store) store.dispatch(), но, что более вероятно, вы будете получать доступ к ней при помощи чего-то типа connect() из react-redux. Вы можете использовать функцию bindActionCreators() для автоматического привязывания большого количества генераторов экшенов (action creators) к функции dispatch().

Генератор экшены так же могут быть асинхронными и иметь сайд-эффекты. Вы можете почитать про асинхронные экшены в расширенном руководстве, чтобы узнать, как обрабатывать ответы AJAX и создавать генераторы действий в асинхронном потоке управления. Не переходите к асинхронным экшенам до тех пор, пока вы не завершите базовое руководство, так как оно охватывает другие важные концепции, которые необходимы для продвинутого руководства и асинхронных экшенов.

### Исходный код
	
**actions.js**
	
```jsx harmony	
/*
 * типы экшенов
 */

export const ADD_TODO = 'ADD_TODO'
export const TOGGLE_TODO = 'TOGGLE_TODO'
export const SET_VISIBILITY_FILTER = 'SET_VISIBILITY_FILTER'

/*
 * другие константы
 */

export const VisibilityFilters = {
  SHOW_ALL: 'SHOW_ALL',
  SHOW_COMPLETED: 'SHOW_COMPLETED',
  SHOW_ACTIVE: 'SHOW_ACTIVE'
}

/*
 * генераторы экшенов
 */

export function addTodo(text) {
  return { type: ADD_TODO, text }
}

export function toggleTodo(index) {
  return { type: TOGGLE_TODO, index }
}

export function setVisibilityFilter(filter) {
  return { type: SET_VISIBILITY_FILTER, filter }
}	
```
    
  **[⬆ Наверх](#top)**
	
353. ### <a name="353"></a> reducer

 ### Редьюсеры (Reducers)
	
Редьюсеры определяют, как состояние приложения изменяется в ответ на экшены, отправленные в стор. Помните, что экшены только описывают, _что произошло, но не описывают, как изменяется состояние приложения.

### Проектирование структуры состояния (State)
	
В Redux все состояние приложения хранится в виде единственного объекта. Подумать о его структуре перед написанием кода — довольно неплохая идея. Каково минимальное представление состояния Вашего приложения в виде объекта?

Для нашего todo-приложения, мы хотим хранить две разные сущности:
- Состояние фильтра видимости;
- Актуальный список todo-задач.
	
Часто вы будете понимать, что вам нужно хранить некоторые данные, а также некоторые состояния пользовательского интерфейса в дереве состояний. Это нормально, только старайтесь такие данные не смешивать с данными, которые описывают состояние UI.
```jsx harmony
{
  visibilityFilter: 'SHOW_ALL',
  todos: [
    {
      text: 'Consider using Redux',
      completed: true,
    },
    {
      text: 'Keep all state in a single tree',
      completed: false
    }
  ]
}
```	

### Обработка экшенов
	
Теперь, когда мы определились с тем, как должны выглядеть наши объекты состояния (state objects), мы готовы написать редьюсер для них.
	
`Редьюсер` (reducer) — это чистая функция, которая принимает предыдущее состояние и экшен (state и action) и возвращает следующее состояние (новую версию предыдущего).
```jsx harmony
(previousState, action) => newState
```	
Функция называется редьюсером (reducer) потому, что ее можно передать в Array.prototype.reduce(reducer, ?initialValue). Очень важно, чтобы редьюсеры оставались чистыми функциями. Вот список того, чего никогда нельзя делать в редьюсере:
- Непосредственно изменять то, что пришло в аргументах функции;
- Выполнять какие-либо сайд-эффекты: обращаться к API или осуществлять переход по роутам;
- Вызывать не чистые функции, например Date.now() или Math.random().
	
Мы рассмотрим способы выполнения сайд-эффектов в продвинутом руководстве. На данный момент просто запомните, что редьюсер должен быть чистым. Получая аргументы одного типа, редьюсер должен вычислять новую версию состояния и возвращать ее. Никаких сюрпризов. Никаких сайд-эффектов. Никаких обращений к стороннему API. Никаких изменений (mutations). Только вычисление новой версии состояния.

Исходя из вышенаписанных принципов, давайте начнем писать редьюсер, постепенно обучая его понимать экшены (actions), которые мы описали чуть раньше.

Мы начнем с определения начального состояния (initial state). В первый раз Redux вызовет редьюсер с неопределенным состоянием(state === undefined). Это наш шанс инициализировать начальное состояние приложения:
```jsx harmony
import { VisibilityFilters } from './actions'

const initialState = {
  visibilityFilter: VisibilityFilters.SHOW_ALL,
  todos: []
}

function todoApp(state, action) {
  if (typeof state === 'undefined') {
    return initialState
  }

  // Пока не обрабатываем никаких экшенов
  // и просто возвращаем состояние, которое приняли в качестве параметра
  return state
}
```	
Использование синтаксиса аргументов по умолчанию из ES6 для более компактного написания — просто аккуратный трюк:
```jsx harmony
function todoApp(state = initialState, action) {
  // Пока не обрабатываем никаких экшенов
  // и просто возвращаем состояние, которое приняли в качестве параметра
  return state
}
```	
Теперь давайте начнем обрабатывать экшен SET_VISIBILITY_FILTER. Все, что нужно сделать — это изменить visibilityFilter в состоянии приложения. Это просто:
```jsx harmony
import {
  SET_VISIBILITY_FILTER,
  VisibilityFilters
} from './actions'

...

function todoApp(state = initialState, action) {
  switch (action.type) {
    case SET_VISIBILITY_FILTER:
      return Object.assign({}, state, {
        visibilityFilter: action.filter
      })
    default:
      return state
  }
}
```	
Обратите внимание:
- Мы не изменяем state. Мы создаем копию с помощью Object.assign(). Object.assign(state, { visibilityFilter: action.filter }) тоже неверный вариант: в этом случае первый аргумент будет изменен. Вы должны передать первым аргументом пустой объект. Вы также можете подключить object spread operator proposal, чтобы вместо этого писать { ...state, ...newState } .

- Мы возвращаем предыдущую версию состояния (state) в default ветке. Очень важно возвращать предыдущую версию состояния (state) для любого неизвестного/необрабатываемого экшена (action).


### Обрабатываем больше экшенов
	
У нас есть еще два экшена, которые должны быть обработаны! Так же, как мы сделали с SET_VISIBILITY_FILTER мы имортируем ADD_TODO и TOGGLE_TODO экшены и затем допишем наш редьюсер для обработки ADD_TODO.
```jsx harmony
import {
  ADD_TODO,
  TOGGLE_TODO,
  SET_VISIBILITY_FILTER,
  VisibilityFilters
} from './actions'

...

function todoApp(state = initialState, action) {
  switch (action.type) {
    case SET_VISIBILITY_FILTER:
      return Object.assign({}, state, {
        visibilityFilter: action.filter
      })
    case ADD_TODO:
      return Object.assign({}, state, {
        todos: [
          ...state.todos,
          {
            text: action.text,
            completed: false
          }
        ]
      })
    default:
      return state
  }
}
```	
Как и раньше, мы никогда не изменяем непосредственно state или его поля. Вместо этого мы возвращаем новый объект. Новый todos равен старому todos, в конец которого добавлен новый элемент todo. Свежий tod был создан с использованием информации, полученной из action.

Ну и наконец, имплементация обработчика для экшена TOGGLE_TODO не должна стать для Вас большим сюрпризом:
```jsx harmony
case TOGGLE_TODO:
  return Object.assign({}, state, {
    todos: state.todos.map((todo, index) => {
      if (index === action.index) {
        return Object.assign({}, todo, {
          completed: !todo.completed
        })
      }
      return todo
    })
  })
```	
Поскольку мы хотим обновить конкретный элемент в массиве, не прибегая к мутациям, мы должны создать новый массив с теми же элементами, за исключением элемента по индексу. Если вы часто пишете такие операции, рекомендуется использовать хэлперы, такие как [immutability-helper] (https://github.com/kolodny/immutability-helper), [updeep] (https://github.com/essential/updeep) или даже такую библиотеку, как [Immutable] (http://facebook.github.io/immutable-js/), которая имеет встроенную поддержку для глубоких обновлений. Просто запомните, что нельзя присваивать ничего внутри state, пока вы его не склонировали.

### Разделение редьюсеров
	
Вот так выглядит наш код на данный момент. Выглядит излишне многословным:
```jsx harmony
function todoApp(state = initialState, action) {
  switch (action.type) {
    case SET_VISIBILITY_FILTER:
      return Object.assign({}, state, {
        visibilityFilter: action.filter
      })
    case ADD_TODO:
      return Object.assign({}, state, {
        todos: [
          ...state.todos,
          {
            text: action.text,
            completed: false
          }
        ]
      })
    case TOGGLE_TODO:
      return Object.assign({}, state, {
        todos: state.todos.map((todo, index) => {
          if (index === action.index) {
            return Object.assign({}, todo, {
              completed: !todo.completed
            })
          }
          return todo
        })
      })
    default:
      return state
  }
}
```	
Есть ли способ облегчить понимание? Кажется, что todos и visibilityFilter обновляются совершенно независимо. Иногда поля состояния (state fields) зависят от других полей и требуется большая связанность, но в нашем случаем мы безболезненно можем вынести обновление todos в отдельную функцию:
```jsx harmony
function todos(state = [], action) {
  switch (action.type) {
    case ADD_TODO:
      return [
        ...state,
        {
          text: action.text,
          completed: false
        }
      ]
    case TOGGLE_TODO:
      return state.map((todo, index) => {
        if (index === action.index) {
          return Object.assign({}, todo, {
            completed: !todo.completed
          })
        }
        return todo
      })
    default:
      return state
  }
}

function todoApp(state = initialState, action) {
  switch (action.type) {
    case SET_VISIBILITY_FILTER:
      return Object.assign({}, state, {
        visibilityFilter: action.filter
      })
    case ADD_TODO:
      return Object.assign({}, state, {
        todos: todos(state.todos, action)
      })
    case TOGGLE_TODO:
      return Object.assign({}, state, {
        todos: todos(state.todos, action)
      })
    default:
      return state
  }
}
```	
Обратите внимание, что функция todos также принимает state, но state — это массив! Теперь todoApp просто передает срез состояния в функцию todos, которая, свою очередь, точно знает, как обновить именно этот кусок состояния. Это называется композицией редьюсеров и является фундаментальным шаблоном построения Redux-приложений.

Давайте рассмотрим композицию редьюсеров подробнее. Можем ли мы извлечь редьюсер, который будет управлять только visibilityFilter? Конечно можем:

Ниже нашего импорта давайте использовать ES6 Object Destructuring, чтобы объявить SHOW_ALL:
```jsx harmony
const { SHOW_ALL } = VisibilityFilters
```	
Затем:
```jsx harmony
function visibilityFilter(state = SHOW_ALL, action) {
  switch (action.type) {
    case SET_VISIBILITY_FILTER:
      return action.filter
    default:
      return state
  }
}
```	
Теперь мы можем переписать наш главный редьюсер в виде функции, которая вызывает другие редьюсеры, обрабатывающие части состояния и собирает отдельно обработанные части состояния в один цельный объект. Также главному редьюсеру больше нет необходимости знать полное начальное состояние. Достаточно того, что каждый дочерний редьюсер возвращает свое начальное состояние, если при первом вызове получает undefined вместо state.
```jsx harmony
function todos(state = [], action) {
  switch (action.type) {
    case ADD_TODO:
      return [
        ...state,
        {
          text: action.text,
          completed: false
        }
      ]
    case TOGGLE_TODO:
      return state.map((todo, index) => {
        if (index === action.index) {
          return Object.assign({}, todo, {
            completed: !todo.completed
          })
        }
        return todo
      })
    default:
      return state
  }
}

function visibilityFilter(state = SHOW_ALL, action) {
  switch (action.type) {
    case SET_VISIBILITY_FILTER:
      return action.filter
    default:
      return state
  }
}

function todoApp(state = {}, action) {
  return {
    visibilityFilter: visibilityFilter(state.visibilityFilter, action),
    todos: todos(state.todos, action)
  }
}
```	
Обратите внимание на то, что каждый из этих дочерних редьюсеров управляет только какой-то одной частью глобального состояния. Параметр state разный для каждого отдельного дочернего редьюсера и соответствует той части глобального состояния, которой управляет этот дочерний редьюсер.

Уже выглядит лучше! Когда приложение разрастается, мы можем выносить редьюсеры в отдельные файлы и поддерживать их совершенно независимыми, что дает нам возможность управлять различными разделами наших данных.

Наконец, Redux предоставляет утилиту, называемую combineReducers(), которая реализует точно такой же логический шаблон, который мы только что реализовали в todoApp. С ее помощью мы можем переписать todoApp следующим образом:
```jsx harmony
import { combineReducers } from 'redux'

const todoApp = combineReducers({
  visibilityFilter,
  todos
})

export default todoApp
```	
Обратите внимание, что это полностью эквивалентно такому коду:
```jsx harmony
export default function todoApp(state = {}, action) {
  return {
    visibilityFilter: visibilityFilter(state.visibilityFilter, action),
    todos: todos(state.todos, action)
  }
}
```	
Вы также можете назначать им разные ключи или вызывать функции по-разному. Есть два совершенно равноценных способа писать комбинированные редьюсеры:
```jsx harmony
const reducer = combineReducers({
  a: doSomethingWithA,
  b: processB,
  c: c
})
```
```jsx harmony	
function reducer(state = {}, action) {
  return {
    a: doSomethingWithA(state.a, action),
    b: processB(state.b, action),
    c: c(state.c, action)
  }
}
```	
Все, что делает combineReducers() — это генерирует функцию, которая вызывает ваши редьюсеры c частью глобального состояния, которая выбирается в соответствии с их ключами, и затем снова собирает результаты всех вызовов в один объект. Тут нет никакой магии. И, как и другие редьюсеры, combineReducers() не создает новый объект, если все предоставленные ему редьюсеры не изменяют состояние.

Заметка для сообразительных пользователей синтаксиса ES6
Т.к. combineReducers ожидает на входе объект, мы можем поместить все редьюсеры верхнего уровня в разные файлы, экспортировать каждую функцию-редьюсер и использовать import * as reducers для получения их в формате объекта, ключами которого будут имена экспортируемых функций.
```jsx harmony
import { combineReducers } from 'redux'
import * as reducers from './reducers'

const todoApp = combineReducers(reducers)
```	
Поскольку import * — это все еще новый синтаксис, мы не используем его нигде в документации во избежание путаницы, но вы можете случайно наткнуться на него в каких-нибудь примерах кода из сообщества.

### Исходный код
	
**reducers.js**
```jsx harmony	
import { combineReducers } from 'redux'
import {
  ADD_TODO,
  TOGGLE_TODO,
  SET_VISIBILITY_FILTER,
  VisibilityFilters
} from './actions'
const { SHOW_ALL } = VisibilityFilters

function visibilityFilter(state = SHOW_ALL, action) {
  switch (action.type) {
    case SET_VISIBILITY_FILTER:
      return action.filter
    default:
      return state
  }
}

function todos(state = [], action) {
  switch (action.type) {
    case ADD_TODO:
      return [
        ...state,
        {
          text: action.text,
          completed: false
        }
      ]
    case TOGGLE_TODO:
      return state.map((todo, index) => {
        if (index === action.index) {
          return Object.assign({}, todo, {
            completed: !todo.completed
          })
        }
        return todo
      })
    default:
      return state
  }
}

const todoApp = combineReducers({
  visibilityFilter,
  todos
})

export default todoApp
```
    
  **[⬆ Наверх](#top)**
	
354. ### <a name="354"></a> middleware

 ### Mидлвар (Middleware)
	
Вы видели мидлвары в действии в примере асинхронных экшенов. Если вы когда-либо использовали такие серверные библиотеки, как Express и Koa, то, вероятно, вы уже хорошо знакомы с концепцией мидлвар. В этих фреймворках мидлвары — это части кода, которые вы можете поместить между фреймворком, принимающим запрос и фреймворком, генерирующим ответ. Например, мидлвары из Express или Koa могут добавлять CORS-заголовки, логирование, сжатие и т.д. Лучшая особенность мидлваров заключается в том, что их можно соединять в цепочки/последовательности. Вы можете использовать множество независимых сторонних мидлваров в одном проекте.

Redux-мидлвары, в отличие от мидлваров Express или Koa, решают немного другие проблемы, но концептуально схожим способом. Они предоставляют стороннюю точку расширения, между отправкой экшена и моментом, когда этот экшен достигает редьюсера. Люди используют Redux-мидлвары для логирования, сообщения об ошибках, общения с асинхронным API, роутинга и т.д.

Эта статья разделена на углубленное введение, которое поможет вам хорошо разобраться в концепции, и пару практических примеров в самом конце, которые покажут вам всю силу мидлваров. Вам может показаться полезным периодическое переключение между этими частями, так же, как между скукой и вдохновением.

Понимание мидлваров
Т.к. мидлвары могут использоваться для различных задач, в том числе и для асинхронных обращений к API, то очень важно, чтобы вы понимали, откуда они пришли. Мы покажем вам ход мыслей, шаг за шагом ведущий к мидлварам, используя логирование и сообщения об ошибках в качестве примера.

Проблема: логирование
Одно из достоинств Redux — он делает изменения состояния приложения предсказуемыми и прозрачными. Каждый раз, когда посылается экшен, новое состояние вычисляется и сохраняется. Состояние не может измениться самостоятельно, оно может меняться только, как последовательность определенных экшенов.

Разве не было бы хорошо, если бы мы записывали каждое действие, которое происходило в приложении, вместе с состоянием, которое было вычислено после этого действия? Когда что-то идет не так, мы можем просмотреть наш лог и понять, какой именно экшен испортил наше состояние.
	
<img width="556" alt="687474703a2f2f692e696d6775722e636f6d2f426a47426c45532e706e67" src="https://user-images.githubusercontent.com/80325645/129259099-f288d0bb-cd34-44a4-a6ec-86414b08df47.png">

*Попытка #1*: Логируем вручную
Простейшее решение - самостоятельно записывать экшен и состояние каждый раз, когда вы вызываете store.dispatch(action). На самом деле это не слишком хорошее решение, это просто первый шаг на пути к пониманию проблемы.

Обратите внимание
Если вы используете react-redux или похожий биндинг, у вас, скорее всего, не будет прямого доступа к экземпляру стора в ваших компонентах. Для следующих нескольких параграфов представьте, что вы передаете состояние явно.

Например, вы вызываете такой код, когда создаете todo-элемент:
```jsx harmony
store.dispatch(addTodo('Use Redux'))
```	
Для того чтобы логировать экшен и состояние, вы можете изменить код примерно так:
```jsx harmony
let action = addTodo('Use Redux')

console.log('dispatching', action)
store.dispatch(action)
console.log('next state', store.getState())
```	
Это даст желаемый эффект, но вы бы не хотели делать так каждый раз.

*Попытка #2*: Оборачиваем Dispatch
Вы можете вынести логирование в функцию:
```jsx harmony
function dispatchAndLog(store, action) {
  console.log('dispatching', action)
  store.dispatch(action)
  console.log('next state', store.getState())
}
```	
Вы можете использовать ее везде вместо обычного store.dispatch():
```jsx harmony
dispatchAndLog(store, addTodo('Use Redux'))
```	
Мы бы могли закончить на этом, но не очень удобно импортировать специальную функцию каждый раз.

*Попытка #3*: Monkeypatching для Dispatch
	
Что, если мы просто заменим функцию dispatch в экземпляре стора? Redux стор — это простой объект с парой методов, а мы пишем на JavaScript, следовательно, мы можем применить технику monkeypatch для реализации dispatch:
```jsx harmony
const next = store.dispatch
store.dispatch = function dispatchAndLog(action) {
  console.log('dispatching', action)
  let result = next(action)
  console.log('next state', store.getState())
  return result
}
```	
Это уже ближе к тому, что нам нужно! Не важно, откуда мы посылаем экшен, он гарантированно будет залогирован. Monkeypatching никогда не покажется правильным ходом, но пока мы можем с этим жить.

### Проблема: Сообщения об ошибках.
	
Что, если мы захотим применить больше одного такого преобразования к dispatch?

Другое такое изменение, которое приходит мне в голову, это сообщения о JavaScript-ошибках в продакшене. Глобальное событие window.onerror не надежно потому, что оно в некоторых старых браузерах не предоставляет информацию о стеке вызовов, которая важна для понимания того, почему же произошла ошибка.

Разве не было бы полезно, если бы каждый раз, когда ошибка выбрасывалась, как результат отправки какого-либо экшена, мы могли бы отправить ее (ошибку), вместе со стеком вызовов, экшеном, который вызвал ошибку и актуальным состоянием в сервис сообщения об ошибках, такой как Sentry. В таком случае гораздо легче воспроизвести ошибку в разработке.

Однако важно, чтобы мы держали логирование и сообщения об ошибках раздельно. В идеальном случае, мы хотим получить их, как разные модули из разных пакетов. В противном случае, мы не сможем иметь экосистему из такого рода утилит. (Подсказка: мы медленно подходим к тому, что такое мидлвары!)

Если логирование и сообщения об ошибках являются отдельными утилитами, то они могут выглядеть так:
```jsx harmony
function patchStoreToAddLogging(store) {
  const next = store.dispatch
  store.dispatch = function dispatchAndLog(action) {
    console.log('dispatching', action)
    let result = next(action)
    console.log('next state', store.getState())
    return result
  }
}

function patchStoreToAddCrashReporting(store) {
  const next = store.dispatch
  store.dispatch = function dispatchAndReportErrors(action) {
    try {
      return next(action)
    } catch (err) {
      console.error('Caught an exception!', err)
      Raven.captureException(err, {
        extra: {
          action,
          state: store.getState()
        }
      })
      throw err
    }
  }
}
```	
Если эти функции опубликованы, как отдельные модули, то позже мы можем использовать их для изменения нашего стора:
```jsx harmony
patchStoreToAddLogging(store)
patchStoreToAddCrashReporting(store)
```	
Но это все еще не очень хорошо.

*Попытка #4*: Прячем Monkeypatching
	
Monkeypatching — это хак. "Замените любой метод, который хотите" — что это за вид API? Давайте разберемся в его сути. Ранее наши функции заменяли store.dispatch. Что если бы они вместо этого возвращали новую функцию dispatch?
```jsx harmony
function logger(store) {
  let next = store.dispatch

  // ранее было так:
  // store.dispatch = function dispatchAndLog(action) {

  return function dispatchAndLog(action) {
    console.log('dispatching', action)
    let result = next(action)
    console.log('next state', store.getState())
    return result
  }
}
```	
Мы могли бы предоставить функцию-помощник внутри Redux, которая могла бы применять актуальный monkeypatching, как часть имплементации:
```jsx harmony
function applyMiddlewareByMonkeypatching(store, middlewares) {
  middlewares = middlewares.slice()
  middlewares.reverse()

  // Изменяем функцию dispatch каждым мидлваром.
  middlewares.forEach(middleware =>
    store.dispatch = middleware(store)
  )
}
```	
Мы можем использовать такой подход для применения нескольких мидлваров:
```jsx harmony
applyMiddlewareByMonkeypatching(store, [ logger, crashReporter ])
```	
Тем не менее - это все еще monkeypatching. Факт того, что мы прячем его внутри библиотеки, не отменяет использования monkeypatching.

*Попытка #5*: Убираем Monkeypatching
	
Зачем мы перезаписываем dispatch? Конечно же для того, чтобы иметь возможность потом его вызвать. Но есть еще и другая причина: каждый мидлвар имеет доступ (и возможность вызвать) ранее обернутый store.dispatch:
```jsx harmony
function logger(store) {
  // Обязательно нужно закешировать функцию, которую вернул предыдущий мидлвар:
  let next = store.dispatch

  return function dispatchAndLog(action) {
    console.log('dispatching', action)
    let result = next(action)
    console.log('next state', store.getState())
    return result
  }
}
```	
Это важно для возможности объединять мидлвары в цепочки!

Если applyMiddlewareByMonkeypatching не сохранит store.dispatch сразу после обработки первого мидлвара, store.dispatch будет продолжать ссылаться на оригинальную функцию dispatch. Следовательно второй мидлвар тоже будет связан с оригинальной функцией dispatch.

Но есть еще другой метод реализации объединения мидлваров в цепочки (chaining). Мидлвар мог бы принимать функцию отправки экшена next() в параметрах вместо того, чтобы читать ее из экземпляра стора.
```jsx harmony
function logger(store) {
  return function wrapDispatchToAddLogging(next) {
    return function dispatchAndLog(action) {
      console.log('dispatching', action)
      let result = next(action)
      console.log('next state', store.getState())
      return result
    }
  }
}
```	
Это тот момент, когда “we need to go deeper”, так что имеет смысл потратить некоторе время на это. Каскад функций выглядит пугающим. Стрелочные функции из ES6 делают это каррирование чуть более простым для глаз:
```jsx harmony
const logger = store => next => action => {
  console.log('dispatching', action)
  let result = next(action)
  console.log('next state', store.getState())
  return result
}

const crashReporter = store => next => action => {
  try {
    return next(action)
  } catch (err) {
    console.error('Caught an exception!', err)
    Raven.captureException(err, {
      extra: {
        action,
        state: store.getState()
      }
    })
    throw err
  }
}
```	
Именно так выглядят мидлвары в Redux.

Теперь мидлвар принимает функцию отправки экшена next() и возвращает другую функцию отправки экшена, которая, в свою очередь, является функцией отправки экшена next() для мидлвара слева. Все еще полезно иметь доступ к некоторым методам стора, например к getState(), следовательно, store остается доступен, как аргумент самого верхнего уровня.

*Попытка #6*: Простейшее применение мидлваров
Вместо applyMiddlewareByMonkeypatching() мы могли бы написать функцию applyMiddleware(), которая сначала получает финальную, полностью обернутую функцию dispatch() и возвращает копию стора, которая использует эту функцию:
```jsx harmony
// Осторожно: Простейшая имплементация!
// Это *не* Redux API.
function applyMiddleware(store, middlewares) {
  middlewares = middlewares.slice()
  middlewares.reverse()
  let dispatch = store.dispatch
  middlewares.forEach(middleware => (dispatch = middleware(store)(dispatch)))
  return Object.assign({}, store, { dispatch })
}
```	
Реализация applyMiddleware(), которая поставляется с Redux, похожа на эту, но отличается тремя важными аспектами:

Она предоставляет мидлвару только подмножество API стора: методы dispatch(action) и getState().

Она использует некоторые хитрости для того, чтобы убедиться, что, экшен снова пройдет через всю цепочку мидлваров, включая текущий, если вы вызываете store.dispatch(action) из вашего мидлвара вместо next(action). Это полезно для асинхронных мидлваров, как мы ранее видели.

Для того чтобы гарантировать, что вы можете применить мидлвар только один раз, она работает с createStore(), а не с самим store. Вместо (store, middlewares) => store, ее сигнатурой является (...middlewares) => (createStore) => createStore.

Предостережение: отправка во время установки
Пока applyMiddleware выполняет и настраивает ваши мидлвари, функция store.dispatch будет указывать на оригинальную версию, предоставляемую createStore. Отправка приведет к тому, что никакой другой мидлвар не будет применен. Если вы ожидаете взаимодействия с другим мидлваром во время настройки, вы, вероятно, будете разочарованы. Из-за этого неожиданного поведения applyMiddleware выдаст ошибку, если вы попытаетесь отправить экшен до завершения установки. Вместо этого вам следует, либо напрямую связываться с этим другим мидлваром через общий объект (для мидлвара, вызывающего API, это может быть ваш клиентский объект API), либо ждать, пока мидлвар не будет создан с колбэком.

Финальный подход
Дан мидлвар который мы только что написали:
```jsx harmony
const logger = store => next => action => {
  console.log('dispatching', action)
  let result = next(action)
  console.log('next state', store.getState())
  return result
}

const crashReporter = store => next => action => {
  try {
    return next(action)
  } catch (err) {
    console.error('Caught an exception!', err)
    Raven.captureException(err, {
      extra: {
        action,
        state: store.getState()
      }
    })
    throw err
  }
}
```	
Вот так можно его применить к Redux стору:
```jsx harmony
import { createStore, combineReducers, applyMiddleware } from 'redux'

const todoApp = combineReducers(reducers)
const store = createStore(
  todoApp,
  // applyMiddleware() tells createStore() how to handle middleware
  applyMiddleware(logger, crashReporter)
)
```	
Вот и все! Теперь любые экшены, отправленные в экземпляр стора, будут проходить через logger и crashReporter:
```jsx harmony
// будет проходить через `logger` и `crashReporter`!
store.dispatch(addTodo('Use Redux'))
```
	
*Семь примеров*
	
Если ваша голова вскипела от прочтения предыдущего раздела, представьте, каково было написать это. Этот раздел предназначен для расслабления меня и вас и поможет запустить ваши шестеренки.

Каждая из функций, приведенных ниже, является валидным Redux-мидлваром. Они не являются в равной степени полезными, но, по крайней мере, они в равной степени забавны.
```jsx harmony
/**
 * Логирует все экшены и состояния после того, как они будут отправлены.
 */
const logger = store => next => action => {
  console.group(action.type)
  console.info('dispatching', action)
  let result = next(action)
  console.log('next state', store.getState())
  console.groupEnd(action.type)
  return result
}

/**
 * Отправляет отчеты об ошибках когда обновляется состояние и уведомляются слушатели.
 */
const crashReporter = store => next => action => {
  try {
    return next(action)
  } catch (err) {
    console.error('Caught an exception!', err)
    Raven.captureException(err, {
      extra: {
        action,
        state: store.getState()
      }
    })
    throw err
  }
}

/**
 * Планирует экшены с { meta: { delay: N } }, которые будут отложены на N миллисекунд.
 * Создает `dispatch`, возвращающий функцию, для отмены таймаута.
 */
const timeoutScheduler = store => next => action => {
  if (!action.meta || !action.meta.delay) {
    return next(action)
  }

  let timeoutId = setTimeout(
    () => next(action),
    action.meta.delay
  )

  return function cancel() {
    clearTimeout(timeoutId)
  }
}

/**
 * Планирует экшены с { meta: { raf: true } }, которые будут отправлены внутри 
 * фрейма rAF цикла. Создает  `dispatch`, который возвращает функцию для удаления 
 * экшена из очереди.
 */
const rafScheduler = store => next => {
  const queuedActions = []
  let frame = null

  function loop() {
    frame = null
    try {
      if (queuedActions.length) {
        next(queuedActions.shift())
      }
    } finally {
      maybeRaf()
    }
  }

  function maybeRaf() {
    if (queuedActions.length && !frame) {
      frame = requestAnimationFrame(loop)
    }
  }

  return action => {
    if (!action.meta || !action.meta.raf) {
      return next(action)
    }

    queuedActions.push(action)
    maybeRaf()

    return function cancel() {
      queuedActions = queuedActions.filter(a => a !== action)
    }
  }
}

/**
 * Позволяет вам отправлять промисы в дополнение к экшенам.
 * Если промис зарезолвен, его результат будет отправлен как экшен.
 * Промис возвращается из `dispatch`, т.о. вызывающая функция может 
 * обрабатывать отказ (rejection) промиса.
 */
const vanillaPromise = store => next => action => {
  if (typeof action.then !== 'function') {
    return next(action)
  }

  return Promise.resolve(action).then(store.dispatch)
}

/**
 * Позволяет вам отправлять специальные экшены с полем { promise }.
 * Этот мидлвар превратит их в единственный экшен в начале,
 * и в единственный успешный (или неудачный) экшен, когда `promise` будет зарезолвен.
 *
 * Для удобства `dispatch` будет возвращать промис, т.е. вызывающая функция 
 * может ожидать разрешения этого промиса.
 */
const readyStatePromise = store => next => action => {
  if (!action.promise) {
    return next(action)
  }

  function makeAction(ready, data) {
    const newAction = Object.assign({}, action, { ready }, data)
    delete newAction.promise
    return newAction
  }

  next(makeAction(false))
  return action.promise.then(
    result => next(makeAction(true, { result })),
    error => next(makeAction(true, { error }))
  )
}

/**
 * Позволяет вам отправлять функцию вместо экшена.
 * Функция будет принимать `dispatch` и `getState` в качестве аргументов.
 *
 * Полезно для раннего выхода (условия над `getState()`), а также для 
 * асинхронного потока управления (может `dispatch()` что-то другое)
 * 
 * `dispatch` будет возвращать значение отправляемой функции.
 */
const thunk = store => next => action =>
  typeof action === 'function' ?
    action(store.dispatch, store.getState) :
    next(action)

// Вы можете использовать их все! (Это не значит, что вы должны.)
const todoApp = combineReducers(reducers)
const store = createStore(
  todoApp,
  applyMiddleware(
    rafScheduler,
    timeoutScheduler,
    thunk,
    vanillaPromise,
    readyStatePromise,
    logger,
    crashReporter
  )
)	
```
    
  **[⬆ Наверх](#top)**
	
355. ### <a name="355"></a> Redux, Actions, Reducer, Store - примеры

 `Пример`	
	
```jsx
const ON_CLICK = 'ON_CLICK'

const increaseCounter = () => ({
	type: ON_CLICK
})

const reducer = (state = 0, action) => {
	if (action.type === ON_CLICK) {
		return state++;
	}

	return state;
}

const Status = () => {
	const count = useSelector((state) => state);

	return (<span>{count}</span>)
}

const Changer = () => {
	const dispatch = useDispatch();

	const onClick = () => dispatch(increaseCounter());

	return (<button onClick={onClick}>Change</button>)
}

class ClassComponentWithStore extends Component {
	constructor(props) {
		super(props);
	}


	render() {
		const { onClick, count } = this.props

		return (
			<div>
				<span>{count}</span>
				<button onClick={onClick}>Change</button>
			</div>
		)
	}
}

const ClassComponent = connect(
	(state) => ({
		count: state
	}),
	(dispatch) => ({
		onClick: () => dispatch(increaseCounter)
	})
)(ClassComponentWithStore)

const store = createStore(reducer)

const App = () => {
	return (
		<Provider store={store}>
			<Status />
			<Changer />
			<ClassComponent />
		</Provider>
	)
}


ReactDOM.render(<App />, document.getElementById('root'))	
```	

### Назовите ключевые концепции Redux***

<p align="center">
  <img src="../assets/img-v2/redux-components.jpg" alt="Redux Components" width="400px" />
</p>

**1. Операция (action)**

Операция - это статическая информация о событии, инициализирующем изменение состояния. Обновление состояния в Redux всегда начинается с операции. Операции - это объекты, содержащие обязательное свойство `type` и опциональное свойство `payload`. Операции вызываются с помощью метода `store.dispatch()`. Операция создается с помощью "создателя операций" (`action creator`).

**Создатели операций** - функции, помогающие создавать операции. Создатель операции возвращает объект операции, который передается редуктору.

*Пример*

```js
const setLoginStatus = (name, password) => {
  return {
    type: "LOGIN",
    payload: {
      username: "foo",
      password: "bar"
    }
  }
}
```

**2. Редуктор (reducer)**

Редукторы - это "чистые" функции, принимающие текущее состояние приложения, выполняющие над ним операцию и возвращающие новое состояние. Новое состояние - объект, описывающий изменения состояния, произошедшие в ответ на вызванную операцию.

Это похоже на функцию `reduce()` в JavaScript, когда значение вычисляется на основе нескольких значений после выполнения коллбека.

```js
const LoginComponent = (state = initialState, action) => {
    switch (action.type) {

      // данный редуктор обрабатывает операции с типом "LOGIN"
      case "LOGIN":
          return state.map(user => {
              if (user.username !== action.username) {
                  return user
              }

              if (user.password == action.password) {
                  return {
                      ...user,
                      login_status: "LOGGED IN"
                  }
              }
          });
      default:
          return state;
      }
}
```

**Комбинация нескольких редукторов**: вспомогательная функция `combineReducers()` преобразует объект с несколькими редукторами в один редуктор для передачи в `createStore()`.

*Синтаксис*

```js
const rootReducert = combineReducer(reducer1, reducer2)
```

**3. Состояние (state)**

Состояние - это объект, содержащий состояние приложения. При обновлении состояния, обновляются все подписанные на него компоненты. Хранилище отвечает за запись, чтение и обновление состояния.

*Пример*

```js
import React from 'react'
import { render } from 'react-dom'
import { Provider } from 'react-redux'
import { createStore } from 'redux'
import rootReducer from './reducers'
import App from './components/App'

const store = createStore(rootReducer)
 render (
   <provider store="{store}">
     <app>
   </app></provider>,
   document.getElementById('root')
 )
```

При использовании Redux с React состояние не требует подъема. Это также облегчает идентификацию операции, которая вызвала изменение состояния.

**4. Отправка (dispatch)**

Отправка - это передача операции с типом и полезной нагрузкой редуктору.

```js
store.dispatch()
```

**5. Подписка (subscribe)**

Подписка - это метод, испольуземый для подписки на данные/состояние хранилища.

```js
store.subscribe()
```

**6. Провайдер (provider)**

Провайдер - это компонент, содержащий ссылку на хранилище и передающий данные из хранилища дочерним компонентам.

**7. Подключение (connect)**

Подключение - это функция, взаимодействующая с провайдером.

**8. Промежуточное программное обеспечение, промежуточный слой, посредник (middleware)**

Посредник - это способ расширения Redux дополнительным функционалом. Посредники используются для отправки асинхронных операций. Они настраиваются в момент создания хранилища.

*Синтаксис*

```js
const store = createStore(reducers, initialState, middleware);
```	
	
	
### Объясните назначение редуктора?

Редуктор - это функция, определяющая изменения состояния приложения. Она использует операции для определения характера изменений. Redux управляет состоянием приложения с помощью единственного хранилища, так что они действуют согласованно. Redux во многом зависит от редукторов, которые принимают предыдущее состояние и операцию для производства нового состояния.

**1. Состояние**

Изменение состояния зависит от действий пользователя или сетевых запросов. Если состояние приложения управляется Redux, изменения происходят в редукторе - это единственное место, в котором происходит изменение состояния. Редуктор использует текущее состояние приложение и операцию для определения нового состояния.

*Синтаксис*

```js
const contactReducer = (state = initialState, action) => {
  // ...
}
```

**2. Параметр `state`**

Параметр `state`, передаваемый в редуктор, должен быть текущим состоянием приложения. В данном случае, мы передаем редуктору `initialState`, т.е. начальное состояние, которому ничего не предшествовало.

```js
contactReducer(initialState, action)
```

*Пример*

Предположим, что начальным состоянием нашего приложения является пустой массив для списка контактов, а операцией - добавление нового контакта в этот список.

```js
const initialState = {
  contacts: []
}
```

**3. Параметр `action`**

`action` - это объект, содержащий две пары ключ/значение. Обновление состояния, происходящее в редукторе, зависит от значения свойства `action.type`.

```js
const action = {
  type: 'NEW_CONTACT',
  payload: {
    name: 'Иван Петров',
    location: 'Москва',
    email: 'mail@example.com'
  }
}
```

Обычно, также имеется свойство `payload`, содержащее данные, отправленные пользователем, используемые для обновления состояния. Следует отметить, что `action.type` является обязательным, а `action.payload` опциональным.

**4. Обновление состояния**

Состояние должно быть иммутабельным. Это означает, что его нельзя изменять напрямую. Для обновления состояния можно использовать `Object.assign()` или *spread-оператор*.

*Пример*

```js
const contactReducer = (state, action) => {
  switch (action.type) {
    case 'NEW_CONTACT':
    return {
        ...state, contacts:
        [...state.contacts, action.payload]
    }
    default:
      return state
  }
}
```

Это позволяет обеспечить сохранность текущего состояния при добавлении нового элемента.

```js
const initialState = {
  contacts: [{
    name: 'Иван Петров',
    age: 30
  }]
}

const contactReducer = (state = initialState, action) => {
  switch (action.type) {
    case "NEW_CONTACT":
      return Object.assign({}, state, {
        contacts: [...state.contacts, action.payload]
      });
    default:
      return state
  }
}

class App extends React.Component {
  constructor(props) {
    super(props)
    this.name = React.createRef()
    this.age = React.createRef()
    this.state = initialState
  }

  handleSubmit = e => {
    e.preventDefault()
    const action = {
      type: "NEW_CONTACT",
      payload: {
        name: this.name.current.value,
        age: this.age.current.value
      }
    }
    const newState = contactReducer(this.state, action)
    this.setState(newState)
  }

  render() {
    const { contacts } = this.state
    return (
      <div className="box">
        <div className="content">
          <pre>{JSON.stringify(this.state, null, 2)}</pre>
        </div>

        <div className="field">
          <form onSubmit={this.handleSubmit}>
            <div className="control">
              <input className="input" placeholder="Имя" type="text" ref={this.name} />
            </div>
            <div className="control">
              <input className="input" placeholder="Возраст" type="number" ref={this.age} />
            </div>
            <div>
              <button type="submit" className="button">Отправить</button>
            </div>
          </form>
        </div>
      </div>
    )
  }
}

ReactDOM.render(
  <App />,
  document.getElementById('root')
)
```	

### Как реализовать "создателя операции" (action creator)?

**Тип операции**

*Action type* - это строка, описывающая тип операции. Обычно, типы определяются в виде констант или перечислений (enumerations).

*Пример*

```js
export const Actions = {
  GET_USER_DETAILS_REQUEST: 'GET_USER_DETAILS_REQUEST',
  GET_USER_DETAILS_SUCCESS: 'GET_USER_DETAILS_SUCCESS',
  GET_USER_DETAILS_FAILURE: 'GET_USER_DETAILS_FAILURE',
  ...
}
```

**Операция**

Операция похожа на сообщение, отправляемое (dispatch) в хранилище. Теоретически, она может выглядеть как угодно. Однако, лучше придерживаться следующего соглашения (определение типа с помощью TypeScript):

```ts
type Action = {
  type: string;    // операция ДОЛЖНА иметь тип
  payload?: any;   // операция МОЖЕТ иметь полезную нагрузку
  meta?: any;      // операция МОЖЕТ иметь мета (дополнительную) информацию
  error?: boolean; // операция МОЖЕТ иметь поле для ошибки
                    // при истинном значении данного поля, полезная нагрузка ДОЛЖНА включать Error
}
```

Операция получения пользователя по имени "Иван" может выглядеть так:

```js
{
    type: 'GET_USER_DETAILS_REQUEST',
    payload: 'Иван'
}
```

**Создатель операции**

```js
export const getUserDetailsRequest = id => ({
  type: Actions.GET_USER_DETAILS_REQUEST,
  payload: id,
})
```

В простых случаях создатель операции возвращает операцию. После этого она отправляется в хранилище:

```js
store.dispatch(getUserDetailsRequest('Иван'))
```

На практике это, как правило, реализуется через свойство `dispatch()`, передаваемое в React-компонент:

```js
export const mapDispatchToProps = dispatch => ({
  onClick: () => dispatch(getUserDetailsRequest('Alex'))
})
```	

### Как установить начальное состояние?

**1. Инициализация состояния**

В Redux состояние всего приложения находится в хранилище, которое является древовидным объектом. Единственным способом изменить состояние является отправка операции.

Операции - это объекты, содержащие свойства "тип" и "полезная нагрузка". Они создаются и отправляются специальными функциями, которые называются "создателями операций".

*Пример*

Создаем хранилище:

```js
import { createStore } from 'redux'

function todosReducer(state = [], action) {
  switch (action.type) {
    case 'ADD_TODO':
      return state.concat([action.payload])
    default:
      return state
  }
}

const store = createStore(todosReducer)
```

Обновляем состояние:

```js
const ADD_TODO = 'ADD_TODO'; // создаем тип операции
const newTodo = ["Написать статью"];
function todoActionCreator (newTodo) {
  const action = {
    type: ADD_TODO,
    payload: newTodo
  }
  dispatch(action)
}
```

После создания хранилища, Redux отправляет операцию в редуктор для записи в хранилище начального состояния.

**2. `createStore()`**

Метод `createStore()` может принимать опциональное значение `preloadedState` в качестве второго аргумента. В нашем примере мы не используем данный параметр. Когда такое значение передается, оно становится начальным состоянием.

```js
const initialState = ["питаться", "кодить", "спать"];
const store = createStore(todosReducer, initialState)
```

**3. Редуктор**

Редукторы также могут определять начальное состояние в случае, когда значением передаваемого им аргумента `state` является `undefined`:

```js
function todosReducer(state = [], action) {
  switch (action.type) {
    case 'ADD_TODO':
      return state.concat([action.payload])
    default:
      return state
  }
}
/**
* начальное состояние равняется []. Будет использовано только при неопределенном значении начального состояния,
* т.е. когда оно не было передано в `createStore()`
**/
```

Как правило, `preloadedState` имеет более высокий приоритет, чем состояние, определенное в `reducer`. Это позволяет редукторам определять данные в качестве аргументов по умолчанию, а также загружать существующие данные (полностью или частично) при гидратации хранилища из некоторого постоянного хранилища или сервера.	

	
### Что такое `mapStateToProps()` и `mapDispatchToProps()`?

Библиотека `react-redux` предоставляет 3 функции: `connect()`, `mapStapteToProps()` и `mapDispatchToProps()`. `connect()` - это функция высшего порядка, принимающая `mapStateToProps()` и `mapDispatchToProps()` в качестве параметров.

**1. `mapStateToProps()`**

Функция `mapStatetoProps()` извлекает состояние определенного редуктора из глобального хранилища и сопоставляет его с пропами компонента. Данная функция вызывается при каждом обновлении хранилища.

**2. `mapDispatchToProps()`**

Функция `mapDispatchToProp()` принимает функции отправки в компоненте и выполняет их в соответствующих редукторах. Данная функция позволяет отправлять изменения состояния в хранилище.

Говоря проще,

**mapStateToProps**: подключает состояние Redux к пропам React-компонента
**mapDispatchToProps**: подключает операции Redux к пропам React-компонента

*Пример*

```js
const { createStore } = Redux
const { connect, Provider } = ReactRedux
const initialState = { collection: ["prima", "altera", "triera"] }

function reducer(state = initialState, action) {
    if (action.type === "REVERSE") {
      return Object.assign({}, state, {
         Collection: state.collection.slice().reverse()
      })
    }
    return state
}

const store = createStore(reducer)

function mapStateToProps(state) {
  return state
}

const PresentationalComponent = React.createClass({
    render: function() {
        return (
          <div>
            <h2>Состояние хранилища (в виде пропа)</h2>
            <pre> {JSON.stringify(this.props.collection)}</pre>
            <StateChangerUI />
          </div>
          )
    }
})

// изменение состояния UI
const StateChangerUI = React.createClass({
  // отправка операции
  handleClick: function() {
     store.dispatch({
         type: 'REVERSE'
      })
  },
  render: function() {
    return (
      <button type="button" className="btn btn-success" onClick={this.handleClick}>Инвертировать</button>
    )
  }
})

PresentationalComponent = connect(mapStateToProps)(PresentationalComponent)

ReactDOM.render(
  <Provider store={store}>
    <PresentationalComponent />
  </Provider>,
  document.getElementById('App')
)
```		

### Что такое "чистые" функции и почему редуктор должен быть такой функцией?

**"Чистая" функция**

Функция, которая не изменяет входные данные и не зависит от внешних данных (например, базы данных, DOM или глобальных переменных) и возвращает одинаковый результат для одних и тех же аргументов, является "чистой".

Таким образом, функция является "чистой", если она удовлетворяет следующим условиям:

* Возвращает одинаковый результат для одних и тех же аргументов
* Оценивается без побочных эффектов, т.е. не изменяет входные данные
* Не изменяет локальные или глобальные переменные
* Не зависит от внешних данных

*Пример*

Приведенная ниже функция `add()` не изменяет параметры `a` и `b`, не зависит от внешних данных, и всегда возвращает одинаковый результат для одних и тех же аргументов:

```js
const add = (a, b) => a + b // "чистая" функция
```

**Почему редуктор должен быть "чистой" функцией?**

Redux берет текущее состояние (объект) и передает его каждому редуктору в цепочке (при комбинации редукторов). Редуктор должен вернуть новый объект в случае изменения состояния. При отсутствии изменений редуктор должен вернуть старый объект.

Redux проверяет, отличаются ли старый и новый объекты, сравнивая их места в памяти. Поэтому, если мы изменим старый объект в редукторе, старое и новое состояния будут ссылаться на один и тот же объект. Redux сделает вывод о том, что ничего не изменилось, и логика приложения будет нарушена.
    
  **[⬆ Наверх](#top)**
	
356. ### <a name="356"></a> redux-forms в экосистеме React + Redux

*Redux Form* работает с React и Redux, позволяя формам в React хранить состояние в Redux. Redux Form может использоваться с обычными HTML5-инпутами, а также с популярными UI-фреймворками, такими как Material UI, React Widgets и React Bootstrap.
	
Вот некоторые из основных особенностей Redux Form:

1. Значения полей записываются в хранилище Redux
2. Синхронная/асинхронная валидация полей и отправка формы
3. Форматирование, разбор и нормализация значений полей
    
  **[⬆ Наверх](#top)**
	
357. ### <a name="357"></a> Redux пример

### Пример простого кода	  
```jsx harmony
import React from 'react';
import ReactDOM from 'react-dom';
import { createStore } from 'redux';

const initialState = {value: 0};

const reducer = (state = initialState, action) => {
    switch (action.type) {
        case "INC":
            return {
                ...state,
                value: state.value + 1
            };
        case "DEC":
            return {
                ...state,
                value: state.value - 1
            };
        case "RND":
            return {
                ...state,
                value: state.value * action.payload
            };
        default:
            return state;
    }
}

const store = createStore(reducer);

const update = () => {
    document.getElementById('counter').textContent = store.getState().value;
}

store.subscribe(update);

const inc = () => ({type: 'INC'});
const dec = () => ({type: 'DEC'});
const rnd = (value) => ({type: 'RND', payload: value});

document.getElementById('inc').addEventListener('click', () => {
    store.dispatch(inc());
});

document.getElementById('dec').addEventListener('click', () => {
    store.dispatch(dec());
});

document.getElementById('rnd').addEventListener('click', () => {
    const value = Math.floor(Math.random() * 10);
    store.dispatch(rnd(value));
});

ReactDOM.render(
  <React.StrictMode>
    <>
    
    </>
  </React.StrictMode>,
  document.getElementById('root')
);	  
```	  

### Пример 

### index.js	  
```jsx harmony
import React from 'react';
import ReactDOM from 'react-dom';
import {createStore} from 'redux';
import reducer from './reducer';
import {Provider} from 'react-redux';

import App from './components/App';

const store = createStore(reducer);

ReactDOM.render(
  <React.StrictMode>
    <Provider store={store}>
      <App />
    </Provider>
  </React.StrictMode>,
  document.getElementById('root')
);	  
```	  

### reducer.js
```jsx harmony
const initialState = {counter: 0};

const reducer = (state = initialState, action) => {
	switch (action.type) {
		case 'INC':
			return {
				...state,
				counter: state.counter + 1
			};
		case 'DEC':
			return {
				...state,
				counter: state.counter - 1
			};
		case 'RND':
			return {
				...state,
				counter: state.counter * action.payload
			};
		default:
			return state;
	}
}

export default reducer;	  
```	  

### actions.js
```jsx harmony
export const inc = () => ({type: 'INC'})
export const dec = () => ({type: 'DEC'})
export const rnd = () => ({type: 'RND', payload: Math.floor(Math.random() * 10)})	  
```	  

### App.js
```jsx harmony
import Counter from './Counter';

const App = () => {
	return <Counter />
}

export default App;	  
```	  

### Counter.js
```jsx harmony
import {inc, dec, rnd} from '../actions';
import {useSelector, useDispatch} from 'react-redux';

const Counter = () => {

	const counter = useSelector(state => state.counter);

	const dispatch = useDispatch();

	return (
		<div className="jumbotron">
			<h1>{counter}</h1>
			<button onClick={() => dispatch(dec())} className="btn btn-primary">DEC</button>
			<button onClick={() => dispatch(inc())} className="btn btn-primary">INC</button>
			<button onClick={() => dispatch(rnd())} className="btn btn-primary">RND</button>
		</div>
	)
}

export default Counter;	  
```	  
	  
  **[⬆ Наверх](#top)**
	
358. ### <a name="358"></a> Соединяем React и Redux при помощи connect и хуков

### При помощи connect	  
```jsx harmony
import { Component } from "react";
import { connect } from "react-redux";
import * as actions from '../actions';

// const Counter = ({counter, inc, dec, rnd}) => {
//     return (
//         <div className="jumbotron">
//             <h1>{counter}</h1>
//             <button onClick={dec} className="btn btn-primary">DEC</button>
//             <button onClick={inc} className="btn btn-primary">INC</button>
//             <button onClick={rnd} className="btn btn-primary">RND</button>
//         </div>
//     )
// }

class Counter extends Component {
    render() {
        const {counter, inc, dec, rnd} = this.props;
        return (
            <div className="jumbotron">
                <h1>{counter}</h1>
                <button onClick={dec} className="btn btn-primary">DEC</button>
                <button onClick={inc} className="btn btn-primary">INC</button>
                <button onClick={rnd} className="btn btn-primary">RND</button>
            </div>
        )
    }
}

const mapStateToProps = (state) => {
    return {
        counter: state.value
    }
}
	  
// const mapDispatchToProps = (dispatch) => {
// 	return bindActionCreators(actions, dispatch)
// }	  

export default connect(mapStateToProps, actions)(Counter);	  
```	  

### При помощи хуков
	  
```jsx harmony
import {inc, dec, rnd} from '../actions';
import { useSelector, useDispatch } from "react-redux";

const Counter = () => {

    const counter = useSelector(state => state.counter);
    const dispatch = useDispatch();
    
    return (
        <div className="jumbotron">
            <h1>{counter}</h1>
            <button onClick={() => dispatch(dec())} className="btn btn-primary">DEC</button>
            <button onClick={() => dispatch(inc())} className="btn btn-primary">INC</button>
            <button onClick={() => dispatch(rnd())} className="btn btn-primary">RND</button>
        </div>
    )
}

export default Counter;	  
```	  
	  
  **[⬆ Наверх](#top)**
	
359. ### <a name="359"></a> combineReducers и reducers

```jsx harmony
import { createStore, combineReducers } from 'redux';
import heroes from '../reducers/heroes';
import filters from '../reducers/filters';

const store = createStore( combineReducers({heroes, filters}),
    window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__());

export default store;	  
```	  

```jsx harmony
const initialState = {
    filters: [],
    filtersLoadingStatus: 'idle',
    activeFilter: 'all'
}

const filters = (state = initialState, action) => {
    switch (action.type) {
        case 'FILTERS_FETCHING':
            return {
                ...state,
                filtersLoadingStatus: 'loading'
            }
        case 'FILTERS_FETCHED':
            return {
                ...state,
                filters: action.payload,
                filtersLoadingStatus: 'idle'
            }
        case 'FILTERS_FETCHING_ERROR':
            return {
                ...state,
                filtersLoadingStatus: 'error'
            }
        case 'ACTIVE_FILTER_CHANGED':
            return {
                ...state,
                activeFilter: action.payload
            }
        default: return state
    }
}

export default filters;	  
```	  

```jsx harmony
const initialState = {
    heroes: [],
    heroesLoadingStatus: 'idle'
}

const heroes = (state = initialState, action) => {
    switch (action.type) {
        case 'HEROES_FETCHING':
            return {
                ...state,
                heroesLoadingStatus: 'loading'
            }
        case 'HEROES_FETCHED':
            return {
                ...state,
                heroes: action.payload,
                heroesLoadingStatus: 'idle'
            }
        case 'HEROES_FETCHING_ERROR':
            return {
                ...state,
                heroesLoadingStatus: 'error'
            }
        case 'HERO_CREATED':
            return {
                ...state,
                heroes: [...state.heroes, action.payload]
            }
        case 'HERO_DELETED': 
            return {
                ...state,
                heroes: state.heroes.filter(item => item.id !== action.payload)
            }
        default: return state
    }
}

export default heroes;	  
```	  
	  
  **[⬆ Наверх](#top)**
	
360. ### <a name="360"></a> createSelector from 'reselect'

```jsx harmony
import {useHttp} from '../../hooks/http.hook';
import { useEffect, useCallback } from 'react';
import { useDispatch, useSelector } from 'react-redux';
import { CSSTransition, TransitionGroup} from 'react-transition-group';
import { createSelector } from 'reselect';

import { heroesFetching, heroesFetched, heroesFetchingError, heroDeleted } from '../../actions';
import HeroesListItem from "../heroesListItem/HeroesListItem";
import Spinner from '../spinner/Spinner';

import './heroesList.scss';

const HeroesList = () => {

    const filteredHeroesSelector = createSelector(
        (state) => state.filters.activeFilter,
        (state) => state.heroes.heroes,
        (filter, heroes) => {
            if (filter === 'all') {
                console.log('render');
                return heroes;
            } else {
                return heroes.filter(item => item.element === filter);
            }
        }
    );

    const filteredHeroes = useSelector(filteredHeroesSelector);
    const heroesLoadingStatus = useSelector(state => state.heroes.heroesLoadingStatus);
    const dispatch = useDispatch();
    const {request} = useHttp();

    useEffect(() => {
        dispatch(heroesFetching());
        request("http://localhost:3001/heroes")
            .then(data => dispatch(heroesFetched(data)))
            .catch(() => dispatch(heroesFetchingError()))

        // eslint-disable-next-line
    }, []);

    const onDelete = useCallback((id) => {
        request(`http://localhost:3001/heroes/${id}`, "DELETE")
            .then(data => console.log(data, 'Deleted'))
            .then(dispatch(heroDeleted(id)))
            .catch(err => console.log(err));
        // eslint-disable-next-line  
    }, [request]);

    if (heroesLoadingStatus === "loading") {
        return <Spinner/>;
    } else if (heroesLoadingStatus === "error") {
        return <h5 className="text-center mt-5">Ошибка загрузки</h5>
    }

    const renderHeroesList = (arr) => {
        if (arr.length === 0) {
            return (
                <CSSTransition
                    timeout={0}
                    classNames="hero">
                    <h5 className="text-center mt-5">Героев пока нет</h5>
                </CSSTransition>
            )
        }

        return arr.map(({id, ...props}) => {
            return (
                <CSSTransition 
                    key={id}
                    timeout={500}
                    classNames="hero">
                    <HeroesListItem  {...props} onDelete={() => onDelete(id)}/>
                </CSSTransition>
            )
        })
    }

    const elements = renderHeroesList(filteredHeroes);
    return (
        <TransitionGroup component="ul">
            {elements}
        </TransitionGroup>
    )
}

export default HeroesList;	  
```	  
    
  **[⬆ Наверх](#top)**
	
361. ### <a name="361"></a> enhancer

```jsx harmony
import { createStore, combineReducers, compose } from 'redux';
import heroes from '../reducers/heroes';
import filters from '../reducers/filters';

const enhancer = (createStore) => (...args) => {
    const store = createStore(...args);

    const oldDispatch = store.dispatch;
    store.dispatch = (action) => {
        if (typeof action === 'string') {
            return oldDispatch({
                type: action
            })
        }
        return oldDispatch(action)
    }
    return store;
}

const store = createStore( 
                    combineReducers({heroes, filters}),
                    compose(
                        enhancer,
                        window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__()
                    ));

export default store;			
```			
    
  **[⬆ Наверх](#top)**
	
362. ### <a name="362"></a> applyMiddleware

```jsx harmony
import { createStore, combineReducers, compose, applyMiddleware } from 'redux';
import heroes from '../reducers/heroes';
import filters from '../reducers/filters';

const stringMiddleware = () => (next) => (action) => {
    if (typeof action === 'string') {
        return next({
            type: action
        })
    }
    return next(action)
};

const store = createStore( 
                    combineReducers({heroes, filters}),
                    compose(applyMiddleware(stringMiddleware),
                            window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__())
                    );

export default store;			
```			
    
  **[⬆ Наверх](#top)**
	
363. ### <a name="363"></a> ReduxThunk

```jsx harmony
import { createStore, combineReducers, compose, applyMiddleware } from 'redux';
import ReduxThunk from 'redux-thunk';
import heroes from '../reducers/heroes';
import filters from '../reducers/filters';

const stringMiddleware = () => (next) => (action) => {
    if (typeof action === 'string') {
        return next({
            type: action
        })
    }
    return next(action)
};

const store = createStore( 
                combineReducers({heroes, filters}),
                compose(applyMiddleware(ReduxThunk, stringMiddleware),
                        window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__())
                );

export default store;			
```			
    
  **[⬆ Наверх](#top)**
	  
364. ### <a name="364"></a> 

    
  **[⬆ Наверх](#top)**

365. ### <a name="365"></a> 

    
  **[⬆ Наверх](#top)**
			
366. ### <a name="366"></a> 

    
  **[⬆ Наверх](#top)**			

377. ### <a name="377"></a> 

 
    
  **[⬆ Наверх](#top)**	
		
378. ### <a name="378"></a> 

 
    
  **[⬆ Наверх](#top)**	
		
379. ### <a name="379"></a> 

 
    
  **[⬆ Наверх](#top)**	
		
380. ### <a name="380"></a> 


    
  **[⬆ Наверх](#top)**
