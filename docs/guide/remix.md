---
sidebar_position: 2.4
title: Руководство по Remix
description: Руководство по Remix
keywords: [javascript, js, react.js, reactjs, react, remix, progressive enhancement single page apps, pespa, guide, руководство, мета-фреймворк]
tags: [javascript, js, react.js, reactjs, react, remix, progressive enhancement single page apps, pespa, guide, руководство, мета-фреймворк]
---

# Remix

> [Remix](https://remix.run/) - фреймворк для создания клиент-серверных веб-приложений на JavaScript ([React](https://ru.reactjs.org/)) со встроенной поддержкой [TypeScript](https://www.typescriptlang.org/).

Remix позволяет разрабатывать так называемые PESPA (Progressive Enhancement Single Page Apps - одностраничные приложения с возможностью прогрессивного улучшения). Это означает следующее:

- почти весь код приложения "живет" на сервере;
- приложение остается функциональным даже при отсутствии JS;
- JS используется только для прогрессивного улучшения UX (User Experience - пользовательский опыт).

Подробнее о PESPA и других архитектурах веб-приложений можно почитать [здесь](https://habr.com/ru/company/timeweb/blog/695798/).

## Маршрутизация / Routing

Маршрутизация (роутинг) - это, пожалуй, самая важная концепция в Remix. Все начинается с маршрутов (роутов): компилятор, первоначальный запрос документа и обработка почти всех последующих действий пользователя.

Начнем с определения понятий:

- вложенные роуты (nested routes) - связь (map) роутов с сегментами URL обеспечивает соответствие URL определенным компонентам и данным, известным перед рендерингом страницы;
- URL - полный путь в поисковой строке браузера пользователя. Один URL может совпадать (соответствовать - match) с несколькими роутами. _Обратите внимание_: роут и URL - разные вещи в Remix;
- роут (route) или модуль роута (route module) - модуль JS с определенными экспортами (`loader`, `action`, `default function` (компонент) и др.), который соответствует одному или нескольким сегментам URL. Поскольку роут соответствует сегменту URL, по одному пути могут рендерится несколько модулей. Иерархия компонентов соответствует сегментам URL (в основном);
- путь (path) или путь роута (route path) - сегмент URL, которому соответствует отдельный модуль. Путь роута определяется названием файла в директории `app/routes`;
- родительский макет (parent layout route) или родительский роут (parent route) - модуль, который рендерит макет для дочерних компонентов через компонент `Outlet`;
- макет без пути (pathless layout route) или роут без пути (pathless route) - модуль, который не добавляет сегменты к URL, но добавляет компонент в иерархию UI (User Interface - пользовательский интерфейс) при совпадении его дочерних роутов;
- дочерний роут (child route) - модуль, который рендерится внутри родительского `Outlet` при совпадении его пути с URL;
- индексный роут (index route) - модуль, который имеет такой же путь, как его родительский роут, но рендерится в качестве дефолтного дочернего роута внутри `Outlet`;
- динамический сегмент (dynamic segment) - сегмент пути роута, извлекаемый из URL и передаваемый в приложение, такой как идентификатор (ID) записи или слаг (slug) поста;
- сплат (splat) - замыкающая звездочка (trailing wildcard) в пути роута, который благодаря этому совпадает со всеми сегментами URL (включая последующий `/`);
- аутлет (outlet) - компонент, который рендерится внутри родительского модуля, предназначенный для рендеринга дочерних модулей. Другими словами, аутлет определяет локацию дочерних роутов.

### Вложенный роутинг

Вложенный роутинг - это связь между сегментами URL и иерархией компонентов в UI. Сегменты URL определяют:

- макеты, формирующие страницу;
- загрузку JS-кода, используемого на странице;
- загрузку данных, используемых на странице.

__Определение роутов__

Роуты определяются посредством создания файлов в директории `app/routes`. Вот как может выглядеть иерархия роутов приложения:

```
app
├── root.jsx
└── routes
    ├── accounts.jsx
    ├── dashboard.jsx
    ├── expenses.jsx
    ├── index.jsx
    ├── reports.jsx
    ├── sales
    │   ├── customers.jsx
    │   ├── deposits.jsx
    │   ├── index.jsx
    │   ├── invoices
    │   │   ├── $invoiceId.jsx
    │   │   └── index.jsx
    │   ├── invoices.jsx
    │   └── subscriptions.jsx
    └── sales.jsx
```

- `root.jsx` - это корневой роут, служащий макетом для всего приложения. Другие роуты рендерятся внутри его `Outlet`;
- _обратите внимание_ на файлы, названия которых совпадают с названиями директорий, в которых эти файлы находятся. Эти файлы предназначены для формирования иерархии макетов компонентов. Например, `sales.jsx` - это родительский роут для всех дочерних роутов внутри директории `app/routes/sales`. При совпадении с URL любого роута из этой директории, он будет рендерится внутри `Outlet` модуля `sales.jsx`;
- роут `index.jsx` будет рендерится внутри `Outlet` при совпадении URL с путем директории (например, пути `example.com/sales` соответствует роут `app/routes/sales/index.jsx`).

__Рендеринг иерархии макета роута__

Предположим, что URL имеет вид `/sales/invoices/123`. С этим URL будут совпадать следующие роуты:

- `root.jsx`;
- `routes/sales.jsx`;
- `routes/sales/invoices.jsx`;
- `routes/sales/invoices/$invoiceId.jsx`.

При посещении этой страницы пользователем Remix отрендерит такую иерархию компонентов:

```javascript
<Root>
  <Sales>
    <Invoices>
      <InvoiceId />
    </Invoices>
  </Sales>
</Root>
```

Иерархия компонентов полностью соответствует иерархии файлов в директории `app/routes`:

```
app
├── root.jsx
└── routes
    ├── sales
    │   ├── invoices
    │   │   └── $invoiceId.jsx
    │   └── invoices.jsx
    ├── sales.jsx
    └── accounts.jsx
```

Иерархия компонентов для URL `/accounts` будет такой:

```javascript
<Root>
  <Accounts />
</Root>
```

Для рендеринга дочерних роутов внутри родительского используется `Outlet`. `root.jsx` рендерит основной макет, боковую панель и аутлет для дочерних роутов:

```javascript
import { Outlet } from "@remix-run/react";

export default function Root() {
  return (
    <Document>
      <Sidebar />
      {/* ! */}
      <Outlet />
    </Document>
  );
}
```

В свою очередь, `sales.jsx` рендерит аутлет для всех его дочерних роутов (`app/routes/sales/*`):

```javascript
import { Outlet } from "@remix-run/react";

export default function Sales() {
  return (
    <div>
      <h1>Sales</h1>
      <SalesNav />
      {/* ! */}
      <Outlet />
    </div>
  );
}
```

__Индексные роуты__

Индексный роут - это дефолтный дочерний роут. При отсутствии других дочерних роутов рендерится индексный модуль. Например, URL `exmaple.com/sales` соответствует индексный роут `app/routes/sales/index.jsx`.

Индексные роуты не должны рендерить дочерние модули, они являются тупиком для URL. Например, вместо рендеринга глобальной панели навигации в `app/routes/index.jsx`, ее следует рендерить в `app/root.jsx`.

__Параметр строки запроса `?index`__

Данный параметр позволяет отличать индексные роуты от их родительский модулей, которые рендерят макеты. Предположим, что у нас имеется такая иерархия роутов:

```
└── app
    ├── root.jsx
    └── routes
        ├── sales
        │   ├── invoices
        │   │   └── index.jsx
        │   └── invoices.jsx
```

Какому роуту будет соответствовать путь `/sales/invoices`? Роуту `/sales/invoices.jsx` или роуту `/sales/invoices/index.jsx`? Ответ: роуту `/sales/invoices.jsx`. Для совпадения с роутом `/sales/invoices/index.jsx` путь должен заканчиваться параметром строки запроса `?index`:

```
└── app
    ├── root.jsx
    └── routes
        ├── sales
        │   ├── invoices
        │   │   └── index.jsx   <-- /sales/invoices?index
        │   └── invoices.jsx    <-- /sales/invoices
```

В некоторых случаях добавление `?index` происходит автоматически (например, при отправке формы в индексном или его родительском роуте), в других - это делается вручную (например, при использовании `fetcher.submit()` или `fetcher.load()`).

### Вложенные URL без вложенных макетов

Иногда может потребоваться добавить вложенный URL без добавления компонента в иерархию UI. Рассмотрим страницу редактирования счета:

- мы хотим, чтобы URL имел вид `/sales/invoices/$invoiceId/edit`;
- мы хотим, чтобы соответствующий компонент был прямым потомком корневого компонента.

Другими словами, мы не хотим этого:

```javascript
<Root>
  <Sales>
    <Invoices>
      <InvoiceId>
        <EditInvoice />
      </InvoiceId>
    </Invoices>
  </Sales>
</Root>
```

Мы хотим это:

```javascript
<Root>
  <EditInvoice />
</Root>
```

Для создания плоской иерархии UI используется плоское название файла - использование `.` в названии файла позволяет добавлять сегменты URL без добавления компонентов в иерархию UI:

```
└── app
    ├── root.jsx
    └── routes
        ├── sales
        │   ├── invoices
        │   │   └── $invoiceId.jsx
        │   └── invoices.jsx
        ├── sales.invoices.$invoiceId.edit.jsx 👈 не является вложенным
        └── sales.jsx
```

Пути `example.com/sales/invoices/123/edit` будет соответствовать такая иерархия компонентов:

```javascript
<Root>
  <EditInvoice />
</Root>
```

А пути `example.com/sales/invoices/123` (без `/edit`) такая:

```javascript
<Root>
  <Sales>
    <Invoices>
      <InvoiceId />
    </Invoices>
  </Sales>
</Root>
```

### Макеты без пути

Иногда, наоборот, может потребоваться добавить компонент в иерархию UI без добавления сегментов в URL. Для этого используются макеты без пути.

Предположим, что мы хотим получить такую иерархию UI:

```javascript
<Root>
  <Auth>
    <Login />
  </Auth>
</Root>
```

В данном случае иерархия роутов может выглядеть так:

```
app
├── root.jsx
└── routes
    ├── auth
    │   ├── login.jsx
    │   ├── logout.jsx
    │   └── signup.jsx
    └── auth.jsx
```

У нас имеется правильная иерархия UI, но, возможно, мы не хотим, чтобы каждый URL содержал префикс `/auth`, например, вместо `/auth/login` мы хотим видеть просто `/login`.

Для удаления вложенности URL при сохранении вложенности UI достаточно добавить к названиям роута и директории 2 нижних подчеркивания:

```
app
├── root.jsx
└── routes
    ├── __auth
    │   ├── login.jsx
    │   ├── logout.jsx
    │   └── signup.jsx
    └── __auth.jsx
```

### Динамические сегменты

Если название файла содержит префикс `$`, соответствующая часть пути роута становится динамическим сегментом. Это означает, что любое значение в URL для данного сегмента будет извлекаться из URL и передаваться в приложение.

Рассмотрим роут `$invoiceId.jsx`. При переходе по адресу `/sales/invoices/123` строка `123` будет извлечена из URL и передана в `loader`, `action` и компонент в виде одноименного свойства объекта `params`:

```javascript
import { useParams } from "@remix-run/react";

export async function loader({ params }) {
  const id = params.invoiceId;
}

export async function action({ params }) {
  const id = params.invoiceId;
}

export default function Invoice() {
  const params = useParams();
  const id = params.invoiceId;
}
```

Роуты могут содержать несколько параметров. Параметры могут быть директориями.

```
app
├── root.jsx
└── routes
    ├── projects
    │   ├── $projectId
    │   │   └── $taskId.jsx
    │   └── $projectId.jsx
    └── projects.jsx
```

В данном случае при переходе по адресу `/projects/123/abc` параметры буду следующими:

```
params.projectId; // "123"
params.taskId; // "abc"
```

### Сплаты

Если название файла содержит только `$` (`$.jsx`), то такой роут является сплатом. С таким роутом совпадает любое значение URL для оставшейся части URL до конца. В отличие от динамических сегментов, сплат не останавливается при достижении следующего `/`.

Рассмотрим такую иерархию роутов:

```
app
├── root.jsx
└── routes
    ├── files
    │   ├── $.jsx
    │   ├── mine.jsx
    │   └── recent.jsx
    └── files.jsx
```

При переходе по адресу `example.com/files/images/work/flyer.jpg`, сегменты URL, начиная с `files` будут перехвачены сплатом и доступны в приложении через `params["*"]`:

```javascript
export async function loader({ params }) {
  params["*"]; // "images/work/flyer.jpg"
}
```

Сплаты могут использоваться для реализации кастомных страниц 404 с данными из `loader` (при отсутствии кастомной страницы 404 рендерится корневой `CatchBoundary`, не позволяющий загружать данные для страницы при отсутствии совпадения с роутами).

## Ресурсные роуты / Resource Routes

Ресурсные роуты не являются частью UI, но являются частью приложения. Они могут возвращать любые ответы.

Большая часть роутов в Remix является роутами UI, т.е. роутами, которые рендерят компоненты. Но роут не обязательно должен это делать. Роуты, которые не экспортируют дефолтные компоненты, являются ресурсными. Случаи их использования:

- JSON API для мобильных приложений, которые повторно используют серверный код с Remix UI;
- динамическая генерация PDF;
- динамическая генерация иконок социальных сетей для постов блога или других страниц;
- веб-хуки для сервисов вроде Stripe или GitHub;
- CSS-файлы, которые динамически рендерят кастомные свойства для темы, выбранной пользователем.

### Создание ресурсного роута

Ресурсный роут должен экспортировать либо `loader` (для обработки GET-запросов), либо `action` (для обработки других запросов).

Рассмотрим роут для рендеринга отчета (внимание на ссылку):

```javascript
// app/routes/reports/$id.tsx
export async function loader({ params }: LoaderArgs) {
  return json(await getReport(params.id));
}

export default function Report() {
  const report = useLoaderData<typeof loader>();

  return (
    <div>
      <h1>{report.name}</h1>
      <Link to="pdf" reloadDocument>
        PDF
      </Link>
      {/* ... */}
    </div>
  );
}
```

Ссылка ведет на PDF-версию страницы. Для ее создания необходимо реализовать ресурсный роут:

```javascript
// app/routes/reports/$id/pdf.tsx
export async function loader({ params }: LoaderArgs) {
  const report = await getReport(params.id);

  const pdf = await generateReportPDF(report);

  return new Response(pdf, {
    status: 200,
    headers: {
      "Content-Type": "application/pdf",
    },
  });
}
```

Когда пользователь нажимает на ссылку, он получает отчет в формате PDF.

_Обратите внимание_: в качестве ссылки на ресурсный роут следует использовать либо компонент `Link` с атрибутом `reloadDocument`, либо HTML-элемент `a`. `Link` без `reloadDocument` считается ссылкой на роут UI.

Для того, чтобы добавить расширение файла к пути ресурсного роута, можно обернуть расширение или `.` в `[]`:

```bash
# /reports/123/pdf
app/routes/reports/$id/pdf.ts

# /reports/123.pdf
app/routes/reports/$id[.pdf].ts

# /reports/123.pdf
app/routes/reports/$id[.]pdf.ts
```

### Обработка разных методов

Для обработки GET-запросов из ресурсного роута экспортируется `loader`:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";

export const loader = async ({ request }: LoaderArgs) => {
  return json({ success: true }, 200);
};
```

Для обработки других запросов из ресурсного роута экспортируется `action`:

```javascript
import type { ActionArgs } from "@remix-run/node";

export const action = async ({ request }: ActionArgs) => {
  switch (request.method) {
    case "POST": {
      // ...
    }
    case "PUT": {
      // ...
    }
    case "PATCH": {
      // ...
    }
    case "DELETE": {
      // ...
    }
    default: {
      throw new Response("Неизвестный метод", {
        status: 400
      })
    }
  }
};
```

### Веб-хуки

Пример веб-хука для получения уведомлений о создании нового коммита в репозитории GitHub:

```javascript
import type { ActionArgs } from "@remix-run/node";
import { json } from "@remix-run/node";
import crypto from "crypto";

export const action = async ({ request }: ActionArgs) => {
  if (request.method !== "POST") {
    return json({ message: "Метод запрещен" }, 405);
  }

  const payload = await request.json();

  /* валидируем веб-хук */
  const signature = request.headers.get(
    "X-Hub-Signature-256"
  );
  const generatedSignature = `sha256=${crypto
    .createHmac("sha256", process.env.GITHUB_WEBHOOK_SECRET)
    .update(JSON.stringify(payload))
    .digest("hex")}`;

  if (signature !== generatedSignature) {
    return json({ message: "Signature mismatch" }, 401);
  }

  /* обрабатываем веб-хук (например, помещаем фоновую задачу в очередь) */

  return json({ success: true }, 200);
};
```

## Интерфейс роутов / API Routes

Рассмотрим такой роут:

```javascript
// routes/teams.tsx
export async function loader() {
  return json(await getTeams());
}

export default function Teams() {
  return (
    <TeamsView teams={useLoaderData<typeof loader>()} />
  );
}
```

При клике пользователем по `<Link to="/teams" />` Remix запрашивает данные у сервера в `loader` и рендерит модуль. Таким образом, нам не нужен отдельный роут для взаимодействия с API.

Что если мы хотим получить данные из `loader` без участия пользователя? Хорошим примером такой ситуации является компонент Combobox, который получает записи из БД и предлагает их пользователю.

Для этого можно использовать хук `useFetcher`.

Предположим, что у нас есть такой роут для обработки поиска:

```javascript
// routes/city-search.tsx
export async function loader({ request }: LoaderArgs) {
  const url = new URL(request.url);

  return json(
    await searchCities(url.searchParams.get("q"))
  );
}
```

Вызываем `useFetcher()` в соответствующем компоненте:

```javascript
function CitySearchCombobox() {
  const cities = useFetcher();

  return (
    <cities.Form method="get" action="/city-search">
      <Combobox aria-label="Cities">
        <div>
          <ComboboxInput
            name="q"
            onChange={(event) =>
              cities.submit(event.target.form)
            }
          />
          {cities.state === "submitting" ? (
            <Spinner />
          ) : null}
        </div>

        {cities.data ? (
          <ComboboxPopover className="shadow-popup">
            {cities.data.error ? (
              <p>Не удалось загрузить список городов</p>
            ) : cities.data.length ? (
              <ComboboxList>
                {cities.data.map((city) => (
                  <ComboboxOption
                    key={city.id}
                    value={city.name}
                  />
                ))}
              </ComboboxList>
            ) : (
              <span>Подходящих городов не найдено</span>
            )}
          </ComboboxPopover>
        ) : null}
      </Combobox>
    </cities.Form>
  );
}
```

## Бэкенд для фронтенда / Backend for frontend

Несмотря на то, что Remix предназначен для разработки фуллстек-приложений, он отлично вписывается в архитектуру "Бэкенд для фронтенда". Эта архитектура предполагает использование Remix в качестве посредника между UI и существующими серверными сервисами.

Поскольку Remix "полифиллит" Web Fetch API, мы можем использовать `fetch` прямо в `loader` и `action` для получения данных от сервера:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";
import escapeHtml from "escape-html";

export async function loader({ request }: LoaderArgs) {
  const apiUrl = "http://api.example.com/some-data.json";

  const res = await fetch(apiUrl, {
    headers: {
      Authorization: `Bearer ${process.env.API_TOKEN}`,
    },
  });

  const data = await res.json();

  const prunedData = data.map((record) => {
    return {
      id: record.id,
      title: record.title,
      formattedBody: escapeHtml(record.content),
    };
  });

  return json(prunedData);
}
```

Такой подход позволяет:

- упростить интеграцию со сторонними сервисами, а также хранить токены и секреты вне сборки для клиента;
- сократить количество данных, передаваемых по сети, что может существенно повысить производительность приложения;
- перенести большое количество кода на сервер, что также хорошо влияет на производительность приложения.

## Загрузка данных / Data Loading

Одним из главных преимуществ Remix является упрощение взаимодействия с сервером для получения данных в компонентах. Remix автоматически:

- рендерит страницы на сервере;
- является устойчивым к изменениям сетевых условий;
- загружает только те данные, которые необходимы для обновления страницы;
- загружает данные, JS-модули, CSS и другие ресурсы параллельно при переходе с одной страницы на другую. Это позволяет избежать водопадов (waterfalls) рендеринг+получение данных, что приводит к более согласованному UI;
- обеспечивает синхронизацию между данными в UI и на сервере путем повторного запуска `action`;
- обеспечивает восстановление прокрутки;
- обрабатывает серверные ошибки с помощью предохранителей (error boundaries);
- обеспечивает хороший UX для "Не найдено" и "Не авторизован" с помощью перехватчиков (catch boundaries).

### Основы

Каждый модуль может экспортировать компонент и функцию `loader`. Хук `useLoaderData` позволяет получать данные из `loader` в компоненте:

```javascript
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

export const loader = async () => {
  return json([
    { id: "1", name: "Pants" },
    { id: "2", name: "Jacket" },
  ]);
};

export default function Products() {
  const products = useLoaderData<typeof loader>();

  return (
    <div>
      <h1>Список товаров</h1>
      {products.map((product) => (
        <div key={product.id}>{product.name}</div>
      ))}
    </div>
  );
}
```

Компонент рендерится как на сервере, так и в браузере. `loader` выполняется только на сервере. Это означает, что массив товаров не включается в сборку для браузера. Это также означает, что мы можем безопасно использовать серверные API и SDK для базы данных, обработки платежей, CMS и т.д.

Если серверные модули включаются в клиентскую сборку, импорт этих модулей следует перенести в файл с названием, содержащим суффикс `.server.ts` (`{something}.server.ts`).

### Параметры роута

Когда в названии файла содержится символ `$`, например, `routes/users/$userId.tsx` или `routes/users/$userId/projects/$projectId.tsx`, динамические сегменты (начинающиеся с `$`) извлекаются из URL и передаются в `loader` в качестве объекта `params`:

```javascript
import type { LoaderArgs } from "@remix-run/node";

export const loader = async ({ params }: LoaderArgs) => {
  console.log(params.userId);
  console.log(params.projectId);
};
```

Эти параметры могут использоваться для поиска необходимых данных:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";

export const loader = async ({ params }: LoaderArgs) => {
  return json(
    await fakeDb.project.findMany({
      where: {
        userId: params.userId,
        projectId: params.projectId,
      },
    })
  );
};
```

__Типы параметров__

Поскольку параметры содержатся в URL, а не в исходном коде, мы не можем быть уверены в том, что они всегда будут определены. Поэтому типом ключей параметров является `string | undefined`. Хорошей практикой является валидация параметров перед их использованием, например, с помощью `invariant`:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import invariant from "tiny-invariant";

export const loader = async ({ params }: LoaderArgs) => {
  invariant(params.userId, "Ожидается params.userId");
  invariant(params.projectId, "Ожидается params.projectId");

  params.projectId; // <-- TS теперь знает, что типом `projectId` является `string`
};
```

Для обработки таких исключений используются предохранители (error boundaries).

### Внешние API

Remix предоставляет полифилл для `fetch` на сервере, что облегчает получение данных из существующих JSON API. Вместо управления состоянием, обработки ошибок, решения проблем, связанных с гонкой условий (race conditions) и т.п., мы просто запрашиваем данные в `loader` (на сервере), а Remix делает все остальное:

```javascript
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

export async function loader() {
  const res = await fetch("https://api.github.com/gists");

  return json(await res.json());
}

export default function GistsRoute() {
  const gists = useLoaderData<typeof loader>();

  return (
    <ul>
      {gists.map((gist) => (
        <li key={gist.id}>
          <a href={gist.html_url}>{gist.id}</a>
        </li>
      ))}
    </ul>
  );
}
```

### База данных

Поскольку Remix выполняется на сервере, мы можем напрямую подключаться к БД в модулях. Пример подключения к Postgres с помощью [Prisma](https://prisma.io/):

```javascript
// app/db.server.ts
import { PrismaClient } from "@prisma/client";
const db = new PrismaClient();
export default db;
```

```javascript
// app/routes/products/$categoryId.tsx
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import db from "~/db.server";

export const loader = async ({ params }: LoaderArgs) => {
  return json(
    await db.product.findMany({
      where: {
        categoryId: params.categoryId,
      },
    })
  );
};

export default function ProductCategory() {
  const products = useLoaderData<typeof loader>();

  return (
    <div>
      <p>{products.length} Товаров</p>
      {/* ... */}
    </div>
  );
}
```

Для типизации данных можно использовать типы, генерируемые Prisma Client, при вызове `useLoaderData()`:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import db from "~/db.server";

async function getLoaderData(productId: string) {
  const product = await db.product.findUnique({
    where: {
      id: productId,
    },
    select: {
      id: true,
      name: true,
      imgSrc: true,
    },
  });

  return product;
}

export const loader = async ({ params }: LoaderArgs) => {
  return json(await getLoaderData(params.productId));
};

export default function Product() {
  const product = useLoaderData<typeof loader>();

  return (
    <div>
      <p>Товар {product.id}</p>
      {/* ... */}
    </div>
  );
}
```

### Не найдено

При отсутствии записи в БД достаточно выбросить ответ в `loader` и Remix остановит выполнение кода и передаст управление ближайшему перехватчику (catch boundary):

```javascript
export const loader = async ({
  params,
  request,
}: LoaderArgs) => {
  const product = await db.product.findOne({
    where: { id: params.productId },
  });

  if (!product) {
    // мы не можем отрендерить компонент,
    // поэтому выбрасываем ответ для остановки выполнения кода
    // и отображения страницы "Не найдено"
    throw new Response("Not Found", { status: 404 });
  }

  const cart = await getCart(request);

  return json({
    product,
    inCart: cart.includes(product.id),
  });
};
```

### Параметры строки запроса

Параметры строки запроса (поисковой строки) (URL Search Params) - это часть URL, следующая за `?`. Эти параметры доступны в `request.url`:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";

export const loader = async ({ request }: LoaderArgs) => {
  const url = new URL(request.url);
  const term = url.searchParams.get("term");

  return json(await fakeProductSearch(term));
};
```

Здесь:

- объект [request](https://developer.mozilla.org/en-US/docs/Web/API/Request) содержит свойство `url`;
- конструктор [URL](https://developer.mozilla.org/en-US/docs/Web/API/URL) преобразует строку URL в объект;
- `url.searchParams` - это экземпляр [URLSearchParams](https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams), содержащий преобразованную в объект строку запроса.

__Перезагрузка данных__

При изменении строки запроса в случае с рендерингом нескольких вложенных роутов, все эти роуты перезагружаются. Это связано с тем, что параметры строки запроса могут использоваться любым `loader` в этих роутах. Для предотвращения рендеринга отдельных роутов можно использовать [shouldReload](https://remix.run/docs/en/v1/route/should-reload) (данный интерфейс пока является нестабильным, поэтому в рамках этого руководства не рассматривается).

__Параметры строки запроса в компонентах__

Иногда требуется читать и обновлять параметры строки запроса в компонентах, а не в `loader` или `action`. Существует несколько способов это делать.

_Установка параметров строки запроса_

Пример модификации строки запроса пользователем:

```javascript
// app/products/shoes
export default function ProductFilters() {
  return (
    <Form method="get">
      <label htmlFor="nike">Nike</label>
      <input
        type="checkbox"
        id="nike"
        name="brand"
        value="nike"
      />

      <label htmlFor="adidas">Adidas</label>
      <input
        type="checkbox"
        id="adidas"
        name="brand"
        value="adidas"
      />

      <button type="submit">Обновить</button>
    </Form>
  );
}
```

Если пользователь выбрал один бренд, например, Nike, то строка запроса будет иметь вид `/products/shoes?brand=nike`, если оба, то `/products/shoes?brand=nike&brand=adidas`.

_Обратите внимание_, что `brand` повторяется в строке запроса, поскольку оба чекбокса называются `brand`. Для доступа к этим значениям в `loader` предназначен метод `searchParams.getAll`:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";

export async function loader({ request }: LoaderArgs) {
  const url = new URL(request.url);
  const brands = url.searchParams.getAll("brand");

  return json(await getProducts({ brands }));
}
```

__Дополнение URL строкой запроса__

URL легко дополняется строкой запроса с помощью компонента `Link`:

```javascript
<Link to="?brand=nike">Nike (только)</Link>
```

__Чтение параметров строки запроса в компонентах__

Для доступа к параметрам строки запроса в компонентах используется хук `useSearchParams`:

```javascript
import { useSearchParams } from "@remix-run/react";

export default function ProductFilters() {
  const [searchParams] = useSearchParams();
  const brands = searchParams.getAll("brand");

  return (
    <Form method="get">
      <label htmlFor="nike">Nike</label>
      <input
        type="checkbox"
        id="nike"
        name="brand"
        value="nike"
        defaultChecked={brands.includes("nike")}
      />

      <label htmlFor="adidas">Adidas</label>
      <input
        type="checkbox"
        id="adidas"
        name="brand"
        value="adidas"
        defaultChecked={brands.includes("adidas")}
      />

      <button type="submit">Обновить</button>
    </Form>
  );
}
```

С помощью хука `useSubmit` можно отправлять форму при изменении значения любого поля:

```javascript
import {
  useSubmit,
  useSearchParams,
} from "@remix-run/react";

export default function ProductFilters() {
  const submit = useSubmit();
  const [searchParams] = useSearchParams();
  const brands = searchParams.getAll("brand");

  return (
    <Form
      method="get"
      onChange={(e) => submit(e.currentTarget)}
    >
      {/* ... */}
    </Form>
  );
}
```

__Параметры строки запроса и управляемые инпуты__

Что если мы хотим синхронизировать состояние чекбоксов со строкой запроса? В случае с управляемыми инпутами (controlled inputs) сделать это не так просто, как может показаться на первый взгляд.

Предположим, что для изменения бренда в компоненте может использоваться как `<input type="checkbox">` так и `<Link />`:

```javascript
import { useSearchParams } from "@remix-run/react";

export default function ProductFilters() {
  const [searchParams] = useSearchParams();
  const brands = searchParams.getAll("brand");

  return (
    <Form method="get">
      <p>
        <label htmlFor="nike">Nike</label>
        <input
          type="checkbox"
          id="nike"
          name="brand"
          value="nike"
          defaultChecked={brands.includes("nike")}
        />
        <Link to="?brand=nike">Nike</Link>
      </p>

      <button type="submit">Обновить</button>
    </Form>
  );
}
```

Если пользователь выбирает чекбокс и отправляет форму, URL обновляется вместе с состоянием чекбокса. Но если пользователь нажимает на ссылку, то обновляется только URL, а состояние чекбокса остается прежним. Что если переключиться с `defaultChecked` на `checked`?

```javascript
<input
  type="checkbox"
  id="adidas"
  name="brand"
  value="adidas"
  checked={brands.includes("adidas")}
/>
```

Возникает другая проблема: при клике по ссылке меняется как URL, так и состояние чекбокса, но сам чекбокс больше не работает, поскольку React не позволяет изменять состояние чекбокса до изменения контролирующего его URL.

Существует, как минимум, 2 решения.

Самым простым является автоматическая отправка формы при выборе чекбокса:

```javascript
import {
  useSubmit,
  useSearchParams,
} from "@remix-run/react";

export default function ProductFilters() {
  const submit = useSubmit();
  const [searchParams] = useSearchParams();
  const brands = searchParams.getAll("brand");

  return (
    <Form method="get">
      <p>
        <label htmlFor="nike">Nike</label>
        <input
          type="checkbox"
          id="nike"
          name="brand"
          value="nike"
          onChange={(e) => submit(e.currentTarget.form)}
          checked={brands.includes("nike")}
        />
        <Link to="?brand=nike">Nike</Link>
      </p>

      {/* ... */}
    </Form>
  );
}
```

_Обратите внимание_: при отправке формы в `onChange()` следует предотвращать распространение события `submit` с помощью `stopPropagation()` во избежание всплытия (bubble) события до формы и ее повторной отправки.

Второе решение предполагает наличие локального состояния для чекбокса:

- инициализируем состояние с помощью параметров строки запроса;
- обновляем состояние при выборе чекбокса пользователем;
- обновляем состояние при изменении строки запроса.

```javascript
import {
  useSubmit,
  useSearchParams,
} from "@remix-run/react";

export default function ProductFilters() {
  const submit = useSubmit();
  const [searchParams] = useSearchParams();
  const brands = searchParams.getAll("brand");

  const [nikeChecked, setNikeChecked] = React.useState(
    // инициализируем состояние с помощью параметров строки запроса
    brands.includes("nike")
  );

  // обновляем состояние при изменении строки запроса
  // (отправка формы или нажатие ссылки)
  React.useEffect(() => {
    setNikeChecked(brands.includes("nike"));
  }, [brands, searchParams]);

  return (
    <Form method="get">
      <p>
        <label htmlFor="nike">Nike</label>
        <input
          type="checkbox"
          id="nike"
          name="brand"
          value="nike"
          onChange={(e) => {
            // обновляем состояние чекбокса без отправки формы
            setNikeChecked(true);
          }}
          checked={nikeChecked}
        />
        <Link to="?brand=nike">Nike</Link>
      </p>

      {/* ... */}
    </Form>
  );
}
```

Эту логику работы с чекбоксами можно абстрагировать следующим образом:

```javascript
<div>
  <SearchCheckbox name="brand" value="nike" />
  <SearchCheckbox name="brand" value="reebok" />
  <SearchCheckbox name="brand" value="adidas" />
</div>;

function SearchCheckbox({ name, value }) {
  const [searchParams] = useSearchParams();
  const all = searchParams.getAll(name);
  const [checked, setChecked] = React.useState(
    all.includes(value)
  );

  React.useEffect(() => {
    setChecked(all.includes(value));
  }, [all, searchParams, value]);

  return (
    <input
      type="checkbox"
      name={name}
      value={value}
      checked={checked}
      onChange={(e) => setChecked(e.target.checked)}
    />
  );
}
```

### Оптимизации

Remix перезагружает все роуты в трех случаях:

- вызов `action` (формы, `useSubmit()`, `fetcher.submit()`);
- изменение строки запроса;
- переход пользователя на текущую страницу (когда пользователь кликает по ссылке, ведущей на страницу, на которой он уже находится).

### Управление состоянием

Remix спроектирован таким образом, что исключает необходимость использования каких-либо библиотек для управления состоянием приложения, вроде  `React Query`, `SWR`, `Apollo`, `Relay`, `urql` и т.д. Однако он вовсе не исключает возможность их использования в случаях, когда возможностей, предоставляемых Remix, недостаточно для реализации функционала приложения.

### Заметки

`loader` выполняется на сервере с помощью `fetch`, предоставляемого браузером, поэтому данные сериализуются с помощью `JSON.stringify()`. Это означает, что данные, возвращаемые загрузчиком, должны быть сериализуемыми. Пример частично несериализуемых данных:

```javascript
export async function loader() {
  return {
    date: new Date(),
    someMethod() {
      return "некоторое значение";
    },
  };
}

export default function RouteComp() {
  const data = useLoaderData<typeof loader>();
  console.log(data);
  // '{"date":"..."}'
}
```

Для доступа к данным, возвращаемым загрузчиком, нельзя использовать `loader`:

```javascript
export const loader = async () => {
  return json(await fakeDb.products.findMany());
};

export default function RouteComp() {
  // не работает
  const data = loader();
}
```

## Запись данных / Data Writes

Запись данных в Remix основана на двух фундаментальных веб-интерфейсах: `<form>` и HTTP. Несмотря на использование прогрессивного улучшения для реализации оптимистичного обновления UI, индикаторов загрузки и отображения результатов валидации, модель программирования по-прежнему основывается на формах HTML.

При отправке формы Remix:

- вызывает `action()` для формы;
- перезагружает все данные (`loader()`) для всех роутов страницы.

Существует несколько способов вызвать `action()` и выполнить повторную валидацию роутов:

- `<Form>`
- `useSubmit()`
- `useFetcher()`

В данном разделе мы будем говорить только о формах.

### Формы

Нативные формы поддерживают 2 глагола (verbs) HTTP: `GET` и `POST`. Эти глаголы сообщают Remix о наших намерениях. В случае с `GET` Remix определяет, какие части страницы меняются и запрашивает данные только для этих частей, а данные для частей, оставшихся прежними, доставляются из кэша. В случае с `POST` Remix перезагружает все данные для обеспечения их согласованности с серверными данными.

__GET__

`GET` - это обычная навигация (navigation), когда данные формы конвертируются в строку запроса URL. Рассмотрим такую форму:

```javascript
<form method="get" action="/search">
  <label>Искать <input name="term" type="text" /></label>
  <button type="submit">Поиск</button>
</form>
```

Когда пользователь заполняет поле `term` и нажимаем "Поиск", браузер преобразуется данные формы в строку запроса и добавляет ее к URL, указанному в `action`. Предположим, что пользователь ввел `Remix`. Тогда браузер выполнит перенаправление к `/search?term=remix`. Если названием инпута будет `q`, браузер выполнит перенаправление к `/search?q=remix`.

Пример с бОльшим количеством полей:

```javascript
<form method="get" action="/search">
  <fieldset>
    <legend>Brand</legend>
    <label>
      <input name="brand" value="nike" type="checkbox" />
      Nike
    </label>
    <label>
      <input name="brand" value="reebok" type="checkbox" />
      Reebok
    </label>
    <label>
      <input name="color" value="white" type="checkbox" />
      Белый
    </label>
    <label>
      <input name="color" value="black" type="checkbox" />
      Черный
    </label>
    <button type="submit">Поиск</button>
  </fieldset>
</form>
```

В зависимости от того, какие чекбоксы выбрал пользователь, браузер будет выполнять перенаправления к таким URL:

```
/search?brand=nike&color=black
/search?brand=nike&brand=reebok&color=white
```

__POST__

Для создания, обновления или удаления данных используется метод `POST`. И речь идет не только о больших формах, например, для редактирования профиля пользователя, но и о кнопках типа "Нравится", обернутых в форму. Рассмотрим такую форму для создания нового проекта:

```javascript
<form method="post" action="/projects">
  <label>Название: <input name="name" type="text" /></label>
  <label>Описание: <textarea name="description"></textarea></label>
  <button type="submit">Создать</button>
</form>
```

Когда пользователь нажимает "Создать", браузер преобразует данные формы в тело запроса (request body) и отправляет запрос на сервер. После этого данные становятся доступными для обработчика запросов на сервере, что позволяет создать ноую запись в БД. Обработчик должен вернуть ответ. Вероятно, после создания записи нам следует перенаправить пользователя на страницу с только что созданным проектом:

```javascript
export async function action({ request }: ActionArgs) {
  const body = await request.formData();
  // создаем проект
  const project = await createProject(body);
  // выполняем перенаправление
  return redirect(`/projects/${project.id}`);
}
```

Собственно, это все, что требуется для выполнения мутации данных в Remix.

### Пример продвинутой мутации

В этом примере мы реализуем следующее:

- опциональное использование JS;
- валидация формы;
- обработка ошибок;
- индикаторы загрузки (прогрессивное улучшение);
- отображение ошибок (прогрессивное улучшение).

_Обратите внимание_: для мутации данных в примере будет использоваться компонент `Form`. Использование этого компонента вместо нативного элемента `form` частично отключает дефолтное поведение браузера по обработке отправки формы. Если вы не планируете реализовывать кастомные индикаторы загрузки и оптимистичное обновление UI, передайте `Form` проп `reloadDocument`. Это сделает `Form` и `form` полностью идентичными.

__Форма__

Допустим, что в `app/routes/projects/new.tsx` у нас имеется такая форма:

```javascript
import { Form } from "@remix-run/react";

export default function NewProject() {
  return (
    <Form method="post" action="/projects/new">
      <p>
        <label>
          Название: <input name="name" type="text" />
        </label>
      </p>
      <p>
        <label>
          Описание:
          <br />
          <textarea name="description" />
        </label>
      </p>
      <p>
        <button type="submit">Создать</button>
      </p>
    </Form>
  );
}
```

Добавляем `action()` для этой формы (POST-запросы обрабатываются `action()`, а GET-запросы - `loader()`):

```javascript
import type { ActionArgs } from "@remix-run/node";
import { redirect } from "@remix-run/node";

export const action = async ({ request }: ActionArgs) => {
  const formData = await request.formData();
  // создаем проект
  const project = await createProject(formData);
  // выполняем перенаправление
  return redirect(`/projects/${project.id}`);
};

export default function NewProject() {
  // ...
}
```

__Валидация__

Предположим, что наш API возвращает ошибки валидации следующим образом:

```javascript
const [errors, project] = await createProject(formData);
```

При наличии ошибок мы возвращаемся к форме и показываем их:

```javascript
export const action = async ({ request }: ActionArgs) => {
  const formData = await request.formData();
  const [errors, project] = await createProject(formData);

  if (errors) {
    const values = Object.fromEntries(formData);
    return json({ errors, values });
  }

  return redirect(`/projects/${project.id}`);
};
```

Для доступа к данным, возвращаемым функцией `action` используется хук `useActionData`:

```javascript
import type { ActionArgs } from "@remix-run/node";
import { redirect } from "@remix-run/node";
import { useActionData } from "@remix-run/react";

export const action = async ({ request }: ActionArgs) => {
  // ...
};

export default function NewProject() {
  const actionData = useActionData<typeof action>();

  return (
    <form method="post" action="/projects/new">
      <p>
        <label>
          Название:{" "}
          <input
            name="name"
            type="text"
            defaultValue={actionData?.values.name}
          />
        </label>
      </p>

      {actionData?.errors.name ? (
        <p style={{ color: "red" }}>
          {actionData.errors.name}
        </p>
      ) : null}

      <p>
        <label>
          Описание:
          <br />
          <textarea
            name="description"
            defaultValue={actionData?.values.description}
          />
        </label>
      </p>

      {actionData?.errors.description ? (
        <p style={{ color: "red" }}>
          {actionData.errors.description}
        </p>
      ) : null}

      <p>
        <button type="submit">Создать</button>
      </p>
    </form>
  );
}
```

_Обратите внимание_ на атрибут `defaultValue`. При отсутствии этого атрибута форма будет очищаться при каждой отправке.

__Состояние ожидания__

Для доступа к состоянию ожидания или перехода (transition) используется хук `useTransition`:

```javascript
import { redirect } from "@remix-run/node";
import {
  useActionData,
  Form,
  useTransition,
} from "@remix-run/react";

// ...

export default function NewProject() {
  const transition = useTransition();
  const actionData = useActionData<typeof action>();

  return (
    <Form method="post">
      <fieldset
        disabled={transition.state === "submitting"}
      >
        <p>
          <label>
            Название:{" "}
            <input
              name="name"
              type="text"
              defaultValue={
                actionData
                  ? actionData.values.name
                  : undefined
              }
            />
          </label>
        </p>

        {actionData && actionData.errors.name ? (
          <p style={{ color: "red" }}>
            {actionData.errors.name}
          </p>
        ) : null}

        <p>
          <label>
            Описание:
            <br />
            <textarea
              name="description"
              defaultValue={
                actionData
                  ? actionData.values.description
                  : undefined
              }
            />
          </label>
        </p>

        {actionData && actionData.errors.description ? (
          <p style={{ color: "red" }}>
            {actionData.errors.description}
          </p>
        ) : null}

        <p>
          <button type="submit">
            {transition.state === "submitting"
              ? "Создание..."
              : "Создать"}
          </button>
        </p>
      </fieldset>
    </Form>
  );
}
```

Теперь при нажатии "Создать" пользователем происходит блокировка полей формы и текст кнопки меняется на "Создание...".

Кроме данных о состоянии отправки формы, содержащихся в `transition.submission`, мы можем получить доступ к данным формы через `transition.formData`.

__Сообщения об ошибках__

Реализуем простой компонент для анимирования высоты и прозрачности сообщений об ошибках:

```javascript
type Props = {
  error?: string;
  isSubmitting: boolean;
}

function ValidationMessage({ error, isSubmitting }: Props) {
  const [show, setShow] = useState(!!error);

  useEffect(() => {
    const id = setTimeout(() => {
      const hasError = !!error;
      setShow(hasError && !isSubmitting);
    });
    return () => clearTimeout(id);
  }, [error, isSubmitting]);

  return (
    <div
      style={{
        opacity: show ? 1 : 0,
        height: show ? "1em" : 0,
        color: "red",
        transition: "all 300ms ease-in-out",
      }}
    >
      {error}
    </div>
  );
}
```

Оборачиваем сообщения об ошибках в этот компонент и меняем цвет границ инпутов на красный при наличии ошибки:

```javascript
export default function NewProject() {
  const transition = useTransition();
  const actionData = useActionData<typeof action>();

  return (
    <Form method="post">
      <fieldset
        disabled={transition.state === "submitting"}
      >
        <p>
          <label>
            Название:{" "}
            <input
              name="name"
              type="text"
              defaultValue={
                actionData
                  ? actionData.values.name
                  : undefined
              }
              style={{
                borderColor: actionData?.errors.name
                  ? "red"
                  : "",
              }}
            />
          </label>
        </p>

        {actionData?.errors.name ? (
          <ValidationMessage
            isSubmitting={transition.state === "submitting"}
            error={actionData?.errors?.name}
          />
        ) : null}

        <p>
          <label>
            Описание:
            <br />
            <textarea
              name="description"
              defaultValue={actionData?.values.description}
              style={{
                borderColor: actionData?.errors.description
                  ? "red"
                  : "",
              }}
            />
          </label>
        </p>

        <ValidationMessage
          isSubmitting={transition.state === "submitting"}
          error={actionData?.errors.description}
        />

        <p>
          <button type="submit">
            {transition.state === "submitting"
              ? "Создание..."
              : "Создать"}
          </button>
        </p>
      </fieldset>
    </Form>
  );
}
```

## Оптимистичное обновление UI / Optimistic UI

Оптимистичное обновление UI (оптимистичный UI) - это паттерн, позволяющий обновлять UI моментально с помощью "фейковых" (в том смысле, что они отличаются от серверных) данных без отображения индикаторов загрузки на время, необходимое серверу для обновления реальных данных. Как правило, на клиенте у нас для этого имеется достаточно данных. Если в процессе обновления данных на сервере возникла ошибка, мы восстанавливаем предыдущее состояние UI и сообщаем о проблеме пользователю. Однако в большинстве случаев обновление данных на сервере проходит успешно.

В Remix оптимистичное обновление UI реализуется с помощью хуков `useTransition` и `useFetcher`.

### Стратегия

1. Пользователь отправляет форму (или мы делаем это сами с помощью `useSubmit()` или `fetcher.submit()`).
2. Remix выполняет отправку формы и предоставляет в наше распоряжение данные формы в `transition.submission` или `fetcher.submission`.
3. Приложение использует `submission.formData` для рендеринга оптимистичной версии страницы, т.е. той страницы, которая должна рендериться в случае успешной отправки формы.
4. Remix автоматически ревалидирует все данные:
   - при успешной отправке формы пользователь ничего не замечает;
   - при неудачной отправке восстанавливается исходное состояние страницы, а пользователь получает сообщение об ошибке.

### Пример

Рассмотрим процесс создания нового проекта.

Роут проекта загружает проект и рендерит его:

```javascript
// app/routes/project/$id.tsx
import type { LoaderArgs } from "@remix-run/node";
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import { ProjectView } from "~/components/project";

export async function loader({ params }: LoaderArgs) {
  return json(await findProject(params.id));
}

export default function ProjectRoute() {
  const project = useLoaderData<typeof loader>();

  return <ProjectView project={project} />;
}
```

Критически важным здесь является то, что роут проекта рендерит повторно используемый компонент `ProjectView`, который в дальнейшем будет использоваться для оптимистичного обновления UI. Этот компонент может выглядеть так:

```javascript
// app/components/project.tsx
export type { Project } from "~/types";

type Props = {
  project: Project
}

export function ProjectView({ project }: Props) {
  return (
    <div>
      <h2>{project.title}</h2>
      <p>{project.description}</p>
      <ul>
        {project.tasks.map((task) => (
          <li key={task.id}>{task.name}</li>
        ))}
      </ul>
    </div>
  );
}
```

Реализуем роут создания проекта:

```javascript
// app/routes/projects/new.tsx
import type { ActionArgs } from "@remix-run/node";
import { redirect } from "@remix-run/node";
import { Form } from "@remix-run/react";

import { createProject } from "~/utils";

export const action = async ({ request }: ActionArgs) => {
  const body = await request.formData();
  const newProject = Object.fromEntries(body);

  const project = await createProject(newProject);

  return redirect(`/projects/${project.id}`);
};

export default function NewProject() {
  return (
    <>
      <h2>Новый проект</h2>
      <Form method="post">
        <label>
          Название: <input name="title" type="text" />
        </label>
        <label htmlFor="description">Описание:</label>
        <textarea name="description" id="description" />
        <button type="submit">Создать</button>
      </Form>
    </>
  );
}
```

`useTransition()` позволяет легко реализовать индикатор загрузки на время отправки формы, создания новой записи в БД и ответа сервера в виде перенаправления на страницу проекта:

```javascript
import type { ActionArgs } from "@remix-run/node";
import { redirect } from "@remix-run/node";
// !
import { Form, useTransition } from "@remix-run/react";

import { createProject } from "~/utils";

export const action = async ({ request }: ActionArgs) => {
  const body = await request.formData();
  const newProject = Object.fromEntries(body);
  const project = await createProject(newProject);
  return redirect(`/projects/${project.id}`);
};

export default function NewProject() {
  // !
  const transition = useTransition();

  return (
    <>
      <h2>Новый проект</h2>
      <Form method="post">
        <label>
          Название: <input name="title" type="text" />
        </label>
        <label htmlFor="description">Описание:</label>
        <textarea name="description" id="description" />
        <button
          type="submit"
          // !
          disabled={transition.submission}
        >
          {transition.submission
            ? "Создание..."
            : "Создать"}
        </button>
      </Form>
    </>
  );
}
```

Однако, поскольку мы знаем, что создание проекта на сервере почти наверняка будет успешным, имеем все необходимые данные и знаем, как будет выглядеть страница, мы может заменить индикатор загрузки компонентом `ProjectView`:

```javascript
import type { ActionArgs } from "@remix-run/node";
import { redirect } from "@remix-run/node";
import { Form, useTransition } from "@remix-run/react";

// !
import { ProjectView } from "~/components/project";
import { createProject } from "~/utils";

export const action = async ({ request }: ActionArgs) => {
  const body = await request.formData();
  const newProject = Object.fromEntries(body);
  const project = await createProject(newProject);
  return redirect(`/projects/${project.id}`);
};

export default function NewProject() {
  const transition = useTransition();
  // !
  return transition.submission ? (
    <ProjectView
      project={Object.fromEntries(
        transition.submission.formData
      )}
    />
  ) : (
    <>
      <h2>Новый проект</h2>
      <Form method="post">
        <label>
          Название: <input name="title" type="text" />
        </label>
        <label htmlFor="description">Описание:</label>
        {/* ! */}
        <textarea name="description" id="description" />
        <button type="submit">Создать</button>
      </Form>
    </>
  );
}
```

Теперь после того как пользователь нажал "Создать", UI обновляется мгновенно. После успешного создания проекта, пользователь перенаправляется на его страницу. Поскольку в обоих случаях для рендеринга UI используется компонент `ProjectView`, все, что может заметить пользователь, это изменение URL.

Самой сложной частью оптимистичного обновления UI является обработка потенциальных ошибок и уведомление пользователя о том, что операция провалилась. Здесь существует 2 варианта: позволить Remix обработать ошибку автоматически посредством рендеринга ближайшего `ErrorBoundary` или вернуть ошибку из `loader()`. Рассмотрим второй вариант:

```javascript
import type { ActionArgs } from "@remix-run/node";
import { json, redirect } from "@remix-run/node";
import {
  Form,
  useActionData,
  useTransition,
} from "@remix-run/react";

import { ProjectView } from "~/components/project";
import { createProject } from "~/utils";

export const action = async ({ request }: ActionArgs) => {
  const body = await request.formData();
  const newProject = Object.fromEntries(body);

  try {
    const project = await createProject(newProject);

    return redirect(`/projects/${project.id}`);
  } catch (e: unknown) {
    console.error(e);

    return json("Во время создания проекта произошла ошибка", {
      status: 500,
    });
  }
};

export default function NewProject() {
  const error = useActionData<typeof action>();
  const transition = useTransition();

  return transition.submission ? (
    <ProjectView
      project={Object.fromEntries(
        transition.submission.formData
      )}
    />
  ) : (
    <>
      <h2>Новый проект</h2>
      <Form method="post">
        <label>
          Название: <input name="title" type="text" />
        </label>
        <label htmlFor="description">Описание:</label>
        <textarea name="description" id="description" />
        <button type="submit">Создать</button>
      </Form>
      {error ? <p>{error}</p> : null}
    </>
  );
}
```

Теперь при возникновении ошибки пользователь возвращается к форме и видит соответствующее сообщение.

### Валидация на стороне клиента

Во избежание лишних ошибок, связанных с отсутствием или неверным форматом данных, необходимых для создания проекта, может быть полезным валидировать значения полей формы на клиенте. К счастью, это легко реализовать с помощью встроенных механизмов HTML-элементов:

```javascript
import type { ActionArgs } from "@remix-run/node";
import { json, redirect } from "@remix-run/node";
import {
  Form,
  useActionData,
  useTransition,
} from "@remix-run/react";

import { ProjectView } from "~/components/project";
import { createProject } from "~/utils";

export const action = async ({ request }: ActionArgs) => {
  const body = await request.formData();
  const newProject = Object.fromEntries(body);
  try {
    const project = await createProject(newProject);
    return redirect(`/projects/${project.id}`);
  } catch (e: unknown) {
    console.error(e);
    return json("Во время создания проекта произошла ошибка", {
      status: 500,
    });
  }
};

export default function NewProject() {
  const error = useActionData<typeof action>();
  const transition = useTransition();

  return transition.submission ? (
    <ProjectView
      project={Object.fromEntries(
        transition.submission.formData
      )}
    />
  ) : (
    <>
      <h2>Новый проект</h2>
      <Form method="post">
        <label>
          Название:{" "}
          <input
            // минимальная длина названия проекта - 3 символа
            minLength={3}
            name="title"
            // название проекта является обязательным
            required
            type="text"
          />
        </label>
        <label htmlFor="description">Описание:</label>
        <textarea name="description" id="description" />
        <button type="submit">Создать</button>
      </Form>
      {error ? <p>{error}</p> : null}
    </>
  );
}
```

К слову, шаблон поля для ввода email может выглядеть так:

```javascript
<input
  type="email"
  name="email"
  // !
  pattern="[^@\s]+@[^@\s]+\.[^@\s]+"
  required
/>
```

## Ограничения модулей / Module Constraints

Поскольку приложение Remix выполняется как на сервере, так и в браузере, следует проявлять осторожность в отношении побочных эффектов модулей (module side effects).

- серверный код - Remix не сможет удалить серверный код из сборки для браузера при наличии побочных эффектов, использующих серверный код;
- клиентский код - Remix рендерит страницы на сервере, поэтому модули на верхнем уровне не должны содержать код, обращающийся в браузерным API.

### Удаление серверного кода из сборки для браузера

Для удаления серверного кода из сборки для клиента Remix делает следующее:

- создает "проксирующий" модуль для роута;
- этот модуль импортирует только браузерные экспорты.

Рассмотрим модуль, экспортирующий функции `loader`, `meta` и компонент:

```javascript
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import PostsView from "../PostsView";
import { prisma } from "../db";

export async function loader() {
  return json(await prisma.post.findMany());
}

export function meta() {
  return { title: "Список постов" };
}

export default function Posts() {
  const posts = useLoaderData<typeof loader>();
  return <PostsView posts={posts} />;
}
```

Серверу требуются весь код модуля, а браузеру - только компонент и `meta()`. Если `prisma` попадет в клиентскую сборку, то модуль сломается, поскольку `prisma` использует большое количество API Node.js.

Прокси-модуль для этого роута выглядит так:

```javascript
export { meta, default } from "./routes/posts.tsx";
```

А код для клиентской сборки так:

```javascript
import { useLoaderData } from "@remix-run/react";

import PostsView from "../PostsView";

export function meta() {
  return { title: "Список постов" };
}

export default function Posts() {
  const posts = useLoaderData<typeof loader>();

  return <PostsView posts={posts} />;
}
```

__Побочные эффекты модулей__

Простыми словами, побочный эффект - это код, который что-то делает, а побочный эффект модуля - это код, который что-то делает при загрузке модуля.

Например, добавление такой строки кода в предыдущий пример сломает модуль:

```javascript
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import PostsView from "../PostsView";
import { prisma } from "../db";
// !
console.log(prisma);

export async function loader() {
  return json(await prisma.post.findMany());
}

export function meta() {
  return { title: "Список постов" };
}

export default function Posts() {
  const posts = useLoaderData<typeof loader>();
  return <PostsView posts={posts} />;
}
```

Импортируемый серверный модуль `prisma` выводится в консоль, поэтому код для клиентской сборки будет выглядеть следующим образом:

```javascript
import { useLoaderData } from "@remix-run/react";

import PostsView from "../PostsView";
// !
import { prisma } from "../db"; // 😬
// !
console.log(prisma); // 🥶

export function meta() {
  return { title: "Список постов" };
}

export default function Posts() {
  const posts = useLoaderData<typeof loader>();
  return <PostsView posts={posts} />;
}
```

`loader()` была удалена, но импорт `prisma` остался.

В данном случае проблему легко устранить путем перемещения логгирования в `loader()`:

```javascript
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import PostsView from "../PostsView";
import { prisma } from "../db";

export async function loader() {
  // !
  console.log(prisma);
  return json(await prisma.post.findMany());
}

export function meta() {
  return { title: "Список постов" };
}

export default function Posts() {
  const posts = useLoaderData<typeof loader>();
  return <PostsView posts={posts} />;
}
```

Теперь импорт `prisma` будет удален вместе с `loader()`.

Если вы столкнулись с ситуацией, когда серверный код попадает в сборку для браузера при отсутствии побочных эффектов модулей, перенесите соответствующий код в файл, название которого содержит суффикс `server`, например, `db.server.ts`. Это сообщит Remix, что такой код используется только на сервере.

### Функции более высокого порядка

При работе с Remix велик соблазн абстрагировать `loader()` с помощью функций более высокого порядка (higher order functions), например, так:

```javascript
import { redirect } from "@remix-run/node";

export function removeTrailingSlash(loader) {
  return function (arg) {
    const { request } = arg;
    const url = new URL(request.url);
    if (
      url.pathname !== "/" &&
      url.pathname.endsWith("/")
    ) {
      return redirect(request.url.slice(0, -1), {
        status: 308,
      });
    }
    return loader(arg);
  };
}
```

И использовать их следующим образом:

```javascript
import { removeTrailingSlash } from "~/http";

export const loader = removeTrailingSlash(({ request }) => {
  return { some: "data" };
});
```

Это делает `loader()` побочным эффектом модуля, поэтому он не будет удален из клиентской сборки.

Для того, чтобы реализовать ранний возврат ответа, достаточно выбросить ответ в `loader()`:

```javascript
import { redirect } from "@remix-run/node";

export function removeTrailingSlash(url) {
  if (url.pathname !== "/" && url.pathname.endsWith("/")) {
    throw redirect(request.url.slice(0, -1), {
      status: 308,
    });
  }
}
```

Пример использования:

```javascript
import { json } from "@remix-run/node";

import { removeTrailingSlash } from "~/http";

export const loader = async ({ request }: LoaderArgs) => {
  removeTrailingSlash(request.url);
  return json({ some: "data" });
};
```

Это позволит Remix исключить `loader` из сборки для браузера. Кроме того, такой код легче читать. Сравните следующие блоки кода:

```javascript
// 1
export const loader = async ({ request }: LoaderArgs) => {
  return removeTrailingSlash(request.url, () => {
    return withSession(request, (session) => {
      return requireUser(session, (user) => {
        return json(user);
      });
    });
  });
};

// 2
export const loader = async ({ request }: LoaderArgs) => {
  removeTrailingSlash(request.url);
  const session = await getSession(request);
  const user = await requireUser(session);
  return json(user);
};
```

Какой вам нравится больше? Полагаю, ответ очевиден. В данном случае можно провести аналогию между использованием `async/await` вместо промисов и коллбэков.

### Браузерный код на сервере

Remix не удаляет браузерный код из сборки для сервера, поскольку модули нуждаются в каждом экспорте для успешного серверного рендеринга. Это означает, что ответственность за изоляцию кода, который должен выполняться только в браузере, ложится на плечи разработчика.

Следующий пример сломает приложение:

```javascript
import { loadStripe } from "@stripe/stripe-js";

// переменная `window` не определена, поскольку код выполняется на сервере
const stripe = await loadStripe(window.ENV.stripe);

export async function redirectToStripeCheckout(sessionId) {
  return stripe.redirectToCheckout({ sessionId });
}
```

__Инициализация браузерных API__

Существует несколько способов инициализации браузерных интерфейсов при импорте модуля.

_Защитник документа (document guard)_

```javascript
import firebase from "firebase/app";

// !
if (typeof document !== "undefined") {
  firebase.initializeApp(document.ENV.firebase);
}

export { firebase };
```

Если переменная `document` определена, значит средой выполнения кода является браузер. Проверка "определенности" `document` является более надежным способом идентификации браузера, чем `window`, потому что в Deno, например, имеется глобальная переменная `window`.

_Ленивая инициализация_

Суть данного подхода состоит в том, что браузерный API инициализируется при использовании библиотеки (вызове функции):

```javascript
import { loadStripe } from "@stripe/stripe-js";

export async function redirectToStripeCheckout(sessionId) {
  // !
  const stripe = await loadStripe(window.ENV.stripe);
  return stripe.redirectToCheckout({ sessionId });
}
```

Во избежание множественной инициализации достаточно записать интерфейс в глобальную (в пределах модуля) переменную:

```javascript
import { loadStripe } from "@stripe/stripe-js";

let _stripe;
async function getStripe() {
  if (!_stripe) {
    _stripe = await loadStripe(window.ENV.stripe);
  }
  return _stripe;
}

export async function redirectToStripeCheckout(sessionId) {
  const stripe = await getStripe();
  return stripe.redirectToCheckout({ sessionId });
}
```

__Рендеринг с браузерными API__

Другим распространенным случаем является обращение к браузерным интерфейсам в процессе рендеринга.

Следующим пример сломает приложение, поскольку сервер попытается использовать локальное хранилище (local storage):

```javascript
function useLocalStorage(key) {
  const [state, setState] = useState(
    localStorage.getItem(key)
  );

  const setWithLocalStorage = (nextState) => {
    setState(nextState);
  };

  return [state, setWithLocalStorage];
}
```

Для решения проблемы достаточно перенести инициализацию состояния в хук `useEffect`:

```javascript
function useLocalStorage(key) {
  const [state, setState] = useState(null);

  useEffect(() => {
    setState(localStorage.getItem(key));
  }, [key]);

  const setWithLocalStorage = (nextState) => {
    setState(nextState);
  };

  return [state, setWithLocalStorage];
}
```

Напоследок, рассмотрим кастомный хук, позволяющий безопасно использовать хук `useLayoutEffect`:

```javascript
import React from "react";

const canUseDOM = typeof document !== "undefined";

const useLayoutEffect = canUseDOM
  ? React.useLayoutEffect
  : () => {};
```

## Обработка ошибок / Error Handling

Remix автоматически перехватывает (catch) ошибку и рендерит ближайший (к месту ее возникновения) `ErrorBoundary` (предохранитель) в случаях, когда ошибка возникла в процессе:

- рендеринга в браузере;
- рендеринга на сервере;
- в `loader()` при первоначальном запросе на серверный рендеринг документа;
- в `action()` при первоначальном запросе на серверный рендеринг документа;
- в `loader()` при переходе на стороне клиента в браузере (Remix сериализует ошибку и отправляет ее по сети в браузер);
- в `action()` при переходе на стороне клиента в браузере.

### Корневой предохранитель

При использовании стартового шаблона в файле `root.{tsx|jsx}` имеется такой предохранитель:

```javascript
export function ErrorBoundary({ error }) {
  console.error(error);

  return (
    <html>
      <head>
        <title>О, нет!</title>
        <Meta />
        <Links />
      </head>
      <body>
        {/* UI, который будет рендериться при возникновении ошибки */}
        <Scripts />
      </body>
    </html>
  );
}
```

При рендеринге корневого предохранителя перемонтируется весь документ - это объясняет необходимость рендеринга компонентов `Meta`, `Links` и `Scripts`.

### Вложенные предохранители

Каждый роут может содержать собственный предохранитель. Преимущество такого подхода состоит в том, что при возникновении ошибки в роуте с предохранителем только определенная часть UI окажется сломанной, остальная страница будет выглядеть как задумывалось.

Рассмотрим такую иерархию роутов:

```routes
├── sales
│   ├── invoices
│   │   └── $invoiceId.js
│   └── invoices.js
└── sales.js
```

Если `$invoiceId.js` экспортирует `ErrorBoundary` и ошибка возникает в его компоненте, `loader()` или `action()`, сломается только раздел счета (invoice), остальная часть страницы будет успешно отрендерена.

Если роут не содержит собственного предохранителя, ошибка "всплывает" до ближайшего родительского предохранителя, поэтому нет необходимости экспортировать `ErrorBoundary` из каждого модуля.

## Обработка ошибки 404 / Not Found Handling

Случаи отправки статус-кода 404:

- URL не совпадает ни с одним роутом;
- `loader()` не обнаружил необходимых данных.

Первый случай обрабатывается Remix автоматически, обработка второго случая - задача разработчика.

При отсутствии данных, запрашиваемых пользователем, необходимо выбросить ответ:

```javascript
export async function loader({ params }: LoaderArgs) {
  const page = await db.page.findOne({
    where: { slug: params.slug },
  });

  if (!page) {
    throw new Response("Не найдено", {
      status: 404,
    });
  }

  return json(page);
}
```

Remix перехватывает такой ответ и передает управление ближайшему перехватчику (catch boundary). Перехватчик похож на предохранитель (error boundary), только вместо компонента `ErrorBoundary` из модуля должен экспортироваться компонент `CatchBoundary`.

Когда выбрасывается ответ, код `loader()` перестает выполняться. Это означает, что нам не нужно заботиться об обработке состояния ожидания, ошибок и отсутствия данных в компоненте.

__Корневой перехватчик__

Корневой перехватчик может выглядеть так:

```javascript
export function CatchBoundary() {
  const caught = useCatch();

  return (
    <html>
      <head>
        <title>Упс!</title>
        <Meta />
        <Links />
      </head>
      <body>
        <h1>
          {caught.status} {caught.statusText}
        </h1>
        <Scripts />
      </body>
    </html>
  );
}
```

__Вложенные перехватчики__

Каждый роут может экспортировать собственного перехватчика:

```javascript
import type { LoaderArgs } from "@remix-run/node";
import {
  Form,
  useLoaderData,
  useParams,
} from "@remix-run/react";

export async function loader({ params }: LoaderArgs) {
  const page = await db.page.findOne({
    where: { slug: params.slug },
  });

  if (!page) {
    throw new Response("Не найдено", {
      status: 404,
    });
  }

  return json(page);
}

export function CatchBoundary() {
  const params = useParams();

  return (
    <div>
      <h2>Запрашиваемая страница отсутствует</h2>
      <Form action="../create">
        <button
          type="submit"
          name="slug"
          value={params.slug}
        >
          Создать {params.slug}?
        </button>
      </Form>
    </div>
  );
}

export default function Page() {
  return <PageView page={useLoaderData<typeof loader>()} />;
}
```

Понятно, что так могут обрабатываться любые ответы, а не только 404.

## Переменные среды окружения / Environment Variables

Remix имеет встроенную поддержку [dotenv](https://www.npmjs.com/package/dotenv) в режиме разработки, поэтому при выполнении команды `remix dev` переменные среды окружения доступны через `process.env`.

Создаем файл `.env` в корне проекта:

```bash
touch .env
```

Редактируем этот файл:

```bash
SOME_SECRET=super-secret
```

Получаем доступ к этой переменной в `loader()` или `action()`:

```javascript
export async function loader() {
  console.log(process.env.SOME_SECRET);
}
```

При выполнении команды `remix serve` переменные среды окружения в `process.env` не загружаются, они должны устанавливаться производственным сервером. Способы их установки зависят от используемого хостинга.

При необходимости доступа к переменным на клиенте можно сделать следующее:

- вернуть `ENV` из корневого `loader()`:

```javascript
export async function loader() {
  return json({
    ENV: {
      STRIPE_PUBLIC_KEY: process.env.STRIPE_PUBLIC_KEY,
      FAUNA_DB_URL: process.env.FAUNA_DB_URL,
    },
  });
}

export function Root() {
  return (
    <html lang="en">
      <head>
        <Meta />
        <Links />
      </head>
      <body>
        <Outlet />
        <Scripts />
      </body>
    </html>
  );
}
```

- записать `ENV` в глобальный объект `window`:

```javascript
export async function loader() {
  return json({
    ENV: {
      STRIPE_PUBLIC_KEY: process.env.STRIPE_PUBLIC_KEY,
    },
  });
}

export function Root() {
  const data = useLoaderData<typeof loader>();

  return (
    <html lang="en">
      <head>
        <Meta />
        <Links />
      </head>
      <body>
        <Outlet />
        <script
          dangerouslySetInnerHTML={{
            __html: `window.ENV = ${JSON.stringify(
              data.ENV
            )}`,
          }}
        />
        <Scripts />
      </body>
    </html>
  );
}
```

```javascript
import { loadStripe } from "@stripe/stripe-js";

export async function redirectToStripeCheckout(
  sessionId
) {
  const stripe = await loadStripe(
    window.ENV.STRIPE_PUBLIC_KEY
  );
  return stripe.redirectToCheckout({ sessionId });
}
```

## Стилизация / Styling

Основным способом стилизации веб-приложений является добавление `<link rel="stylesheet">` на страницу. В Remix это делается посредством экспорта из роута функции `links`. Когда роут является активным, таблица стилей добавляется на страницу. Когда роут больше не является активным, таблица стилей удаляется со страницы.

```javascript
export function links() {
  return [
    {
      rel: "stylesheet",
      href: "https://unpkg.com/modern-css-reset@1.4.0/dist/reset.min.css",
    },
  ];
}
```

`links()` вложенных роутов объединяются и рендерятся по порядку (начиная с корневого роута) в виде тегов `link` с помощью компонента `Link` в разделе `head` в файле `app/root.jsx`:

```javascript
import { Links } from "@remix-run/react";

export default function Root() {
  return (
    <html>
      <head>
        <Links />
        {/* ... */}
      </head>
      {/* ... */}
    </html>
  );
}
```

Файлы CSS могут импортироваться в модули напрямую. В этом случае Remix:

- копирует файл в директорию для клиентской сборки;
- создает отпечаток (fingerprint) файла для долгосрочного кэширования;
- возвращает URL для использования в модуле в процессе рендеринга.

```javascript
import styles from "~/styles/global.css";

export function links() {
  return [{ rel: "stylesheet", href: styles }];
}
```

Преимущества использования `<link>` для загрузки стилей заключаются в следующем:

- URL может кэшироваться браузером и CDN;
- один и тот же URL может использоваться разными страницами приложения;
- таблица стилей может загружаться одновременно с JS;
- ресурсы CSS могут запрашиваться предварительно с помощью `<link rel="prefetch" />`;
- изменения в компонентах не ломают кэш для стилей;
- изменения в стилях не ломают кэш для JS.

### Обычные таблицы стилей

__Стили роутов__

Каждый роут может добавлять собственные стили на страницу:

```javascript
// app/routes/dashboard.tsx
import styles from "~/styles/dashboard.css";

export function links() {
  return [{ rel: "stylesheet", href: styles }];
}
```

```javascript
// app/routes/accounts.tsx
import styles from "~/styles/accounts.css";

export function links() {
  return [{ rel: "stylesheet", href: styles }];
}
```

```javascript
// app/routes/sales.tsx
import styles from "~/styles/sales.css";

export function links() {
  return [{ rel: "stylesheet", href: styles }];
}
```

Соотношение URL и загружаемых стилей может выгялдеть так:

- `/dashboard` - `dashboard.css`;
- `/dashboard/accounts` - `dashboard.css` и `accounts.css`;
- `/dashboard/sales` - `dashboard.css` и `sales.css`.

Такой подход к загрузке стилей решает многие проблемы, связанные со стилизацией приложения: загрузка только используемых на текущей странице стилей, совпадение селекторов и названий классов, загрузка старых стилей, которые больше не используются и т.д.

__Распределенные стили__

В любом приложении имеются общие (распределенные - shared) компоненты: формы, кнопки, макеты и др. В Remix для стилизации таких компонентов рекомендуется использовать один из 2 подходов.

_Глобальная таблица стилей_

Создаем файл `shared.css` (или `global.css`):

```css
/* app/styles/shared.css */
/* используем названия классов */
.PrimaryButton {
  /* ... */
}

.TileGrid {
  /* ... */
}

/* или data-атрибуты */
[data-primary-button] {
  /* ... */
}

[data-tile-grid] {
  /* ... */
}
```

Импортируем этот файл в `app/root.tsx`:

```javascript
// app/root.tsx
import styles from "~/styles/shared.css";

export function links() {
  return [{ rel: "stylesheet", href: styles }];
}
```

_Совместное использование стилей_

Создаем CSS-файл для каждого компонента и загружаем стили в роуте, который его использует.

Предположим, что у нас имеется компонент `Button` в `app/components/button/index.js` со стилями в `app/components/button/styles.css`, а также компонент `PrimaryButton`, расширяющий `Button`.

```css
/* app/components/button/styles.css */
.btn {
  border: solid 1px;
  background: white;
  color: #454545;
}
```

```javascript
// app/components/button/index.jsx
import styles from "./styles.css";

export const links = () => [
  { rel: "stylesheet", href: styles },
];

export const Button = React.forwardRef(
  ({ children, ...props }, ref) => {
    return <button {...props} ref={ref} className="btn" />;
  }
);
Button.displayName = "Button";
```

_Обратите внимание_, что `Button` экспортирует `links()`, хотя не является роутом.

```css
/* app/components/button-primary/styles.css */
.btn-primary {
  background: blue;
  color: white;
}
```

```javascript
// app/components/button-primary/index.jsx
import { Button, links as buttonLinks } from "../button";
import styles from "./styles.css";

export const links = () => [
  ...buttonLinks(),
  { rel: "stylesheet", href: styles },
];

export const PrimaryButton = React.forwardRef(
  ({ children, ...props }, ref) => {
    return (
      <Button {...props} ref={ref} className="btn btn-primary" />
    );
  }
);
PrimaryButton.displayName = "PrimaryButton";
```

_Обратите внимание_, что `PrimaryButton` включает стили для `Button`.

Поскольку кнопки не являются роутами, т.е. не связаны с сегментами URL, Remix не знает, когда предварительно запрашивать, загружать и выгружать их стили. Поэтому импорт и добавление на страницу стилей для кнопок должен дублироваться в роуте, который использует кнопки:

```javascript
import styles from "~/styles/index.css";

import {
  PrimaryButton,
  links as primaryButtonLinks,
} from "~/components/button-primary";

export function links() {
  return [
    ...primaryButtonLinks(),
    { rel: "stylesheet", href: styles },
  ];
}
```

_Предварительная загрузка ресурсов_

С помощью тега `link` могут загружаться не только стили, но и другие ресурсы, используемые на странице, например, изображения:

```css
/* app/components/copy-to-clipboard/style.css */
.copy-to-clipboard {
  background: url("/icons/clipboard.svg");
}
```

```javascript
// app/components/copy-to-clipboard/index.jsx
import styles from "./styles.css";

export const links = () => [
  {
    rel: "preload",
    href: "/icons/clipboard.svg",
    as: "image",
    type: "image/svg+xml",
  },
  { rel: "stylesheet", href: styles },
];

export const CopyToClipboard = React.forwardRef(
  ({ children, ...props }, ref) => {
    return (
      <Button {...props} ref={ref} className="copy-to-clipboard" />
    );
  }
);
CopyToClipboard.displayName = "CopyToClipboard";
```

_Медиа-запросы_

Атрибут `media` позволяет загружать определенные стили на основе ширины экрана пользователя и т.п.:

```javascript
export function links() {
  return [
    {
      rel: "stylesheet",
      href: mainStyles,
    },
    {
      rel: "stylesheet",
      href: largeStyles,
      media: "(min-width: 1024px)",
    },
    {
      rel: "stylesheet",
      href: xlStyles,
      media: "(min-width: 1280px)",
    },
    {
      rel: "stylesheet",
      href: darkStyles,
      media: "(prefers-color-scheme: dark)",
    },
  ];
}
```

### TailwindCSS

Устанавливаем зависимости:

```bash
npm i -D npm-run-all tailwindcss
```

Инициализируем [Tailwind](https://tailwindcss.com/):

```bash
npx tailwindcss init
```

Редактируем `tailwind.config.js`:

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./app/**/*.{js,jsx,ts,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

Обновляем раздел `scripts` в файле `package.json`:

```json
{
  "scripts": {
    "build": "run-s \"build:*\"",
    "build:css": "npm run generate:css -- --minify",
    "build:remix": "remix build",
    "dev": "run-p \"dev:*\"",
    "dev:css": "npm run generate:css -- --watch",
    "dev:remix": "remix dev",
    "generate:css": "npx tailwindcss -o ./app/tailwind.css",
    "start": "remix-serve build"
  }
}
```

Импортируем генерируемый файл CSS в приложение:

```javascript
// app/root.tsx
import type { LinksFunction } from "@remix-run/node"; // or cloudflare/deno

import styles from "./tailwind.css";

export const links: LinksFunction = () => [
  { rel: "stylesheet", href: styles },
];
```

Для кастомизации стилей Tailwind с помощью директивы `@apply` необходимо создать CSS-файл в корневой директории, например, `styles/tailwind.css`:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer components {
  .custom-class {
    @apply ...;
  }
}
```

И отредактировать команду `generate:css` в `package.json`:

```json
"generate:css": "npx tailwindcss -i ./styles/tailwind.css -o ./app/tailwind.css"
```

Рекомендуется добавить генерируемый файл в `.gitignore`:

```
node_modules

/.cache
/build
/public/build
.env

/app/tailwind.css
```

### PostCSS

Устанавливаем зависимости:

```bash
npm i -D postcss-cli postcss autoprefixer
```

Создаем файл `postcss.config.js` в корневой директории:

```javascript
module.exports = {
  plugins: {
    autoprefixer: {},
  },
};
```

Создаем CSS-файл в корневой директории, например, `styles/app.css`.

Добавляем скрипты в `package.json`:

```json
"dev:css": "postcss styles --base styles --dir app/styles -w",
"build:css": "postcss styles --base styles --dir app/styles --env production"
```

Данные команды преобразуют файлы из директории `styles` и помещают их в директорию `app/styles`.

Импортируем генерируемый файл в `app/root.tsx`:

```javascript
import type { LinksFunction } from "@remix-run/node";

import styles from "./styles/app.css";

export const links: LinksFunction = () => {
  return [{ rel: "stylesheet", href: styles }];
};
```

Для запуска [PostCSS](https://postcss.org/) и Remix одной командой можно использовать npm-пакет [concurrently](https://www.npmjs.com/package/concurrently):

```bash
npm i -D concurrently
```

```json
"scripts": {
  "dev": "concurrently \"npm run dev:css\" \"remix dev\""
}
```

### SASS

Устанавливаем [SASS](https://sass-lang.com/):

```bash
npm i -D sass
```

Добавляем скрипт в `package.json`:

```json
"sass": "sass --watch app/:app/"
```

Предполагается, что файлы SASS находятся в директории `app`. Флаг `--watch` означает наблюдение за добавлением, удалением и модификацией файлов.

Команда для одновременного запуска SASS и Remix:

```json
"dev": "concurrently \"npm run sass\" \"remix dev\""
```

## TypeScript

Remix поддерживает JS и TS из коробки, но компилятор Remix не выполняет проверку типов (он просто их удаляет). Однако для проверки типов достаточно добавить в `package.json` такой скрипт:

```json
"typecheck": "tsc -b"
```

Определения типов TS также встроены в Remix. При использовании начального шаблона создается файл `remix.env.d.ts`:

```javascript
/// <reference types="@remix-run/dev" />
/// <reference types="@remix-run/node" />
```

Ссылка на этот файл содержится в `tsconfig.json`:

```json
"include": ["remix.env.d.ts", "**/*.ts", "**/*.tsx"]
```

## Интерфейс модуля роута / Route Module API

Как правило, роут используется для рендеринга определенной части пользовательского интерфейса (User Interface, UI) приложения, такого как компонент React с серверными хуками жизненного цикла.

### Функция, экспортируемая по умолчанию

Это компонент, который рендерится при совпадении с роутом (его путем или адресом):

```javascript
export default function SomeRouteComponent() {
  return (
    <div>
      <h1>Посмотрите-ка!</h1>
      <p>Я использую React уже 7 лет.</p>
    </div>
  );
}
```

### loader

Каждый роут может определять функцию загрузки - `loader`, которая вызывается на сервере перед рендерингом для предоставления данных роуту. `loader()` можно рассматривать как обработчик запроса GET, поэтому мы не должны читать в ней тело запроса (request body) - это задача функции `action` (см. ниже).

```javascript
import { json } from "@remix-run/node";
import type { LoaderFunction } from "@remix-run/node";

export const loader: LoaderFunction = async () => {
  // функция `json` конвертирует сериализуемый объект в ответ в формате JSON
  return json({ ok: true });
};
```

Данная функция выполняется только на сервере. При начальном рендеринге она предоставляет данные для документа HTML. При навигации в браузере Remix вызывает ее с помощью `fetch()`. Это означает, что в `action()` можно напрямую обращаться к базе данных, использовать секреты серверных интерфейсов и т.д. Код, который не используется для рендеринга UI, удаляется из сборки для браузера.

Пример использования объектно-реляционного отображения (Object-Relational Mapping, ORM) `Prisma`:

```javascript
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import { prisma } from "../db";

export const loader = async () => {
  // получаем данные всех пользователей из БД
  return json(await prisma.user.findMany());
};

export default function Users() {
  const users = useLoaderData();

  return (
    <ul>
      {users.map((user) => (
        <li key={user.id}>{user.name}</li>
      ))}
    </ul>
  );
}
```

Remix предоставляет ("полифилит") `fetch()` для сервера, который можно использовать в `loader()`.

__Аргументы, передаваемые `loader()`__

_params_

Параметры строки запроса роута передаются `loader()`. Например, если у нас есть `loader()` по адресу `data/invoices/$invoiceId.tsx`, Remix извлечет `invoiceId` и передаст его `loader()`. Это может быть полезным для получения определенных данных из API или БД:

```javascript
// предположим, что пользователь посетил /invoices/123
export const loader: LoaderFunction = async ({
  params,
}) => {
  console.log(params.invoiceId); // "123"
};
```

_request_

Экземпляр [Fetch Request](https://developer.mozilla.org/en-US/docs/Web/API/Request) с информацией о запросе.

Данный аргумент может использоваться для чтения заголовков HTTP запроса, URL или [URLSearchParams](https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams), например:

```javascript
export const loader: LoaderFunction = async ({
  request,
}) => {
  // читаем куки
  const cookie = request.headers.get("Cookie");

  // разбираем параметры строки запроса
  const searchParams = new URLSearchParams(request.url);
  const search = searchParams.get("search");
};
```

_context_

Контекст, передаваемый функции `getLoadContext` адаптера сервера. Это способ построить мост между API запроса/ответа адаптера и приложением Remix.

Допустим, наш сервер `Express` выглядит так:

```javascript
const {
  createRequestHandler,
} = require("@remix-run/express");

app.all(
  "*",
  createRequestHandler({
    getLoadContext(req, res) {
      // это становится контекстом `loader()`
      return { expressUser: req.user };
    },
  })
);
```

Получаем доступ к контексту в `loader()`:

```javascript
export const loader: LoaderFunction = async ({
  context,
}) => {
  const { expressUser } = context;
  // ...
};
```

__Ответ, возвращаемый `loader()`__

`loader()` должна возвращать [Fetch Response](https://developer.mozilla.org/en-US/docs/Web/API/Response):

```javascript
export const loader: LoaderFunction = async () => {
  const users = await db.users.findMany();
  const body = JSON.stringify(users);

  return new Response(body, {
    headers: {
      "Content-Type": "application/json",
    },
  });
};
```

Утилита `json` упрощает этот процесс:

```javascript
import { json } from "@remix-run/node";

export const loader: LoaderFunction = async () => {
  const users = await fakeDb.users.findMany();

  return json(users);
};
```

`json()` позволяет добавлять в ответ дополнительную информацию, такую как заголовки HTTP или статус-код:

```javascript
import { json } from "@remix-run/node";

export const loader: LoaderFunction = async ({
  params,
}) => {
  const user = await fakeDb.project.findOne({
    where: { id: params.id },
  });

  if (!user) {
    return json("Пользователь не найден", { status: 404 });
  }

  return json(user);
};
```

__Выброс ответа в `loader()`__

Вместо возврата ответа в `loader()`, его можно выбросить (`throw`). Это позволяет "прорваться" сквозь стек вызовов (call stack) и отобразить альтернативный `UI` с контекстуальными данными с помощью `CatchBoundary` (см. ниже).

Пример создания утилиты, выбрасывающей ответ в `loader()`, что останавливает процесс выполнения кода и приводит к рендерингу резервного `UI`:

```javascript
// app/db.ts
import { json } from "@remix-run/node";
import type { ThrownResponse } from "@remix-run/react";

export type InvoiceNotFoundResponse = ThrownResponse<
  404,
  string
>;

export function getInvoice(id, user) {
  const invoice = db.invoice.find({ where: { id } });

  if (!invoice) {
    throw json("Счет не найден", { status: 404 });
  }

  return invoice;
}
```

```javascript
// app/http.ts
import { redirect } from "@remix-run/node";
import { getSession } from "./session";

export async function requireUserSession(request) {
  const session = await getSession(
    request.headers.get("cookie")
  );

  if (!session) {
    // поскольку утилиты `redirect` и `json` возвращают ответы,
    // их также можно выбрасывать
    throw redirect("/login", 302);
  }

  return session.get("user");
}
```

```javascript
// app/routes/invoice/$invoiceId.tsx
import { useCatch, useLoaderData } from "@remix-run/react";
import type { ThrownResponse } from "@remix-run/react";

import { requireUserSession } from "~/http";
import { getInvoice } from "~/db";
import type {
  Invoice,
  InvoiceNotFoundResponse,
} from "~/db";

type InvoiceCatchData = {
  invoiceOwnerEmail: string;
};

type ThrownResponses =
  | InvoiceNotFoundResponse
  | ThrownResponse<401, InvoiceCatchData>;

export const loader = async ({ request, params }) => {
  const user = await requireUserSession(request);
  const invoice: Invoice = getInvoice(params.invoiceId);

  if (!invoice.userIds.includes(user.id)) {
    const data: InvoiceCatchData = {
      invoiceOwnerEmail: invoice.owner.email,
    };

    throw json(data, { status: 401 });
  }

  return json(invoice);
};

export default function InvoiceRoute() {
  const invoice = useLoaderData<Invoice>();

  return <InvoiceView invoice={invoice} />;
}

export function CatchBoundary() {
  // сигнатура `caught` - `{ status, statusText, data }`
  const caught = useCatch<ThrownResponses>();

  switch (caught.status) {
    case 401:
      return (
        <div>
          <p>У вас нет доступа к этому счету.</p>
          <p>
            Свяжитесь с {caught.data.invoiceOwnerEmail} для получения доступа.
          </p>
        </div>
      );
    case 404:
      return <div>Счет не найден</div>;
  }

  // если сделать так, то ошибка будет перехвачена ближайшим `ErrorBoundary` (см. ниже)
  // throw new Error("Неизвестный статус в catch boundary");
  return (
    <div>
      Что-то пошло не так: {caught.status}{" "}
      {caught.statusText}
    </div>
  );
}
```

### action

Как и `loader()`, `action` - это серверная функция для обработки мутаций данных и других операций. Если к роуту выполняется не GET-запрос (POST, PUT, PATCH, DELETE), то `action()` вызывается перед `loader()`.

`action()` имеет такой же интерфейс, что и `loader()`. Разница в том, когда они вызываются.

Это позволяет размещать совместно (co-locate) все, что связано с данными, в одном модуле роута: чтение данных, компонент, отвечающий за рендеринг данных, и запись данных.

```javascript
import { json, redirect } from "@remix-run/node";
import { Form } from "@remix-run/react";

import { fakeGetTodos, fakeCreateTodo } from "~/utils/db";
import { TodoList } from "~/components/TodoList";

export async function loader() {
  return json(await fakeGetTodos());
}

export async function action({ request }) {
  const body = await request.formData();

  const todo = await fakeCreateTodo({
    title: body.get("title"),
  });

  return redirect(`/todos/${todo.id}`);
}

export default function Todos() {
  const data = useLoaderData();

  return (
    <div>
      <TodoList todos={data} />
      <Form method="post">
        <input type="text" name="title" />
        <button type="submit">Создать задачу</button>
      </Form>
    </div>
  );
}
```

_Обратите внимание_: форма без пропа `action` (`<Form method="post">`) будет отправлять данные роуту, в котором она находится.

### headers

Каждый роут может определять собственные заголовки HTTP. Одним из популярных заголовков является Cache-Control, указывающий браузеру и сети доставки контента (Content Delivery Network, CDN) где и на протяжении какого времени кэшировать страницу.

```javascript
export function headers({
  actionHeaders,
  loaderHeaders,
  parentHeaders,
}) {
  return {
    "X-Stretchy-Pants": "забавы ради",
    "Cache-Control": "max-age=300, s-maxage=3600",
  };
}
```

Заголовки `loader()` и `action()` передаются `headers()`:

```javascript
export function headers({ loaderHeaders }) {
  return {
    "Cache-Control": loaderHeaders.get("Cache-Control"),
  };
}
```

`actionHeaders` и `loaderHeaders` являются экземплярами класса [Headers](https://developer.mozilla.org/en-US/docs/Web/API/Headers).

В случае с вложенными роутами, "побеждает" `headers()` последнего (самого глубоко вложенного) роута. Заголовки родительского роута доступны в аргументе `parentHeaders`, передаваемом `headers()` дочернего роута.

Глобальные заголовки HTTP можно определить в файле `entry.server.ts`:

```javascript
import { renderToString } from "react-dom/server";
import { RemixServer } from "@remix-run/react";
import type { EntryContext } from "@remix-run/node";

export default function handleRequest(
  request: Request,
  responseStatusCode: number,
  responseHeaders: Headers,
  remixContext: EntryContext
) {
  const markup = renderToString(
    <RemixServer context={remixContext} url={request.url} />
  );

  responseHeaders.set("Content-Type", "text/html");
  // !
  responseHeaders.set("X-Powered-By", "Hugs");

  return new Response("<!DOCTYPE html>" + markup, {
    status: responseStatusCode,
    headers: responseHeaders,
  });
}
```

### meta

Функция `meta` позволяет определять мета-тэги HTML-документа. Рекомендуется устанавливать заголовок и описание в каждом роуте, за исключением роутов макета (layout route) (для таких роутов мета-тэги устанавливаются их основными или индексными роутами (index routes)).

```javascript
import type { MetaFunction } from "@remix-run/node";

export const meta: MetaFunction = () => {
  return {
    title: "Нечто клевое",
    description: "Превью в результатах поиска.",
  };
};
```

Мета-тэги вложенных роутов объединяются.

__Контекст страницы в `meta()`__

`meta()` принимает объект со следующими свойствами:

- `data` - данные, экспортируемые `loader()`;
- `location` - объект подобный `window.location` с информацией о текущем роуте;
- `params` - объект, содержащий параметры строки запроса роута;
- `parentsData` - хэш-таблица данных, экспортируемых `loader()` текущего и всех родительских роутов.

### links

Функция `links` определяет элементы `link`, которые добавляются на страницу при посещении страницы пользователем:

```javascript
import type { LinksFunction } from "@remix-run/node";

export const links: LinksFunction = () => {
  return [
    {
      rel: "icon",
      href: "/favicon.png",
      type: "image/png",
    },
    {
      rel: "stylesheet",
      href: "https://example.com/some/styles.css",
    },
    { page: "/users/123" },
    {
      rel: "preload",
      href: "/images/banner.jpg",
      as: "image",
    },
  ];
};
```

Использование `links()` является стандартным способом стилизации контента в Remix.

### CatchBoundary

`CatchBoundary` - это компонент React, который рендерится, когда `loader()` или `action()` выбрасывают ответ.

`CatchBoundary` работает как компонент роута. Он имеет доступ к статус-коду и выброшенному ответу через хук `useCatch`:

```javascript
import { useCatch } from "@remix-run/react";

export function CatchBoundary() {
  const caught = useCatch();

  return (
    <div>
      <h1>Перехват</h1>
      <p>Статус: {caught.status}</p>
      <pre>
        <code>{JSON.stringify(caught.data, null, 2)}</code>
      </pre>
    </div>
  );
}
```

### ErrorBoundary

`ErrorBoundary` - это компонент React, который рендерится при возникновении любой ошибки в роуте, как при рендеринге, так и при получении данных. Он позволяет перехватывать необработанные исключения (uncaught exceptions).

`ErrorBoundary` работает как обычные [предохранители](https://reactjs.org/docs/error-boundaries.html) React с некоторыми дополнительными возможностями.

Данный компонент получает один проп - возникшую ошибку:

```javascript
export function ErrorBoundary({ error }) {
  return (
    <div>
      <h1>Ошибка</h1>
      <p>{error.message}</p>
      <p>Трассировка стека:</p>
      <pre>{error.stack}</pre>
    </div>
  );
}
```

### handle

Функция `handle` позволяет взаимодействовать с хуком `useMatches` (см. ниже). Она может возвращать любые значения:

```javascript
export const handle = {
  its: "all yours",
};
```

### Импорт статических ресурсов

Любой файл, находящийся в директории `app`, может импортироваться в модуль. В этом случае Remix делает следующее:

- копирует файл в директорию сборки для браузера;
- создает отпечаток (fingerprint) файла для долгосрочного кэширования (long-term caching);
- возвращает публичный URL, используемый модулей при рендеринге.

```javascript
import type { LinksFunction } from "@remix-run/node";

import styles from "./styles/app.css";
import banner from "./images/banner.jpg";

export const links: LinksFunction = () => {
  return [{ rel: "stylesheet", href: styles }];
};

export default function Page() {
  return (
    <div>
      <h1>Некая страница</h1>
      <img src={banner} />
    </div>
  );
}
```

##  Компоненты / Components

### Links, LiveReload, Meta, Scripts, ScrollRestoration

Эти компоненты используются один раз в корневом роуте (`root.tsx`):

```javascript
import type {
  LinksFunction,
  MetaFunction,
} from "@remix-run/node";
import {
  Links,
  LiveReload,
  Meta,
  Outlet,
  Scripts,
  ScrollRestoration,
} from "@remix-run/react";

import globalStylesheetUrl from "./global-styles.css";

export const links: LinksFunction = () => {
  return [{ rel: "stylesheet", href: globalStylesheetUrl }];
};

export const meta: MetaFunction = () => ({
  charset: "utf-8",
  title: "Мое восхитительное приложение",
  viewport: "width=device-width,initial-scale=1",
});

export default function App() {
  return (
    <html lang="en">
      <head>
        {/* Все экспорты `meta()` всех роутов */}
        <Meta />

        {/* Все экспорты `links()` всех роутов */}
        <Links />
      </head>
      <body>
        {/* Дочерние роуты */}
        <Outlet />

        {/* Управляет позицией прокрутки при переходах на клиенте */}
        <ScrollRestoration />

        {/* Теги `script` */}
        <Scripts />

        {/* Выполняет автоматическую перезагрузку страницы при изменении кода в режиме разработки */}
        <LiveReload />
      </body>
    </html>
  );
}
```

### Link

Этот компонент рендерит тег `a`, который является основным средством навигации в приложении. Он оборачивает компонент `Link` из `React Router`, предоставляя дополнительный функционал, связанный с предварительным получением ресурсов (resource prefetching).

```javascript
import { Link } from "@remix-run/react";

export default function GlobalNav() {
  return (
    <nav>
      <Link to="/dashboard">Панель управления</Link>{" "}
      <Link to="/account">Аккаунт</Link>{" "}
      <Link to="/support">Поддержка</Link>
    </nav>
  );
}
```

Предварительное получение ресурсов определяется пропом `prefetch`:

```javascript
<>
  <Link /> {/* по умолчанию "none" */}
  <Link prefetch="none" />
  <Link prefetch="intent" />
  <Link prefetch="render" />
</>
```

- `none` - поведение по умолчанию. Предварительное получение данных не выполняется. Рекомендуется использовать для ссылок на страницы, использующие данные пользовательской сессии, которые браузер не сможет получить предварительно;
- `intent` - предварительное получение данных выполняется, когда пользователь выражает намерение перейти на страницу. Это намерение выражается наведением курсора или установкой фокуса на ссылку. Рекомендуемый способ;
- `render` - предварительное получение данных выполняется при рендеринге ссылки.

### PrefetchPageLinks

Данный компонент рендерит все теги `<link rel="prefetch">` и `<link rel="modulepreload"/>` для всех ресурсов указанной страницы (путь к странице должен быть абсолютным):

```javascript
<PrefetchPageLinks page="/absolute/path/to/page" />
```

### NavLink

`NavLink` - это специальный тип `Link`, содержащий информацию об "активности" ссылки. Это может быть полезным при разработке меню навигации, такого как хлебные крошки или набор вкладок, для отображения выбранного элемента.

По умолчанию активному `NavLink` добавляется класс `active`. Проп `style` рассматриваемого компонента принимает функцию, позволяющую кастомизировать контент ссылки на основе ее состояния.

```javascript
import { NavLink } from "@remix-run/react";

function NavList() {
  // эти стили будут применяться только к выбранной ссылке
  const activeStyle = {
    textDecoration: "underline",
  };
  const activeClassName = "underline";

  return (
    <nav>
      <ul>
        <li>
          <NavLink
            to="messages"
            style={({ isActive }) =>
              isActive ? activeStyle : undefined
            }
          >
            Сообщения
          </NavLink>
        </li>
        <li>
          <NavLink
            to="tasks"
            className={({ isActive }) =>
              isActive ? activeClassName : undefined
            }
          >
            Задачи
          </NavLink>
        </li>
      </ul>
    </nav>
  );
}
```

Проп `end` определяет, что компонент будет активным только при совпадении его собственного пути, т.е. без учета совпадений путей его дочерних роутов:

```javascript
<NavLink to="/" end>
  Главная
</NavLink>
```

### Form

`Form` - это декларативный способ модификации данных, те.е их создания, обновления и удаления:

```javascript
import { Form } from "@remix-run/react";

function NewEvent() {
  return (
    <Form method="post" action="/events">
      <input type="text" name="title" />
      <input type="text" name="description" />
    </Form>
  );
}
```

- операции с данными будут выполняться независимо от присутствия JavaScript на странице;
- после отправки формы все `loader()` на странице перезагружаются. Это позволяет обеспечить соответствие данных и UI;
- `Form` автоматически сериализует данные (по аналогии с тем, как это делает браузер при отсутствии JS);
- хук `useTransition` (см. ниже) позволяет реализовывать оптимистичное обновление `UI`.

__Пропы `Form`__

_action_

В большинстве случаев этот проп не требуется. Формы без пропа `action` (`<Form method="post">`) автоматически отправляют данные роуту, в котором они находятся. Это облегчает совместное размещение компонента, а также функций чтения и записи данных.

`action()` позволяет отправлять данные другому роуту:

```javascript
<Form action="/projects/new" method="post" />
```

В отличие от `loader()`, которые вызываются при отправке запроса GET во всех роутах, совпадающих с URL, `action()` при отправке запроса POST вызывается только в самом глубоко вложенном совпадающем роуте до тех пор, пока речь не идет об индексном роуте. В последнем случае вызывается `action()` родительского роута.

Если мы хотим отправить данные основному роуту, следует использовать параметр строки запроса `index` в `action()`: `<Form action="/accounts?index" method="post" />`.

_method_

Определяет [метод запроса HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods): GET, POST, PUT, PATCH, DELETE. Дефолтным методом является GET.

```javascript
<Form method="post" />
```

Нативный элемент `form` поддерживает только запросы GET и POST. При отсутствии JS на странице Remix преобразует все не GET-запросы в POST-запросы. Эту проблему можно решить с помощью скрытого инпута `<input type="hidden" name="_method" value="delete" />`. При наличии JS об этом можно не беспокоиться.

_encType_

По умолчанию имеет значение `application/x-www-form-urlencoded`, для загрузки файлов следует использовать `multipart/form-data`.

_replace_

Указывает форме заменить текущую сущность в стеке истории вместо добавления новой. Может быть полезным, когда предполагается множественная отправка формы, чтобы пользователь мог вернуться на предыдущую страницу, нажав кнопку "Назад" один раз.

_reloadDocument_

Если имеет значение `true`, форма отправляется браузером, а не JS. Данный проп является обязательным для `Form`, отправляющей данные ресурсному роуту.

## Хуки / Hooks

### useLoaderData

Этот хук позволяет получить доступ к разобранным данным, возвращаемым `loader()` текущего роута:

```javascript
import { json } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

export async function loader() {
  return json(await fakeDb.invoices.findAll());
}

export default function Invoices() {
  const invoices = useLoaderData();
  // ...
}
```

### useActionData

Этот хук позволяет получить доступ к разобранным данным, возвращаемым `action()` текущего роута. Если форма еще не отправлялась, `useActionData()` возвращает `undefined`:

```javascript
import { json } from "@remix-run/node";
import { useActionData, Form } from "@remix-run/react";

export async function action({ request }) {
  const body = await request.formData();

  const name = body.get("visitorsName");

  return json({ message: `Привет, ${name}` });
}

export default function Invoices() {
  const data = useActionData();

  return (
    <Form method="post">
      <p>
        <label>
          Как Вас зовут?
          <input type="text" name="visitorsName" />
        </label>
      </p>
      <p>{data ? data.message : "Waiting..."}</p>
    </Form>
  );
}
```

Типичным случаем использования `useActionData()` является валидация формы:

```javascript
import { redirect, json } from "@remix-run/node";
import { Form, useActionData } from "@remix-run/react";

export async function action({ request }) {
  const form = await request.formData();
  const email = form.get("email");
  const password = form.get("password");
  const errors = {};

  // валидируем поля
  if (typeof email !== "string" || !email.includes("@")) {
    errors.email = "Это не похоже на адрес электронной почты";
  }

  if (typeof password !== "string" || password.length < 6) {
    errors.password = "Пароль должен состоять минимум из 6 символов";
  }

  // возвращаем ошибки
  if (Object.keys(errors).length) {
    return json(errors, { status: 422 });
  }

  // создаем пользователя и выполняем перенаправление
  await createUser(form);
  return redirect("/dashboard");
}

export default function Signup() {
  const errors = useActionData();

  return (
    <>
      <h1>Регистрация</h1>
      <Form method="post">
        <p>
          <input type="text" name="email" />
          {errors?.email ? (
            <span>{errors.email}</span>
          ) : null}
        </p>
        <p>
          <input type="text" name="password" />
          {errors?.password ? (
            <span>{errors.password}</span>
          ) : null}
        </p>
        <p>
          <button type="submit">Зарегистрироваться</button>
        </p>
      </Form>
    </>
  );
}
```

### useSubmit

Этот хук возвращает функцию, которая позволяет отправлять форму программно. Он похож на хук `useNavigate` из `React Router` для формы. Это может быть полезным, например, для сохранения данных пользователя при заполнении любого поля:

```javascript
import { json } from "@remix-run/node";
import { useSubmit, useTransition } from "@remix-run/react";

export async function loader() {
  return json(await getUserPreferences());
}

export async function action({ request }) {
  await updatePreferences(await request.formData());

  return redirect("/prefs");
}

function UserPreferences() {
  const submit = useSubmit();
  const transition = useTransition();

  function handleChange(event) {
    submit(event.currentTarget, { replace: true });
  }

  return (
    <Form method="post" onChange={handleChange}>
      <label>
        <input type="checkbox" name="darkMode" value="on" />{" "}
        Темная тема
      </label>
      {transition.state === "submitting" ? (
        <p>Сохранение...</p>
      ) : null}
    </Form>
  );
}
```

Это также может быть полезным для выполнения выхода пользователя из системы при отсутствии его активности в течение определенного времени, например, 5 минут:

```javascript
import { useSubmit, useTransition } from "@remix-run/react";
import { useEffect } from "react";

function AdminPage() {
  useSessionTimeout();

  return <div>{/* ... */}</div>;
}

function useSessionTimeout() {
  const submit = useSubmit();
  const transition = useTransition();

  useEffect(() => {
    const timer = setTimeout(() => {
      submit(null, { method: "post", action: "/logout" });
    }, 5 * 60_000);

    return () => clearTimeout(timer);
  }, [submit, transition]);
}
```

### useTransition

Этот хук предоставляет всю необходимую информацию о переходе страницы для создания индикаторов загрузки и оптимистичного обновления при модификации данных. Он отлично подходит для реализации следующих вещей:

- глобальные индикаторы загрузки;
- спиннеры ссылок;
- блокировка формы на период мутации данных;
- спиннеры кнопок;
- оптимистичное отображение новой записи до ее создания на сервере;
- оптимистичное отображение нового состояния до его обновления на сервере.

```javascript
import { useTransition } from "@remix-run/react";

function SomeComponent() {
  const transition = useTransition();
  // transition.state;
  // transition.type;
  // transition.submission;
  // transition.location;
}
```

_state_

Состояние перехода:

- `idle` - переход отсутствует;
- `submitting` - форма отправлена, вызвана либо `loader()` (при запросе GET), либо `action()` (при другом запросе);
- `loading` - вызвана `loader()` следующего роута для рендеринга следующей страницы.

Переход при навигации:

```
idle → loading → idle
```

Переход при отправке формы методом GET:

```
idle → submitting → idle
```

Переход при отправке формы другим методом:

```
idle → submitting → loading → idle
```

```javascript
function SubmitButton() {
  const transition = useTransition();

  const text =
    transition.state === "submitting"
      ? "Сохранение..."
      : transition.state === "loading"
        ? "Сохранено"
        : "Вперед";

  return <button type="submit">{text}</button>;
}
```

_type_

Тип перехода, который зависит от состояния перехода:

- `state === 'idle'`:
  - `idle`;
- `state === 'submitting'`:
  - `loaderSubmission` - форма отправлена методом GET, вызвана `loader()`;
  - `actionSubmission` - форма отправлена другим методом, вызвана `action()`;
- `state === 'loading'`:
  - `loaderSubmissionRedirect` - `loader()` выполнила перенаправление, загружается следующий роут;
  - `actionRedirect` - `action()` выполнила перенаправление, загружается следующий роут;
  - `actionReload` - `action()` вернула данные, все `loader()` на странице перезагружаются;
  - `fetchActionRedirect` - `fetcher` в `action()` выполнил перенаправление, загружается следующий роут;
  - `normalRedirect` - `loader()` обычной навигации (или перенаправления) выполнила перенаправление, загружается новый роут;
  - `normalLoad` - обычная загрузка обычной навигации.

```javascript
function SubmitButton() {
  const transition = useTransition();

  const loadTexts = {
    actionRedirect: "Данные сохранены, выполняется перенаправление...",
    actionReload: "Данные сохранены, загружаются свежие данные...",
  };

  const text =
    transition.state === "submitting"
      ? "Сохранение..."
      : transition.state === "loading"
      ? loadTexts[transition.type] || "Загрузка..."
      : "Вперед";

  return <button type="submit">{text}</button>;
}
```

_submission_

Индикатор выполнения перехода состояния.

_location_

Информация о следующей локации. Пример компонента `Link`, который "знает", когда его страница загружается и собирается стать активной:

```javascript
import { Link, useResolvedPath } from "@remix-run/react";

function PendingLink({ to, children }) {
  const transition = useTransition();
  const path = useResolvedPath(to);

  const isPending =
    transition.state === "loading" &&
    transition.location.pathname === path.pathname;

  return (
    <Link
      data-pending={isPending ? "true" : null}
      to={to}
      children={children}
    />
  );
}
```

### useFetcher

Этот хук позволяет подключить UI к `action()` и `loader()`, т.е. осуществить взаимодействие с сервером без навигации, которая выполняется элементами `a` и `form` или их эквивалентами в Remix - компонентами `Link` и `Form`.

Это может быть полезным в следующих случаях:

- получение данных, не связанных с роутами UI (всплывающие окна, динамические формы и т.д.);
- отправка данных в `action()` без навигации (распределенные компоненты типа подписки на новостную рассылку);
- обработка нескольких одновременных отправок в списке (тривиальный "список задач", где нажатие одной кнопки приводит к блокировке остальных);
- бесконечная прокрутка и др.

_Обратите внимание_: рекомендуемым способом загрузки и обновления данных являются рассмотренные ранее интерфейсы:

- `useLoaderData()`;
- `Form`;
- `useActionData()`;
- `useTransition()`.

```javascript
import { useFetcher } from "@remix-run/react";

function SomeComponent() {
  const fetcher = useFetcher();

  const formOptions = {/* ... */}

  // выполняем запрос
  <fetcher.Form {...formOptions} />;

  useEffect(() => {
    fetcher.submit(data, options);
    fetcher.load(href);
  }, [fetcher]);

  // формируем UI
  // fetcher.state;
  // fetcher.type;
  // fetcher.submission;
  // fetcher.data;
}
```

Несколько заметок о том, как это работает:

- автоматическая обработка отмены запроса на уровне браузера;
- при отправке формы не GET-методом, сначала вызывается `action()`;
  - после завершения `action()` все `loader()` на странице перезагружаются для получения свежих данных с целью синхронизации UI с серверным состоянием;
- когда одновременно выполняется несколько запросов:
  - доставляются (commit) самые свежие доступные данные после выполнения;
  - самые свежие данные не перезаписываются, независимо от порядка ответов;
- обработка необработанных ошибок ближайшим `ErrorBoundary`;
- если вызванный `action/loader` возвращает `redirect()`, выполняется перенаправление.

__Свойства `fetcher`__

_state_

- `idle` - ничего не запрашивается;
- `submitting` - форма отправлена. Если она отправлена методом GET, вызывается `loader()`, если другим методом - `action()`;
- `loading` - `loader()` роута перезагружаются после выполнения `action()`.

_type_

- `state === 'idle'`:
  - `init` - начальное состояние `fetcher`;
  - `done` - `fetcher` ничего не делает в данный момент, но выполнение предыдущего запроса завершено, данные доступны в `fetcher.data`;
- `state === 'submitting'`:
  - `actionSubmission` - см. `useTransition()`;
  - `loaderSubmission` - см. `useTransition()`;
- `state === 'loading'`:
  - `actionReload` - см. `useTransition()`;
  - `actionRedirect` - см. `useTransition()`;
  - `normalLoad` - `loader()` вызван без отправки формы (`fetcher.load()`).

_submission_

При использовании `<fetcher.Form>` или `fetcher.submit()` данное свойство может применяться для формирования оптимистичного UI. Оно недоступно, когда `fetcher` находится в состоянии `idle` или `loading`.

_data_

Здесь хранится ответ `loader()` или `action()`. После записи данные сохраняются даже при перезагрузках и повторных отправках формы.

_Form_

Аналог `Form`, но без навигации:

```javascript
function SomeComponent() {
  const fetcher = useFetcher();

  return (
    <fetcher.Form method="post" action="/some/route">
      <input type="text" />
    </fetcher.Form>
  );
}
```

_submit()_

Аналог `useSubmit()`, но без навигации:

```javascript
function SomeComponent() {
  const fetcher = useFetcher();

  const onClick = () =>
    fetcher.submit({ some: "value" }, { method: "post" });

  // ...
}
```

_load()_

Загружает данные из `loader()`:

```javascript
function SomeComponent() {
  const fetcher = useFetcher();

  useEffect(() => {
    if (fetcher.type === "init") {
      fetcher.load("/some/route");
    }
  }, [fetcher]);

  // данные из `loader()`
  // fetcher.data
}
```

__Примеры__

_Форма подписки на новостную рассылку_

Предположим, что мы хотим иметь форму подписки на новостную рассылку в подвале каждой страницы нашего сайта. Для этого отлично подойдет `useFetcher()`. Создаем ресурсный роут:

```javascript
// routes/newsletter/subscribe.ts
export async function action({ request }) {
  const email = (await request.formData()).get("email");

  try {
    await subscribe(email);
    return json({ ok: true });
  } catch (error) {
    return json({ error: error.message });
  }
}
```

Затем рендерим в `root.tsx` приложения такой компонент:

```javascript
// ...

function NewsletterSignup() {
  const newsletter = useFetcher();
  const ref = useRef();

  useEffect(() => {
    if (newsletter.type === "done" && newsletter.data.ok) {
      ref.current.reset();
    }
  }, [newsletter]);

  return (
    <newsletter.Form
      ref={ref}
      method="post"
      action="/newsletter/subscribe"
    >
      <p>
        <input type="text" name="email" />{" "}
        <button
          type="submit"
          disabled={newsletter.state === "submitting"}
        >
          Подписаться
        </button>
      </p>

      {newsletter.type === "done" ? (
        newsletter.data.ok ? (
          <p>Спасибо за подписку!</p>
        ) : newsletter.data.error ? (
          <p data-error>{newsletter.data.error}</p>
        ) : null
      ) : null}
    </newsletter.Form>
  );
}
```

_Обратите внимание_: это будет работать только при наличии JS на странице.

_Автоматическая пометка статьи как прочитанной_

Предположим, что мы хотим помечать статью как прочитанную и выполнять прокрутку вниз после того, как пользователь находится на странице какое-то время:

```javascript
function useMarkAsRead({ articleId, userId }) {
  const marker = useFetcher();

  useSpentSomeTimeHereAndScrolledToTheBottom(() => {
    marker.submit(
      { userId },
      {
        method: "post",
        action: `/article/${articleId}/mark-as-read`,
      }
    );
  });
}
```

_Отображение данных пользователя при наведении указателя на его аватар_

Предположим, что мы хотим запрашивать и отображать некоторые данные о пользователя при наведении пользователем указателя на свой аватар:

```javascript
export async function loader({ params }) {
  return json(
    await fakeDb.user.find({ where: { id: params.id } })
  );
}

function UserAvatar({ partialUser }) {
  const userDetails = useFetcher();
  const [showDetails, setShowDetails] = useState(false);

  useEffect(() => {
    if (showDetails && userDetails.type === "init") {
      userDetails.load(`/users/${user.id}/details`);
    }
  }, [showDetails, userDetails]);

  return (
    <div
      onMouseEnter={() => setShowDetails(true)}
      onMouseLeave={() => setShowDetails(false)}
    >
      <img src={partialUser.profileImageUrl} />
      {showDetails ? (
        userDetails.type === "done" ? (
          <UserPopup user={userDetails.data} />
        ) : (
          <UserPopupLoading />
        )
      ) : null}
    </div>
  );
}
```

### useMatches

Этот хук возвращает все роуты страницы. Это может быть полезным для создания абстракций макета текущего роута:

```javascript
function SomeComponent() {
  const matches = useMatches();

  // ...
}
```

`matches` имеет следующую форму:

```javascript
[
  { id, pathname, data, params, handle }, // корневой роут
  { id, pathname, data, params, handle }, // роут макета
  { id, pathname, data, params, handle }, // дочерний роут
  // etc.
];
```

Тот факт, что Remix знает все роуты и данные дерева элементов React, позволяет добавлять теги `meta`, `link` и `script` в начало документа, даже при условии, что они определяются во вложенных роутах.

Использование `useMatches()` совместно с `handle()` позволяет разрабатывать собственные абстракции, похожие на `<Meta>`, `<Links>` и `<Scripts>`.

Рассмотрим пример создания хлебных крошек.

Мы можем возвращать из `handle()` что угодно. В данном случае мы возвращаем `breadcrumb()`.

1. Добавляем обработку хлебных крошек в родительский роут:

```javascript
// routes/parent.tsx
export const handle = {
  breadcrumb: () => <Link to="/parent">Родительский роут</Link>,
};
```

2. Делаем тоже самое в дочернем роуте:

```javascript
// routes/parent/child.tsx
export const handle = {
  breadcrumb: () => (
    <Link to="/parent/child">Дочерний роут</Link>
  ),
};
```

3. Собираем хлебные крошки в корневом роуте с помощью `useMatches()`:

```javascript
// root.tsx
import {
  Links,
  Scripts,
  useLoaderData,
  useMatches,
} from "@remix-run/react";

export default function Root() {
  const matches = useMatches();

  return (
    <html lang="en">
      <head>
        <Links />
      </head>
      <body>
        <header>
          <ol>
            {matches
              // пропускаем роуты, не имеющие хлебных крошек
              .filter(
                (match) =>
                  match.handle && match.handle.breadcrumb
              )
              // рендерим хлебные крошки
              .map((match, index) => (
                <li key={index}>
                  {match.handle.breadcrumb(match)}
                </li>
              ))}
          </ol>
        </header>

        <Outlet />
      </body>
    </html>
  );
```

Доступ к данным роута можно получить через `match.data`.

### useBeforeUnload

Этот хук представляет собой абстракцию над `window.onbeforeunload`. Он позволяет сохранять важную информацию перед выгрузкой документа:

```javascript
import { useBeforeUnload } from "@remix-run/react";

function SomeForm() {
  const [state, setState] = React.useState(null);

  // сохраняем информацию перед выгрузкой страницы
  useBeforeUnload(
    React.useCallback(() => {
      localStorage.setItem('stuff', JSON.stringify(state));
    }, [state])
  );

  // читаем сохраненную информацию после загрузки страницы
  React.useEffect(() => {
    if (state === null && localStorage.getItem('stuff')) {
      setState(JSON.parse(localStorage.getItem('stuff')));
    }
  }, [state]);

  return <>{/*... */}</>;
}
```

## Утилиты HTTP / HTTP Helpers

### json

Утилита для создания ответов `application/json`. Предполагается, что используется кодировка `utf-8`:

```javascript
import { json } from "@remix-run/node";

export const loader = async () => {
  // это является сокращением...
  return json({ any: "thing" });

  // для этого
  return new Response(JSON.stringify({ any: "thing" }), {
    headers: {
      "Content-Type": "application/json; charset=utf-8",
    },
  });
};
```

`json()` позволяет указывать статус-код ответа и дополнительные заголовки HTTP:

```javascript
export const loader = async () => {
  return json(
    { not: "coffee" },
    {
      status: 418,
      headers: {
        "Cache-Control": "no-store",
      },
    }
  );
};
```

### redirect

Утилита для отправки ответов `30x` - выполнения перенаправлений:

```javascript
import { redirect } from "@remix-run/node";

export const action = async () => {
  const userSession = await getUserSession();

  if (!userSession) {
    return redirect("/login");
  }

  return json({ ok: true });
};
```

По умолчанию отправляется статус-код `302`. Это можно изменить:

```javascript
redirect(path, 301);
redirect(path, 303);
```

Мы также можем отправлять `ResponseInit` для установки заголовков HTTP, например, о сессии:

```javascript
redirect(path, {
  headers: {
    "Set-Cookie": await commitSession(session),
  },
});

redirect(path, {
  status: 302,
  headers: {
    "Set-Cookie": await commitSession(session),
  },
});
```

Разумеется, вместо `redirect()` можно возвращать обычный `Response`:

```javascript
// это является сокращением...
return redirect("/else/where", 303);

// для этого
return new Response(null, {
  status: 303,
  headers: {
    Location: "/else/where",
  },
});
```

## Куки / Cookies

[Куки](https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies) - это небольшая часть данных, которые сервер отправляет в возвращаемом ответе, и которые прикрепляются к последующим запросам браузера. Куки часто используются для реализации такого функционала, как аутентификация (см. ниже), корзина товаров, предпочтения пользователя и т.д.

Интерфейс `Cookie` предоставляет логический повторно используемый контейнер для метаданных куки.

### Использование куки

Хотя куки можно создавать вручную, рекомендуется использовать хранилище сессии (см. ниже).

В Remix работа с куки, как правило, осуществляется в `loader()` или `action()`.

Предположим, что на нашем сайте есть баннер с акционными товарами. Баннер располагается в верхней части страницы и содержит кнопку для отключения виджета на неделю.

Создаем куки:

```javascript
import { createCookie } from "@remix-run/node";

export const userPrefs = createCookie("user-prefs", {
  maxAge: 604_800, // одна неделя
});
```

Эту куки можно импортировать и использовать в `loader()` или `action()`. `loader()` проверяет предпочтения пользователя для решения вопроса о необходимости рендеринга баннера. При нажатии кнопки отключения виджета форма вызывает `action()` на сервере и повторно рендерит страницу, но уже без баннера.

_Обратите внимание_: в настоящее время рекомендуется создавать все куки в файле `app/cookies.js` и импортировать их в соответствующие модули. Это позволяет Remix исключать куки из сборки для браузера.

```javascript
import { json, redirect } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";
// !
import { userPrefs } from "~/cookies";

export async function loader({ request }) {
  const cookieHeader = request.headers.get("Cookie");
  // !
  const cookie =
    (await userPrefs.parse(cookieHeader)) || {};
  return json({ showBanner: cookie.showBanner });
}

export async function action({ request }) {
  const cookieHeader = request.headers.get("Cookie");
  // !
  const cookie =
    (await userPrefs.parse(cookieHeader)) || {};
  const bodyParams = await request.formData();

  if (bodyParams.get("bannerVisibility") === "hidden") {
    cookie.showBanner = false;
  }

  return redirect("/", {
    headers: {
      "Set-Cookie": await userPrefs.serialize(cookie),
    },
  });
}

export default function Home() {
  const { showBanner } = useLoaderData();

  return (
    <div>
      {showBanner ? (
        <div>
          <Link to="/sale">Не пропустите распродажу!</Link>
          <Form method="post">
            <input
              type="hidden"
              name="bannerVisibility"
              value="hidden"
            />
            <button type="submit">Скрыть</button>
          </Form>
        </div>
      ) : null}
      <h1>Добро пожаловать!</h1>
    </div>
  );
}
```

### Атрибуты куки

Куки имеют [несколько атрибутов](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie#attributes), определяющих их время жизни, доступность, путь и др. Эти атрибуты могут устанавливаться как в `createCookie(name, options)`, так и в `serialize()` при генерации заголовка `Set-Cookie`.

```javascript
const cookie = createCookie("user-prefs", {
  // дефолтные настройки для этой куки
  domain: "remix.run",
  path: "/",
  sameSite: "lax",
  httpOnly: true,
  secure: true,
  expires: new Date(Date.now() + 60_000),
  maxAge: 60,
});

// используем настройки по умолчанию
cookie.serialize(userPrefs);

// или перезаписываем некоторые из них
cookie.serialize(userPrefs, { sameSite: "strict" });
```

### Подписание куки

Подписание (signing) позволяет автоматически проверять/подтверждать содержимое куки при ее получении. Данная техника применяется в отношении чувствительной информации, такой как данные об аутентификации.

Для подписания достаточно указать массив секретов при создании куки:

```javascript
const cookie = createCookie("user-prefs", {
  secrets: ["s3cret1"],
});
```

Ротация секретов выполняется посредством добавления нового секрета в начало массива `secrets`. Куки, подписанные с помощью старых секретов будут успешно декодироваться в `cookie.parse()`, а новые секреты будут использоваться для подписания куки, создаваемых в `cookie.serialize()`:

```javascript
// app/cookies.js
const cookie = createCookie("user-prefs", {
  secrets: ["n3wsecr3t", "olds3cret"],
});

// в роуте
export async function loader({ request }) {
  const oldCookie = request.headers.get("Cookie");
  // `oldCookie` может быть подписан с помощью `olds3cret`, но будет успешно разобран
  const value = await cookie.parse(oldCookie);

  new Response("...", {
    headers: {
      // `Set-Cookie` подписывается с помощью `n3wsecr3t`
      "Set-Cookie": await cookie.serialize(value),
    },
  });
}
```

__createCookie__

Эта утилита создает логический контейнер для управления браузерными куки на стороне сервера:

```javascript
import { createCookie } from "@remix-run/node";

const cookie = createCookie("cookie-name", {
  // все эти дефолтные настройки могут быть перезаписаны в процессе выполнения кода (runtime)
  domain: "remix.run",
  expires: new Date(Date.now() + 60_000),
  httpOnly: true,
  maxAge: 60,
  path: "/",
  sameSite: "lax",
  secrets: ["s3cret1"],
  secure: true,
});
```

__isCookie__

Эта утилита возвращает `true`, если объект является контейнером для куки:

```javascript
import { isCookie } from "@remix-run/node";

const cookie = createCookie("user-prefs");
console.log(isCookie(cookie)); // true
```

### Интерфейс Cookie

Контейнер, возвращаемый `createCookie()`, содержит несколько полезных свойств и методов.

_name_

Название куки, используется в заголовках `Cookie` и `Set-Cookie`.

_parse()_

Извлекает и возвращает значение куки, содержащегося в заголовке `Cookie`:

```javascript
const value = await cookie.parse(
  request.headers.get("Cookie")
);
```

_serialize()_

Сериализует значение и объединяет его с настройками куки для создания заголовка `Set-Cookie`, подходящего для использования в исходящем `Response`:

```javascript
new Response("...", {
  headers: {
    "Set-Cookie": await cookie.serialize({
      showBanner: true,
    }),
  },
});
```

_isSigned_

Возвращает `true`, если куки подписана с помощью `secrets`.

_expires_

Дата (объект `Date`), когда истекает срок действия куки. _Обратите внимание_: если куки содержит `maxAge` и `expires`, значением `expires` будет текущая дата + `maxAge`, поскольку `Max-Age` имеет приоритет перед `Expires`.

## Сессии / Sessions

Сессии являются важной частью веб-сайтов, поскольку позволяют серверу идентифицировать запросы, исходящие от одного и того же лица. Они часто используются для реализации системы аутентификации.

В Remix сессии управляются на основе роутов в методах `loader` и `action` с помощью "хранилища сессии" (которое реализует интерфейс `SessionStorage`). Хранилище сессии умеет парсить и генерировать куки, а также записывать данные сессии в базу данных или файловую систему.

Remix предоставляет несколько встроенных хранилищ сессии для наиболее распространенных сценариев и метод для создания собственного хранилища:

- `createCookieSessionStorage()`;
- `createMemorySessionStorage()`;
- `createFileSessionStorage()`;
- `createSessionStorage()` для создания кастомного хранилища.

### Использование сессий

Пример создания хранилища сессии, основанного на куки:

```javascript
// app/sessions.js
import { createCookieSessionStorage } from "@remix-run/node";

const { getSession, commitSession, destroySession } =
  createCookieSessionStorage({
    // куки из `createCookie()` или настройки для ее создания
    cookie: {
      name: "__session",

      // все эти настройки являются опциональными
      domain: "remix.run",
      httpOnly: true,
      maxAge: 60,
      path: "/",
      sameSite: "lax",
      secrets: ["s3cret1"],
      secure: true,
    },
  });

export { getSession, commitSession, destroySession };
```

Хранилище сессии рекомендуется создавать в файле `app/session.js`.

Входными и выходными данными хранилища сессии являются куки HTTP. `getSession()` извлекает текущую сессию из заголовка `Cookie` входящего запроса, а `commitSession()` и `destroySession()` устанавливают заголовок `Set-Cookie` для исходящего ответа.

Эти методы используются в `loader()` и `action()` для доступа к данным сессии.

Форма авторизации может выглядеть так:

```javascript
import { json, redirect } from "@remix-run/node";
import { useLoaderData } from "@remix-run/react";

import { getSession, commitSession } from "../sessions";

export async function loader({ request }) {
  const session = await getSession(
    request.headers.get("Cookie")
  );

  if (session.has("userId")) {
    // перенаправляем пользователя на главную страницу, если он уже авторизован
    return redirect("/");
  }

  const data = { error: session.get("error") };

  return json(data, {
    headers: {
      "Set-Cookie": await commitSession(session),
    },
  });
}

export async function action({ request }) {
  const session = await getSession(
    request.headers.get("Cookie")
  );
  const form = await request.formData();
  const username = form.get("username");
  const password = form.get("password");

  const userId = await validateCredentials(
    username,
    password
  );

  if (userId == null) {
    session.flash("error", "Неверное имя пользователя/пароль");

    // возвращаемся на страницу авторизации с ошибками
    return redirect("/login", {
      headers: {
        "Set-Cookie": await commitSession(session),
      },
    });
  }

  session.set("userId", userId);

  // авторизация прошла успешно, перенаправляем пользователя на главную страницу
  return redirect("/", {
    headers: {
      "Set-Cookie": await commitSession(session),
    },
  });
}

export default function Login() {
  const { currentUser, error } = useLoaderData();

  return (
    <div>
      {error ? <div className="error">{error}</div> : null}
      <form method="POST">
        <div>
          <p>Авторизация</p>
        </div>
        <label>
          Имя пользователя: <input type="text" name="username" />
        </label>
        <label>
          Пароль: <input type="password" name="password" />
        </label>
      </form>
    </div>
  );
}
```

Форма для выхода из системы может выглядеть так:

```javascript
import { getSession, destroySession } from "../sessions";

export const action: ActionFunction = async ({
  request,
}) => {
  const session = await getSession(
    request.headers.get("Cookie")
  );

  return redirect("/login", {
    headers: {
      "Set-Cookie": await destroySession(session),
    },
  });
};

export default function LogoutRoute() {
  return (
    <>
      <p>Вы уверены, что хотите выйти из системы?</p>
      <Form method="post">
        <button>Выйти из системы</button>
      </Form>
      <Link to="/">Я передумал</Link>
    </>
  );
}
```

### Особенности работы с сессиями

Из-за вложенных роутов для генерации страницы может вызываться несколько `loader()`. Поэтому при использовании `session.flash()` или `session.unset()` необходимо убедиться, что другие `loader()`, участвующие в запросе, не будут читать данные сессии, в противном случае, мы получим гонку условий (race conditions).

_isSession()_

Возвращает `true`, если объект является сессией Remix:

```javascript
import { isSession } from "@remix-run/node";

const sessionData = { foo: "bar" };
const session = createSession(sessionData, "remix-session");
console.log(isSession(session)); // true
```

_createSessionStorage()_

Remix позволяет хранить сессии в собственной БД. `createSessionStorage()` требует `cookie` (или настроек для ее создания) и набор методов для создания, чтения, обновления и удаления данных сессии. Куки используется для хранения идентификатора сессии.

Пример создания хранилища сессии с помощью клиента БД общего назначения:

```javascript
import { createSessionStorage } from "@remix-run/node";

function createDatabaseSessionStorage({
  cookie,
  host,
  port,
}) {
  // настраиваем клиента БД
  const db = createDatabaseClient(host, port);

  return createSessionStorage({
    cookie,
    async createData(data, expires) {
      // `expires` - это дата, после которой данные считаются невалидными.
      // Мы можем использовать это свойство для инвалидации данных или
      // автоматического удаления записи из БД
      const id = await db.insert(data);
      return id;
    },
    async readData(id) {
      return (await db.select(id)) || null;
    },
    async updateData(id, data, expires) {
      await db.update(id, data);
    },
    async deleteData(id) {
      await db.delete(id);
    },
  });
}
```

Пример использования этой утилиты:

```javascript
const { getSession, commitSession, destroySession } =
  createDatabaseSessionStorage({
    host: "localhost",
    port: 1234,
    cookie: {
      name: "__session",
      sameSite: "lax",
    },
  });
```

_createCookieSessionStorage()_

Позволяет создавать сессии, основанные на куки.

Главным преимуществом такой сессии является то, что для ее использования не требуются дополнительные серверные сервисы или БД. Однако размер такого хранилища весьма ограничен и, как правило, составляет 4 Кб.

Недостатком является необходимость вызывать `commitSession()` почти в каждой `loader()` и `action()`. Это означает, что если мы вызываем `session.flash()` в одной `action()`, и затем - `session.get()` в другой, мы должны зафиксировать состояние для очистки данных:

```javascript
import { createCookieSessionStorage } from "@remix-run/node";

const { getSession, commitSession, destroySession } =
  createCookieSessionStorage({
    cookie: {
      name: "__session",
      secrets: ["r3m1xr0ck5"],
      sameSite: "lax",
    },
  });
```

_createMemorySessionStorage()_

При использовании этого хранилища куки хранится в памяти сервера. _Обратите внимание_: это хранилище следует использовать только в режиме разработки.

```javascript
import {
  createCookie,
  createMemorySessionStorage,
} from "@remix-run/node";

const sessionCookie = createCookie("__session", {
  secrets: ["r3m1xr0ck5"],
  sameSite: true,
});

const { getSession, commitSession, destroySession } =
  createMemorySessionStorage({
    cookie: sessionCookie,
  });

export { getSession, commitSession, destroySession };
```

_createFileSessionStorage()_

При использовании этого хранилища вся информация о сессии хранится в файловой системе.

Преимуществом является то, что в куки хранится только идентификатор сессии, остальные данные хранятся в файле или на диске, что отлично подходит для сессии, размер которой превышает 4 Кб.

```javascript
import {
  createCookie,
  createFileSessionStorage,
} from "@remix-run/node";

const sessionCookie = createCookie("__session", {
  secrets: ["r3m1xr0ck5"],
  sameSite: true,
});

const { getSession, commitSession, destroySession } =
  createFileSessionStorage({
    // корневая директория для записи файлов
    // убедитесь, что она доступна для записи
    dir: "/app/sessions",
    cookie: sessionCookie,
  });

export { getSession, commitSession, destroySession };
```

### Интерфейс объекта сессии

_has(key)_

Возвращает `true`, если сессия содержит переменную `key`:

```javascript
session.has("userId");
```

_set(key, value)_

Устанавливает переменную `key` в значение `value`:

```javascript
session.set("userId", "1243");
```

_flash(key, value)_

Определяет значение, которое будет удалено при первом чтении. Может быть полезным для "флэш-сообщений" (flash messages) и сообщений о результатах валидации формы на сервере:

```javascript
import { getSession, commitSession } from "../sessions";

export async function action({ request, params }) {
  const session = await getSession(
    request.headers.get("Cookie")
  );
  const deletedProject = await archiveProject(
    params.projectId
  );

  session.flash(
    "globalMessage",
    `Проект ${deletedProject.name} успешно перемещен в архив`
  );

  return redirect("/dashboard", {
    headers: {
      "Set-Cookie": await commitSession(session),
    },
  });
}
```

После этого мы можем прочитать сообщение в `loader()`:

```javascript
import { json } from "@remix-run/node";
import {
  Meta,
  Links,
  Scripts,
  Outlet,
} from "@remix-run/react";

import { getSession, commitSession } from "./sessions";

export async function loader({ request }) {
  const session = await getSession(
    request.headers.get("Cookie")
  );
  const message = session.get("globalMessage") || null;

  return json(
    { message },
    {
      headers: {
        // требуется только при использовании `cookieSessionStorage`
        "Set-Cookie": await commitSession(session),
      },
    }
  );
}

export default function App() {
  const { message } = useLoaderData();

  return (
    <html>
      <head>
        <Meta />
        <Links />
      </head>
      <body>
        {message ? (
          <div className="flash">{message}</div>
        ) : null}
        <Outlet />
        <Scripts />
      </body>
    </html>
  );
}
```

_get(key)_

Возвращает значение переменной `key` (из предыдущего запроса):

```javascript
session.get("userId");
```

_unset(key)_

Удаляет переменную `key` из сессии:

```javascript
session.unset("userId");
```

_Обратите внимание_: при использовании `cookieSessionStorage`, после удаления переменной состояние сессии необходимо зафиксировать:

```javascript
export async function loader({ request }) {
  // ...

  return json(data, {
    headers: {
      "Set-Cookie": await commitSession(session),
    },
  });
}
```
