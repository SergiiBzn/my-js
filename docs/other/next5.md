<a name="top"></a>

[На главную](../../README.md)

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
|   | Next.js Grundlagen |
|1 | [Was ist Next.js und wofür wird es verwendet?](#1) |
|2 | [Worin unterscheidet sich Next.js von Create React App?](#2) |
|3 | [Welche Vorteile bietet Next.js für die Entwicklung?](#3) |
|4 | [Was ist „file-based routing“ (dateibasierte Routen)?](#4) |
|5 | [Was ist der Unterschied zwischen dem pages- und dem app-Verzeichnis?](#5) |
|6 | [Was ist der App Router (Next.js 13+) und wie unterscheidet er sich vom Pages Router?](#6) |
|7 | [Was ist Server-Side Rendering (SSR)?](#7) |
|8 | [Was ist Static Site Generation (SSG)?](#8) |
|9 | [Was ist Client-Side Rendering (CSR)?](#9) |
|10 | [Was ist Incremental Static Regeneration (ISR)?](#10) |
|11 | [Wann sollte man SSR, SSG und ISR verwenden?](#11) |
|12 | [Was macht der Befehl npx create-next-app?](#12) |
|13 | [Wie funktioniert Hydration in Next.js?](#13) |
|14 | [Was bedeutet „pre-rendering“?](#14) |
|15 | [Welche Sprachen und Technologien unterstützt Next.js out of the box?](#15) |
|16 | [Wie richtet man TypeScript in Next.js ein?](#16) |
|17 | [Was machen next dev, next build, next start?](#17) |
|18 | [Welche Einschränkungen hat Next.js?](#18) |
|   | Routing (Routen) |
|19 | [Wie funktioniert das Routing in Next.js?](#19) |
|20 | [Wie erstellt man dynamische Routen ([id].tsx)?](#20) |
|21 | [Wie funktionieren Catch-All-Routen ([...slug].tsx)?](#21) |
|22 | [Was sind optionale Catch-All-Routen ([[...slug]])?](#22) |
|23 | [Wie funktioniert Nested Routing (verschachtelte Routen)?](#23) |
|24 | [Wie übergibt man Query-Parameter in Routen?](#24) |
|25 | [Wie kann man Routenparameter auf dem Server abrufen?](#25) |
|26 | [Wie implementiert man Redirects in Next.js?](#26) |
|27 | [Was ist Middleware in Next.js und wofür wird sie benötigt?](#27) |
|28 | [Wie funktioniert Internationalisierung (i18n) in Next.js?](#28) |
|29 | [Was ist der Unterschied zwischen Routing im pages- und im app-Verzeichnis?](#29) |
|   | Rendering und Daten |
|30 | [Was macht getStaticProps?](#30) |
|31 | [Was macht getServerSideProps?](#31) |
|32 | [Was macht getStaticPaths?](#32) |
|33 | [Wann sollte man getStaticProps vs. getServerSideProps verwenden?](#33) |
|34 | [Wie funktioniert revalidate im ISR?](#34) |
|35 | [Wie ruft man Daten im App Router (Next.js 13) ab?](#35) |
|36 | [Was ist der Unterschied zwischen fetch auf dem Server und auf dem Client?](#36) |
|37 | [Wie funktionieren Server Components (Next.js 13)?](#37) |
|38 | [Was ist der Unterschied zwischen Client Components und Server Components?](#38) |
|39 | [Wie bindet man externe Bibliotheken in Server Components ein?](#39) |
|40 | [Welche Einschränkungen haben Server Components?](#40) |
|   | API Routes |
|41 | [Was sind API Routes in Next.js?](#41) |
|42 | [Wie erstellt man einen API-Endpunkt (pages/api/...)?](#42) |
|43 | [Wie funktionieren API Routes im App Router (route.ts)?](#43) |
|44 | [Wie übergibt man Query-Parameter an API Routes?](#44) |
|45 | [Wie verarbeitet man POST-Anfragen in API Routes?](#45) |
|46 | [Wie verwendet man Middleware in API Routes?](#46) |
|47 | [Worin besteht der Unterschied zwischen API Routes und einem separaten Backend-Server?](#47) |
|48 | [Kann man Next.js API Routes als Production-Backend verwenden?](#48) |
|   | Statische Dateien und Assets |
|49 | [Wie funktioniert der public-Ordner?](#49) |
|50 | [Wie bindet man Bilder in Next.js ein?](#50) |
|51 | [Was macht next/image und wofür wird es benötigt?](#51) |
|52 | [Welche Vorteile hat next/image im Vergleich zu <img>?](#52) |
|53 | [Wie funktioniert Image Optimization?](#53) |
|54 | [Kann man dynamische Bilder im public-Ordner speichern?](#54) |
|55 | [Wie bindet man Schriftarten in Next.js ein?](#55) |
|56 | [Was ist next/font?](#56) |
|   | Styling |
|57 | [Welche Styling-Methoden unterstützt Next.js?](#57) |
|58 | [Wie verwendet man CSS-Module?](#58) |
|59 | [Wie verwendet man SASS/SCSS in Next.js?](#59) |
|60 | [Wie integriert man TailwindCSS in Next.js?](#60) |
|61 | [Was ist styled-jsx?](#61) |
|62 | [Wie verwendet man styled-components in Next.js?](#62) |
|63 | [Welche Best Practices gibt es für Styling in großen Next.js-Projekten?](#63) |
|   | Performance-Optimierung |
|64 | [Was macht automatisches Code-Splitting in Next.js?](#64) |
|65 | [Wie funktioniert Lazy Loading?](#65) |
|66 | [Wie optimiert man Bilder in Next.js?](#66) |
|67 | [Wie verwendet man next/script zum Laden von Skripten?](#67) |
|68 | [Was ist Static Optimization?](#68) |
|69 | [Wie reduziert man die Bundle-Größe in Next.js?](#69) |
|70 | [Wie optimiert man Lighthouse-Scores?](#70) |
|71 | [Wie funktioniert der eingebaute SWC-Compiler?](#71) |
|72 | [Was sind Edge Functions und wie unterscheiden sie sich von Serverless Functions?](#72) |
|   | Sicherheit |
|73 | [Welche Sicherheitsrisiken gibt es in Next.js-Projekten?](#73) |
|74 | [Wie schützt man API Routes?](#74) |
|75 | [Wie implementiert man Authentifizierung in Next.js?](#75) |
|76 | [Was ist NextAuth.js und wie funktioniert es?](#76) |
|77 | [Wie speichert man Sessions in Next.js?](#77) |
|78 | [Wie schützt man Seiten vor unautorisiertem Zugriff?](#78) |
|79 | [Wie arbeitet man mit Environment Variablen (.env.local)?](#79) |
|   | Deployment und DevOps |
|80 | [Wo kann man Next.js-Anwendungen deployen?](#80) |
|81 | [Worin unterscheidet sich Vercel von Netlify?](#81) |
|82 | [Wie deployt man Next.js auf Vercel?](#82) |
|83 | [Kann man Next.js mit Docker deployen?](#83) |
|84 | [Wie deployt man Next.js auf AWS?](#84) |
|85 | [Was ist der Unterschied zwischen Serverless-Deployment und Edge-Deployment?](#85) |
|86 | [Welche Probleme können beim Deployment von Next.js auftreten?](#86) |
|   | Internationalisierung (i18n) |
|87 | [Wie aktiviert man die integrierte i18n-Unterstützung in Next.js?](#87) |
|88 | [Wie implementiert man Mehrsprachigkeit im App Router?](#88) |
|89 | [Welche i18n-Bibliotheken werden am häufigsten mit Next.js verwendet?](#89) |
|90 | [Wie funktioniert automatisches Redirect nach Browsersprache?](#90) |
|   | Fortgeschrittene Themen |
|91 | [Was ist Middleware und wie wird sie verwendet?](#91) |
|92 | [Was ist Edge Runtime?](#92) |
|93 | [Wie funktionieren Streaming und Suspense in Next.js 13?](#93) |
|94 | [Wie funktionieren Parallel Routes?](#94) |
|95 | [Was sind Intercepting Routes?](#95) |
|96 | [Wie bindet man eine GraphQL-API in Next.js ein?](#96) |
|97 | [Wie integriert man Redux Toolkit mit Next.js?](#97) |
|98 | [Wie integriert man Zustand mit Next.js?](#98) |
|99 | [Wie integriert man React Query mit Next.js?](#99) |
|100 | [Wie implementiert man SSR mit Redux in Next.js?](#100) |
|101 | [Wie richtet man eine PWA in Next.js ein?](#101) |
|102 | [Wie implementiert man dynamische Meta-Informationen (head)?](#102) |
|103 | [Wie funktioniert die metadata API im App Router?](#103) |
|104 | [Wie fügt man eine Sitemap in Next.js hinzu?](#104) |
|105 | [Wie fügt man eine robots.txt in Next.js hinzu?](#105) |
|106 | [Wie integriert man WebSockets in Next.js?](#106) |
|107 | [Wie verwendet man Next.js in einem Monorepo (z. B. Turborepo)?](#107) |
|108 | [Wie funktioniert Hot Reloading in Next.js?](#108) |
|109 | [Was sind App Router Layouts?](#109) |
|110 | [Was ist der Unterschied zwischen Root Layout und Nested Layout?](#110) |
|111 | [](#111) |
|112 | [](#112) |
|113 | [](#113) |
|114 | [](#114) |
|115 | [](#115) |
|116 | [](#116) |
|117 | [](#117) |
|118 | [](#118) |
|119 | [](#119) |
|120 | [](#120) |
|121 | [](#121) |
|122 | [](#122) |
|123 | [](#123) |
|124 | [](#124) |
|125 | [](#125) |
|126 | [](#126) |
|127 | [](#127) |
|128 | [](#128) |
|129 | [](#129) |
|130 | [](#130) |
|131 | [](#131) |
|132 | [](#132) |
|133 | [](#133) |
|134 | [](#134) |
|135 | [](#135) |
|136 | [](#136) |
|137 | [](#137) |
|138 | [](#138) |
|139 | [](#139) |
|140 | [](#140) |
|141 | [](#141) |
|142 | [](#142) |
|143 | [](#143) |
|144 | [](#144) |
|145 | [](#145) |
|146 | [](#146) |
|147 | [](#147) |
|148 | [](#148) |
|149 | [](#149) |
|150 | [](#150) |
|151 | [](#151) |
|152 | [](#152) |
|153 | [](#153) |
|154 | [](#154) |
|155 | [](#155) |
|156 | [](#156) |
|157 | [](#157) |
|158 | [](#158) |
|159 | [](#159) |
|160 | [](#160) |
|161 | [](#161) |
|162 | [](#162) |
|163 | [](#163) |
|164 | [](#164) |
|165 | [](#165) |
|166 | [](#166) |
|167 | [](#167) |
|168 | [](#168) |
|169 | [](#169) |
|170 | [](#170) |
|171 | [](#171) |
|172 | [](#172) |
|173 | [](#173) |
|174 | [](#174) |
|175 | [](#175) |
|176 | [](#176) |
|177 | [](#177) |
|178 | [](#178) |
|179 | [](#179) |
|180 | [](#180) |
|181 | [](#181) |
|182 | [](#182) |
|183 | [](#183) |
|184 | [](#184) |
|185 | [](#185) |
|186 | [](#186) |
|187 | [](#187) |
|188 | [](#188) |
|189 | [](#189) |
|190 | [](#190) |
|191 | [](#191) |
|192 | [](#192) |
|193 | [](#193) |
|194 | [](#194) |
|195 | [](#195) |
|196 | [](#196) |
|197 | [](#197) |
|198 | [](#198) |
|199 | [](#199) |
|200 | [](#200) |



<a name="questions"></a>

## Next.js 

  **[⬆ Наверх](#top)**
  
1. ### <a name="1"></a> Was ist Next.js und wofür wird es verwendet?

**Definition:**
Next.js ist ein **React-Framework** für die Entwicklung von modernen Webanwendungen. Es erweitert React um Funktionen wie **Server-Side Rendering (SSR)**, **Static Site Generation (SSG)**, **API-Routen**, **Dateibasierte Routing-Struktur** und **optimierte Performance**.

**Verwendung:**

* Erstellung von **SEO-freundlichen Webseiten**, da Inhalte serverseitig oder statisch gerendert werden können.
* Entwicklung von **Full-Stack-Anwendungen**, da sowohl Frontend als auch Backend-Logik (über API-Routen) möglich sind.
* Nutzung in **großen Projekten**, da Next.js Performance-Optimierungen (Code-Splitting, automatische Bildoptimierung, Caching) integriert hat.

**Einfaches Beispiel:**

```js
// app/page.js in Next.js 13+ (App Router)
// React-Komponente für die Startseite
export default function Home() {
  return (
    <main>
      <h1>Willkommen bei Next.js!</h1>
      <p>Dies ist eine serverseitig gerenderte Seite.</p>
    </main>
  )
}
```

**Zusammenfassung:**
Next.js ist ein **Full-Stack React-Framework**, das für performante, SEO-optimierte und skalierbare Webanwendungen genutzt wird. Es kombiniert Frontend- und Backend-Funktionen und bietet moderne Rendering-Strategien.

📖 Quelle: [Next.js Docs – Getting Started](https://nextjs.org/docs/app/getting-started/installation)

---

  **[⬆ Наверх](#top)**

2. ### <a name="2"></a> Worin unterscheidet sich Next.js von Create React App?

**Hauptunterschiede zwischen Next.js und Create React App (CRA):**

1. **Rendering-Strategien**

   * **CRA**: Nur **Client-Side Rendering (CSR)** – der Browser rendert Inhalte erst nach dem Laden von JavaScript.
   * **Next.js**: Unterstützt **Server-Side Rendering (SSR)**, **Static Site Generation (SSG)**, **Incremental Static Regeneration (ISR)** und CSR.

2. **Routing**

   * **CRA**: Kein integriertes Routing – man muss **react-router-dom** oder eine andere Bibliothek verwenden.
   * **Next.js**: **Dateibasiertes Routing** – jede Datei im `pages/` oder `app/` Verzeichnis wird automatisch zu einer Route.

3. **SEO**

   * **CRA**: Schlechter für SEO, da der initiale HTML-Inhalt leer ist und erst clientseitig gefüllt wird.
   * **Next.js**: Bessere SEO, da Inhalte schon beim ersten Request vom Server oder statisch ausgeliefert werden.

4. **API-Integration**

   * **CRA**: Nur Frontend – für Backend muss ein separater Server geschrieben werden.
   * **Next.js**: Bietet **API-Routen** (`/pages/api/*` oder `app/api/*`), womit Backend-Endpunkte direkt in der App möglich sind.

5. **Performance & Features**

   * **CRA**: Keine integrierte Bildoptimierung oder Code-Splitting über die Standardfunktionen hinaus.
   * **Next.js**: Eingebaute **Bildoptimierung (`next/image`)**, **automatisches Code-Splitting**, **Prefetching von Links** und **Internationalisierung**.

---

**Code-Vergleich – Routing**

*React mit CRA (manuell mit react-router-dom):*

```js
// src/App.js
import { BrowserRouter, Route, Routes } from "react-router-dom";
import Home from "./Home";
import About from "./About";

export default function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/about" element={<About />} />
      </Routes>
    </BrowserRouter>
  );
}
```

*Next.js (automatisch über Datei-Struktur):*

```js
// app/page.js
export default function Home() {
  return <h1>Startseite</h1>;
}

// app/about/page.js
export default function About() {
  return <h1>Über uns</h1>;
}
```

---

**Zusammenfassung:**

* **CRA** ist ein **Frontend-Tooling-Setup** für React ohne Server-Features.
* **Next.js** ist ein **vollwertiges React-Framework** mit SSR, SSG, API-Routen, Bildoptimierung und besserer SEO.
* CRA eignet sich für **kleine SPAs**, Next.js für **skalierbare und produktionsreife Anwendungen**.

📖 Quelle: [Next.js Docs – Why Next.js](https://nextjs.org/docs)

---

  **[⬆ Наверх](#top)**

3. ### <a name="3"></a> Welche Vorteile bietet Next.js für die Entwicklung?

**Vorteile von Next.js für die Entwicklung:**

1. **Flexible Rendering-Optionen**

   * Unterstützung von **SSR**, **SSG**, **ISR** und **CSR** → optimale Kombination aus Performance und SEO.

2. **SEO-Optimierung**

   * Inhalte werden bereits beim ersten Request ausgeliefert → bessere Sichtbarkeit in Suchmaschinen.

3. **Dateibasiertes Routing**

   * Kein zusätzlicher Router nötig → jede Datei in `pages/` oder `app/` wird automatisch eine Route.

4. **API-Routen**

   * Backend-Logik direkt in die App integrierbar → einfache Full-Stack-Entwicklung.

5. **Performance**

   * Automatisches **Code-Splitting**, **Prefetching von Links**, **Optimierung für Bilder und Fonts**.

6. **Developer Experience**

   * Hot Reloading, TypeScript-Support, integrierte Linter und einfache Konfiguration.

7. **Internationalisierung (i18n)**

   * Eingebaute Unterstützung für Mehrsprachigkeit.

8. **Deployment**

   * Nahtlose Integration mit **Vercel**, aber auch mit anderen Plattformen nutzbar.

---

**Beispiel – Bildoptimierung:**

```js
// app/page.js
import Image from "next/image";

export default function Home() {
  return (
    <main>
      <h1>Next.js Vorteile</h1>
      <Image src="/logo.png" alt="Logo" width={200} height={200} />
      {/* Bild wird automatisch optimiert und responsive ausgeliefert */}
    </main>
  );
}
```

---

**Zusammenfassung:**
Next.js bietet **hohe Performance, SEO-Freundlichkeit, einfache Full-Stack-Entwicklung und ein effizientes Entwicklererlebnis**. Es ist besonders vorteilhaft für **skalierbare, produktionsreife Anwendungen**.

📖 Quelle: [Next.js Docs – Features](https://nextjs.org/docs)

---

  **[⬆ Наверх](#top)**

4. ### <a name="4"></a> Was ist „file-based routing“ (dateibasierte Routen)?

**Definition:**
„File-based Routing“ bedeutet, dass die **Ordner- und Dateistruktur im Projekt automatisch die Routen der Anwendung bestimmt**. Jede Datei im Verzeichnis `pages/` (Pages Router) oder `app/` (App Router ab Next.js 13) wird zu einer Route. Ein zusätzlicher Router wie `react-router-dom` ist nicht nötig.

---

**Beispiele (App Router in Next.js 13+):**

```js
// app/page.js  → Route: /
export default function Home() {
  return <h1>Startseite</h1>;
}

// app/about/page.js  → Route: /about
export default function About() {
  return <h1>Über uns</h1>;
}

// app/blog/[id]/page.js  → Dynamische Route: /blog/123
export default function BlogPost({ params }) {
  return <h1>Blogeintrag: {params.id}</h1>;
}
```

* `[id]` = **dynamischer Routen-Parameter**
* `app/blog/[id]/page.js` → `/blog/1`, `/blog/2` usw.

---

**Besonderheiten:**

* **Statische Routen:** Jede Datei wird direkt einer URL zugeordnet.
* **Dynamische Routen:** Über `[param]` können Parameter in der URL verarbeitet werden.
* **Verschachtelte Routen:** Durch Unterordner entsteht automatisch eine hierarchische URL-Struktur.
* **Layout-Unterstützung (App Router):** Gemeinsame Layouts (`layout.js`) können für mehrere Routen definiert werden.

---

**Zusammenfassung:**
File-based Routing in Next.js bedeutet, dass die Verzeichnisstruktur automatisch die **Routing-Logik** bestimmt. Dadurch entfällt die manuelle Router-Konfiguration, und dynamische sowie verschachtelte Routen lassen sich einfach über Dateinamen abbilden.

📖 Quelle: [Next.js Docs – Routing](https://nextjs.org/docs/app/building-your-application/routing)

---

  **[⬆ Наверх](#top)**

5. ### <a name="5"></a> Was ist der Unterschied zwischen dem pages- und dem app-Verzeichnis?

**Unterschied zwischen `pages/` (Pages Router) und `app/` (App Router):**

---

### 1. **Einführung**

* **`pages/` (Pages Router)**: Klassisches Routing-System von Next.js (seit den Anfängen).
* **`app/` (App Router)**: Neu ab **Next.js 13**. Baut auf **React Server Components (RSC)** auf und bietet moderne Features wie Streaming, Suspense und Layouts.

---

### 2. **Routing**

* **Pages Router (`pages/`)**

  * Jede Datei in `pages/` wird automatisch zu einer Route.
  * Dynamische Routen mit `[id].js`.
  * Nur eine Ebene von Layouts möglich (z. B. `_app.js`).

* **App Router (`app/`)**

  * Dateibasiertes Routing bleibt, aber mit klarer Struktur: `page.js`, `layout.js`, `loading.js`, `error.js`.
  * Verschachtelte Layouts pro Verzeichnis möglich.
  * Bessere Trennung von UI- und Datenlogik.

---

### 3. **Rendering**

* **Pages Router:**

  * Unterstützt **SSR**, **SSG**, **ISR**, **CSR**.
  * Serverlogik über `getServerSideProps`, `getStaticProps`, `getStaticPaths`.

* **App Router:**

  * Nutzt **React Server Components** → weniger Client-JS nötig.
  * Datenfetching direkt im Server-Teil via `fetch()` möglich.
  * Automatisches Streaming von UI-Inhalten.

---

### 4. **API-Routen**

* **Pages Router:** `pages/api/*` → klassische API-Endpoints.
* **App Router:** Noch im Übergang, aber weiterhin nutzbar über `pages/api/*` oder neue Routen-Handler in `app/api/*/route.js`.

---

### 5. **Code-Beispiele**

**Pages Router (`pages/`):**

```js
// pages/index.js
export default function Home() {
  return <h1>Startseite (Pages Router)</h1>;
}
```

**App Router (`app/`):**

```js
// app/page.js
export default function Home() {
  return <h1>Startseite (App Router)</h1>;
}

// app/dashboard/layout.js → Layout für alle Unterseiten
export default function DashboardLayout({ children }) {
  return (
    <section>
      <h2>Dashboard</h2>
      {children}
    </section>
  )
}
```

---

### **Zusammenfassung:**

* **Pages Router (`pages/`)**: Klassisch, stabil, einfacher Einstieg, aber limitiert (kein echtes Layout-System).
* **App Router (`app/`)**: Modern, basiert auf React Server Components, unterstützt verschachtelte Layouts, Streaming und bessere Performance.

📖 Quelle: [Next.js Docs – App Router vs. Pages Router](https://nextjs.org/docs/app/building-your-application/routing#the-app-router)

---

  **[⬆ Наверх](#top)**

6. ### <a name="6"></a> Was ist der App Router (Next.js 13+) und wie unterscheidet er sich vom Pages Router?

**App Router (Next.js 13+)**
Der **App Router** ist das neue Routing-System in Next.js (seit Version 13), das auf **React Server Components (RSC)** basiert. Er erlaubt **verschachtelte Layouts**, **Streaming**, **Suspense** und ein moderneres Datenfetching.

---

### **Unterschiede zum Pages Router**

| Kriterium         | Pages Router (`pages/`)                                                   | App Router (`app/`)                                                  |
| ----------------- | ------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| **Architektur**   | Klassisches React mit CSR, SSR, SSG, ISR                                  | React Server Components (RSC)                                        |
| **Routing**       | Jede Datei = Route, nur `_app.js` & `_document.js` für globale Strukturen | `page.js`, `layout.js`, `loading.js`, `error.js` für jede Route      |
| **Layouts**       | Nur global via `_app.js`                                                  | Verschachtelte Layouts pro Ordner möglich                            |
| **Datenfetching** | `getServerSideProps`, `getStaticProps`, `getStaticPaths`                  | Direkt mit `fetch()` im Server Component (kein spezielles API nötig) |
| **Rendering**     | SSR, SSG, ISR, CSR                                                        | SSR, SSG, ISR, CSR + Streaming & Suspense                            |
| **API-Routen**    | `pages/api/*`                                                             | `app/api/*/route.js`                                                 |
| **Performance**   | Mehr Client-JavaScript notwendig                                          | Weniger Client-JavaScript, schneller durch RSC                       |
| **Status**        | Stabil, weit verbreitet                                                   | Zukunftsgerichtet, Standard seit Next.js 13                          |

---

### **Code-Beispiele**

**Pages Router (`pages/`):**

```js
// pages/index.js
export default function Home() {
  return <h1>Startseite mit Pages Router</h1>;
}

// Datenfetching mit getServerSideProps
export async function getServerSideProps() {
  const res = await fetch("https://api.example.com/data");
  const data = await res.json();
  return { props: { data } };
}
```

**App Router (`app/`):**

```js
// app/page.js
export default function Home() {
  return <h1>Startseite mit App Router</h1>;
}

// app/dashboard/page.js
export default function Dashboard() {
  return <p>Dashboard-Inhalt</p>;
}

// app/dashboard/layout.js
export default function DashboardLayout({ children }) {
  return (
    <section>
      <h2>Dashboard Layout</h2>
      {children}
    </section>
  );
}
```

---

**Zusammenfassung:**
Der **App Router** bringt mit Next.js 13 ein modernes, komponentenbasiertes Routing, das **Server Components**, **verschachtelte Layouts**, **Streaming** und ein vereinfachtes Datenfetching nutzt. Er unterscheidet sich vom klassischen **Pages Router**, indem er mehr **Flexibilität, bessere Performance und eine feinere Strukturierung** ermöglicht.

📖 Quelle: [Next.js Docs – App Router](https://nextjs.org/docs/app/building-your-application/routing#the-app-router)

---

  **[⬆ Наверх](#top)**

7. ### <a name="7"></a> Was ist Server-Side Rendering (SSR)?

**Definition:**
**Server-Side Rendering (SSR)** bedeutet, dass eine Seite **auf dem Server gerendert** wird, bevor sie an den Browser geschickt wird. Der Client erhält also bereits **fertiges HTML**, das sofort angezeigt werden kann. Erst danach wird das React-JavaScript gebunden (**Hydration**), um Interaktivität zu ermöglichen.

---

### **Vorteile von SSR**

* **SEO-freundlich**: Suchmaschinen sehen direkt fertigen Inhalt.
* **Schnellere Time-to-First-Byte (TTFB)** für den Nutzer.
* **Datenaktualität**: Inhalte werden bei jedem Request neu generiert.

---

### **Nachteile von SSR**

* Höhere **Server-Last**, da bei jedem Request Rendering stattfindet.
* Kann langsamer sein als **Static Site Generation (SSG)**, wenn viele gleichartige Anfragen kommen.

---

### **Beispiel – SSR in Next.js (Pages Router):**

```js
// pages/index.js
export default function Home({ data }) {
  return (
    <main>
      <h1>Server-Side Rendering</h1>
      <p>Daten: {data.message}</p>
    </main>
  );
}

export async function getServerSideProps() {
  // Wird bei jedem Request aufgerufen
  const res = await fetch("https://api.example.com/message");
  const data = await res.json();

  return { props: { data } };
}
```

### **Beispiel – SSR im App Router (Next.js 13+):**

```js
// app/page.js
export default async function Home() {
  const res = await fetch("https://api.example.com/message", { cache: "no-store" });
  const data = await res.json();

  return (
    <main>
      <h1>Server-Side Rendering (App Router)</h1>
      <p>Daten: {data.message}</p>
    </main>
  );
}
```

* `cache: "no-store"` erzwingt frisches Laden bei jedem Request → SSR.

---

**Zusammenfassung:**
SSR bedeutet, dass eine Seite **bei jeder Anfrage auf dem Server gerendert** wird. Vorteil: **aktuelle Inhalte und gute SEO**, Nachteil: **höhere Server-Last**.

📖 Quelle: [Next.js Docs – Data Fetching](https://nextjs.org/docs/app/building-your-application/data-fetching/fetching)

---

  **[⬆ Наверх](#top)**

8. ### <a name="8"></a> Was ist Static Site Generation (SSG)?

**Definition:**
**Static Site Generation (SSG)** bedeutet, dass Seiten **zur Build-Zeit** (also beim Deployment) einmalig **als statisches HTML** erzeugt werden. Diese Dateien werden dann **direkt vom CDN oder Server ausgeliefert**, ohne dass der Server bei jedem Request erneut rendern muss.

---

### **Vorteile von SSG**

* **Sehr schnelle Ladezeiten** durch statische Auslieferung.
* **Hohe Skalierbarkeit**, da kein Server-Rendering pro Request nötig ist.
* **Kosteneffizient**, da Seiten aus Cache/CDN geliefert werden können.

---

### **Nachteile von SSG**

* Inhalte sind **nicht dynamisch aktuell** (nur so aktuell wie der letzte Build).
* Bei häufig wechselnden Daten ist ein Rebuild erforderlich → kann teuer/langsam sein.

---

### **Beispiel – SSG in Next.js (Pages Router):**

```js
// pages/index.js
export default function Home({ data }) {
  return (
    <main>
      <h1>Static Site Generation</h1>
      <p>Daten: {data.message}</p>
    </main>
  );
}

export async function getStaticProps() {
  // Wird nur einmal bei Build-Time ausgeführt
  const res = await fetch("https://api.example.com/message");
  const data = await res.json();

  return { props: { data } };
}
```

---

### **Beispiel – SSG im App Router (Next.js 13+):**

```js
// app/page.js
export default async function Home() {
  // Standardmäßig: fetch wird bei Build-Time ausgeführt (SSG)
  const res = await fetch("https://api.example.com/message");
  const data = await res.json();

  return (
    <main>
      <h1>Static Site Generation (App Router)</h1>
      <p>Daten: {data.message}</p>
    </main>
  );
}
```

* **Default-Verhalten** von `fetch()` im App Router = **SSG mit Caching** (`force-cache`).

---

**Zusammenfassung:**
SSG bedeutet, dass Seiten **einmalig zur Build-Zeit generiert** und dann **als statische Dateien ausgeliefert** werden. Vorteil: **extrem schnell und skalierbar**, Nachteil: **weniger dynamisch**.

📖 Quelle: [Next.js Docs – Static Rendering](https://nextjs.org/docs/app/building-your-application/rendering/static-and-dynamic-rendering)

---

  **[⬆ Наверх](#top)**

9. ### <a name="9"></a> Was ist Client-Side Rendering (CSR)?

**Definition:**
**Client-Side Rendering (CSR)** bedeutet, dass eine Anwendung **im Browser gerendert** wird. Der Server liefert nur ein minimales HTML-Grundgerüst (`<div id="root"></div>`), und der gesamte Inhalt wird **per JavaScript auf dem Client erzeugt**. React mountet die Komponenten nach dem Laden und macht die Seite interaktiv.

---

### **Vorteile von CSR**

* Sehr **dynamische User Experience** (Single Page Applications, SPAs).
* Weniger Last auf dem Server, da Rendering komplett im Browser passiert.
* Gute Grundlage für interaktive Dashboards oder Apps mit vielen Client-States.

---

### **Nachteile von CSR**

* **Schlechtere SEO**, da Suchmaschinen beim ersten Request nur ein leeres HTML sehen.
* **Längere Time-to-First-Contentful-Paint (FCP)** → der Nutzer sieht erst etwas, wenn das JS geladen und ausgeführt wurde.
* Schlechtere Performance auf langsamen Geräten oder bei schwacher Internetverbindung.

---

### **Beispiel – CSR in Next.js**

Next.js rendert standardmäßig serverseitig (SSR/SSG).
CSR wird genutzt, wenn man **dynamische Daten erst nach Page Load** im Browser holt, z. B. mit `useEffect()`.

```js
// app/page.js
"use client"; // macht die Komponente zu einer Client Component

import { useEffect, useState } from "react";

export default function ClientPage() {
  const [data, setData] = useState(null);

  useEffect(() => {
    // Daten werden nur im Browser geladen
    fetch("/api/message")
      .then(res => res.json())
      .then(data => setData(data));
  }, []);

  return (
    <main>
      <h1>Client-Side Rendering</h1>
      <p>{data ? data.message : "Lade Daten..."}</p>
    </main>
  );
}
```

* Hier wird das HTML initial leer ausgeliefert, der Inhalt erscheint erst nach JS-Ausführung.

---

**Zusammenfassung:**
CSR bedeutet, dass das Rendering **vollständig im Browser** passiert. Vorteil: **dynamische, interaktive Apps**, Nachteil: **schlechtere SEO und längere Ladezeiten**.

📖 Quelle: [Next.js Docs – Client Components](https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns#using-client-components)

---

  **[⬆ Наверх](#top)**

10. ### <a name="10"></a> Was ist Incremental Static Regeneration (ISR)?

**Definition:**
**Incremental Static Regeneration (ISR)** ist eine Rendering-Strategie von Next.js, die **statische Seiten** (wie bei SSG) erzeugt, diese aber **inkrementell und zeitgesteuert aktualisieren** kann. Dadurch erhält man die Performance von SSG **plus** die Möglichkeit, Inhalte regelmäßig zu regenerieren, ohne die gesamte App neu zu deployen.

---

### **Wie funktioniert ISR?**

* Seite wird beim **Build** statisch erzeugt.
* Bei der ersten Anfrage nach Ablauf einer definierten Zeit (`revalidate`) wird die Seite im Hintergrund **neu generiert**.
* Nutzer bekommen bis dahin die alte Seite, danach wird die neue Version automatisch ausgeliefert.

---

### **Vorteile von ISR**

* **Performance von SSG** + **aktuelle Inhalte**.
* Kein vollständiges Rebuild bei jeder Datenänderung nötig.
* Sehr **skalierbar** für große Webseiten mit vielen Seiten (z. B. Blogs, Shops).

---

### **Beispiel – ISR im Pages Router:**

```js
// pages/index.js
export default function Home({ data }) {
  return (
    <main>
      <h1>Incremental Static Regeneration</h1>
      <p>Daten: {data.message}</p>
    </main>
  );
}

export async function getStaticProps() {
  const res = await fetch("https://api.example.com/message");
  const data = await res.json();

  return {
    props: { data },
    revalidate: 10, // Seite wird alle 10 Sekunden im Hintergrund regeneriert
  };
}
```

---

### **Beispiel – ISR im App Router (Next.js 13+):**

```js
// app/page.js
export default async function Home() {
  const res = await fetch("https://api.example.com/message", { next: { revalidate: 10 } });
  const data = await res.json();

  return (
    <main>
      <h1>ISR mit App Router</h1>
      <p>Daten: {data.message}</p>
    </main>
  );
}
```

* `next: { revalidate: 10 }` = Seite wird alle **10 Sekunden neu generiert**.

---

**Zusammenfassung:**
ISR kombiniert die Vorteile von **SSG (Performance, Caching)** und **SSR (aktuelle Daten)**, indem statische Seiten **zeitgesteuert inkrementell regeneriert** werden.

📖 Quelle: [Next.js Docs – ISR](https://nextjs.org/docs/app/building-your-application/data-fetching/fetching#revalidating-data)

---

  **[⬆ Наверх](#top)**

11. ### <a name="11"></a> Wann sollte man SSR, SSG und ISR verwenden?

**Wann welche Rendering-Strategie sinnvoll ist:**

---

### **Server-Side Rendering (SSR)**

**Wann verwenden?**

* Wenn Inhalte **bei jedem Request aktuell** sein müssen.
* Bei **personalisierten Daten** (z. B. Nutzer-Dashboards, Authentifizierung).
* Wenn SEO wichtig ist und Daten dynamisch vom Server kommen.

**Beispiele:**

* E-Commerce mit ständig wechselnden Preisen
* Nutzerprofile, die individuelle Daten anzeigen
* News-Portale mit Live-Inhalten

---

### **Static Site Generation (SSG)**

**Wann verwenden?**

* Wenn Inhalte **selten oder gar nicht geändert** werden.
* Für **SEO-optimierte Seiten mit statischem Content**.
* Ideal für **kleine bis mittlere Websites** mit vordefinierten Inhalten.

**Beispiele:**

* Marketing-Seiten
* Dokumentationen
* Landing Pages

---

### **Incremental Static Regeneration (ISR)**

**Wann verwenden?**

* Wenn Inhalte **häufig, aber nicht in Echtzeit** aktualisiert werden.
* Für große Seitenmengen, bei denen ein kompletter Rebuild zu teuer wäre.
* Gute Balance zwischen **Performance (SSG)** und **Aktualität (SSR)**.

**Beispiele:**

* Blogs, bei denen neue Artikel im Hintergrund aktualisiert werden
* Produktseiten in einem Online-Shop
* Verzeichnis-Seiten (z. B. Immobilien, Jobangebote)

---

### **Vergleichs-Tabelle**

| Strategie | Generierung                           | Aktualität                    | Performance          | Typische Nutzung                      |
| --------- | ------------------------------------- | ----------------------------- | -------------------- | ------------------------------------- |
| **SSR**   | Bei **jedem Request**                 | Sehr hoch                     | Mittel (Server-Last) | Personalisierte & dynamische Seiten   |
| **SSG**   | **Build-Time**                        | Niedrig (nur bei neuem Build) | Sehr hoch            | Statische Inhalte (Landing, Docs)     |
| **ISR**   | Build-Time + **Revalidate-Intervall** | Mittel bis hoch               | Sehr hoch            | Viele Seiten mit regelmäßigen Updates |

---

**Zusammenfassung:**

* **SSR:** Echtzeitdaten, personalisierte Inhalte.
* **SSG:** Statischer, seltener Content.
* **ISR:** Dynamisch, aber zeitgesteuert aktualisiert – ideal für große Projekte mit häufigem Content-Update.

📖 Quelle: [Next.js Docs – Rendering](https://nextjs.org/docs/app/building-your-application/rendering)

---

  **[⬆ Наверх](#top)**

12. ### <a name="12"></a> Was macht der Befehl npx create-next-app?

**Definition:**
Der Befehl **`npx create-next-app`** erstellt ein **neues Next.js-Projekt** mit allen notwendigen Abhängigkeiten, Ordnerstrukturen und einer vorkonfigurierten Entwicklungsumgebung. Er ist das **offizielle CLI-Werkzeug** zum Starten eines Next.js-Projekts.

---

### **Funktionen von `create-next-app`**

* Erstellt automatisch eine Projektstruktur:

  * `app/` oder `pages/` (je nach gewähltem Router)
  * `public/` für statische Dateien
  * `next.config.js` für Konfiguration
* Installiert alle nötigen Pakete:

  * `react`, `react-dom`, `next`
* Integriert **TypeScript**, **ESLint**, **Tailwind CSS** oder andere Tools (optional).
* Richtet **Hot Reloading** und ein lokales Dev-Server-Skript (`npm run dev`) ein.

---

### **Verwendung**

```bash
npx create-next-app@latest my-app
```

* Erstellt ein neues Projekt im Ordner `my-app`.
* Fragt interaktiv ab:

  * TypeScript verwenden?
  * ESLint aktivieren?
  * Tailwind CSS integrieren?
  * App Router oder Pages Router nutzen?
  * Import alias `@/*` einrichten?

---

### **Projekt starten**

```bash
cd my-app
npm run dev
```

→ Lokaler Dev-Server läuft standardmäßig unter `http://localhost:3000`.

---

**Zusammenfassung:**
`npx create-next-app` ist das CLI-Tool, um **schnell ein neues Next.js-Projekt mit vorkonfigurierter Struktur und Abhängigkeiten** aufzusetzen.

📖 Quelle: [Next.js Docs – Installation](https://nextjs.org/docs/app/getting-started/installation)

---

  **[⬆ Наверх](#top)**

13. ### <a name="13"></a> Wie funktioniert Hydration in Next.js?

**Definition:**
**Hydration** bedeutet, dass der Browser nach dem Laden einer serverseitig oder statisch gerenderten HTML-Seite das dazugehörige **React-JavaScript** lädt und die bereits gerenderte HTML-Struktur **mit interaktiver Logik „verbindet“**.
Ohne Hydration wäre die Seite nur statisches HTML – durch Hydration wird sie eine **voll funktionsfähige React-App**.

---

### **Ablauf der Hydration in Next.js**

1. **Serverseitiges Rendering (SSR/SSG/ISR):**
   Der Server erzeugt fertiges HTML und schickt es zum Client.
   → Der Nutzer sieht sofort Inhalte (**SEO + schnelle Initialanzeige**).

2. **JavaScript-Bundle laden:**
   Der Client lädt React + die Komponentenlogik (JS-Bundle).

3. **Vergleich & Verbindung:**
   React überprüft, ob die HTML-Struktur im DOM mit dem „virtuellen DOM“ übereinstimmt, und **bindet Event-Handler, State und Interaktivität**.

4. **Interaktive App:**
   Ab diesem Zeitpunkt können Nutzer mit der Seite interagieren (z. B. Klicks, Formulare, Routing).

---

### **Hydration in Next.js – Beispiel**

```js
// app/page.js (SSR oder SSG liefert HTML aus)
"use client"; // macht Komponente interaktiv (Client Component)

import { useState } from "react";

export default function Counter() {
  const [count, setCount] = useState(0);

  return (
    <main>
      <h1>Hydration Beispiel</h1>
      <p>Zähler: {count}</p>
      <button onClick={() => setCount(count + 1)}>+1</button>
    </main>
  );
}
```

* **Ohne Hydration:** Nutzer würde nur „Zähler: 0“ sehen, aber Button hätte keine Funktion.
* **Mit Hydration:** React verbindet das HTML mit JS → Button wird klickbar.

---

### **Wichtige Punkte**

* Hydration kann **verzögert oder unterbrochen** werden, wenn JS groß oder langsam ist.
* Deshalb sind in Next.js **Server Components** wichtig:

  * Sie reduzieren die JS-Menge, die hydratisiert werden muss.
  * Nur **Client Components** brauchen Hydration.

---

**Zusammenfassung:**
Hydration ist der Prozess, bei dem Next.js das bereits gerenderte HTML im Browser **mit React-JavaScript verbindet**, um Interaktivität herzustellen. Server Components reduzieren dabei die Menge an notwendiger Hydration und verbessern die Performance.

📖 Quelle: [Next.js Docs – Rendering](https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns#using-client-components)

---

  **[⬆ Наверх](#top)**

14. ### <a name="14"></a> Was bedeutet „pre-rendering“?

**Definition:**
**Pre-Rendering** bedeutet, dass Next.js die HTML-Seiten **bereits vor der Auslieferung an den Client generiert** – entweder **zur Build-Zeit** (SSG) oder **bei jedem Request** (SSR).
Im Gegensatz zu klassischem React (CRA), wo die Seite erst im Browser per CSR erzeugt wird, sehen Nutzer und Suchmaschinen bei Next.js sofort **fertiges HTML**.

---

### **Arten des Pre-Renderings in Next.js**

1. **Static Site Generation (SSG):**

   * HTML wird **zur Build-Zeit** erstellt.
   * Schnell & skalierbar, aber weniger dynamisch.

2. **Server-Side Rendering (SSR):**

   * HTML wird **bei jedem Request auf dem Server** erstellt.
   * Immer aktuelle Inhalte, aber höhere Serverlast.

3. **Incremental Static Regeneration (ISR):**

   * HTML wird **statisch erstellt und inkrementell erneuert**.
   * Kombination aus Performance und Aktualität.

---

### **Beispiel – Pre-Rendering mit SSG**

```js
// pages/index.js
export default function Home({ data }) {
  return (
    <main>
      <h1>Pre-Rendering Beispiel</h1>
      <p>Daten: {data.message}</p>
    </main>
  );
}

export async function getStaticProps() {
  const res = await fetch("https://api.example.com/message");
  const data = await res.json();

  return { props: { data } }; // Seite wird bei Build-Time gerendert
}
```

---

### **Vorteile von Pre-Rendering**

* **Bessere Performance:** Nutzer sehen sofort Inhalte, nicht erst nach JS-Ausführung.
* **SEO-Optimierung:** Suchmaschinen bekommen fertiges HTML.
* **Bessere User Experience:** Schnellere „Time-to-Content“.

---

**Zusammenfassung:**
Pre-Rendering bedeutet, dass Next.js Seiten **vorab in HTML generiert** (SSG, SSR, ISR), sodass Nutzer und Suchmaschinen sofort Inhalte sehen können. Vorteil: **schneller, SEO-freundlicher und stabiler** als reines CSR.

📖 Quelle: [Next.js Docs – Rendering](https://nextjs.org/docs/app/building-your-application/rendering)

---

  **[⬆ Наверх](#top)**

15. ### <a name="15"></a> Welche Sprachen und Technologien unterstützt Next.js out of the box?

**Sprachen und Technologien, die Next.js „out of the box“ unterstützt:**

---

### **1. JavaScript & TypeScript**

* **JavaScript (ESM)** → Standard.
* **TypeScript** wird automatisch unterstützt (keine separate Config nötig, `tsconfig.json` wird generiert).

---

### **2. React**

* Next.js basiert direkt auf **React**.
* Unterstützt **React Server Components (RSC)**, **Client Components**, **Suspense**, **Hooks**.

---

### **3. CSS & Styling**

* **Globale CSS-Dateien** (`app/globals.css`).
* **CSS-Modules** (`*.module.css`) für scoped Styles.
* **Sass/SCSS** (`*.scss`) ohne zusätzliche Config.
* Unterstützung für **PostCSS** (bereits integriert).

---

### **4. Images & Fonts**

* **`next/image`** für automatische Bildoptimierung (Resizing, Lazy Loading, CDN).
* **`next/font`** für optimierte Google Fonts und lokale Fonts.

---

### **5. Routing & Internationalisierung**

* **File-based Routing** (`app/` oder `pages/`).
* **Dynamic Routes** (`[id]`).
* **Internationalisierung (i18n)** direkt in `next.config.js`.

---

### **6. API & Backend-Funktionalität**

* **API-Routen**: `pages/api/*` oder `app/api/*/route.js`.
* Server-seitiges Datenfetching (`fetch` mit `cache`, `revalidate`, `no-store`).
* Middleware für Edge-Funktionen.

---

### **7. Deployment & Optimierungen**

* **Code-Splitting** automatisch.
* **Prefetching** von Links mit `next/link`.
* **Edge & Serverless Functions** (z. B. bei Vercel).

---

### **Beispiel – TypeScript + SCSS**

```tsx
// app/page.tsx
import styles from "./page.module.scss";

export default function Home() {
  return (
    <main className={styles.container}>
      <h1>Next.js unterstützt TypeScript + SCSS!</h1>
    </main>
  );
}
```

```scss
/* app/page.module.scss */
.container {
  color: blue;
  font-weight: bold;
}
```

---

**Zusammenfassung:**
Next.js unterstützt **JavaScript, TypeScript, React, CSS/SCSS, CSS-Modules, PostCSS, Bild- und Font-Optimierung, API-Routen und i18n** sofort ohne zusätzliche Konfiguration.

📖 Quelle: [Next.js Docs – Getting Started](https://nextjs.org/docs/app/getting-started/installation)

---

  **[⬆ Наверх](#top)**

16. ### <a name="16"></a> Wie richtet man TypeScript in Next.js ein?

**Kurzantwort:**
TypeScript ist in Next.js **eingebaut**. Neu: direkt mit `create-next-app --ts`. Bestehende Projekte: eine Datei in `.ts/.tsx` umbenennen und `next dev` starten – Next.js installiert TS-Deps, erzeugt `tsconfig.json` und `next-env.d.ts` automatisch. ([nextjs.org][1])

---

### Neues Projekt (App Router, TypeScript)

```bash
npx create-next-app@latest my-app --ts --app
cd my-app
npm run dev
```

* `--ts` initialisiert TypeScript (seit Next.js 15 standardmäßig aktivierbar über Flag/Prompt). ([nextjs.org][1])

---

### TypeScript zu bestehendem Projekt hinzufügen

1. Eine Datei zu `.ts`/`.tsx` umbenennen (z. B. `app/page.tsx`).
2. `next dev` bzw. `next build` ausführen → Next.js installiert TS-Pakete und legt **`tsconfig.json`** (empfohlene Defaults) an; **`next-env.d.ts`** wird erzeugt. ([nextjs.org][2])

---

### Minimales Beispiel (App Router, TSX)

```js
// app/page.tsx
export default function Home(): JSX.Element {
  return (
    <main>
      <h1>Next.js + TypeScript</h1>
    </main>
  );
}
```

```js
// app/api/hello/route.ts  – typisierte Route (Edge/Node je nach Runtime)
import { NextResponse } from 'next/server';

export function GET(): NextResponse {
  return NextResponse.json({ ok: true });
}
```

---

### Hinweise

* `create-next-app` fragt optional nach **ESLint**, **Tailwind**, **App Router**, **Import-Alias (`@/*`)**. ([nextjs.org][1])
* TS-Konfiguration wird automatisch empfohlen; bestehende `jsconfig`-`paths` ggf. in `tsconfig` übernehmen. ([nextjs.org][2])

---

**Zusammenfassung:**

* Neu: `create-next-app --ts` oder Prompt verwenden.
* Bestehend: Datei umbenennen → `next dev` → Next.js richtet TS auto. ein (`tsconfig.json`, `next-env.d.ts`).
* TS funktioniert nahtlos mit App Router (Server/Client Components, Route Handler). ([nextjs.org][3])

📖 Weiterlesen: [Installation & Setup](https://nextjs.org/docs/app/getting-started/installation) ([nextjs.org][3])

[1]: https://nextjs.org/docs/pages/api-reference/cli/create-next-app "CLI: create-next-app CLI | Next.js"
[2]: https://nextjs.org/docs/14/app/building-your-application/configuring/typescript?utm_source=chatgpt.com "Configuring: TypeScript"
[3]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"

  **[⬆ Наверх](#top)**

17. ### <a name="17"></a> Was machen next dev, next build, next start?

**Die drei wichtigsten Next.js-Befehle:**

---

### **1. `next dev`**

* Startet den **Entwicklungsserver** (`localhost:3000` standardmäßig).
* Features: **Hot Reloading**, **Fehlermeldungen in Echtzeit**, **schnelles Feedback**.
* Nutzt **nicht optimierten Code**, sondern schnelle Builds für die Entwicklung.

**Beispiel:**

```bash
npm run dev
# ruft intern `next dev` auf
```

---

### **2. `next build`**

* Erstellt eine **optimierte Produktionsversion** der App.
* Wandelt Seiten in **SSG, SSR, ISR** entsprechend der Konfiguration um.
* Führt **Linting, TypeScript-Checks, Code-Splitting, Minifizierung** durch.
* Output wird in `.next/` gespeichert.

**Beispiel:**

```bash
npm run build
# ruft intern `next build` auf
```

---

### **3. `next start`**

* Startet einen **Produktionsserver**, der den zuvor erstellten Build ausliefert.
* Nutzt die Dateien aus `.next/`.
* Ohne `next build` vorher funktioniert `next start` nicht.

**Beispiel:**

```bash
npm run start
# ruft intern `next start` auf
```

---

### **Zusammenfassung:**

* **`next dev`** → Entwicklungsmodus mit Hot Reload.
* **`next build`** → Produktions-Build erstellen.
* **`next start`** → Produktionsserver mit dem Build starten.

📖 Quelle: [Next.js Docs – CLI](https://nextjs.org/docs/app/api-reference/cli)

---

  **[⬆ Наверх](#top)**

18. ### <a name="18"></a> Welche Einschränkungen hat Next.js?

**Einschränkungen von Next.js:**

---

### **1. Komplexität bei Projekten**

* Mehr Lernaufwand als bei reinem React (z. B. SSR, SSG, ISR, App Router vs. Pages Router).
* Entwickler müssen Rendering-Strategien verstehen und bewusst einsetzen.

---

### **2. Build- und Deployment-Zeit**

* **SSG/ISR** bei sehr großen Projekten (z. B. E-Commerce mit 100k+ Seiten) → lange Build-Zeiten.
* Workaround: ISR oder On-Demand-Revalidation, aber Setup komplexer.

---

### **3. Server-Komponenten (App Router)**

* **Noch nicht alle React-Ökosystem-Libraries** funktionieren problemlos mit Server Components.
* Client/Server-Trennung kann zu Missverständnissen führen („`use client`“-Direktive).

---

### **4. Vendor-Lock-in Tendenz**

* Next.js ist stark auf **Vercel** optimiert (Edge Functions, Image Optimization, Middleware).
* Bei anderen Hostings (AWS, Netlify) muss teilweise nachkonfiguriert werden.

---

### **5. API-Routen**

* Gut für kleine Backends, aber **nicht geeignet für komplexe Backend-Systeme**.
* Für umfangreiche Business-Logik braucht man meist ein separates Backend (z. B. NestJS, Express, FastAPI).

---

### **6. SEO und Performance**

* **SSR** kann die Time-to-First-Byte (TTFB) erhöhen → langsamer bei hoher Serverlast.
* **CSR-Komponenten** brauchen weiterhin Hydration → Performance-Kosten auf dem Client.

---

### **7. Edge Cases**

* **Internationalisierung (i18n)** ist integriert, aber oft einfacher mit Libraries (z. B. `next-i18next`).
* **Image-Optimierung** funktioniert nicht überall (z. B. bei Self-Hosting ohne spezielle Loader).

---

**Zusammenfassung:**
Next.js bringt viel Komfort (SSR, SSG, ISR, API-Routen, App Router), hat aber **Einschränkungen** bei sehr großen Projekten (Build-Zeit), **Kompatibilität** (Server Components), **Flexibilität** (Hosting außerhalb Vercel) und bei **umfangreicher Backend-Logik**.

📖 Quelle: [Next.js Docs – Limitations](https://nextjs.org/docs/app/building-your-application/routing#limitations)

---

  **[⬆ Наверх](#top)**

19. ### <a name="19"></a> Wie funktioniert das Routing in Next.js?

**Routing in Next.js** basiert auf dem Prinzip des **file-based routing**: Jede Datei im `pages/`- oder `app/`-Verzeichnis wird automatisch zu einer Route.

---

### **1. App Router (ab Next.js 13)**

* Struktur: `app/`
* Besondere Dateien:

  * `page.js` → definiert eine Seite
  * `layout.js` → Layout für eine Route und ihre Kind-Routen
  * `loading.js` → Ladezustand für Suspense
  * `error.js` → Fehlerbehandlung pro Route
* **Dynamische Routen:** `[id]` (z. B. `app/blog/[id]/page.js`)
* **Verschachtelung:** Unterordner erzeugen automatisch **Nested Routes**

**Beispiel:**

```js
// app/page.js → /
export default function Home() {
  return <h1>Startseite</h1>;
}

// app/about/page.js → /about
export default function About() {
  return <h1>Über uns</h1>;
}

// app/blog/[id]/page.js → /blog/123
export default function BlogPost({ params }) {
  return <h1>Blogpost: {params.id}</h1>;
}
```

---

### **2. Pages Router (klassisch bis Next.js 12, weiterhin nutzbar)**

* Struktur: `pages/`
* Jede Datei = Route
* Dynamische Routen über `[param].js`
* API-Routen über `pages/api/*`

**Beispiel:**

```js
// pages/index.js → /
export default function Home() {
  return <h1>Startseite</h1>;
}

// pages/about.js → /about
export default function About() {
  return <h1>Über uns</h1>;
}

// pages/blog/[id].js → /blog/123
export default function BlogPost({ params }) {
  return <h1>Blogpost</h1>;
}
```

---

### **3. Navigation**

* Mit `next/link` für interne Links (automatisches Prefetching).
* Mit `next/navigation` (App Router) für programmatic navigation (`useRouter`).

```js
// app/page.js
import Link from "next/link";

export default function Home() {
  return (
    <main>
      <h1>Startseite</h1>
      <Link href="/about">Über uns</Link>
    </main>
  );
}
```

---

**Zusammenfassung:**
Next.js-Routing basiert auf der **Dateistruktur** (`app/` oder `pages/`).

* **App Router:** modern, unterstützt verschachtelte Layouts, Server Components, Streaming.
* **Pages Router:** klassisch, einfach, weiterhin stabil.
  Navigation erfolgt mit **`next/link`** oder Hooks (`useRouter`).

📖 Quelle: [Next.js Docs – Routing](https://nextjs.org/docs/app/building-your-application/routing)

---

  **[⬆ Наверх](#top)**

20. ### <a name="20"></a> Wie erstellt man dynamische Routen ([id].tsx)?

**Dynamische Routen – Grundprinzip**
Ein **dynamisches Segment** entsteht durch eckige Klammern im Dateinamen, z. B. `[id]`. Der Wert wird aus der URL gelesen und in der Seite verfügbar gemacht. ([nextjs.org][1])

---

### App Router (`app/`, Next.js 13+)

**1) Einfache dynamische Route**

```js
// app/products/[id]/page.js  → /products/123
import { notFound } from "next/navigation";

export default async function ProductPage({ params }) {
  const { id } = params; // "123"
  const res = await fetch(`https://api.example.com/products/${id}`, { cache: "no-store" });
  if (!res.ok) notFound();
  const product = await res.json();
  return <h1>{product.name}</h1>;
}
```

* `params` kommt als Prop in Server Components an. `cache: "no-store"` erzwingt SSR. ([nextjs.org][1])

**2) Statisches Vor-Rendern ausgewählter IDs (SSG/ISR)**

```js
// app/products/[id]/page.js
export async function generateStaticParams() {
  const ids = await fetch("https://api.example.com/products")
    .then(r => r.json())
    .then(list => list.slice(0, 50).map(p => ({ id: String(p.id) }))); // Beispiel
  return ids; // → [{ id: "1" }, { id: "2" }, ...]
}
```

* `generateStaticParams()` erzeugt Build-Time-Seiten für die angegebenen Parameter. Mit `export const revalidate = 60` aktivierst du ISR. ([nextjs.org][2])

**3) Parameter in Client Components**

```js
// app/products/[id]/client-info.js
"use client";
import { useParams } from "next/navigation";

export default function ClientInfo() {
  const { id } = useParams(); // string | string[]
  return <small>Produkt-ID: {id}</small>;
}
```

* `useParams()` liefert die ausgefüllten dynamischen Segmente. ([nextjs.org][3])

**4) Catch-all & optionale Catch-all**

* `app/docs/[...slug]/page.js`  → `/docs/a/b/c` → `params.slug` ist `string[]`.
* `app/docs/[[...slug]]/page.js` → optional, `/docs` funktioniert ebenfalls. ([nextjs.org][1])

---

### Pages Router (`pages/`)

**1) Einfache dynamische Route (SSR/CSR/SSG möglich)**

```js
// pages/products/[id].tsx
import type { GetStaticProps, GetStaticPaths, InferGetStaticPropsType } from "next";

export default function Product({ product }: InferGetStaticPropsType<typeof getStaticProps>) {
  return <h1>{product.name}</h1>;
}

export const getStaticPaths: GetStaticPaths = async () => {
  const list = await fetch("https://api.example.com/products").then(r => r.json());
  return {
    paths: list.slice(0, 50).map((p: any) => ({ params: { id: String(p.id) } })),
    fallback: "blocking", // ISR-kompatibel
  };
};

export const getStaticProps: GetStaticProps = async ({ params }) => {
  const res = await fetch(`https://api.example.com/products/${params!.id}`);
  const product = await res.json();
  return { props: { product }, revalidate: 60 }; // ISR
};
```

* Dynamische Seiten + SSG benötigen `getStaticPaths`. `revalidate` aktiviert ISR. ([nextjs.org][4])

**2) Catch-all im Pages Router**

* `pages/posts/[...id].js` fängt beliebig tiefe Segmente als Array ab. ([nextjs.org][5])

---

### Navigation zu dynamischen Routen

```js
// App Router
import Link from "next/link";
export default function List({ items }) {
  return items.map(p => <Link key={p.id} href={`/products/${p.id}`}>{p.name}</Link>);
}
```

* `<Link />` prefetched standardmäßig (optimiert Navigation). ([nextjs.org][6])

---

**Zusammenfassung**

* **Erzeugen:** `[id]` im Dateinamen (App: `app/…/page.js`, Pages: `pages/… .js`).
* **App Router:** `params`-Prop, `generateStaticParams()` für SSG, `revalidate` für ISR, `useParams()` in Clients.
* **Pages Router:** `getStaticPaths` + `getStaticProps` für SSG/ISR.
* **Varianten:** Catch-all `[...slug]`, optional `[[...slug]]`.
  Quellen: [Dynamic Route Segments (App)](https://nextjs.org/docs/app/api-reference/file-conventions/dynamic-routes), [useParams](https://nextjs.org/docs/app/api-reference/functions/use-params), [getStaticPaths (Pages)](https://nextjs.org/docs/pages/building-your-application/data-fetching/get-static-paths), [Linking & Navigating](https://nextjs.org/docs/app/getting-started/linking-and-navigating). ([nextjs.org][1])

[1]: https://nextjs.org/docs/app/api-reference/file-conventions/dynamic-routes?utm_source=chatgpt.com "Dynamic Route Segments"
[2]: https://nextjs.org/docs/app/api-reference/functions/generate-static-params?utm_source=chatgpt.com "Functions: generateStaticParams"
[3]: https://nextjs.org/docs/app/api-reference/functions/use-params?utm_source=chatgpt.com "Functions: useParams"
[4]: https://nextjs.org/docs/pages/building-your-application/data-fetching/get-static-paths?utm_source=chatgpt.com "Data Fetching: getStaticPaths"
[5]: https://nextjs.org/learn/pages-router/dynamic-routes-dynamic-routes-details?utm_source=chatgpt.com "Pages Router: Dynamic Routes Details"
[6]: https://nextjs.org/docs/app/getting-started/linking-and-navigating?utm_source=chatgpt.com "Getting Started: Linking and Navigating"

  **[⬆ Наверх](#top)**

21. ### <a name="21"></a> Wie funktionieren Catch-All-Routen ([...slug].tsx)?

**Definition:**
Catch-All-Routen in Next.js fangen **mehrere URL-Segmente** gleichzeitig ab. Statt nur einen Parameter wie `[id]`, kann man mit `[...slug]` oder `[[...slug]]` **beliebig viele Segmente** in einem Array verarbeiten.

---

### **1. App Router (`app/`)**

**Beispiel:**

```js
// app/docs/[...slug]/page.js
export default function DocsPage({ params }) {
  // /docs/a/b/c  → params.slug = ["a", "b", "c"]
  return (
    <main>
      <h1>Docs Route</h1>
      <p>Slug: {params.slug.join(" / ")}</p>
    </main>
  );
}
```

* `/docs/installation` → `params.slug = ["installation"]`
* `/docs/react/hooks` → `params.slug = ["react", "hooks"]`

👉 Optional Catch-All:

```js
// app/docs/[[...slug]]/page.js
// erlaubt auch /docs ohne weitere Segmente
```

* `/docs` → `params.slug = undefined`
* `/docs/react` → `params.slug = ["react"]`

---

### **2. Pages Router (`pages/`)**

**Beispiel:**

```js
// pages/docs/[...slug].tsx
import { GetStaticPaths, GetStaticProps } from "next";

export default function Docs({ slug }: { slug: string[] }) {
  return <h1>Slug: {slug.join(" / ")}</h1>;
}

export const getStaticPaths: GetStaticPaths = async () => {
  return {
    paths: [
      { params: { slug: ["installation"] } },
      { params: { slug: ["react", "hooks"] } }
    ],
    fallback: "blocking"
  };
};

export const getStaticProps: GetStaticProps = async ({ params }) => {
  return { props: { slug: params!.slug as string[] } };
};
```

---

### **Einsatzmöglichkeiten**

* Dokumentationen mit tiefen Hierarchien (`/docs/react/hooks/useEffect`)
* Shops mit Kategorien & Unterkategorien (`/shop/clothes/men/shirts`)
* SEO-freundliche URLs ohne manuelles Definieren aller Ebenen

---

**Zusammenfassung:**

* `[...slug]` → fängt beliebig viele Segmente als **Array** ab.
* `[[...slug]]` → wie `[...slug]`, aber auch ohne Segmente gültig.
* Im **App Router** via `params.slug`, im **Pages Router** via `params.slug` in `getStaticProps`.

📖 Quelle: [Next.js Docs – Dynamic Routes](https://nextjs.org/docs/app/building-your-application/routing/dynamic-routes#catch-all-segments)

---

  **[⬆ Наверх](#top)**

22. ### <a name="22"></a> Was sind optionale Catch-All-Routen ([[...slug]])?

**Definition:**
Optionale Catch-All-Routen (`[[...slug]]`) sind eine Variante der Catch-All-Routen (`[...slug]`), bei der das Vorhandensein von Segmenten **optional** ist.
Das bedeutet: Die Route funktioniert **sowohl mit als auch ohne zusätzliche Segmente**.

---

### **1. App Router (`app/`)**

```js
// app/docs/[[...slug]]/page.js
export default function DocsPage({ params }) {
  // params.slug ist entweder undefined oder ein Array
  return (
    <main>
      <h1>Docs</h1>
      <p>Slug: {params.slug ? params.slug.join(" / ") : "Root-Seite"}</p>
    </main>
  );
}
```

* `/docs` → `params.slug = undefined`
* `/docs/react` → `params.slug = ["react"]`
* `/docs/react/hooks` → `params.slug = ["react", "hooks"]`

---

### **2. Pages Router (`pages/`)**

```js
// pages/docs/[[...slug]].tsx
import { GetStaticProps } from "next";

export default function Docs({ slug }: { slug?: string[] }) {
  return <h1>{slug ? slug.join(" / ") : "Docs Root"}</h1>;
}

export const getStaticProps: GetStaticProps = async ({ params }) => {
  return { props: { slug: params?.slug as string[] | undefined } };
};
```

* `/docs` → `slug = undefined`
* `/docs/intro/getting-started` → `slug = ["intro", "getting-started"]`

---

### **Einsatzmöglichkeiten**

* **Docs-Systeme**: `/docs` als Einstieg + Unterseiten `/docs/...`
* **Kategorie-Seiten**: `/shop` und `/shop/clothes/men/shirts`
* **Flexibles URL-Design**, wenn Wurzelroute + beliebig viele Unterebenen unterstützt werden sollen

---

**Zusammenfassung:**

* **`[...slug]`** → benötigt mindestens ein Segment (`/docs/react`).
* **`[[...slug]]`** → Segmente sind **optional** (`/docs` oder `/docs/react`).
* Praktisch für **Root-Seiten mit Unterrouten**, ohne separate Datei für `/docs` anlegen zu müssen.

📖 Quelle: [Next.js Docs – Catch-All Segments](https://nextjs.org/docs/app/building-your-application/routing/dynamic-routes#catch-all-segments)

---

  **[⬆ Наверх](#top)**

23. ### <a name="23"></a> Wie funktioniert Nested Routing (verschachtelte Routen)?

**Definition:**
**Nested Routing (verschachtelte Routen)** bedeutet, dass in Next.js die **Ordnerstruktur im Projekt der URL-Struktur entspricht**. Dabei können **Unterordner verschachtelte Routen** erzeugen, die automatisch **Layout-Vererbung** und **hierarchische Navigation** unterstützen.

---

## **1. App Router (`app/` – Next.js 13+)**

* Jeder **Ordner** = ein Segment der URL.
* Jede **`page.js`** = eine Seite.
* Jede **`layout.js`** = ein Layout, das **für diesen Ordner und alle Kinder gilt**.

**Beispiel:**

```
app/
 ├─ dashboard/
 │   ├─ layout.js
 │   ├─ page.js
 │   ├─ settings/
 │   │   └─ page.js
 │   └─ analytics/
 │       └─ page.js
```

**URLs:**

* `/dashboard` → `app/dashboard/page.js`
* `/dashboard/settings` → `app/dashboard/settings/page.js`
* `/dashboard/analytics` → `app/dashboard/analytics/page.js`

**Code – Layout + Nested Pages:**

```js
// app/dashboard/layout.js
export default function DashboardLayout({ children }) {
  return (
    <section>
      <h2>Dashboard Layout</h2>
      {children}
    </section>
  );
}

// app/dashboard/page.js
export default function Dashboard() {
  return <p>Dashboard Startseite</p>;
}

// app/dashboard/settings/page.js
export default function Settings() {
  return <p>Einstellungen</p>;
}
```

👉 Ergebnis: Alle Unterseiten (`/settings`, `/analytics`) nutzen das **gemeinsame Dashboard-Layout**.

---

## **2. Pages Router (`pages/`)**

* Verschachtelung funktioniert ebenfalls über **Ordnerstruktur**.
* Kein Layout-System, nur **seitenbasierte Struktur**.

**Beispiel:**

```
pages/
 ├─ dashboard/
 │   ├─ index.js        → /dashboard
 │   ├─ settings.js     → /dashboard/settings
 │   └─ analytics.js    → /dashboard/analytics
```

**Code:**

```js
// pages/dashboard/settings.js
export default function Settings() {
  return <h1>Einstellungen</h1>;
}
```

👉 Unterschied: Hier gibt es **kein automatisches Layout**, nur Seiten. Gemeinsame Elemente müssen manuell (z. B. via `_app.js`) eingebunden werden.

---

### **Vorteile von Nested Routing**

* **App Router:** Gemeinsame Layouts + logische Gruppierung der Routen.
* **Pages Router:** Einfache Struktur, aber weniger flexibel.

---

**Zusammenfassung:**

* **App Router:** Nested Routing basiert auf Ordnern, unterstützt verschachtelte Layouts, Error Boundaries, Loading States → sehr mächtig.
* **Pages Router:** Ebenfalls dateibasiert, aber ohne Layout-Vererbung – nur reine Seitenstruktur.

📖 Quelle: [Next.js Docs – Nested Routes](https://nextjs.org/docs/app/building-your-application/routing/nested-routes)

---

  **[⬆ Наверх](#top)**

24. ### <a name="24"></a> Wie übergibt man Query-Parameter in Routen?

**Definition:**
Query-Parameter sind **zusätzliche Schlüssel-Wert-Paare** in der URL, die nach einem `?` beginnen.
Beispiel:

```
/products?id=123&ref=promo
```

Hier: `id=123`, `ref=promo`.

In Next.js kann man Query-Parameter sowohl im **App Router** (`app/`) als auch im **Pages Router** (`pages/`) auslesen.

---

## **1. App Router (Next.js 13+)**

### a) Mit `useSearchParams()` (Client Component)

```js
"use client";

import { useSearchParams } from "next/navigation";

export default function Products() {
  const searchParams = useSearchParams();
  const id = searchParams.get("id"); // z.B. "123"
  const ref = searchParams.get("ref"); // z.B. "promo"

  return (
    <main>
      <h1>Produktseite</h1>
      <p>ID: {id}</p>
      <p>Ref: {ref}</p>
    </main>
  );
}
```

### b) Mit `searchParams` (Server Component)

```js
// app/products/page.js
export default function Products({ searchParams }) {
  return (
    <main>
      <h1>Produktseite</h1>
      <p>ID: {searchParams.id}</p>
      <p>Ref: {searchParams.ref}</p>
    </main>
  );
}
```

---

## **2. Pages Router**

### a) Mit `useRouter()` (Client-Side)

```js
// pages/products.js
import { useRouter } from "next/router";

export default function Products() {
  const { query } = useRouter();
  return (
    <main>
      <h1>Produktseite</h1>
      <p>ID: {query.id}</p>
      <p>Ref: {query.ref}</p>
    </main>
  );
}
```

### b) Mit SSR-Funktionen

```js
// pages/products.js
export default function Products({ id, ref }) {
  return (
    <main>
      <h1>Produktseite</h1>
      <p>ID: {id}</p>
      <p>Ref: {ref}</p>
    </main>
  );
}

export async function getServerSideProps({ query }) {
  return {
    props: {
      id: query.id || null,
      ref: query.ref || null,
    },
  };
}
```

---

## **Navigation mit Query-Params**

```js
import Link from "next/link";

export default function Home() {
  return (
    <Link href={{ pathname: "/products", query: { id: 123, ref: "promo" } }}>
      Zum Produkt 123
    </Link>
  );
}
```

➡ erzeugt URL: `/products?id=123&ref=promo`

---

**Zusammenfassung:**

* **App Router:** Query-Parameter über `searchParams` (Server Components) oder `useSearchParams()` (Client Components).
* **Pages Router:** Über `useRouter().query` oder via SSR-Funktionen (`getServerSideProps`).
* Navigation mit Query-Params geht einfach über `next/link`.

📖 Quelle: [Next.js Docs – useSearchParams](https://nextjs.org/docs/app/api-reference/functions/use-search-params)

---

  **[⬆ Наверх](#top)**

25. ### <a name="25"></a> Wie kann man Routenparameter auf dem Server abrufen?

**Serverseitiges Auslesen von Routenparametern in Next.js**

---

### **App Router (`app/`, Next.js 13+)**

**`params` und `searchParams` als Props in Server Components**

```js
// app/products/[id]/page.js  → /products/123
export default async function ProductPage({ params, searchParams }) {
  const { id } = params;              // "123"
  const { ref } = await searchParams; // Next.js ≥15: Promise (künftig Pflicht)
  // ...Server-seitiges Fetching, Rendering
  return <h1>Produkt {id} (ref={ref})</h1>;
}
```

* Dynamische Segmente werden als **`params`** übergeben (z. B. `{ id: '123' }`).
* **`searchParams`** enthält Query-Parameter (in Next.js 15 als Promise). ([nextjs.org][1])

**In `generateMetadata`/Layouts nutzbar**

```js
// app/products/[id]/page.js
export async function generateMetadata({ params }) {
  return { title: `Produkt ${params.id}` };
}
```

* **`params`** ist auch in `layout.js`, `page.js`, `generateMetadata` verfügbar. ([nextjs.org][1])

---

### **Route Handler (App Router, `app/**/route.ts`)**

```js
// app/items/[slug]/route.ts  → /items/foo
export async function GET(_req, { params }) {
  return new Response(JSON.stringify({ slug: params.slug }), {
    headers: { "content-type": "application/json" },
  });
}
```

* Der **zweite Parameter** enthält `{ params }` mit den dynamischen Segmenten. ([nextjs.org][2])

---

### **Pages Router (`pages/`)**

**SSR: `getServerSideProps`**

```js
// pages/products/[id].tsx
export default function Page({ id }: { id: string }) {
  return <h1>Produkt {id}</h1>;
}
export async function getServerSideProps({ params, query }) {
  return { props: { id: params!.id, ref: query.ref ?? null } };
}
```

* **`context.params`** enthält die dynamischen Segmente; **`context.query`** die Query-Parameter. ([nextjs.org][3])

**SSG/ISR: `getStaticPaths` + `getStaticProps`**

```js
// pages/blog/[slug].tsx
export async function getStaticPaths() {
  return { paths: [{ params: { slug: "hello" } }], fallback: "blocking" };
}
export async function getStaticProps({ params }) {
  return { props: { slug: params!.slug }, revalidate: 60 };
}
```

* Dynamische Seiten benötigen **`getStaticPaths`**; Revalidierung via **`revalidate`**. ([nextjs.org][3])

---

**Zusammenfassung**

* **App Router:** `params`/`searchParams` als Props in Server Components; Route Handler erhalten `{ params }` als 2. Argument.
* **Pages Router:** Serverseitig über `context.params`/`context.query` in `getServerSideProps` bzw. `getStaticProps`.
  Quellen: Dynamic Routes, `page.js`-Konventionen, `useSearchParams`, `getServerSideProps`, Route Handlers, sowie Installation/Getting Started. ([nextjs.org][1])

[1]: https://nextjs.org/docs/app/api-reference/file-conventions/dynamic-routes?utm_source=chatgpt.com "Dynamic Route Segments"
[2]: https://nextjs.org/docs/app/api-reference/file-conventions/route?utm_source=chatgpt.com "File-system conventions: route.js"
[3]: https://nextjs.org/docs/pages/api-reference/functions/get-server-side-props?utm_source=chatgpt.com "Functions: getServerSideProps"

  **[⬆ Наверх](#top)**

26. ### <a name="26"></a> Wie implementiert man Redirects in Next.js?

**Redirects in Next.js** können sowohl **serverseitig** (Build-Time oder Request-Time) als auch **clientseitig** erfolgen.

---

## **1. Serverseitige Redirects über `next.config.js`**

Ideal für **permanente (301)** oder **temporäre (302)** Weiterleitungen.

```js
// next.config.js
module.exports = {
  async redirects() {
    return [
      {
        source: "/old-route",
        destination: "/new-route",
        permanent: true, // 308 (SEO-freundlich, cached)
      },
      {
        source: "/blog/:id",
        destination: "/posts/:id",
        permanent: false, // 307 (nicht gecached)
      },
    ];
  },
};
```

* Läuft beim **Build**, Next.js generiert interne Rewrite-Regeln.
* Unterstützt **Wildcards** (`:id`, `*`) und Bedingungen.

📖 Quelle: [Next.js Docs – Redirects](https://nextjs.org/docs/app/api-reference/next-config-js/redirects)

---

## **2. Redirects im App Router (Server Components / Route Handler)**

### a) **Mit `redirect()`** (Next.js 13+)

```js
// app/page.js
import { redirect } from "next/navigation";

export default function Home() {
  redirect("/dashboard"); // sofortige Weiterleitung
}
```

### b) **In Route Handlern**

```js
// app/api/old/route.js
import { NextResponse } from "next/server";

export function GET() {
  return NextResponse.redirect(new URL("/new", request.url), 301);
}
```

---

## **3. Redirects im Pages Router**

### a) **getServerSideProps**

```js
// pages/old.js
export async function getServerSideProps() {
  return {
    redirect: {
      destination: "/new",
      permanent: true, // 308
    },
  };
}
```

### b) **getStaticProps**

Bei statisch generierten Seiten ist Redirect auch möglich:

```js
// pages/legacy.js
export async function getStaticProps() {
  return {
    redirect: {
      destination: "/new",
      permanent: false,
    },
  };
}
```

---

## **4. Clientseitige Redirects**

### a) Mit `useRouter()` (Pages Router)

```js
import { useRouter } from "next/router";
import { useEffect } from "react";

export default function Old() {
  const router = useRouter();
  useEffect(() => {
    router.replace("/new");
  }, [router]);
  return null;
}
```

### b) Mit `useRouter()` (App Router → `next/navigation`)

```js
"use client";
import { useRouter } from "next/navigation";
import { useEffect } from "react";

export default function Old() {
  const router = useRouter();
  useEffect(() => {
    router.replace("/new");
  }, [router]);
  return null;
}
```

---

## **Zusammenfassung:**

* **Global (Build-Time):** `next.config.js → redirects()` (SEO-freundlich).
* **App Router:** `redirect()` oder `NextResponse.redirect()`.
* **Pages Router:** `getServerSideProps` / `getStaticProps` mit Redirect.
* **Clientseitig:** `useRouter().replace()` oder `router.push()`.

---

  **[⬆ Наверх](#top)**

27. ### <a name="27"></a> Was ist Middleware in Next.js und wofür wird sie benötigt?

**Definition:**
**Middleware** in Next.js ist Code, der **vor dem Rendering einer Seite ausgeführt wird**, direkt am **Edge (CDN/Server)**.
Sie ermöglicht es, **Requests abzufangen und zu verändern**, bevor sie die eigentliche Route erreichen.

---

### **Wofür wird Middleware benötigt?**

* **Authentifizierung & Autorisierung**
  → z. B. Weiterleitung nicht eingeloggter Nutzer auf `/login`.
* **Redirects & Rewrites**
  → URL anpassen oder Nutzer an andere Seiten weiterleiten.
* **Feature Flags / A/B-Testing**
  → unterschiedliche Versionen einer Seite ausliefern.
* **Lokalisierung (i18n)**
  → Nutzer anhand von Geodaten oder Accept-Language Header auf Sprachversion weiterleiten.
* **Caching & Headers**
  → Response-Header hinzufügen oder anpassen.

---

### **Beispiel – Middleware in Next.js**

```js
// middleware.js im Projekt-Root
import { NextResponse } from "next/server";

export function middleware(request) {
  const url = request.nextUrl;

  // Beispiel: Nur eingeloggte Nutzer dürfen /dashboard sehen
  const isLoggedIn = request.cookies.get("authToken");
  if (url.pathname.startsWith("/dashboard") && !isLoggedIn) {
    return NextResponse.redirect(new URL("/login", request.url));
  }

  return NextResponse.next(); // normal weiterleiten
}
```

👉 Middleware läuft **bei jedem Request**, bevor eine Seite oder API-Route erreicht wird.

---

### **Einschränkungen**

* Läuft **immer am Edge** → kein Zugriff auf Node.js-spezifische APIs (z. B. `fs`).
* Muss **schnell** sein (kein aufwendiges Datenfetching).
* Kein direktes Senden von HTML → nur Weiterleitungen, Header-Manipulation, Rewrites.

---

**Zusammenfassung:**
Middleware in Next.js ist Code, der **zwischen Request und Response** ausgeführt wird. Sie wird verwendet für **Auth, Redirects, i18n, Feature Flags und Request-Manipulation** – direkt am Edge, bevor das Rendering startet.

📖 Quelle: [Next.js Docs – Middleware](https://nextjs.org/docs/app/building-your-application/routing/middleware)

---

  **[⬆ Наверх](#top)**

28. ### <a name="28"></a> Wie funktioniert Internationalisierung (i18n) in Next.js?

**Definition:**
Internationalisierung (**i18n**) in Next.js bedeutet, dass eine Anwendung mehrere **Sprachen / Lokalisierungen** unterstützt. Next.js hat eine **eingebaute i18n-Routing-Funktion**, die im `next.config.js` aktiviert wird.

---

## **1. i18n im Pages Router (`pages/`)**

* Konfiguration über `next.config.js`

```js
// next.config.js
module.exports = {
  i18n: {
    locales: ["en", "de", "fr"], // unterstützte Sprachen
    defaultLocale: "en",         // Standardsprache
  },
};
```

* URLs:

  * `/` → `en` (default)
  * `/de/about` → deutsche Version
  * `/fr/about` → französische Version
* Next.js leitet automatisch auf die richtige Sprache um (basierend auf URL oder Accept-Language Header).

---

## **2. i18n im App Router (`app/`)**

Der App Router hat **noch keine eingebaute i18n-Unterstützung im Routing** (Stand Next.js 14). Man löst es so:

* Sprachordner anlegen:

```
app/
 ├─ [locale]/
 │   ├─ page.js
 │   └─ about/page.js
```

* URL: `/en/about`, `/de/about`
* Zugriff auf aktuelle Sprache über `params.locale`.

**Beispiel:**

```js
// app/[locale]/page.js
export default function Home({ params }) {
  return <h1>Sprache: {params.locale}</h1>;
}
```

---

## **3. Übersetzungen verwalten**

Da Next.js keine eingebaute Übersetzungs-Engine mitliefert, nutzt man Libraries:

* [`next-intl`](https://next-intl-docs.vercel.app/)
* [`next-i18next`](https://github.com/i18next/next-i18next)
* [`react-intl`] oder `i18next`

**Beispiel mit `next-intl`:**

```js
// app/[locale]/page.js
import { useTranslations } from "next-intl";

export default function Page() {
  const t = useTranslations("Home");
  return <h1>{t("title")}</h1>;
}
```

`messages/de.json`

```json
{ "Home": { "title": "Willkommen" } }
```

---

## **4. Typische Use-Cases**

* Mehrsprachige Websites (Landing Pages, Marketing, Shops)
* Automatische Weiterleitung je nach Sprache
* Dynamische Sprachumschaltung per Switch

---

**Zusammenfassung:**

* **Pages Router**: eingebaute i18n-Unterstützung über `next.config.js`.
* **App Router**: i18n aktuell manuell über `[locale]`-Routen + Libraries wie `next-intl`.
* Übersetzungen selbst kommen aus JSON/externen Tools.

📖 Quelle: [Next.js Docs – i18n Routing](https://nextjs.org/docs/pages/building-your-application/routing/internationalization)

---

  **[⬆ Наверх](#top)**

29. ### <a name="29"></a> Was ist der Unterschied zwischen Routing im pages- und im app-Verzeichnis?

**Unterschied Routing im `pages/`- vs. `app/`-Verzeichnis**

---

### **1. Architektur**

* **Pages Router (`pages/`)**

  * Klassisches Next.js-Routing.
  * Jede Datei = eine Route.
  * Datenfetching über spezielle Funktionen (`getStaticProps`, `getServerSideProps`, `getStaticPaths`).
  * Layouts nur global via `_app.js` oder `_document.js`.

* **App Router (`app/`)**

  * Neu seit Next.js 13.
  * Baut auf **React Server Components (RSC)**.
  * Klare Trennung: **`page.js`**, **`layout.js`**, **`loading.js`**, **`error.js`** pro Route.
  * Nested Routing & Layout-Vererbung möglich.

---

### **2. Dateibasierte Struktur**

* **Pages Router**

```
pages/
 ├─ index.js        → /
 ├─ about.js        → /about
 └─ blog/[id].js    → /blog/123
```

* **App Router**

```
app/
 ├─ page.js               → /
 ├─ about/page.js         → /about
 └─ blog/[id]/page.js     → /blog/123
    └─ layout.js          → Layout für /blog und Kinder
```

---

### **3. Datenfetching**

* **Pages Router**:

  * SSR → `getServerSideProps`
  * SSG → `getStaticProps` + `getStaticPaths`
  * ISR → über `revalidate` in `getStaticProps`
* **App Router**:

  * Einfaches `fetch()` direkt in Server Components
  * Caching via `cache`, `revalidate`, `no-store`
  * Keine speziellen Funktionen mehr nötig

---

### **4. Layouts**

* **Pages Router:** Nur global über `_app.js` → eingeschränkt.
* **App Router:** Beliebig viele verschachtelte Layouts (`layout.js`) pro Segment.

---

### **5. API-Routen**

* **Pages Router:** `pages/api/*`
* **App Router:** `app/api/*/route.js` (modernes API-Handling, Edge-first).

---

### **Vergleichstabelle**

| Merkmal           | Pages Router (`pages/`)            | App Router (`app/`)                            |
| ----------------- | ---------------------------------- | ---------------------------------------------- |
| **Einführung**    | Klassisch, seit Next.js 1          | Neu ab Next.js 13                              |
| **Routing**       | Datei = Route                      | Datei = Route, Layout/Loading/Error integriert |
| **Datenfetching** | getServerSideProps, getStaticProps | `fetch()` mit Cache-Optionen                   |
| **Layouts**       | Nur global (`_app.js`)             | Verschachtelte Layouts pro Route               |
| **Rendering**     | CSR, SSR, SSG, ISR                 | CSR, SSR, SSG, ISR, Streaming, RSC             |
| **API-Routen**    | `pages/api/*`                      | `app/api/*/route.js`                           |

---

**Zusammenfassung:**

* **Pages Router** = klassisch, stabil, einfacher Einstieg, aber eingeschränkte Layout- und Datenfetching-Möglichkeiten.
* **App Router** = modern, basiert auf Server Components, ermöglicht verschachtelte Layouts, flexibles Datenfetching und Streaming.

📖 Quelle: [Next.js Docs – App Router vs. Pages Router](https://nextjs.org/docs/app/building-your-application/routing#the-app-router)

---

  **[⬆ Наверх](#top)**

30. ### <a name="30"></a> Was macht getStaticProps?

**Definition:**
`getStaticProps` ist eine spezielle Funktion im **Pages Router** von Next.js. Sie wird **zur Build-Zeit** ausgeführt, um Daten zu laden und die Seite **statisch vorzurendern (SSG)**.
Die zurückgegebenen Props werden an die React-Komponente übergeben.

---

### **Wann wird `getStaticProps` verwendet?**

* Wenn Inhalte **statisch** sind, aber **Daten aus externen Quellen** benötigen.
* Für **SEO-optimierte Seiten**, die selten aktualisiert werden.
* Beispiel: Blogs, Landing Pages, Marketingseiten.

---

### **Funktionsweise**

* Wird **nur auf dem Server** ausgeführt, niemals im Client.
* Läuft **zur Build-Time** (bei `next build`).
* Kann mit `revalidate` kombiniert werden → **Incremental Static Regeneration (ISR)**.

---

### **Beispiel**

```js
// pages/index.js
export default function Home({ posts }) {
  return (
    <main>
      <h1>Blog</h1>
      <ul>
        {posts.map((p) => (
          <li key={p.id}>{p.title}</li>
        ))}
      </ul>
    </main>
  );
}

export async function getStaticProps() {
  // Daten laden (z. B. aus einer API oder Datenbank)
  const res = await fetch("https://jsonplaceholder.typicode.com/posts?_limit=5");
  const posts = await res.json();

  return {
    props: {
      posts, // wird an die Komponente übergeben
    },
    revalidate: 60, // ISR: Seite wird alle 60 Sekunden neu generiert
  };
}
```

---

### **Wichtige Punkte**

* Nur im **Pages Router** verfügbar (`pages/`).
* Wird nicht im **App Router** genutzt → dort einfach `fetch()` in Server Components.
* Kann keine Hooks nutzen (läuft **außerhalb von React**).
* Muss **ein Objekt** zurückgeben: `{ props: {} }`, optional `{ notFound: true }` oder `{ redirect: { destination: ... } }`.

---

**Zusammenfassung:**
`getStaticProps` wird in Next.js verwendet, um Seiten **zur Build-Zeit mit Daten zu generieren (SSG)**. Optional mit `revalidate` → **ISR**. Vorteil: **schnell, SEO-freundlich, skalierbar**.

📖 Quelle: [Next.js Docs – getStaticProps](https://nextjs.org/docs/pages/building-your-application/data-fetching/get-static-props)

---

  **[⬆ Наверх](#top)**  

31. ### <a name="31"></a> Was macht getServerSideProps?

**Definition:**
`getServerSideProps` ist eine spezielle Funktion im **Pages Router** von Next.js. Sie wird **bei jeder Anfrage (Request-Time)** auf dem Server ausgeführt und liefert Props an die Seite zurück.
Damit wird **Server-Side Rendering (SSR)** umgesetzt.

---

### **Wann wird `getServerSideProps` verwendet?**

* Wenn Inhalte **bei jedem Request aktuell** sein müssen.
* Für Seiten mit **dynamischen Daten**, die sich häufig ändern.
* Für **personalisierten Content** (z. B. abhängig von Cookies, Session, Auth).

---

### **Funktionsweise**

* Läuft nur **auf dem Server**, niemals im Browser.
* Wird **bei jedem Request** ausgeführt (anders als `getStaticProps`).
* Gibt Props an die Seite zurück, optional auch Redirects oder 404.

---

### **Beispiel**

```js
// pages/index.js
export default function Home({ time }) {
  return (
    <main>
      <h1>Server-Side Rendering Beispiel</h1>
      <p>Aktuelle Zeit: {time}</p>
    </main>
  );
}

export async function getServerSideProps(context) {
  // Daten werden bei jedem Request geladen
  const time = new Date().toISOString();

  return {
    props: {
      time,
    },
  };
}
```

➡️ Bei jedem Refresh wird die Zeit **neu generiert**.

---

### **Parameter (`context`)**

* `params`: dynamische Routenparameter (`/posts/[id]`)
* `query`: Query-Parameter (`?page=2`)
* `req`, `res`: Zugriff auf Request & Response (nur im Pages Router)

---

### **Besondere Rückgaben**

```js
return { notFound: true }; 
// liefert 404 zurück

return {
  redirect: {
    destination: "/login",
    permanent: false,
  },
}; 
// leitet um
```

---

### **Vergleich zu `getStaticProps`**

| Merkmal             | `getStaticProps` (SSG)        | `getServerSideProps` (SSR)         |
| ------------------- | ----------------------------- | ---------------------------------- |
| **Zeitpunkt**       | Build-Time / Revalidate (ISR) | Request-Time (bei jedem Request)   |
| **Performance**     | Sehr schnell (CDN, Cache)     | Langsamer (Server-Render nötig)    |
| **Datenaktualität** | Nicht immer aktuell           | Immer aktuell                      |
| **Use Cases**       | Blog, Landing Pages           | Dashboards, personalisierte Seiten |

---

**Zusammenfassung:**
`getServerSideProps` ermöglicht **Server-Side Rendering** im Pages Router. Es wird bei jedem Request aufgerufen, liefert Props zurück und eignet sich für **aktuelle oder personalisierte Daten**, allerdings mit **höherer Serverlast**.

📖 Quelle: [Next.js Docs – getServerSideProps](https://nextjs.org/docs/pages/building-your-application/data-fetching/get-server-side-props)

---

  **[⬆ Наверх](#top)**

32. ### <a name="32"></a> Was macht getStaticPaths?

**Definition:**
`getStaticPaths` ist eine spezielle Funktion im **Pages Router** von Next.js. Sie wird mit **`getStaticProps`** kombiniert, um **dynamische Routen statisch zur Build-Zeit** zu erzeugen.
Damit kann Next.js genau wissen, **welche Seiten vorgerendert werden sollen**.

---

## **Wann wird `getStaticPaths` benötigt?**

* Nur bei **dynamischen Routen** (`pages/blog/[id].js`).
* Wenn die Route viele mögliche Werte hat (z. B. Blog-IDs, Produkt-Slugs).
* Zusammen mit `getStaticProps`, um die Seite zur Build-Zeit vorzubereiten.

---

## **Funktionsweise**

* Gibt eine Liste von **Parametern** zurück → Next.js generiert daraus statische HTML-Seiten.
* Unterstützt **Fallback-Strategien**, falls nicht alle Seiten bei Build-Time erzeugt werden sollen.

---

## **Beispiel**

```js
// pages/blog/[id].js
export default function BlogPost({ post }) {
  return (
    <main>
      <h1>{post.title}</h1>
      <p>{post.body}</p>
    </main>
  );
}

// Generiert statische Pfade
export async function getStaticPaths() {
  const res = await fetch("https://jsonplaceholder.typicode.com/posts?_limit=3");
  const posts = await res.json();

  const paths = posts.map((post) => ({
    params: { id: post.id.toString() },
  }));

  return {
    paths,          // z. B. [{ params: { id: "1" }}, { params: { id: "2" }}]
    fallback: "blocking", // siehe unten
  };
}

// Holt Daten für jeden Pfad
export async function getStaticProps({ params }) {
  const res = await fetch(`https://jsonplaceholder.typicode.com/posts/${params.id}`);
  const post = await res.json();

  return {
    props: { post },
    revalidate: 60, // ISR: Alle 60 Sekunden aktualisieren
  };
}
```

---

## **Fallback-Modi**

* **`fallback: false`**

  * Nur die in `paths` definierten Seiten existieren.
  * Andere Routen liefern **404**.

* **`fallback: true`**

  * Nicht definierte Seiten werden beim ersten Request **on the fly generiert**.
  * Nutzer sieht zunächst einen Loading-State.

* **`fallback: "blocking"`**

  * Nicht definierte Seiten werden beim ersten Request generiert.
  * Nutzer wartet, bis HTML fertig ist → kein Loading-Screen sichtbar.

---

## **Zusammenfassung:**

* `getStaticPaths` = notwendig für **dynamische Routen mit SSG**.
* Es definiert, **welche Seiten Next.js statisch vorab baut**.
* In Kombination mit `getStaticProps` + `fallback` können auch **dynamisch neue Seiten on-demand erzeugt** werden (ISR).

📖 Quelle: [Next.js Docs – getStaticPaths](https://nextjs.org/docs/pages/building-your-application/data-fetching/get-static-paths)

---

  **[⬆ Наверх](#top)**

33. ### <a name="33"></a> Wann sollte man getStaticProps vs. getServerSideProps verwenden?

**Kurzantwort:**

* **`getStaticProps` (SSG/ISR):** Für Inhalte, die sich **selten** ändern oder **cachebar** sind; erzeugt HTML **zur Build-Zeit**, optional mit **`revalidate`** für ISR. ([nextjs.org][1])
* **`getServerSideProps` (SSR):** Für Inhalte, die **bei jedem Request** aktuell sein müssen oder **personalisiert** sind (Cookies, Auth, Geo, Header). ([nextjs.org][2])

---

### Entscheidungsleitfaden

**Nutze `getStaticProps`, wenn …**

* Daten **öffentlich cachebar** und **nicht nutzerspezifisch** sind.
* **SEO** wichtig ist und schnelle Antwortzeiten via **CDN** gewünscht sind.
* Änderungen in **Minuten/Stunden**-Takt reichen → **ISR** über `revalidate`. ([nextjs.org][1])

**Nutze `getServerSideProps`, wenn …**

* Inhalte **pro Request** variieren (z. B. **Session**, **Role**, **Geo**, **Header**).
* **Echtzeit** oder **sehr häufig wechselnde** Daten nötig sind.
* Du serverseitig auf **`req`/`res`** zugreifen musst. ([nextjs.org][2])

---

### Minimalbeispiele

```js
// pages/index.js  – SSG + ISR mit getStaticProps
export default function Home({ posts }) {
  return posts.map(p => <div key={p.id}>{p.title}</div>);
}

export async function getStaticProps() {
  const posts = await fetch("https://api.example.com/posts").then(r => r.json());
  return { props: { posts }, revalidate: 300 }; // alle 5 Min. regenerieren
}
```

*Build-Zeit + periodische Revalidierung (ISR).* ([nextjs.org][1])

```js
// pages/dashboard.js  – SSR mit getServerSideProps
export default function Dashboard({ user }) {
  return <h1>Hallo {user.name}</h1>;
}

export async function getServerSideProps({ req }) {
  const token = req.cookies.auth; // personalisiert
  const user = await fetch("https://api.example.com/me", { headers: { Authorization: `Bearer ${token}` }}).then(r => r.json());
  return { props: { user } };
}
```

*Request-Time Rendering, geeignet für personalisierte Daten.* ([nextjs.org][2])

---

### Hinweis zum App Router

Im **App Router** werden `getStaticProps/getServerSideProps` **nicht** verwendet; stattdessen steuerst du Rendering und Aktualität mit `fetch()`-Caching-Optionen (`force-cache`, `revalidate`, `no-store`). ([nextjs.org][3])

---

**Zusammenfassung:**

* **SSG/ISR (`getStaticProps`)** für **cachebare**, **nicht personalisierte** Inhalte mit optionaler zeitgesteuerter Aktualisierung.
* **SSR (`getServerSideProps`)** für **personalisierte** oder **hochdynamische** Inhalte **pro Request**.
* **App Router:** Datenfetching via `fetch()` + Caching/Revalidation statt `get*Props`. ([nextjs.org][2])

[1]: https://nextjs.org/docs/pages/building-your-application/data-fetching/get-static-props?utm_source=chatgpt.com "Data Fetching: getStaticProps"
[2]: https://nextjs.org/docs/pages/building-your-application/data-fetching/get-server-side-props?utm_source=chatgpt.com "Data Fetching: getServerSideProps"
[3]: https://nextjs.org/docs/app/getting-started/fetching-data?utm_source=chatgpt.com "Getting Started: Fetching Data"

  **[⬆ Наверх](#top)**

34. ### <a name="34"></a> Wie funktioniert revalidate im ISR?

**Definition:**
`revalidate` ist die zentrale Option im **Incremental Static Regeneration (ISR)** von Next.js. Sie bestimmt, **nach wie vielen Sekunden** eine statisch generierte Seite **im Hintergrund neu generiert** werden soll. So kombiniert ISR die Geschwindigkeit von SSG mit der Aktualität von SSR.

---

## **Funktionsweise**

1. Beim **Build** wird die Seite statisch generiert (`getStaticProps` oder `fetch()` im App Router).
2. Nutzer erhalten diese statische Seite direkt vom Cache/CDN.
3. Nach Ablauf der definierten Zeit (`revalidate: N`) wird bei der nächsten Anfrage:

   * die **alte Seite** sofort ausgeliefert (**kein Warten**),
   * im Hintergrund aber eine **neue Version** gebaut.
4. Alle folgenden Requests bekommen die **aktualisierte Seite**.

---

## **Beispiel im Pages Router (`getStaticProps`)**

```js
// pages/index.js
export default function Home({ time }) {
  return <p>Aktuelle Build-Zeit: {time}</p>;
}

export async function getStaticProps() {
  return {
    props: { time: new Date().toISOString() },
    revalidate: 10, // alle 10 Sekunden im Hintergrund aktualisieren
  };
}
```

➡ Seite wird nach 10 Sekunden beim nächsten Request neu generiert.

---

## **Beispiel im App Router (`fetch` mit Revalidate)**

```js
// app/page.js
export default async function Home() {
  const res = await fetch("https://api.example.com/data", {
    next: { revalidate: 30 }, // alle 30 Sekunden neu generieren
  });
  const data = await res.json();

  return <p>Daten: {data.message}</p>;
}
```

➡ Standardmäßig wird `fetch()` gecacht (SSG). Mit `revalidate` erzwingst du periodische Aktualisierung (**ISR**).

---

## **On-Demand Revalidation**

Neben dem Zeitintervall kann man per API-Endpunkt **gezielt Seiten neu generieren**, z. B. wenn ein neuer Blogpost veröffentlicht wird.
👉 Funktioniert mit `res.revalidate('/path')` (Pages Router) oder Vercel **On-Demand ISR** (App Router).

---

## **Zusammenfassung:**

* `revalidate` = Zeitintervall für **Hintergrund-Neuerstellung** einer Seite.
* **Pages Router:** Rückgabe in `getStaticProps`.
* **App Router:** als Option in `fetch()` → `next: { revalidate: N }`.
* Vorteil: **SSG-Performance** + **SSR-Aktualität**, ohne kompletten Rebuild.

📖 Quelle: [Next.js Docs – ISR](https://nextjs.org/docs/app/building-your-application/data-fetching/fetching#revalidating-data)

---

  **[⬆ Наверх](#top)**

35. ### <a name="35"></a> Wie ruft man Daten im App Router (Next.js 13) ab?

**Datenfetching im App Router (Next.js 13+)** funktioniert anders als im Pages Router:
Es gibt **keine `getStaticProps` oder `getServerSideProps` mehr**. Stattdessen nutzt man **`fetch()` direkt in Server Components**.

---

## **1. Server Components (Standard)**

* Standardmäßig sind Komponenten im App Router **Server Components**.
* Daten werden **auf dem Server geladen**, bevor die Seite zum Client geschickt wird.

```js
// app/page.js
export default async function Home() {
  const res = await fetch("https://jsonplaceholder.typicode.com/posts/1");
  const post = await res.json();

  return (
    <main>
      <h1>{post.title}</h1>
      <p>{post.body}</p>
    </main>
  );
}
```

➡ Vorteil: kein zusätzliches JS im Browser, besser für **Performance & SEO**.

---

## **2. Caching und Revalidate (ISR/SSR)**

Mit `fetch()` kann man **Caching-Strategien** steuern:

```js
// Statische Daten (SSG)
await fetch("https://api.example.com/data"); 
// default: `force-cache`

// Server-Side Rendering (SSR)
await fetch("https://api.example.com/data", { cache: "no-store" });

// Incremental Static Regeneration (ISR)
await fetch("https://api.example.com/data", { next: { revalidate: 60 } });
```

* **`force-cache`** = Standard (SSG)
* **`no-store`** = immer neu (SSR)
* **`revalidate: N`** = ISR (alle N Sekunden erneuern)

---

## **3. Client Components**

* Mit `"use client"` kann man Client Components erstellen.
* Hier ruft man Daten über **Hooks** wie `useEffect` ab → CSR.

```js
"use client";
import { useEffect, useState } from "react";

export default function ClientData() {
  const [data, setData] = useState(null);

  useEffect(() => {
    fetch("/api/message")
      .then((res) => res.json())
      .then(setData);
  }, []);

  return <p>{data ? data.text : "Lade Daten..."}</p>;
}
```

---

## **4. Serverseitige API-Routen (Route Handler)**

Man kann eigene **API-Routen im App Router** definieren und diese abfragen:

```js
// app/api/hello/route.js
export async function GET() {
  return Response.json({ message: "Hello API" });
}
```

```js
// app/page.js
const res = await fetch("http://localhost:3000/api/hello");
const data = await res.json();
```

---

## **Zusammenfassung:**

* **App Router** nutzt **`fetch()` in Server Components** statt `getStaticProps/getServerSideProps`.
* Datenstrategien:

  * **SSG** → default (Cache)
  * **SSR** → `cache: "no-store"`
  * **ISR** → `next: { revalidate: N }`
* **Client Components** nutzen Hooks (`useEffect`) → CSR.
* Eigene **API-Routen** via `app/api/*/route.js`.

📖 Quelle: [Next.js Docs – Data Fetching](https://nextjs.org/docs/app/building-your-application/data-fetching/fetching)

---

  **[⬆ Наверх](#top)**

36. ### <a name="36"></a> Was ist der Unterschied zwischen fetch auf dem Server und auf dem Client?

**Unterschied `fetch` auf dem Server vs. auf dem Client in Next.js (App Router):**

---

## **1. `fetch` auf dem Server (Server Components)**

* Läuft **vor dem Rendern** auf dem Server.
* Ergebnisse können direkt ins HTML eingebettet werden → **SEO-freundlich**.
* **Caching & Revalidate** werden automatisch unterstützt.
* Kein zusätzliches JavaScript im Browser nötig → bessere Performance.

**Beispiel (Server-Side Fetch, SSG/SSR/ISR):**

```js
// app/page.js (Server Component)
export default async function Home() {
  const res = await fetch("https://api.example.com/posts/1", {
    cache: "no-store", // SSR
  });
  const post = await res.json();

  return <h1>{post.title}</h1>;
}
```

👉 Vorteil: weniger Client-JS, schnell, SEO-freundlich.

---

## **2. `fetch` auf dem Client (Client Components)**

* Läuft erst **nachdem die Seite im Browser geladen** wurde.
* Kein Pre-Rendering → Inhalte erscheinen erst nach Hydration.
* Notwendig, wenn Daten von **Nutzerinteraktionen, Events oder Sessions** abhängen.
* Standard-React-Pattern: `useEffect` + `useState`.

**Beispiel (Client-Side Fetch, CSR):**

```js
"use client";
import { useEffect, useState } from "react";

export default function ClientData() {
  const [data, setData] = useState(null);

  useEffect(() => {
    fetch("/api/hello")
      .then(res => res.json())
      .then(setData);
  }, []);

  return <p>{data ? data.message : "Lade Daten..."}</p>;
}
```

👉 Nachteil: schlechtere SEO, da HTML erst leer ist; Inhalte erscheinen verzögert.

---

## **3. Vergleich**

| Merkmal         | **Server-Fetch**                        | **Client-Fetch**                         |
| --------------- | --------------------------------------- | ---------------------------------------- |
| **Ort**         | Server (vor Rendering)                  | Browser (nach Rendering)                 |
| **SEO**         | Sehr gut (HTML schon gefüllt)           | Schlecht (Content erst nach Hydration)   |
| **Caching**     | `force-cache`, `no-store`, `revalidate` | Manuell mit Zustand/Client-Cache         |
| **Performance** | Weniger Client-JS, schneller LCP        | Mehr Client-JS, langsamer LCP            |
| **Use Cases**   | Statische Daten, SEO-relevante Inhalte  | Interaktive Daten, nutzerabhängige Infos |

---

**Zusammenfassung:**

* **Server-Fetch**: vor Rendering, SEO-freundlich, unterstützt SSG/SSR/ISR.
* **Client-Fetch**: nach Rendering, dynamisch, aber schlechtere SEO und Performance.
* Faustregel: **so viel wie möglich auf dem Server, nur interaktive/nutzerabhängige Daten im Client**.

📖 Quelle: [Next.js Docs – Data Fetching](https://nextjs.org/docs/app/building-your-application/data-fetching/fetching)

---

  **[⬆ Наверх](#top)**

37. ### <a name="37"></a> Wie funktionieren Server Components (Next.js 13)?

**Definition:**
**Server Components (RSC)** in Next.js 13 sind React-Komponenten, die **ausschließlich auf dem Server ausgeführt werden**.
Sie senden **fertiges HTML an den Client**, ohne dass JavaScript für diese Komponenten im Browser ausgeführt oder gebündelt werden muss.

---

## **Wichtige Eigenschaften**

* **Standard im App Router**: Alle Komponenten ohne `"use client"` sind automatisch **Server Components**.
* **Kein Client-JavaScript**: Weniger JS-Bundle, bessere Performance, schnelleres Laden.
* **Direkter Zugriff auf Server-Ressourcen**: Datenbank, Filesystem, Secrets, externe APIs.
* **SEO-freundlich**: Inhalte werden bereits auf dem Server gerendert.
* **Keine Browser-APIs**: Kein `useState`, `useEffect`, `localStorage`, Events – dafür braucht man Client Components.

---

## **Beispiel – Server Component**

```js
// app/page.js (Server Component – default)
export default async function Home() {
  // Daten direkt auf dem Server laden
  const res = await fetch("https://jsonplaceholder.typicode.com/posts/1");
  const post = await res.json();

  return (
    <main>
      <h1>{post.title}</h1>
      <p>{post.body}</p>
    </main>
  );
}
```

👉 Wird auf dem Server ausgeführt, Client erhält reines HTML.

---

## **Kombination mit Client Components**

Man kann **Server und Client Components mischen**:

```js
// app/page.js
import ClientCounter from "./ClientCounter";

export default async function Home() {
  const res = await fetch("https://api.example.com/data");
  const data = await res.json();

  return (
    <main>
      <h1>Server Component mit Client Child</h1>
      <p>Daten: {data.message}</p>
      <ClientCounter /> {/* Interaktive Komponente */}
    </main>
  );
}
```

```js
// app/ClientCounter.js
"use client"; // macht die Komponente interaktiv
import { useState } from "react";

export default function ClientCounter() {
  const [count, setCount] = useState(0);
  return <button onClick={() => setCount(count + 1)}>Zähler: {count}</button>;
}
```

* **Home (Server Component):** Lädt Daten → schnell, kein Client-JS.
* **ClientCounter:** wird hydratisiert → interaktive Logik im Browser.

---

## **Vorteile**

* Kleinere JavaScript-Bundles → bessere Performance.
* Nahtlose **Server/Client-Trennung**.
* Direkter Datenbank- oder API-Zugriff ohne zusätzliche API-Routen.

## **Nachteile**

* Neue Denkweise: man muss verstehen, wann Server- vs. Client-Logik gebraucht wird.
* Nicht alle Bibliotheken sind kompatibel (z. B. die auf Browser-APIs basieren).

---

**Zusammenfassung:**
Server Components in Next.js 13 laufen **nur auf dem Server**, liefern **HTML ohne Client-JS**, können **direkt Daten abrufen** und sind **SEO-optimiert**. Für Interaktivität werden sie mit **Client Components** kombiniert.

📖 Quelle: [Next.js Docs – Server Components](https://nextjs.org/docs/app/building-your-application/rendering/server-components)

---

  **[⬆ Наверх](#top)**

38. ### <a name="38"></a> Was ist der Unterschied zwischen Client Components und Server Components?

**Unterschied zwischen Client Components und Server Components (Next.js 13+):**

---

## **1. Server Components**

* **Standard** im App Router (ohne `"use client"`).
* Laufen **ausschließlich auf dem Server**.
* Können **direkt Datenbanken, APIs, Filesystem** ansprechen.
* Werden zu **fertigem HTML** gerendert → **SEO-freundlich, kleineres Bundle**.
* **Kein JavaScript im Client nötig** → bessere Performance.
* **Nicht erlaubt:** React Hooks wie `useState`, `useEffect`, Browser-APIs (`localStorage`, `window`).

**Beispiel:**

```js
// app/page.js (Server Component – default)
export default async function Home() {
  const res = await fetch("https://jsonplaceholder.typicode.com/posts/1");
  const post = await res.json();

  return <h1>{post.title}</h1>;
}
```

---

## **2. Client Components**

* Mit Direktive `"use client"` am Anfang der Datei.
* Laufen **im Browser** → ermöglichen **Interaktivität**.
* Können React Hooks (`useState`, `useEffect`, `useContext`) und Browser-APIs nutzen.
* Müssen hydratisiert werden → **mehr JavaScript-Bundle**, langsamer als Server Components.

**Beispiel:**

```js
// app/Counter.js
"use client";
import { useState } from "react";

export default function Counter() {
  const [count, setCount] = useState(0);
  return <button onClick={() => setCount(count + 1)}>Zähler: {count}</button>;
}
```

---

## **3. Kombination**

Man kombiniert beide, um **Datenserverseitig** + **Interaktivität clientseitig** zu nutzen:

```js
// app/page.js
import Counter from "./Counter";

export default async function Home() {
  const res = await fetch("https://api.example.com/message");
  const data = await res.json();

  return (
    <main>
      <h1>{data.text}</h1>
      <Counter /> {/* Client Component */}
    </main>
  );
}
```

---

## **Vergleichstabelle**

| Merkmal          | **Server Components**                   | **Client Components**                    |
| ---------------- | --------------------------------------- | ---------------------------------------- |
| **Ort**          | Server                                  | Browser                                  |
| **Default**      | Ja (im App Router)                      | Nein (`"use client"` notwendig)          |
| **JS im Client** | Kein JS nötig (nur HTML)                | JS muss gebündelt & hydratisiert werden  |
| **SEO**          | Sehr gut (fertiges HTML)                | Schlechter (Content erst nach Hydration) |
| **Hooks**        | Nicht erlaubt (`useState`, `useEffect`) | Erlaubt (voller React-Support)           |
| **Use Cases**    | Datenfetching, Layouts, SEO-Inhalte     | Interaktive Elemente, Event-Handling     |

---

**Zusammenfassung:**

* **Server Components**: Datenserverseitig, schnell, kein Client-JS → gut für SEO & Performance.
* **Client Components**: Interaktivität im Browser, nutzen React Hooks, benötigen Hydration.
* Best Practice: **so viel wie möglich Server Components**, nur Interaktivität als Client Components.

📖 Quelle: [Next.js Docs – Server vs Client Components](https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns)

---

  **[⬆ Наверх](#top)**

39. ### <a name="39"></a> Wie bindet man externe Bibliotheken in Server Components ein?

**Regel:**
In **Server Components** (Next.js 13+) darf nur Code laufen, der **auf dem Server funktioniert**.
Das bedeutet: **Bibliotheken ohne Browser-Abhängigkeiten** (kein `window`, `document`, DOM, `localStorage`) können direkt eingebunden werden.
Bibliotheken mit **Browser-APIs** müssen in eine **Client Component** ausgelagert werden.

---

## **1. Externe Bibliothek im Server Component (möglich)**

Beispiel mit einer serverseitigen Bibliothek wie `date-fns`:

```js
// app/page.js (Server Component – default)
import { format } from "date-fns";

export default function Home() {
  const today = format(new Date(), "dd.MM.yyyy");
  return <h1>Heute: {today}</h1>;
}
```

👉 Funktioniert, da `date-fns` nur pure JS-Logik enthält.

---

## **2. Bibliothek, die Browser-APIs braucht (nur Client Component)**

Beispiel: `chart.js` oder `leaflet` (nutzt Canvas/DOM).

```js
// app/Chart.js
"use client";
import { useEffect, useRef } from "react";
import Chart from "chart.js/auto";

export default function MyChart() {
  const canvasRef = useRef(null);

  useEffect(() => {
    const ctx = canvasRef.current.getContext("2d");
    new Chart(ctx, {
      type: "bar",
      data: { labels: ["A", "B"], datasets: [{ data: [10, 20] }] },
    });
  }, []);

  return <canvas ref={canvasRef}></canvas>;
}
```

👉 Muss `use client` haben, da `Chart.js` den DOM braucht.

---

## **3. Pattern: Server + Client kombinieren**

Man kann Bibliotheken **teilweise serverseitig vorbereiten** und das Rendering clientseitig machen:

```js
// app/page.js (Server Component)
import MyChart from "./Chart";

export default async function Page() {
  const data = await fetch("https://api.example.com/stats").then(r => r.json());
  return <MyChart initialData={data} />;
}
```

👉 Datenfetching serverseitig, Rendering clientseitig.

---

## **Best Practices**

* **Immer prüfen:** Läuft die Bibliothek ohne Browser-APIs? → dann im Server Component.
* **Rechenintensive Logik** (Markdown-Parser, Datenbanken, Crypto) → auf dem Server.
* **UI-Bibliotheken** (Chart, Maps, Slider) → Client Component.

---

**Zusammenfassung:**

* In Server Components nur Bibliotheken nutzen, die **kein DOM/Browser** brauchen.
* Browser-abhängige Libraries gehören in **Client Components**.
* Oft kombiniert: **Server für Daten + Client für Interaktivität**.

📖 Quelle: [Next.js Docs – Server vs Client Components](https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns)

---

  **[⬆ Наверх](#top)**

40. ### <a name="40"></a> Welche Einschränkungen haben Server Components?

**Einschränkungen von Server Components in Next.js 13+:**

---

### **1. Kein Zugriff auf Browser-APIs**

* Kein `window`, `document`, `localStorage`, `sessionStorage`.
* Kein direktes DOM-Manipulieren.

---

### **2. Keine React Hooks für Client State**

* **Nicht erlaubt:** `useState`, `useEffect`, `useLayoutEffect`.
* Nur **serverseitige Logik** möglich (z. B. `async/await`, Datenbankzugriffe).

---

### **3. Eingeschränkte Bibliotheken-Nutzung**

* Libraries, die **DOM oder Browser-Events** nutzen (z. B. `chart.js`, `leaflet`), funktionieren nicht.
* Solche Bibliotheken müssen in **Client Components** ausgelagert werden.

---

### **4. Hydration**

* Server Components werden **nicht hydratisiert** → kein Client-JavaScript.
* Wenn Interaktivität benötigt wird → **Client Component einbinden**.

---

### **5. Einschränkungen bei Props**

* Props an Server Components müssen **serialisierbar** sein (JSON).
* Keine Funktionen, Klasseninstanzen oder nicht-serialisierbare Objekte als Props.

---

### **6. Datenfluss**

* Server Components können **Client Components rendern**, aber nicht umgekehrt.
* Das bedeutet: **Top-Down-Hierarchie**:

  * Server Component → Client Component ✅
  * Client Component → Server Component ❌

---

### **7. Asynchronität**

* Server Components dürfen **async** sein und Daten mit `fetch()` laden.
* Aber: Man kann nicht `useEffect` nutzen, um Daten nachzuladen.

---

### **Zusammenfassung:**

Server Components sind mächtig für **Datenfetching, Performance und SEO**, aber:

* **Kein Client-State, keine Browser-APIs**.
* **Keine Hooks wie `useState`, `useEffect`**.
* **Keine nicht-serialisierbaren Props**.
* **Nur Server → Client, nicht umgekehrt**.
  👉 Deshalb: **so viel wie möglich Server Components nutzen, Interaktivität in Client Components auslagern**.

📖 Quelle: [Next.js Docs – Server vs Client Components](https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns)

---

  **[⬆ Наверх](#top)**  

41. ### <a name="41"></a> Was sind API Routes in Next.js?

**Definition:**
API Routes in Next.js sind **serverseitige Endpunkte**, die direkt im Projekt definiert werden. Sie ermöglichen es, neben dem Frontend auch einfache **Backend-Logik** (z. B. Datenverarbeitung, Authentifizierung, Datenbankzugriffe) in einer Next.js-App zu implementieren – ohne separaten Backend-Server.

---

## **1. API Routes im Pages Router (`pages/api/*`)**

* Jede Datei in `pages/api` wird automatisch zu einem API-Endpunkt.
* Standard-Export ist eine Handler-Funktion `(req, res)`.

**Beispiel:**

```js
// pages/api/hello.js → /api/hello
export default function handler(req, res) {
  res.status(200).json({ message: "Hello API" });
}
```

---

## **2. API Routes im App Router (`app/api/*/route.js`)**

* Ab Next.js 13: **Route Handlers** im `app/`-Verzeichnis.
* REST-Methoden (`GET`, `POST`, `PUT`, `DELETE`) werden als benannte Funktionen exportiert.

**Beispiel:**

```js
// app/api/hello/route.js → /api/hello
export async function GET() {
  return Response.json({ message: "Hello API" });
}

export async function POST(request) {
  const body = await request.json();
  return Response.json({ received: body });
}
```

---

## **3. Typische Einsatzfälle**

* Authentifizierung (z. B. JWT, Session-Handling).
* CRUD-Operationen für Datenbanken (z. B. Prisma, MongoDB, PostgreSQL).
* Webhooks von externen Diensten (z. B. Stripe, GitHub).
* Proxy für externe APIs (um API-Keys zu verbergen).

---

## **4. Vorteile**

* **Full-Stack in einer App:** Frontend + Backend in Next.js.
* **Edge-/Serverless-fähig:** Lässt sich optimal mit Vercel, Netlify oder AWS Lambda deployen.
* **Kein separater Express-/Node-Server nötig** für kleine bis mittlere Backends.

---

## **Einschränkungen**

* Nicht für **sehr komplexe Backends** gedacht → dort besser dedizierte Server/Services.
* Kein direkter Zugriff auf Node-spezifische APIs bei **Edge Functions** (z. B. `fs`).

---

**Zusammenfassung:**
API Routes in Next.js sind **serverseitige Endpunkte**, die im Projekt selbst erstellt werden.

* **Pages Router:** `pages/api/*` mit `(req, res)` Handlern.
* **App Router:** `app/api/*/route.js` mit `GET/POST`-Funktionen.
  Ideal für **kleine Backends, Auth, CRUD-Operationen und API-Proxies**.

📖 Quelle: [Next.js Docs – API Routes](https://nextjs.org/docs/pages/building-your-application/routing/api-routes)

---

  **[⬆ Наверх](#top)**

42. ### <a name="42"></a> Wie erstellt man einen API-Endpunkt (pages/api/...)?

**API-Endpunkte im Pages Router (`pages/api/...`)** sind der klassische Weg, um in Next.js **serverseitige Logik** einzubauen. Jede Datei in `pages/api` wird automatisch zu einer API-Route.

---

## **1. Struktur**

```
pages/
 └─ api/
     ├─ hello.js       → /api/hello
     └─ users/
         └─ [id].js    → /api/users/123
```

---

## **2. Einfaches Beispiel**

```js
// pages/api/hello.js → /api/hello
export default function handler(req, res) {
  res.status(200).json({ message: "Hallo von der API!" });
}
```

* `req` = Request-Objekt (inkl. Query, Body, Cookies).
* `res` = Response-Objekt (HTTP-Antwort zurückschicken).

---

## **3. Mit HTTP-Methoden**

```js
// pages/api/users.js → /api/users
export default function handler(req, res) {
  if (req.method === "GET") {
    res.status(200).json({ users: ["Anna", "Tom"] });
  } else if (req.method === "POST") {
    const user = req.body.name;
    res.status(201).json({ message: `User ${user} erstellt` });
  } else {
    res.status(405).json({ error: "Methode nicht erlaubt" });
  }
}
```

* GET: Daten abrufen
* POST: Neue Daten anlegen
* Weitere Methoden (PUT, DELETE) genauso möglich

---

## **4. Dynamische API-Routen**

```js
// pages/api/users/[id].js → /api/users/123
export default function handler(req, res) {
  const { id } = req.query;
  res.status(200).json({ userId: id });
}
```

* Zugriff über `req.query.id`.

---

## **5. Typische Use-Cases**

* CRUD-Endpunkte für Datenbanken (z. B. Prisma, MongoDB).
* Authentifizierung (Login/Logout).
* Proxy zu externen APIs (API-Keys verbergen).
* Webhooks (z. B. Stripe, GitHub).

---

**Zusammenfassung:**
Ein API-Endpunkt im **Pages Router** wird erstellt, indem man in `pages/api/...` eine Datei anlegt und einen **Handler mit `(req, res)`** exportiert.

* **GET/POST/PUT/DELETE** mit `req.method`.
* **Dynamische Routen** über `[id].js`.
* Ideal für kleine Backends und API-Proxies direkt in Next.js.

📖 Quelle: [Next.js Docs – API Routes](https://nextjs.org/docs/pages/building-your-application/routing/api-routes)

---

  **[⬆ Наверх](#top)**

43. ### <a name="43"></a> Wie funktionieren API Routes im App Router (route.ts)?

**API Routes im App Router heißen in Next.js „Route Handlers“.**
Sie werden im Verzeichnis `app/api/.../route.(js|ts)` definiert und ersetzen die klassischen `pages/api/...`-Routen.

---

## **1. Struktur**

```
app/
 └─ api/
     ├─ hello/
     │   └─ route.ts   → /api/hello
     └─ users/
         └─ [id]/
             └─ route.ts → /api/users/123
```

---

## **2. Einfaches Beispiel**

```ts
// app/api/hello/route.ts
export async function GET() {
  return Response.json({ message: "Hallo vom App Router API!" });
}
```

👉 Jeder **HTTP-Verb** (GET, POST, PUT, DELETE, PATCH, OPTIONS) kann als **exportierte Funktion** definiert werden.

---

## **3. Mit Request-Objekt**

```ts
// app/api/users/route.ts
export async function POST(request: Request) {
  const body = await request.json(); // Body-Daten auslesen
  return Response.json({ user: body.name, created: true }, { status: 201 });
}
```

---

## **4. Dynamische API-Routen**

```ts
// app/api/users/[id]/route.ts
export async function GET(
  request: Request,
  { params }: { params: { id: string } }
) {
  return Response.json({ userId: params.id });
}
```

👉 `params` enthält die dynamischen URL-Segmente.

---

## **5. Response-Optionen**

```ts
// Eigene Response mit Status & Header
export async function GET() {
  return new Response("Custom Text", {
    status: 200,
    headers: { "Content-Type": "text/plain" },
  });
}
```

---

## **6. Typische Einsatzfälle**

* Authentifizierung (z. B. JWT, Cookies).
* CRUD-Endpunkte für Datenbanken.
* Webhooks von externen Services (Stripe, GitHub).
* Proxying von APIs (z. B. API-Key im Server verstecken).

---

**Zusammenfassung:**

* **Pages Router:** API in `pages/api/*` mit `(req, res)`-Handlern.
* **App Router:** API in `app/api/*/route.ts` mit **exportierten Funktionen für HTTP-Methoden**.
* Vorteile: **Edge-fähig**, moderner Standard, direktes Arbeiten mit `Request` und `Response`.

📖 Quelle: [Next.js Docs – Route Handlers](https://nextjs.org/docs/app/building-your-application/routing/route-handlers)

---

  **[⬆ Наверх](#top)**

44. ### <a name="44"></a> Wie übergibt man Query-Parameter an API Routes?

**Query-Parameter in API Routes** werden genauso übergeben wie in klassischen REST-Endpunkten – durch Anhängen an die URL, z. B.:

```
/api/users?id=123&active=true
```

---

## **1. Pages Router (`pages/api/...`)**

Hier bekommt man die Query-Parameter über `req.query`:

```js
// pages/api/users.js
export default function handler(req, res) {
  const { id, active } = req.query;
  res.status(200).json({ id, active });
}
```

➡️ Aufruf: `/api/users?id=123&active=true`
Antwort: `{ "id": "123", "active": "true" }`

---

## **2. App Router (`app/api/.../route.ts`)**

Hier greift man auf die Query-Parameter über `request.url` bzw. `request.nextUrl` zu:

```ts
// app/api/users/route.ts
export async function GET(request: Request) {
  const { searchParams } = new URL(request.url);

  const id = searchParams.get("id");
  const active = searchParams.get("active");

  return Response.json({ id, active });
}
```

➡️ Aufruf: `/api/users?id=123&active=true`
Antwort: `{ "id": "123", "active": "true" }`

---

## **3. Dynamische Routen + Query-Params**

Man kann Query-Parameter auch mit **dynamischen Segmenten** kombinieren:

```ts
// app/api/users/[id]/route.ts
export async function GET(request: Request, { params }: { params: { id: string } }) {
  const { searchParams } = new URL(request.url);
  const active = searchParams.get("active");

  return Response.json({ userId: params.id, active });
}
```

➡️ Aufruf: `/api/users/42?active=true`
Antwort: `{ "userId": "42", "active": "true" }`

---

**Zusammenfassung:**

* **Pages Router:** Query-Parameter über `req.query`.
* **App Router:** Query-Parameter über `new URL(request.url).searchParams`.
* Kombinierbar mit dynamischen Routen (`[id]`).

📖 Quelle: [Next.js Docs – API Routes (Pages)](https://nextjs.org/docs/pages/building-your-application/routing/api-routes) · [Route Handlers (App)](https://nextjs.org/docs/app/building-your-application/routing/route-handlers)

---

  **[⬆ Наверх](#top)**

45. ### <a name="45"></a> Wie verarbeitet man POST-Anfragen in API Routes?

**POST-Anfragen in API Routes** ermöglichen es, Daten vom Client an den Server zu senden (z. B. Formulare, JSON, Auth-Daten). Die Verarbeitung ist unterschiedlich im **Pages Router** und **App Router**.

---

## **1. Pages Router (`pages/api/...`)**

Hier wird der Body über `req.body` ausgelesen.
➡ Standardmäßig wird JSON automatisch geparst (sofern `Content-Type: application/json`).

```js
// pages/api/contact.js
export default function handler(req, res) {
  if (req.method === "POST") {
    const { name, email } = req.body; // Body-Daten
    return res.status(200).json({ message: `Hallo ${name}, Email: ${email}` });
  }

  res.status(405).json({ error: "Method Not Allowed" });
}
```

👉 Client-Aufruf:

```js
await fetch("/api/contact", {
  method: "POST",
  headers: { "Content-Type": "application/json" },
  body: JSON.stringify({ name: "Anna", email: "anna@example.com" }),
});
```

---

## **2. App Router (`app/api/.../route.ts`)**

Im App Router arbeitet man direkt mit dem `Request`-Objekt.
➡ Der Body wird mit `await request.json()` oder `await request.formData()` ausgelesen.

```ts
// app/api/contact/route.ts
export async function POST(request: Request) {
  const body = await request.json(); // JSON auslesen
  const { name, email } = body;

  return Response.json({ message: `Hallo ${name}, Email: ${email}` }, { status: 201 });
}
```

👉 Client-Aufruf (gleich wie oben).

---

## **3. Verarbeitung von Formulardaten**

Falls ein HTML-Formular mit `multipart/form-data` gesendet wird:

```ts
// app/api/upload/route.ts
export async function POST(request: Request) {
  const formData = await request.formData();
  const file = formData.get("file"); // z. B. ein hochgeladenes File
  return Response.json({ filename: file.name });
}
```

---

## **Zusammenfassung:**

* **Pages Router:** Body über `req.body`. JSON wird automatisch geparst.
* **App Router:** Body über `await request.json()` oder `await request.formData()`.
* POST eignet sich für **Formulare, Auth, CRUD-Operationen**.

📖 Quelle: [Next.js Docs – API Routes](https://nextjs.org/docs/pages/building-your-application/routing/api-routes) · [Route Handlers](https://nextjs.org/docs/app/building-your-application/routing/route-handlers)

---

  **[⬆ Наверх](#top)**

46. ### <a name="46"></a> Wie verwendet man Middleware in API Routes?

**Middleware in API Routes** bedeutet, dass man **Code vor der eigentlichen Request-Logik** ausführt – z. B. für Authentifizierung, Logging, Rate-Limiting.
In Next.js gibt es **zwei Ansätze**, je nach Router:

---

## **1. Globale Middleware (`middleware.ts`) – App & Pages Router**

* Läuft **vor jedem Request** (Seiten **und** API Routes).
* Liegt im Projekt-Root (`/middleware.ts`).
* Kann Weiterleitungen, Header-Manipulation, Zugriffskontrolle durchführen.

**Beispiel: Auth für API-Route schützen**

```ts
// middleware.ts
import { NextResponse } from "next/server";
import type { NextRequest } from "next/server";

export function middleware(req: NextRequest) {
  const token = req.cookies.get("authToken")?.value;

  // Nur API-Routen schützen
  if (req.nextUrl.pathname.startsWith("/api/") && !token) {
    return NextResponse.json({ error: "Unauthorized" }, { status: 401 });
  }

  return NextResponse.next();
}
```

➡ Diese Middleware blockiert alle API-Requests ohne `authToken`.

---

## **2. Lokale Middleware im Pages Router (per Funktion)**

Da Pages-API-Routen klassische `(req, res)`-Handler sind, kann man Middleware als **Hilfsfunktion** implementieren.

```js
// lib/auth.js
export function requireAuth(handler) {
  return (req, res) => {
    if (!req.headers.authorization) {
      return res.status(401).json({ error: "Unauthorized" });
    }
    return handler(req, res);
  };
}

// pages/api/secret.js
import { requireAuth } from "../../lib/auth";

function handler(req, res) {
  res.status(200).json({ message: "Secret data" });
}

export default requireAuth(handler);
```

➡ Hier wird Middleware wie ein **Wrapper** um den Handler gelegt.

---

## **3. Lokale Middleware im App Router (Route Handlers)**

Auch im App Router kann man Middleware als **Hilfsfunktion** nutzen:

```ts
// lib/auth.ts
export async function requireAuth(request: Request) {
  const token = request.headers.get("authorization");
  if (!token) {
    return new Response(JSON.stringify({ error: "Unauthorized" }), { status: 401 });
  }
  return null; // kein Fehler → weiter
}

// app/api/secret/route.ts
import { requireAuth } from "@/lib/auth";

export async function GET(request: Request) {
  const authError = await requireAuth(request);
  if (authError) return authError;

  return Response.json({ message: "Secret API Data" });
}
```

---

## **Zusammenfassung:**

* **Globale Middleware (`middleware.ts`)** → greift vor allen Requests, inkl. API Routes (ideal für Auth, Logging, Rate Limits).
* **Lokale Middleware** → als Wrapper-Funktion oder Utility, direkt im Handler verwendet.
* **Pages Router:** `(req, res)`-Middleware.
* **App Router:** `Request`-Middleware.

📖 Quelle: [Next.js Docs – Middleware](https://nextjs.org/docs/app/building-your-application/routing/middleware)

---

  **[⬆ Наверх](#top)**

47. ### <a name="47"></a> Worin besteht der Unterschied zwischen API Routes und einem separaten Backend-Server?

**Unterschied API Routes in Next.js vs. separater Backend-Server:**

---

## **1. Architektur**

* **API Routes (Next.js)**

  * Backend-Logik direkt im Next.js-Projekt (`pages/api/*` oder `app/api/*/route.ts`).
  * Läuft als **Serverless Function** (z. B. auf Vercel) oder Edge Function.
  * Frontend & Backend sind im selben Codebase integriert (**Full-Stack in einer App**).

* **Separater Backend-Server**

  * Eigenständige Anwendung (z. B. Express, NestJS, Django, FastAPI).
  * Muss separat deployed, gewartet und skaliert werden.
  * Frontend (Next.js) und Backend sind voneinander entkoppelt.

---

## **2. Einsatzbereich**

* **API Routes:**

  * Ideal für kleine bis mittlere Backends.
  * Authentifizierung, Formulare, Webhooks, CRUD, API-Proxies.
  * Weniger Setup, schnell für Prototypen und kleine Projekte.

* **Separates Backend:**

  * Für komplexe Business-Logik, große Datenverarbeitung, Microservices.
  * Mehr Flexibilität (z. B. WebSockets, Hintergrundjobs, Queues, Worker).
  * Bessere Skalierbarkeit und Lastverteilung.

---

## **3. Skalierung & Performance**

* **API Routes:**

  * Standardmäßig **stateless** (Serverless Functions).
  * Gut für horizontale Skalierung (z. B. viele gleichzeitige Requests).
  * Kein langfristiger State → externe DB/Redis nötig.

* **Separates Backend:**

  * Kann **stateful** arbeiten (z. B. mit Sessions im Speicher).
  * Kann lange Prozesse, Streaming, WebSockets stabiler handhaben.
  * Beliebig optimierbar, da keine Framework-Beschränkungen.

---

## **4. Deployment**

* **API Routes:**

  * Deploy mit dem Frontend zusammen (z. B. auf Vercel).
  * Einfache DevOps (ein Projekt, ein Deployment).

* **Separates Backend:**

  * Eigenes Hosting (Docker, Kubernetes, Server).
  * Mehr Aufwand für Infrastruktur, Monitoring, CI/CD.

---

## **Vergleichstabelle**

| Merkmal         | **API Routes (Next.js)**           | **Separates Backend**                     |
| --------------- | ---------------------------------- | ----------------------------------------- |
| **Ort**         | Teil des Next.js-Projekts (`/api`) | Eigenständige App (Express, NestJS, etc.) |
| **Deployment**  | Zusammen mit dem Frontend          | Separat (eigenes Hosting)                 |
| **Komplexität** | Einfach, wenig Setup               | Höher, mehr Infrastruktur nötig           |
| **Skalierung**  | Gut für stateless, kleine Services | Besser für komplexe, stateful Systeme     |
| **Use Cases**   | Auth, CRUD, Webhooks, kleine APIs  | Enterprise-Logik, Microservices, Echtzeit |

---

**Zusammenfassung:**

* **API Routes**: Einfach, integriert, ideal für kleinere APIs, Prototypen und Full-Stack in einer App.
* **Separates Backend**: Mehr Flexibilität und Skalierbarkeit, aber komplexer im Betrieb – geeignet für große Systeme mit umfangreicher Business-Logik.

📖 Quelle: [Next.js Docs – API Routes](https://nextjs.org/docs/pages/building-your-application/routing/api-routes) · [Next.js Route Handlers](https://nextjs.org/docs/app/building-your-application/routing/route-handlers)

---

  **[⬆ Наверх](#top)**

48. ### <a name="48"></a> Kann man Next.js API Routes als Production-Backend verwenden?

**Kurzantwort:**
Ja – **API Routes/Route Handlers** können in Produktion laufen (Serverless/Edge). Sie eignen sich für **kleine bis mittlere** Backends, Webhooks, Auth, CRUD, Proxies. Für **komplexe, stateful** Systeme, lange Jobs, Streaming/WebSockets oder strenge Performance-/Compliance-Anforderungen ist oft ein **separates Backend** besser. ([nextjs.org][1])

---

### Geeignete Produktions-Use-Cases

* **Auth & Sessions**, Cookie-Handling, Header-Checks (auch via Middleware). ([nextjs.org][2])
* **CRUD/REST-APIs** gegen DBs/Services; **Webhooks** (Stripe/GitHub). ([nextjs.org][1])
* **API-Proxy** zum Verbergen von Secrets/Keys. ([nextjs.org][1])

---

### Wichtige Grenzen & Stolpersteine

* **Antwortgrößenlimit** (Standard ~4 MB) für Pages-API Routes; ggf. anpassen/architekturell umgehen. ([nextjs.org][3])
* **Serverless-Charakter**: stateless, potenzielle **Cold Starts**; Langläufer/Jobs auslagern (Queue/Worker).
* **Edge-Runtime**: keine Node-spezifischen APIs wie `fs`; nur Web-APIs. ([nextjs.org][1])
* **Kein `next export`** mit Pages-API Routes (statischer Export); Route Handlers im App Router sind export-fähig. ([nextjs.org][4])
* **Operations**: Observability, Rate-Limiting, Secrets, CORS, Prod-Checks bewusst konfigurieren. ([nextjs.org][5])

---

### Praxis-Empfehlungen

* **App Router bevorzugen**: `app/api/*/route.ts` (unterstützt alle HTTP-Methoden, Edge/Server-Runtimes). ([nextjs.org][1])
* **Globale Regeln** über **`middleware.ts`** (Auth, Geofencing, A/B). ([nextjs.org][2])
* **On-Demand ISR**, Caching-Header, Timeouts und Retries gezielt setzen; Produktions-Checkliste beachten. ([nextjs.org][5])
* **Für große Systeme**: Next.js-Frontend + **separater Backend-Dienst** (Microservices, Queues, Streaming, WebSockets).

---

**Zusammenfassung**

* **Ja, produktionsfähig** für viele Full-Stack-Szenarien (Auth, CRUD, Webhooks, Proxies).
* **Achte auf Limits** (Größe, Runtime, Stateless-Charakter, Export).
* **Komplex/Stateful** → eher **separates Backend**.
  Weiterlesen: [API Routes (Pages)](https://nextjs.org/docs/pages/building-your-application/routing/api-routes), [Route Handlers (App)](https://nextjs.org/docs/app/building-your-application/routing/route-handlers), [Middleware](https://nextjs.org/docs/app/api-reference/file-conventions/middleware), [Production-Checkliste](https://nextjs.org/docs/app/guides/production-checklist). ([nextjs.org][6])

[1]: https://nextjs.org/docs/app/api-reference/file-conventions/route?utm_source=chatgpt.com "File-system conventions: route.js"
[2]: https://nextjs.org/docs/14/app/building-your-application/routing/middleware?utm_source=chatgpt.com "Middleware - Routing"
[3]: https://nextjs.org/docs/messages/api-routes-response-size-limit?utm_source=chatgpt.com "Addressing \"API Routes Response Size Limited to 4MB ..."
[4]: https://nextjs.org/docs/pages/building-your-application/routing/api-routes?utm_source=chatgpt.com "API Routes"
[5]: https://nextjs.org/docs/app/guides/production-checklist?utm_source=chatgpt.com "Guides: Production"
[6]: https://nextjs.org/learn/pages-router/api-routes-creating-api-routes?utm_source=chatgpt.com "Pages Router: Creating API Routes"

  **[⬆ Наверх](#top)**

49. ### <a name="49"></a> Wie funktioniert der public-Ordner?

**Definition:**
Der `public`-Ordner in Next.js ist ein spezielles Verzeichnis im Projekt-Root, das für **statische Assets** gedacht ist. Alle Dateien dort werden **unverändert** in die Produktion übernommen und sind **öffentlich unter der URL `/` verfügbar**.

---

## **1. Struktur**

```
my-app/
 ├─ public/
 │   ├─ images/
 │   │   └─ logo.png
 │   └─ robots.txt
 └─ app/ oder pages/
```

---

## **2. Zugriff auf Dateien**

* Jede Datei in `public/` ist **direkt über die URL erreichbar**:

  * `public/logo.png` → `/logo.png`
  * `public/images/logo.png` → `/images/logo.png`
* Next.js ändert oder verarbeitet die Dateien **nicht** – sie werden 1:1 ausgeliefert.

**Beispiel in React-Komponente:**

```jsx
// app/page.js oder pages/index.js
export default function Home() {
  return (
    <main>
      <h1>Startseite</h1>
      <img src="/images/logo.png" alt="Logo" width={200} />
    </main>
  );
}
```

---

## **3. Typische Anwendungsfälle**

* **Bilder** (Logos, Favicons, statische Assets).
* **Dokumente** (PDFs, Downloads).
* **Konfigurationsdateien** (robots.txt, sitemap.xml, favicon.ico).
* **Static Files für Third-Party** (z. B. Verifikationsdateien für Google/Bing).

---

## **4. Unterschiede zu `import`**

* Dateien im `public`-Ordner werden **nicht durch Webpack** verarbeitet → kein Hashing, kein Tree Shaking.
* Assets, die man **importiert** (`import img from "@/assets/logo.png"`) landen im **Webpack-Bundle** → besser für optimierte Images mit `next/image`.
* Faustregel:

  * **Für unveränderte, globale Assets → `public/`**
  * **Für importierte, optimierte Assets → `import` + `next/image`**

---

**Zusammenfassung:**

* Alles im `public`-Ordner wird 1:1 im Root-Pfad ausgeliefert.
* Typisch für **statische Assets** (Bilder, PDFs, Konfigurationsdateien).
* Kein Webpack-Prozess → Assets bleiben unverändert.
* Für optimierte Images → lieber `next/image` mit Imports verwenden.

📖 Quelle: [Next.js Docs – Static File Serving](https://nextjs.org/docs/app/building-your-application/optimizing/static-assets#static-file-serving)

---

  **[⬆ Наверх](#top)**

50. ### <a name="50"></a> Wie bindet man Bilder in Next.js ein?

**In Next.js gibt es zwei Möglichkeiten, Bilder einzubinden:**

---

## **1. Über den `public/`-Ordner (klassisch, `<img>`-Tag)**

* Dateien in `public/` sind **statisch unter `/` verfügbar**.
* Werden **nicht optimiert** von Next.js.

**Beispiel:**

```jsx
// Datei: public/images/logo.png
export default function Home() {
  return (
    <main>
      <h1>Startseite</h1>
      <img src="/images/logo.png" alt="Logo" width={200} height={200} />
    </main>
  );
}
```

👉 Einfach, aber **kein automatisches Lazy Loading, kein Optimieren**.

---

## **2. Mit der `next/image` Komponente (empfohlener Weg)**

Next.js bringt eine eigene **Image-Optimierung** mit:

* Automatisches **Responsive Loading** (verschiedene Größen).
* **Lazy Loading** (Bilder außerhalb des Viewports werden erst bei Bedarf geladen).
* Automatische **Formatoptimierung** (z. B. WebP, AVIF).
* Funktioniert sowohl mit `public/`-Bildern als auch mit externen URLs.

**Beispiel (lokales Bild aus `public/`):**

```jsx
import Image from "next/image";

export default function Home() {
  return (
    <main>
      <h1>Startseite</h1>
      <Image
        src="/images/logo.png" // liegt in /public/images/logo.png
        alt="Logo"
        width={200}
        height={200}
      />
    </main>
  );
}
```

**Beispiel (externe URL):**

```jsx
import Image from "next/image";

export default function Avatar() {
  return (
    <Image
      src="https://example.com/avatar.png"
      alt="User Avatar"
      width={100}
      height={100}
    />
  );
}
```

👉 Bei externen URLs muss man sie in `next.config.js` freigeben:

```js
// next.config.js
module.exports = {
  images: {
    domains: ["example.com"],
  },
};
```

---

## **3. Dynamische Bilder**

Mit `fill` kann ein Bild den Container vollständig ausfüllen:

```jsx
<Image
  src="/images/background.jpg"
  alt="Hintergrund"
  fill
  style={{ objectFit: "cover" }}
/>
```

---

## **Vergleich**

| Methode            | Vorteile                              | Nachteile                            |
| ------------------ | ------------------------------------- | ------------------------------------ |
| **`<img>` + public | Einfach, kein Import nötig            | Keine Optimierung, kein Lazy Loading |
| **`next/image`**   | Optimierung, Lazy Loading, Responsive | Erfordert Width/Height, komplexer    |

---

**Zusammenfassung:**

* Für **einfache statische Assets** → `<img src="/...">` über `public/`.
* Für **optimierte Bilder** → `next/image` verwenden (empfohlen für Produktion).

📖 Quelle: [Next.js Docs – Images](https://nextjs.org/docs/app/building-your-application/optimizing/images)

---

  **[⬆ Наверх](#top)**  

51. ### <a name="51"></a> Was macht next/image und wofür wird es benötigt?

**Definition:**
`next/image` ist eine spezielle React-Komponente in Next.js für Bilder. Sie ersetzt den normalen `<img>`-Tag und bietet **automatische Optimierungen** wie **Lazy Loading, Responsive Images, Bildkomprimierung** und **modernere Formate (WebP/AVIF)**. Ziel ist es, Performance, SEO und Core Web Vitals (LCP) zu verbessern.

---

## **Wichtige Features**

* **Automatische Optimierung**: Bilder werden beim ersten Request generiert, gecached und optimiert ausgeliefert.
* **Responsive Größen**: Next.js liefert je nach Bildschirmgröße automatisch das passende Bild.
* **Lazy Loading**: Bilder werden erst geladen, wenn sie im Viewport erscheinen.
* **Automatische Formate**: WebP/AVIF werden bevorzugt, wenn der Browser sie unterstützt.
* **Integration mit `public/` und externen URLs**: funktioniert sowohl für lokale als auch für Remote-Bilder.

---

## **Beispiel: Lokales Bild**

```jsx
import Image from "next/image";

export default function Home() {
  return (
    <Image
      src="/images/logo.png"   // liegt in /public/images/logo.png
      alt="Logo"
      width={200}
      height={200}
    />
  );
}
```

---

## **Beispiel: Externes Bild**

```jsx
import Image from "next/image";

export default function Avatar() {
  return (
    <Image
      src="https://example.com/avatar.jpg"
      alt="User Avatar"
      width={150}
      height={150}
    />
  );
}
```

➡ dafür in `next.config.js` die Domain freigeben:

```js
module.exports = {
  images: {
    domains: ["example.com"],
  },
};
```

---

## **Vorteile gegenüber `<img>`**

| Merkmal               | `<img>`              | `next/image` (empfohlen)           |
| --------------------- | -------------------- | ---------------------------------- |
| **Optimierung**       | Keine                | Automatisch (Größe, Format, Cache) |
| **Lazy Loading**      | Manuell              | Standardmäßig aktiviert            |
| **Responsive**        | Manuell mit `srcset` | Automatisch                        |
| **SEO & Performance** | Geringer             | Bessere Core Web Vitals            |

---

**Zusammenfassung:**
`next/image` wird benötigt, um Bilder **performant, SEO-optimiert und responsive** einzubinden. Es reduziert die Bildgrößen, verbessert Ladezeiten und ist der empfohlene Standard für Bilder in Next.js.

📖 Quelle: [Next.js Docs – Image Component](https://nextjs.org/docs/app/building-your-application/optimizing/images)

---

  **[⬆ Наверх](#top)**

52. ### <a name="52"></a> Welche Vorteile hat next/image im Vergleich zu <img>?

**Vorteile von `next/image` im Vergleich zu `<img>`:**

---

### **1. Automatische Optimierung**

* `next/image` liefert Bilder immer in der **optimierten Größe** aus.
* Reduziert die Dateigröße, ohne dass man manuell Varianten pflegen muss.

---

### **2. Responsive Images**

* Automatisches Erstellen von **verschiedenen Bildgrößen** (srcset).
* Browser lädt immer nur die passende Version für das jeweilige Gerät (Mobile, Tablet, Desktop).

---

### **3. Lazy Loading**

* Standardmäßig aktiviert → Bilder außerhalb des Viewports werden erst geladen, wenn sie sichtbar werden.
* Spart Bandbreite und beschleunigt **First Contentful Paint (FCP)**.

---

### **4. Moderne Bildformate**

* Next.js konvertiert Bilder automatisch in **WebP oder AVIF**, wenn der Browser diese unterstützt.
* Fallback auf PNG/JPG bei nicht unterstützten Browsern.

---

### **5. SEO & Core Web Vitals**

* Durch Optimierung, Lazy Loading und kleinere Dateien verbessert sich die **Performance** und damit Ranking in Google.
* Besonders wichtig für **Largest Contentful Paint (LCP)**.

---

### **6. Integration mit CDN und Caching**

* Bilder werden automatisch gecached und über das Next.js-/Vercel-CDN ausgeliefert.
* Wiederholte Aufrufe sind extrem schnell.

---

### **Vergleichstabelle**

| Merkmal                   | `<img>` (klassisch)          | `next/image` (optimiert)           |
| ------------------------- | ---------------------------- | ---------------------------------- |
| **Optimierung**           | Keine                        | Automatisch (Größe, Format, Cache) |
| **Responsive Images**     | Manuell via `srcset`         | Automatisch generiert              |
| **Lazy Loading**          | Manuell via `loading="lazy"` | Standardmäßig aktiv                |
| **Formate (WebP/AVIF)**   | Manuell konvertieren         | Automatisch, Browser-abhängig      |
| **SEO / Core Web Vitals** | Schwächer                    | Besser (LCP, Performance)          |

---

**Zusammenfassung:**
`next/image` bietet gegenüber `<img>` **deutliche Performance-, SEO- und Komfortvorteile**: automatische Optimierung, Lazy Loading, responsive Bilder und moderne Formate – ohne dass der Entwickler sich selbst um diese Themen kümmern muss.

📖 Quelle: [Next.js Docs – Image Component](https://nextjs.org/docs/app/building-your-application/optimizing/images)

---

  **[⬆ Наверх](#top)**

53. ### <a name="53"></a> Wie funktioniert Image Optimization?

**Image Optimization in Next.js** ist ein integriertes Feature der `next/image`-Komponente, das Bilder automatisch **komprimiert, in passende Formate konvertiert und responsive Größen ausliefert**. Ziel ist es, Ladezeiten zu verkürzen, Bandbreite zu sparen und Core Web Vitals (insbesondere **LCP**) zu verbessern.

---

## **Funktionsweise**

1. **Request**:

   * Ein Bild wird über `next/image` eingebunden.
   * Beispiel: `/images/logo.png`.

2. **Optimierung**:

   * Beim ersten Request generiert Next.js eine optimierte Version:

     * **Skalierung** auf angegebene `width`/`height`.
     * **Komprimierung** (JPEG, PNG, GIF → WebP/AVIF, falls Browser unterstützt).
     * **Caching** (lokal oder über CDN, z. B. Vercel).

3. **Responsive Auslieferung**:

   * Next.js erstellt automatisch mehrere Varianten (`srcset`).
   * Der Browser lädt **immer nur die passende Größe** für das Gerät.

4. **Caching & Wiederverwendung**:

   * Einmal optimierte Bilder werden im `.next/cache` gespeichert oder über das CDN ausgeliefert.
   * Bei wiederholten Requests sofort verfügbar.

---

## **Beispiel**

```jsx
import Image from "next/image";

export default function Home() {
  return (
    <Image
      src="/images/hero.jpg" // Original im /public
      alt="Hero Bild"
      width={1200}
      height={600}
      priority // sofort laden, kein Lazy Loading
    />
  );
}
```

👉 Browser bekommt automatisch:

* Kleinere Versionen (z. B. 640px, 768px, 1200px).
* Modernes Format (WebP oder AVIF, wenn möglich).
* Lazy Loading (außer `priority` ist gesetzt).

---

## **Externe Bilder**

* Für externe URLs muss man Domains freigeben (`next.config.js`):

```js
module.exports = {
  images: {
    domains: ["example.com"],
  },
};
```

---

## **Vorteile**

* Automatische **Performance-Optimierung** ohne manuelle Bearbeitung.
* **SEO-freundlich** durch kleinere Ladezeiten.
* Spart **Bandbreite** (besonders für Mobile).
* Funktioniert **out of the box** mit Vercel-CDN.

---

## **Einschränkungen**

* Funktioniert nur mit `next/image` (nicht mit `<img>`).
* Externe Loader müssen konfiguriert werden, wenn man kein Vercel nutzt.
* Keine GIF-Optimierung → diese werden unverändert ausgeliefert.

---

**Zusammenfassung:**
Die **Image Optimization** in Next.js sorgt dafür, dass Bilder automatisch **skaliert, komprimiert, in moderne Formate umgewandelt und gecached** werden. Dadurch verbessert sich Performance, SEO und User Experience erheblich, ohne dass der Entwickler selbst manuell Varianten oder Konvertierungen pflegen muss.

📖 Quelle: [Next.js Docs – Image Optimization](https://nextjs.org/docs/app/building-your-application/optimizing/images)

---

  **[⬆ Наверх](#top)**

54. ### <a name="54"></a> Kann man dynamische Bilder im public-Ordner speichern?

**Kurzantwort:**
Nein – der `public/`-Ordner in Next.js ist für **statische Dateien** gedacht. Alles, was dort liegt, wird **unverändert** ins Build übernommen und unter `/` ausgeliefert. Dynamische Bilder (z. B. User-Uploads, generierte Thumbnails) gehören **nicht** in `public/`, da Next.js diesen Ordner nicht zur Laufzeit beschreibt.

---

## **Warum nicht `public/` für dynamische Bilder?**

* Inhalte im `public/`-Ordner sind **read-only** nach dem Build.
* Auf Vercel oder anderen Hosting-Plattformen werden Deployments **immutable** – Dateien können nach Deployment nicht geändert oder hinzugefügt werden.
* Dynamische Uploads würden beim nächsten Build überschrieben.

---

## **Alternativen für dynamische Bilder**

1. **Externe Storage-Lösungen**

   * AWS S3, Google Cloud Storage, Supabase, Firebase Storage.
   * Vorteil: Skalierbar, unabhängig vom Next.js-Build.

2. **Datenbank + CDN**

   * Bilder in einer Datenbank speichern (z. B. MongoDB GridFS) und über CDN ausliefern.

3. **Eigene API-Route mit Upload**

   * Beispiel: `/api/upload` speichert das Bild im Filesystem oder einem Cloud Storage.
   * Zugriff dann über `/api/files/[id]`.

---

## **Beispiel: Dynamisches Bild über API Route**

```ts
// app/api/upload/route.ts
export async function POST(request: Request) {
  const formData = await request.formData();
  const file = formData.get("file");
  // TODO: in Cloud oder DB speichern
  return Response.json({ url: `/api/files/${file.name}` });
}
```

👉 Nutzer lädt Bild hoch, App liefert URL zurück.

---

## **Zusammenfassung:**

* **`public/` = nur für statische Assets** (Logos, Favicons, unveränderliche Dateien).
* **Dynamische Bilder (User-Uploads, generierte Bilder)** gehören in **Cloud-Speicher, Datenbanken oder eigene API-Routen**.
* In Produktion ist `public/` schreibgeschützt und daher nicht geeignet für Runtime-Uploads.

📖 Quelle: [Next.js Docs – Static File Serving](https://nextjs.org/docs/app/building-your-application/optimizing/static-assets#static-file-serving)

---

  **[⬆ Наверх](#top)**

55. ### <a name="55"></a> Wie bindet man Schriftarten in Next.js ein?

**Zwei Wege: `next/font` (empfohlen) oder klassisches CSS.**
`next/font` (Google & lokal) **hostet Schriften selbst, erzeugt @font-face, subsettet, verhindert Layout-Shift und entfernt externe Requests**. Nutzung im **App Router über `app/layout.tsx`** bzw. in Komponenten. ([Next.js][1])

---

## `next/font/google` (Google Fonts, selbst gehostet)

```js
// app/layout.tsx
import { Inter, Roboto_Flex } from "next/font/google";

const inter = Inter({ subsets: ["latin"], display: "swap" });          // statische Familie
const roboto = Roboto_Flex({ subsets: ["latin"], axes: ["wdth"], variable: "--font-roboto" }); // Variable Font → CSS-Var

export default function RootLayout({ children }) {
  return (
    <html lang="de" className={roboto.variable}>
      <body className={inter.className}>{children}</body>
    </html>
  );
}
```

* **`subsets`** reduziert Dateigröße, **`display: "swap"`** vermeidet FOUT, **`variable`** legt eine CSS-Variable für Variable Fonts an. ([Next.js][2])

---

## `next/font/local` (lokale/Custom-Fonts)

```js
// app/layout.tsx
import localFont from "next/font/local";

const acme = localFont({
  src: [
    { path: "./fonts/Acme-Regular.woff2", weight: "400", style: "normal" },
    { path: "./fonts/Acme-Bold.woff2",    weight: "700", style: "normal" },
  ],
  variable: "--font-acme",
  display: "swap",
});

export default function RootLayout({ children }) {
  return (
    <html lang="de" className={acme.variable}>
      <body>{children}</body>
    </html>
  );
}
```

* Dateien liegen z. B. unter `app/fonts`. **Self-hosting & Caching** erfolgen automatisch. ([Next.js][1])

---

## Verwendung in Komponenten / mit Tailwind

```js
// app/page.tsx
export default function Page() {
  return (
    <main>
      <h1 className="text-2xl font-bold">Titel</h1>
      <p style={{ fontFamily: "var(--font-acme)" }}>Absatz mit lokaler Schrift</p>
    </main>
  );
}
```

* Alternativ: CSS-Klasse mit `font-family: var(--font-acme);` in deiner globalen CSS-Datei. ([Next.js][1])

---

## Klassisch (nur falls nötig)

Per `<link rel="preconnect" …>` + eigenes `@font-face`. **Nachteil:** externe Requests, manuelle Pflege von Formaten/`srcset`/Fallbacks; keine automatische Optimierung. **Bevorzugt `next/font` verwenden.** ([Next.js][3])

---

**Zusammenfassung**

* **Empfohlen:** `next/font` mit `next/font/google` oder `next/font/local` → **selbstgehostet, performant, kein CLS, Subsetting, Caching**.
* Einbinden über **`app/layout.tsx`**, Anwendung via `.className` oder CSS-Variablen.
* Klassische Einbindung nur ausnahmsweise.
  Weiterlesen: **Installation/Setup** und **Font-Optimierung** in den offiziellen Docs. ([Next.js][4])

[1]: https://nextjs.org/docs/app/getting-started/fonts?utm_source=chatgpt.com "Getting Started: Font Optimization"
[2]: https://nextjs.org/docs/app/api-reference/components/font?utm_source=chatgpt.com "Components: Font"
[3]: https://nextjs.org/docs/14/pages/building-your-application/optimizing/fonts?utm_source=chatgpt.com "Optimizing: Fonts"
[4]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"

  **[⬆ Наверх](#top)**

56. ### <a name="56"></a> Was ist next/font?

**Definition:**
`next/font` ist ein integriertes Next.js-Feature (seit v13), mit dem man **Schriftarten optimiert einbinden** kann. Es ersetzt externe Font-Provider (z. B. Google Fonts `<link>`-Tags) durch **selbstgehostete, automatisch optimierte Fonts**.

---

## **Wichtige Eigenschaften**

* **Self-Hosting**: Schriften werden automatisch heruntergeladen, lokal gehostet und gecached → keine externen Requests.
* **Kein CLS** (*Cumulative Layout Shift*): Schriftarten werden serverseitig vorab gerendert, kein Fallback-Flackern.
* **Subsetting**: Nur die tatsächlich verwendeten Zeichen/Untersets werden geladen (z. B. `latin`, `cyrillic`).
* **Variable Fonts**: Unterstützung für `variable` → per CSS-Variable nutzbar.
* **Einfache Nutzung**: Import direkt in `layout.tsx` oder Komponenten.

---

## **Zwei Varianten**

### 1. **Google Fonts** (`next/font/google`)

Automatisches Laden, Hosting & Subsetting.

```js
// app/layout.tsx
import { Inter } from "next/font/google";

const inter = Inter({ subsets: ["latin"], display: "swap" });

export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body className={inter.className}>{children}</body>
    </html>
  );
}
```

### 2. **Lokale Fonts** (`next/font/local`)

Für eigene oder heruntergeladene Schriftarten.

```js
import localFont from "next/font/local";

const myFont = localFont({
  src: "./fonts/MyFont.woff2",
  weight: "400",
  style: "normal",
  variable: "--font-myfont",
});

export default function RootLayout({ children }) {
  return (
    <html lang="de" className={myFont.variable}>
      <body>{children}</body>
    </html>
  );
}
```

---

## **Vorteile gegenüber klassischem `<link>` oder `@font-face`**

| Merkmal                       | Klassisch (`<link>`) | `next/font`        |
| ----------------------------- | -------------------- | ------------------ |
| **Hosting**                   | Extern (Google CDN)  | Lokal, automatisch |
| **Layout Shift**              | Ja (FOIT/FOUT)       | Nein               |
| **Subsetting**                | Manuell              | Automatisch        |
| **Performance/SEO**           | Schlechter           | Besser             |
| **DX (Developer Experience)** | Eigenes Setup nötig  | Direkt via Import  |

---

**Zusammenfassung:**
`next/font` ist die empfohlene Methode in Next.js, um **Google Fonts oder lokale Schriften** performant, SEO-freundlich und ohne Layout-Verschiebungen einzubinden. Es macht Fonts **zuverlässiger, schneller und einfacher** nutzbar als klassische Methoden.

📖 Quelle: [Next.js Docs – Fonts](https://nextjs.org/docs/app/building-your-application/optimizing/fonts)

---

  **[⬆ Наверх](#top)**

57. ### <a name="57"></a> Welche Styling-Methoden unterstützt Next.js?

**Next.js unterstützt mehrere Styling-Methoden – je nach Projektgröße und Anforderungen:**

---

## **1. Globale CSS-Dateien**

* Definiert in `app/globals.css` oder `pages/_app.js`.
* Gelten für die gesamte App.

```css
/* app/globals.css */
body {
  margin: 0;
  font-family: sans-serif;
}
```

---

## **2. CSS-Module**

* Dateiendung: `*.module.css`.
* Klassen werden automatisch **scoped** (nur in der Komponente gültig).

```css
/* Button.module.css */
.btn {
  background: blue;
  color: white;
}
```

```jsx
import styles from "./Button.module.css";
export default function Button() {
  return <button className={styles.btn}>Klick mich</button>;
}
```

---

## **3. Sass/SCSS (mit Modulen)**

* Direkt unterstützt (`*.scss`, `*.module.scss`).
* Bietet Variablen, Mixins, verschachtelte Syntax.

---

## **4. Tailwind CSS**

* Utility-first CSS-Framework, sehr beliebt mit Next.js.
* Einfache Integration via PostCSS.

```jsx
export default function Card() {
  return <div className="p-4 bg-gray-200 rounded-lg shadow">Inhalt</div>;
}
```

---

## **5. CSS-in-JS**

* Next.js unterstützt Libraries wie **styled-jsx** (eingebaut), **styled-components**, **emotion**.

**Beispiel mit styled-jsx (built-in):**

```jsx
export default function Title() {
  return (
    <>
      <h1>Hallo</h1>
      <style jsx>{`
        h1 {
          color: red;
        }
      `}</style>
    </>
  );
}
```

---

## **6. Frameworks & UI-Bibliotheken**

* Chakra UI, Material UI (MUI), Ant Design, etc.
* Können in Client Components eingebunden werden.

---

## **7. Inline Styles**

* Direkt via `style={{ ... }}`.
* Für dynamische Styles, aber weniger performant.

---

## **8. Next.js Fonts & Theme**

* Mit `next/font` für Schriftarten.
* Globale Theme-Ansätze über Context oder UI-Bibliotheken.

---

## **Zusammenfassung:**

Next.js unterstützt **globale CSS-Dateien, CSS-Module, Sass/SCSS, Tailwind CSS, CSS-in-JS (styled-jsx, styled-components, emotion)**, Inline Styles und externe UI-Bibliotheken.

* **Kleine Projekte:** CSS-Module oder Tailwind.
* **Große Projekte:** Kombination aus Tailwind + Komponenten-Bibliothek oder CSS-in-JS.

📖 Quelle: [Next.js Docs – Styling](https://nextjs.org/docs/app/building-your-application/styling)

---

  **[⬆ Наверх](#top)**

58. ### <a name="58"></a> Wie verwendet man CSS-Module?

**Definition:**
CSS-Module in Next.js sind **lokal isolierte CSS-Dateien**, die nur für die jeweilige Komponente gelten. Dadurch vermeidet man Klassennamen-Konflikte und erhält ein sauberes, komponentenbasiertes Styling.

---

## **1. Dateibenennung**

* CSS-Module haben die Endung **`.module.css`** oder **`.module.scss`**.
* Beispiel: `Button.module.css`.

---

## **2. Beispiel – CSS-Module**

```css
/* Button.module.css */
.btn {
  background-color: blue;
  color: white;
  padding: 10px 20px;
  border-radius: 6px;
  cursor: pointer;
}

.btn:hover {
  background-color: darkblue;
}
```

```jsx
// Button.jsx
import styles from "./Button.module.css";

export default function Button() {
  return <button className={styles.btn}>Klick mich</button>;
}
```

👉 `styles.btn` wird von Next.js intern in einen eindeutigen Klassennamen umgewandelt, z. B. `Button_btn__3XyZ`.

---

## **3. Vorteile**

* **Scoped Styles**: Nur für die jeweilige Komponente gültig.
* **Keine Namenskonflikte**: Automatisch generierte Klassen.
* Funktioniert mit **CSS-Variablen** und **Sass**.

---

## **4. Dynamische Klassen**

Man kann Klassenbedingungen dynamisch kombinieren:

```jsx
import styles from "./Button.module.css";
import clsx from "clsx"; // optionales Hilfs-Paket

export default function Button({ primary }) {
  return (
    <button className={clsx(styles.btn, primary && styles.primary)}>
      Klick mich
    </button>
  );
}
```

```css
/* Button.module.css */
.btn {
  padding: 10px;
  border: none;
}
.primary {
  background: blue;
  color: white;
}
```

---

## **5. Verwendung mit globalem CSS**

* **Globale Styles** kommen in `app/globals.css` oder `pages/_app.js`.
* **Komponenten-Styling** → CSS-Module.

---

**Zusammenfassung:**

* CSS-Module = Dateien mit `.module.css`, automatisch **scoped**.
* Import als Objekt → `styles.className`.
* Vorteil: **keine Konflikte, saubere Komponententrennung**.
* Dynamisch kombinierbar mit Libraries wie `clsx`.

📖 Quelle: [Next.js Docs – CSS Modules](https://nextjs.org/docs/app/building-your-application/styling/css-modules)

---

  **[⬆ Наверх](#top)**

59. ### <a name="59"></a> Wie verwendet man SASS/SCSS in Next.js?

**Definition:**
Next.js unterstützt **Sass/SCSS** out of the box. Du kannst also `.scss`- oder `.sass`-Dateien genau wie CSS verwenden – global oder als **SCSS-Module** für Komponenten.

---

## **1. Installation**

Zuerst das Sass-Paket installieren:

```bash
npm install sass
```

---

## **2. Globale SCSS-Datei**

* Lege `app/globals.scss` (oder `styles/globals.scss`) an.
* Importiere sie im Root-Layout (`app/layout.tsx`) oder in `_app.js` (Pages Router).

```scss
/* globals.scss */
$primary-color: #0070f3;

body {
  margin: 0;
  font-family: sans-serif;
  background: $primary-color;
}
```

```tsx
// app/layout.tsx
import "./globals.scss";

export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body>{children}</body>
    </html>
  );
}
```

---

## **3. SCSS-Module (empfohlen für Komponenten)**

Datei: `Button.module.scss`

```scss
// Button.module.scss
$btn-bg: blue;

.btn {
  background: $btn-bg;
  color: white;
  padding: 10px;
  border-radius: 6px;

  &:hover {
    background: darken($btn-bg, 10%);
  }
}
```

Komponente:

```tsx
// Button.tsx
import styles from "./Button.module.scss";

export default function Button() {
  return <button className={styles.btn}>Klick mich</button>;
}
```

👉 Klassen sind automatisch **scoped** wie bei CSS-Modules.

---

## **4. SCSS Features**

* **Variablen** (`$color`), **Nesting** (`&:hover`), **Mixins**, **Funktionen**.
* Mehr Wiederverwendbarkeit und Struktur als reines CSS.

---

## **5. Best Practices**

* **Globales SCSS** nur für Grundlayout, Resets, Variablen.
* **SCSS-Module** für Komponenten → saubere Kapselung.
* In Kombination mit **Tailwind** nur selten nötig.

---

**Zusammenfassung:**

* Installiere `sass`, nutze `.scss`/`.sass`-Dateien.
* **Global:** `globals.scss` → Layout oder `_app.js`.
* **Komponenten:** `*.module.scss` mit Scoped Styles.
* SCSS bietet **Variablen, Nesting, Mixins** → mehr Struktur und Wiederverwendung.

📖 Quelle: [Next.js Docs – Sass Support](https://nextjs.org/docs/app/building-your-application/styling/sass)

---

  **[⬆ Наверх](#top)**

60. ### <a name="60"></a> Wie integriert man TailwindCSS in Next.js?

**Zwei Wege:**

* **Schnellstart mit CLI:** `create-next-app --tailwind` (Tailwind wird automatisch konfiguriert). ([Next.js][1])
* **Manuell nachrüsten:** Tailwind installieren, `tailwind.config` + PostCSS einrichten, Direktiven in `globals.css` hinzufügen. ([tailwindcss.com][2])

---

## 1) Schnellstart (empfohlen)

```bash
npx create-next-app@latest my-app --ts --app --tailwind
cd my-app
npm run dev
```

* App Router + TypeScript + Tailwind vorkonfiguriert. ([Next.js][1])

---

## 2) Manuelle Integration in bestehendes Projekt

```bash
# Pakete
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

**`tailwind.config.js`** (App Router):

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./app/**/*.{js,ts,jsx,tsx,mdx}",
    "./components/**/*.{js,ts,jsx,tsx,mdx}",
  ],
  theme: { extend: {} },
  plugins: [],
};
```

**`app/globals.css`**:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

* Dev-Server starten: `npm run dev`. ([tailwindcss.com][2])

---

## 3) Nutzung im Code

```js
// app/page.tsx
export default function Home() {
  return (
    <main className="min-h-dvh grid place-items-center bg-gray-50">
      <div className="rounded-xl border p-6 shadow">
        <h1 className="text-2xl font-bold">Next.js + Tailwind</h1>
        <p className="text-gray-600">Ready to build!</p>
      </div>
    </main>
  );
}
```

---

## 4) Hinweise

* Dark Mode per `dark`-Klasse aktivieren (optional): `darkMode: "class"` im `tailwind.config.js`.
* Bei Nutzung von **Pages Router** zusätzlich `./pages/**/*.{js,ts,jsx,tsx}` in `content` aufnehmen. ([Next.js][3])

---

**Zusammenfassung**

* **Am schnellsten:** `create-next-app --tailwind`.
* **Manuell:** Tailwind + PostCSS installieren, `content`-Pfade setzen, `@tailwind`-Direktiven in `globals.css`.
* Danach Klassen direkt in JSX verwenden.
  Weiterlesen: Next.js **Installation** und **Tailwind-Guide**. ([Next.js][4])

[1]: https://nextjs.org/docs/app/api-reference/cli/create-next-app?utm_source=chatgpt.com "CLI: create-next-app"
[2]: https://tailwindcss.com/docs/guides/nextjs?utm_source=chatgpt.com "Install Tailwind CSS with Next.js"
[3]: https://nextjs.org/docs/app/guides/tailwind-v3-css?utm_source=chatgpt.com "Guides: Tailwind CSS v3"
[4]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"

  **[⬆ Наверх](#top)**

61. ### <a name="61"></a> Was ist styled-jsx?

**Definition:**
`styled-jsx` ist eine **eingebaute CSS-in-JS-Lösung** in Next.js, die automatisch mitkommt (keine Extra-Installation). Damit kannst du **komponentenbasiertes, scoped CSS** direkt in React-Komponenten schreiben. Jede Komponente bekommt dadurch **lokal gekapselte Styles**, ohne dass sie globale CSS-Klassen verschmutzt.

---

## **1. Funktionsweise**

* CSS wird in einem `<style jsx>`-Block geschrieben.
* Styles gelten **nur für die Komponente**, in der sie definiert sind.
* Klassen werden intern von Next.js automatisch umbenannt (Hashing).

---

## **2. Beispiel**

```jsx
export default function Button() {
  return (
    <>
      <button>Klick mich</button>
      <style jsx>{`
        button {
          background: blue;
          color: white;
          padding: 10px 20px;
          border-radius: 6px;
          cursor: pointer;
        }
        button:hover {
          background: darkblue;
        }
      `}</style>
    </>
  );
}
```

👉 Das CSS wirkt nur auf **diesen Button**, nicht auf andere Buttons im Projekt.

---

## **3. Globale Styles mit styled-jsx**

Falls nötig, kann man Styles global machen mit `:global(...)`:

```jsx
<style jsx>{`
  :global(body) {
    margin: 0;
    font-family: sans-serif;
  }
`}</style>
```

---

## **4. Vorteile**

* **Built-in in Next.js** → keine Extra-Library nötig.
* Styles sind **scoped** → keine Namenskonflikte.
* Ideal für **kleine Projekte oder einfache Komponenten**.

---

## **5. Nachteile**

* Weniger mächtig als Libraries wie **styled-components** oder **emotion**.
* Keine erweiterte Theming- oder TypeScript-Integration.
* Für große Projekte oft weniger flexibel als Tailwind oder CSS-Module.

---

**Zusammenfassung:**
`styled-jsx` ist die eingebaute CSS-in-JS-Lösung von Next.js, die **scoped CSS direkt in Komponenten** ermöglicht. Vorteile: keine Konflikte, out-of-the-box verfügbar. Nachteile: eingeschränkter Funktionsumfang gegenüber anderen CSS-in-JS-Frameworks.

📖 Quelle: [Next.js Docs – styled-jsx](https://nextjs.org/docs/pages/building-your-application/styling/css-in-js#built-in-css-support)

---

  **[⬆ Наверх](#top)**

62. ### <a name="62"></a> Wie verwendet man styled-components in Next.js?

**Definition:**
`styled-components` ist eine **CSS-in-JS-Bibliothek**, mit der du direkt in JavaScript/TypeScript **gestylte React-Komponenten** definierst. In Next.js kannst du sie nutzen, um **komponentenbasierte, dynamische Styles** zu schreiben – mit voller Unterstützung für Themes, Props und SSR.

---

## **1. Installation**

```bash
npm install styled-components
npm install -D babel-plugin-styled-components
```

---

## **2. Next.js konfigurieren**

Damit SSR funktioniert, braucht es ein Babel-Plugin.
**`next.config.js`:**

```js
/** @type {import('next').NextConfig} */
const nextConfig = {
  compiler: {
    styledComponents: true, // aktiviert SWC-Integration
  },
};

module.exports = nextConfig;
```

👉 Seit Next.js 12+ ist kein eigenes Babel-Setup mehr nötig, nur `compiler.styledComponents`.

---

## **3. Beispiel – Styled Button**

```jsx
"use client"; // nötig im App Router, weil styled-components Client-Side ist
import styled from "styled-components";

const Button = styled.button`
  background: blue;
  color: white;
  padding: 10px 20px;
  border-radius: 6px;
  cursor: pointer;

  &:hover {
    background: darkblue;
  }
`;

export default function Home() {
  return <Button>Klick mich</Button>;
}
```

---

## **4. Dynamische Styles mit Props**

```jsx
"use client";
import styled from "styled-components";

const Button = styled.button`
  background: ${(props) => (props.primary ? "blue" : "gray")};
  color: white;
  padding: 10px;
`;

export default function Home() {
  return (
    <>
      <Button>Standard</Button>
      <Button primary>Primary</Button>
    </>
  );
}
```

---

## **5. Theming**

```jsx
"use client";
import styled, { ThemeProvider } from "styled-components";

const theme = {
  colors: {
    primary: "blue",
    secondary: "gray",
  },
};

const Title = styled.h1`
  color: ${(props) => props.theme.colors.primary};
`;

export default function Page() {
  return (
    <ThemeProvider theme={theme}>
      <Title>Mit Theme</Title>
    </ThemeProvider>
  );
}
```

---

## **6. Besonderheiten im App Router (Next.js 13+)**

* **Alle Komponenten mit styled-components müssen `"use client"`** enthalten.
* SSR funktioniert automatisch mit `compiler.styledComponents: true`.
* Vorteil: Keine FOUC (Flash of Unstyled Content).

---

## **Zusammenfassung:**

* Installation: `styled-components` + SWC-Compiler in `next.config.js`.
* Nutze `"use client"` im App Router.
* Vorteile: **Scoped Styles, Props, Themes, SSR-Support**.
* Ideal für **komplexe UI-Logik** mit dynamischem Styling.

📖 Quelle: [Next.js Docs – CSS-in-JS (styled-components)](https://nextjs.org/docs/app/building-your-application/styling/css-in-js#styled-components)

---

  **[⬆ Наверх](#top)**

63. ### <a name="63"></a> Welche Best Practices gibt es für Styling in großen Next.js-Projekten?

**Best Practices für Styling in großen Next.js-Projekten**

---

### 1) Grundsätze & Architektur

* **Eine Haupt-Strategie wählen** (z. B. Tailwind **oder** CSS-Module + Design Tokens); Mischformen bewusst und sparsam.
* **Styles co-locaten**: Komponentennahe `*.module.css/.scss` statt große, zentrale Stylesheets.
* **Minimales Global-CSS** (Reset/Normierung, Layout-Primitive, Variablen).
* **Namenskonflikte vermeiden**: bevorzugt **CSS-Module** oder Utility-Klassen.

---

### 2) Design Tokens & Theming (CSS-Variablen)

* Farben, Spacing, Typografie als **CSS-Variablen** definieren; Thema per Klasse wechseln (z. B. `dark`).

```js
// app/globals.css
:root{ --color-bg:#fff; --color-fg:#111 }
.dark{ --color-bg:#111; --color-fg:#eee }
```

```js
// app/page.tsx
export default function Page(){
  return <main style={{ background:"var(--color-bg)", color:"var(--color-fg)" }}>…</main>
}
```

* Für Dark-Mode **class-based** Strategie verwenden (kein FOUC, einfacher SSR).

---

### 3) Tooling-Entscheidungen

* **CSS-Module** für komponentennahe Styles; **Sass** optional für Variablen/Mixins.
* **Tailwind CSS** für große Teams/Design-Systeme (einheitliche Tokens, geringe Spezifität, Purge automatisch).
* **CSS-in-JS** (z. B. styled-components) nur wo **dynamisches** Styling zur Laufzeit nötig ist; im App Router auf `"use client"` und Compiler-Option achten.

---

### 4) Performance & Core Web Vitals

* **`next/font`** nutzen (self-hosting, Subsetting, kein CLS).
* **Unnötiges CSS reduzieren** (Tailwind Purge / Content-Konfiguration korrekt setzen).
* **Geringe Spezifität & flaches Nesting** (max. 2–3 Ebenen).
* **Route-spezifisches CSS** per Import in der jeweiligen Seite/Komponente (keine globalen Sammel-Dateien).
* **Images** via `next/image` statt `<img>`.

---

### 5) DX & Qualität

* **Namenskonvention** (z. B. `ComponentName_part__state`) bei CSS-Modulen.
* **Hilfs-Libs** wie `clsx` für konditionale Klassen.
* **Linting** (z. B. Stylelint) + **Prettier**; CI prüft Build/Lint.
* **Storybook**/Playroom für isoliertes Testen der Styles.
* **Variablen/Utilities dokumentieren** (README oder Tokens-Seite).

---

### 6) App-Router-Spezifika (Next.js 13+)

* **Server Components** minimieren Client-JS → bevorzugt Styles, die **kein** Hydration-JS brauchen (CSS-Module/Tailwind).
* CSS-in-JS in **Client Components** kapseln; nur dort einsetzen, wo UI wirklich interaktiv/dynamisch ist.
* Globale Styles **einmal** im `app/layout.tsx` importieren.

---

### 7) Accessibility & System-Preferences

* **Sichtbare Focus-States**, ausreichender Kontrast.
* **`prefers-reduced-motion`** respektieren; Animationen sparsam und performant (transform/opacity).

---

### Kurzbeispiele

**CSS-Module (scoped)**

```js
// components/Button.module.css
.btn{ padding:.625rem 1rem; border-radius:.5rem; background:var(--color-fg); color:var(--color-bg) }
.btn--primary{ background:#3b82f6; color:#fff }
```

```js
// components/Button.tsx
import styles from "./Button.module.css";
export default function Button({ primary=false }){
  return <button className={`${styles.btn} ${primary?styles["btn--primary"]:""}`}>Klick</button>
}
```

**Tailwind (Utilities & Tokens)**

```js
// tailwind.config.js (Ausschnitt)
export default { theme:{ extend:{ colors:{ brand:"#3b82f6" } } } }
```

```js
// app/page.tsx
export default function Page(){
  return <div className="p-6 rounded-lg bg-brand text-white">Card</div>
}
```

---

**Zusammenfassung**

* **Konzentration auf eine Haupt-Strategie** (CSS-Module / Tailwind) + **CSS-Variablen als Tokens**.
* **Co-location, minimales Global-CSS, geringe Spezifität**, `next/font` und `next/image` für Performance.
* **CSS-in-JS selektiv** in Client Components, sonst serverfreundliche Ansätze nutzen.

**Quellen / Weiterlesen:**

* Next.js Installation & Setup: [https://nextjs.org/docs/app/getting-started/installation](https://nextjs.org/docs/app/getting-started/installation)
* Styling (App Router Übersicht): [https://nextjs.org/docs/app/building-your-application/styling](https://nextjs.org/docs/app/building-your-application/styling)
* CSS Modules: [https://nextjs.org/docs/app/building-your-application/styling/css-modules](https://nextjs.org/docs/app/building-your-application/styling/css-modules)
* Sass: [https://nextjs.org/docs/app/building-your-application/styling/sass](https://nextjs.org/docs/app/building-your-application/styling/sass)
* Fonts (`next/font`): [https://nextjs.org/docs/app/building-your-application/optimizing/fonts](https://nextjs.org/docs/app/building-your-application/optimizing/fonts)
* Images: [https://nextjs.org/docs/app/building-your-application/optimizing/images](https://nextjs.org/docs/app/building-your-application/optimizing/images)

  **[⬆ Наверх](#top)**

64. ### <a name="64"></a> Was macht automatisches Code-Splitting in Next.js?

**Definition:**
Automatisches **Code-Splitting** in Next.js bedeutet, dass der JavaScript-Code nicht als **ein großes Bundle**, sondern **seiten- bzw. komponentenbasiert** ausgeliefert wird. Jede Route bekommt nur den Code, den sie tatsächlich benötigt. Das reduziert Ladezeiten und verbessert die **Core Web Vitals**.

---

## **1. Wie funktioniert es?**

* **Per Page/Route:** Jede Datei in `pages/` oder `app/` wird automatisch ein eigener Entry Point.
* **Per Component Import:** Nur die Komponenten/Module, die auf einer Seite verwendet werden, landen im Bundle dieser Seite.
* **Shared Code:** Gemeinsamer Code (z. B. React, Layouts) wird in **separaten Chunks** ausgelagert und wiederverwendet.

---

## **2. Beispiel**

```jsx
// app/page.tsx (Startseite)
import Hero from "@/components/Hero";
export default function Home() {
  return <Hero />;
}
```

```jsx
// app/about/page.tsx (About-Seite)
import AboutSection from "@/components/AboutSection";
export default function About() {
  return <AboutSection />;
}
```

👉 Next.js erzeugt:

* Ein JS-Bundle für `/` (nur `Hero`)
* Ein JS-Bundle für `/about` (nur `AboutSection`)
* Gemeinsames Bundle für React/Next.js Core

➡ Beim Aufruf von `/` wird der Code von `/about` **nicht geladen**.

---

## **3. Dynamische Imports (manuelles Splitting)**

Zusätzlich kann man mit `next/dynamic` einzelne Komponenten **Lazy Loaden**:

```jsx
import dynamic from "next/dynamic";

const HeavyChart = dynamic(() => import("@/components/Chart"), {
  ssr: false, // nur Client-seitig
  loading: () => <p>Lade Chart...</p>,
});

export default function Dashboard() {
  return <HeavyChart />;
}
```

👉 Der Chart-Code wird nur geladen, wenn die Komponente wirklich gebraucht wird.

---

## **4. Vorteile**

* **Schnellere Ladezeiten** (geringeres Initial-Bundle).
* **Bessere Performance für Mobile & langsame Netze**.
* **Skalierbar**: Große Apps bleiben performant, da Nutzer nie den gesamten Code laden müssen.
* **SEO-freundlich** durch SSR + optimierte Bundles.

---

**Zusammenfassung:**
Automatisches Code-Splitting sorgt dafür, dass **nur der notwendige Code pro Seite/Route** ausgeliefert wird. Gemeinsamer Code wird ausgelagert, unnötiger Code nicht geladen. Mit `next/dynamic` lässt sich zusätzlich **Lazy Loading** für einzelne Komponenten aktivieren.

📖 Quelle: [Next.js Docs – Automatic Code Splitting](https://nextjs.org/docs/app/building-your-application/optimizing/automatic-code-splitting)

---

  **[⬆ Наверх](#top)**

65. ### <a name="65"></a> Wie funktioniert Lazy Loading?

**Definition:**
Lazy Loading bedeutet, dass **Ressourcen (z. B. Bilder oder Komponenten) erst dann geladen werden, wenn sie tatsächlich gebraucht werden** – statt direkt beim Initial-Load. Das spart Bandbreite, reduziert die **Initial Render Time** und verbessert Core Web Vitals.

---

## **1. Lazy Loading bei Bildern (`next/image`)**

* Standardmäßig lädt `next/image` Bilder **lazy**, sobald sie im Viewport erscheinen.
* Ausnahme: Wenn `priority` gesetzt ist → dann eager loading.

**Beispiel:**

```jsx
import Image from "next/image";

export default function Gallery() {
  return (
    <Image
      src="/images/photo.jpg"
      alt="Foto"
      width={600}
      height={400}
      // lazy loading ist default
    />
  );
}
```

---

## **2. Lazy Loading bei Komponenten (`next/dynamic`)**

* Große oder selten genutzte Komponenten kann man **on demand** laden.
* Next.js erzeugt dafür ein eigenes JS-Chunk.

**Beispiel:**

```jsx
import dynamic from "next/dynamic";

// Nur laden, wenn wirklich gerendert
const HeavyChart = dynamic(() => import("./Chart"), {
  loading: () => <p>Lade Chart...</p>, // Fallback während des Imports
});

export default function Dashboard() {
  return (
    <div>
      <h1>Dashboard</h1>
      <HeavyChart />
    </div>
  );
}
```

---

## **3. Lazy Loading von Routen**

* Next.js lädt nur den **Code für die aktuelle Route**.
* Navigiert der User zu einer neuen Seite, wird deren JS **nachgeladen**.
* → Dies ist Teil des **automatischen Code-Splittings**.

---

## **4. Vorteile**

* **Performance**: kleineres Initial-Bundle, schnellere Ladezeiten.
* **SEO**: Wichtige Inhalte können direkt gerendert werden, weniger kritische Ressourcen nachgeladen.
* **User Experience**: Ressourcen nur dann, wenn sie wirklich gebraucht werden.

---

**Zusammenfassung:**
Lazy Loading in Next.js bedeutet, dass **Bilder, Komponenten oder Routen erst bei Bedarf geladen werden**. Standardmäßig gilt das für Bilder (`next/image`) und Seiten (Code-Splitting). Für Komponenten wird es mit `next/dynamic` umgesetzt. Ergebnis: **schnellere Initial-Loads, bessere Performance, optimierte UX**.

📖 Quelle: [Next.js Docs – Dynamic Imports & Code Splitting](https://nextjs.org/docs/app/building-your-application/optimizing/automatic-code-splitting)

---

  **[⬆ Наверх](#top)**

66. ### <a name="66"></a> Wie optimiert man Bilder in Next.js?

**Ziele:**
Kleine Dateien, passende Auflösung/Format, spätes Laden. In Next.js geschieht das primär über **`next/image`** (integrierte Bildoptimierung).

---

## Empfohlener Standard: `next/image`

```js
// app/page.tsx
import Image from "next/image";

export default function Home() {
  return (
    <main>
      <Image
        src="/images/hero.jpg"   // aus /public
        alt="Hero"
        width={1200} height={600} // erzeugt responsive Varianten + srcset
        priority                  // Above-the-fold: eager laden
      />
    </main>
  );
}
```

* **Automatisch:** Responsive `srcset`, Lazy Loading (ohne `priority`), Format-Optimierung (WebP/AVIF, wenn möglich), Caching/CDN.

---

## Externe Bilder freigeben

```js
// next.config.js
export default {
  images: {
    domains: ["images.example.com"],
    // oder feiner:
    remotePatterns: [{ protocol: "https", hostname: "cdn.example.com", pathname: "/assets/**" }],
  },
};
```

---

## Responsives Layout & korrekte Größen

```js
// feste Breite/Höhe + 'sizes' für bessere Auswahl der Variante
<Image
  src="/images/card.jpg"
  alt="Card"
  width={800} height={500}
  sizes="(max-width: 768px) 100vw, 800px"
/>

// Vollflächig im Container
<div className="relative h-64">
  <Image src="/images/bg.jpg" alt="" fill style={{ objectFit: "cover" }} />
</div>
```

---

## Placeholder & Qualität

```js
// Blur-Placeholder (UX bei großen Bildern)
<Image
  src="/images/photo.jpg"
  alt="Foto"
  width={1200} height={800}
  placeholder="blur"
  blurDataURL="data:image/jpeg;base64,..." // optional, sonst automatisch bei statischem Import
/>

// Qualitäts-Tradeoff (Default 75)
<Image src="/images/photo.jpg" alt="" width={1200} height={800} quality={70} />
```

---

## Statischer Import (auto-Maße & Blur)

```js
// /public optional, besser: Import aus /app/(oder)/assets
import photo from "@/assets/photo.jpg";

<Image src={photo} alt="Foto" placeholder="blur" /> // Breite/Höhe aus dem Import
```

---

## Konfiguration & Feintuning

```js
// next.config.js – Gerätegrößen/Breakpoints feinjustieren
export default {
  images: {
    deviceSizes: [360, 640, 768, 1024, 1280, 1536],
    imageSizes: [16, 32, 48, 64, 96, 128, 256],
    formats: ["image/avif", "image/webp"],
  },
};
```

---

## Wann kein `next/image`?

* **SVG-Icons/Logos**: inline `<svg>` oder statisches `<img>` (keine Optimierung nötig).
* **GIFs**: lieber Video/animiertes WebP (deutlich kleiner).

---

## Häufige Fehler vermeiden

* **Breite/Höhe fehlen** → immer `width/height` oder `fill` angeben.
* **Falsche `sizes`** → führt zu zu großen Downloads auf Mobile.
* **Nicht freigegebene Domains** → externes Bild wird blockiert.

---

**Zusammenfassung:**
Bilder mit **`next/image`** einbinden, **Domains/Patterns** konfigurieren, **`sizes`** korrekt setzen, **Lazy Loading** nutzen, **AVIF/WebP** aktivieren, bei Bedarf **Blur-Placeholder** und **Qualitätsparameter**. SVG inline, GIF vermeiden.

📖 Quellen:

* Offizieller Einstieg: [https://nextjs.org/docs/app/getting-started/installation](https://nextjs.org/docs/app/getting-started/installation)
* Image Optimization & `next/image`: [https://nextjs.org/docs/app/building-your-application/optimizing/images](https://nextjs.org/docs/app/building-your-application/optimizing/images)

  **[⬆ Наверх](#top)**

67. ### <a name="67"></a> Wie verwendet man next/script zum Laden von Skripten?

**Definition:**
`next/script` ist eine spezielle Next.js-Komponente, um **externe oder interne JavaScript-Skripte performant einzubinden**. Im Gegensatz zu normalem `<script>`-Tag erlaubt sie die Kontrolle über das **Ladeverhalten** (`beforeInteractive`, `afterInteractive`, `lazyOnload`, `worker`) und sorgt für bessere Performance & Core Web Vitals.

---

## **1. Syntax**

```jsx
import Script from "next/script";

export default function Page() {
  return (
    <main>
      <h1>Mit next/script</h1>

      <Script
        src="https://example.com/script.js"
        strategy="afterInteractive"
        onLoad={() => console.log("Script geladen!")}
      />
    </main>
  );
}
```

---

## **2. Lade-Strategien**

* **`beforeInteractive`** → Lädt Skript **vor der Hydration**, wichtig für kritische Polyfills oder Libraries.
* **`afterInteractive`** (Default) → Lädt **nachdem die Seite interaktiv ist**.
* **`lazyOnload`** → Lädt **im Hintergrund**, nachdem die Seite komplett geladen ist.
* **`worker`** → Lädt Skript im **Web Worker** (über Partytown, experimentell).

---

## **3. Inline-Skripte**

Man kann auch Inline-JS einbinden:

```jsx
<Script id="inline-script" strategy="afterInteractive">
  {`console.log("Inline Script geladen!")`}
</Script>
```

---

## **4. Beispiel: Google Analytics**

```jsx
import Script from "next/script";

export default function Layout({ children }) {
  return (
    <html lang="de">
      <body>
        {children}

        {/* GA Library laden */}
        <Script
          src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"
          strategy="afterInteractive"
        />

        {/* GA initialisieren */}
        <Script id="ga-init" strategy="afterInteractive">
          {`
            window.dataLayer = window.dataLayer || [];
            function gtag(){dataLayer.push(arguments);}
            gtag('js', new Date());
            gtag('config', 'GA_TRACKING_ID');
          `}
        </Script>
      </body>
    </html>
  );
}
```

---

## **5. Vorteile gegenüber `<script>`**

* **Kontrolliertes Ladeverhalten** → kein Blockieren von Rendering.
* **Automatisches De-duping** → gleiche Skripte werden nicht doppelt geladen.
* **Bessere Performance** → optimiert für Core Web Vitals.
* **Callbacks (`onLoad`, `onError`)** für Debugging.

---

**Zusammenfassung:**
Mit `next/script` bindet man Skripte in Next.js **performant und kontrolliert** ein.

* Wichtige Strategie: `beforeInteractive`, `afterInteractive`, `lazyOnload`.
* Inline & externe Skripte unterstützt.
* Vorteile: **Performance, kein Blocking, kein doppeltes Laden**.

📖 Quelle: [Next.js Docs – Script](https://nextjs.org/docs/app/building-your-application/optimizing/scripts)

---

  **[⬆ Наверх](#top)**

68. ### <a name="68"></a> Was ist Static Optimization?

**Definition:**
Static Optimization in Next.js bedeutet, dass eine Seite **vollständig als statische HTML-Datei generiert wird**, wenn sie **keine serverseitigen Datenanforderungen** hat. Next.js erkennt dies automatisch und erstellt beim **Build** ein statisches HTML + minimalen JS, statt bei jedem Request den Server einzuschalten.

---

## **1. Wann greift Static Optimization?**

* Die Seite **enthält keine serverseitigen Data-Fetching-Funktionen** wie `getServerSideProps`.
* Sie verwendet **nur statischen Inhalt** oder clientseitiges Data Fetching (`useEffect + fetch`).
* Im App Router: wenn keine `fetch(..., { cache: "no-store" })` oder dynamischen Datenquellen genutzt werden.

👉 Ergebnis: Seite wird als **Static HTML + JS** beim Build erstellt.

---

## **2. Beispiel – Statische Seite**

```jsx
// pages/about.js
export default function About() {
  return <h1>Über uns</h1>;
}
```

➡ Kein Data Fetching → Next.js erstellt `about.html` während des Builds.

---

## **3. Beispiel – Mit Client-Fetching**

```jsx
// pages/index.js
import { useEffect, useState } from "react";

export default function Home() {
  const [data, setData] = useState(null);

  useEffect(() => {
    fetch("/api/hello")
      .then((res) => res.json())
      .then(setData);
  }, []);

  return <div>{data ? data.message : "Lade..."}</div>;
}
```

➡ HTML wird **statisch** gerendert, Daten kommen erst nach Hydration vom Client.

---

## **4. Unterschied zu SSG/SSR**

* **Static Optimization:** automatisch → statisches HTML ohne Data-Fetching.
* **SSG (getStaticProps):** Entwickler bestimmt explizit, welche Daten beim Build geholt werden.
* **SSR (getServerSideProps):** Seite wird bei jedem Request dynamisch auf dem Server erzeugt.

---

## **5. Vorteile**

* **Sehr schnell**: da statische Datei direkt aus CDN geliefert wird.
* **Skalierbar**: kein Server-Overhead bei jedem Request.
* **SEO-freundlich**: HTML liegt schon vor.

---

**Zusammenfassung:**
Static Optimization = **automatisches Erzeugen von statischen HTML-Seiten**, wenn keine serverseitigen Datenfunktionen genutzt werden. Sie macht Seiten extrem schnell und skalierbar, da sie wie klassische **statische Webseiten** aus dem CDN ausgeliefert werden können.

📖 Quelle: [Next.js Docs – Automatic Static Optimization](https://nextjs.org/docs/pages/building-your-application/rendering/automatic-static-optimization)

---

  **[⬆ Наверх](#top)**

69. ### <a name="69"></a> Wie reduziert man die Bundle-Größe in Next.js?

**Ziel:** möglichst wenig Client-JS ausliefern. Setze auf **Server Components**, Route-basiertes **Code-Splitting**, **Lazy Loading**, und „cherry-picked“ Importe.

---

### 1) Client-Bundle klein halten

* **Server Components bevorzugen**, nur wirklich interaktive Teile als Client markieren (`"use client"`). So landet weniger JS im Browser. ([Next.js][1])
* **Automatisches Code-Splitting** nutzen: Jede Route/Segment bekommt eigene Chunks; nur benötigter Code wird geladen. ([Next.js][2])

---

### 2) Große Abhängigkeiten nur bei Bedarf laden

```js
// Lazy Load für eine schwere Client-Komponente
"use client";
import dynamic from "next/dynamic";

const HeavyChart = dynamic(() => import("@/components/Chart"), {
  loading: () => <p>Lade…</p>,
  ssr: false, // falls die Lib Browser-APIs benötigt
});

export default function Page() {
  return <HeavyChart />;
}
```

* **Lazy Loading** reduziert Initial-Bundle; Komponenten/Libs kommen erst, wenn nötig. ([Next.js][3])

---

### 3) Paket-Imposte optimieren (Baum-Schütteln erleichtern)

```js
// next.config.js
export default {
  experimental: {
    optimizePackageImports: ["lucide-react", "@mui/icons-material"],
  },
};
```

* **`optimizePackageImports`** lädt nur tatsächlich genutzte Module – nützlich bei Icon-/UI-Libraries mit vielen Exports. ([Next.js][4])
* Zusätzlich: **modulare Importe** nutzen (z. B. `date-fns/format` statt Top-Level-Import). *(Allgemeine Praxis, ergänzt zu obigem Feature.)*

---

### 4) Analyse & Kontrolle

```js
// next.config.js
const withBundleAnalyzer = require("@next/bundle-analyzer")({
  enabled: process.env.ANALYZE === "true",
});
module.exports = withBundleAnalyzer({});
```

```bash
ANALYZE=true npm run build
```

* Mit **`@next/bundle-analyzer`** große Bundles/Module finden und zielgerichtet reduzieren. ([Next.js][5])

---

### 5) Fonts & Medien „kosten“ oft viel

* **`next/font`**: self-hosting + Subsetting → weniger Requests, kein CLS. ([Next.js][6])
* **`next/image`** nutzen: responsive Varianten, moderne Formate, Lazy Load → kleinere Transfers. *(indirekt hilft das dem JS-Budget, aber primär dem Gesamt-Payload.)* ([Next.js][7])

---

### 6) Weitere Praxistipps

* **Vermeide „Barrel Files“** mit massenhaft Re-Exports (erschwert Tree-Shaking). Setze stattdessen gezielte Imports ein. *(Allgemeine Praxis)*
* **Prefetch** nur da, wo sinnvoll; unnötiges Vorladen vermeiden. ([Next.js][8])
* **Kein globales `"use client"`** in Layouts – macht große Bereiche unnötig zu Client-Code. ([Next.js][1])

---

### Minimal-Checkliste (Quick Wins)

* Server Components Standard lassen ✅ ([Next.js][1])
* Schwere UI-Libs via `next/dynamic` lazy laden ✅ ([Next.js][3])
* `experimental.optimizePackageImports` für „fette“ Pakete aktivieren ✅ ([Next.js][9])
* Bundles regelmäßig mit `@next/bundle-analyzer` prüfen ✅ ([Next.js][5])
* Fonts über `next/font`, Bilder über `next/image` ✅ ([Next.js][6])

---

**Zusammenfassung**

* **Weniger Client-JS** durch Server Components und selektives `"use client"`.
* **Nur nötigen Code laden**: Route-Splitting + `next/dynamic`.
* **Imports schlank halten** mit `optimizePackageImports`.
* **Regelmäßig analysieren** (Bundle Analyzer) und **Medien optimieren** (`next/font`, `next/image`). ([Next.js][1])

📖 Weiterführend:

* Installation & Grundlagen (App Router): [Next.js – Getting Started / Installation]. ([Next.js][10])
* Paket-Bundling optimieren: ([Next.js][4])
* Lazy Loading (Guides): ([Next.js][3])
* Bundle-Analyse (Production Checklist & Plugin): ([Next.js][11])

[1]: https://nextjs.org/docs/app/getting-started/server-and-client-components?utm_source=chatgpt.com "Getting Started: Server and Client Components"
[2]: https://nextjs.org/learn/dashboard-app/navigating-between-pages?utm_source=chatgpt.com "App Router: Navigating Between Pages"
[3]: https://nextjs.org/docs/pages/guides/lazy-loading?utm_source=chatgpt.com "How to lazy load Client Components and libraries"
[4]: https://nextjs.org/docs/app/guides/package-bundling?utm_source=chatgpt.com "How to optimize package bundling"
[5]: https://nextjs.org/docs/14/pages/building-your-application/optimizing/bundle-analyzer?utm_source=chatgpt.com "Optimizing: Bundle Analyzer"
[6]: https://nextjs.org/docs/app/getting-started/fonts?utm_source=chatgpt.com "Getting Started: Font Optimization"
[7]: https://nextjs.org/docs/app?utm_source=chatgpt.com "Next.js Docs: App Router"
[8]: https://nextjs.org/docs/pages/guides/production-checklist?utm_source=chatgpt.com "Guides: Production"
[9]: https://nextjs.org/docs/app/api-reference/config/next-config-js/optimizePackageImports?utm_source=chatgpt.com "next.config.js: optimizePackageImports"
[10]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"
[11]: https://nextjs.org/docs/app/guides/production-checklist?utm_source=chatgpt.com "Guides: Production"

  **[⬆ Наверх](#top)**

70. ### <a name="70"></a> Wie optimiert man Lighthouse-Scores?

**Ziel:**
Lighthouse bewertet **Performance, Accessibility, Best Practices, SEO**. In Next.js erreichst du hohe Scores durch **kleine Bundles, optimierte Assets, korrektes Caching/Rendering** und saubere Semantik.

---

## Performance (LCP/CLS/TBT/TTI)

**Bilder optimieren (`next/image`)**

```js
// app/page.tsx
import Image from "next/image";

export default function Hero() {
  return (
    <Image
      src="/images/hero.jpg"
      alt="Hero"
      width={1600}
      height={900}
      priority // Above-the-fold → kein Lazy
      sizes="(max-width: 768px) 100vw, 1600px"
    />
  );
}
```

**Schriften optimieren (`next/font`)**

```js
// app/layout.tsx
import { Inter } from "next/font/google";
const inter = Inter({ subsets: ["latin"], display: "swap" });

export default function RootLayout({ children }) {
  return <body className={inter.className}>{children}</body>;
}
```

**Skripte nicht blockieren (`next/script`)**

```js
import Script from "next/script";

export default function Page() {
  return (
    <>
      <Script src="https://example.com/analytics.js" strategy="afterInteractive" />
      <Script id="inline" strategy="lazyOnload">{`console.log("ok")`}</Script>
    </>
  );
}
```

**Code-Splitting & Lazy Loading**

```js
import dynamic from "next/dynamic";
const HeavyChart = dynamic(() => import("@/components/Chart"), { ssr: false, loading: () => <p>Lade…</p> });

export default function Dashboard() {
  return <HeavyChart />;
}
```

**Server Components bevorzugen**
Nur interaktive Teile mit `"use client"` markieren → weniger Client-JS, besserer TBT/TTI.

**Cachen/Rendern richtig steuern (App Router)**

```js
// SSG (default, gecacht)
await fetch("https://api.example.com/data");

// SSR (immer frisch)
await fetch("https://api.example.com/data", { cache: "no-store" });

// ISR (periodische Aktualisierung)
await fetch("https://api.example.com/data", { next: { revalidate: 60 } });
```

**Preload/Preconnect für kritische Ressourcen (nur wenn nötig)**

```js
// app/layout.tsx (im <head> via metadata oder manuell)
<link rel="preconnect" href="https://cdn.example.com" />
<link rel="preload" as="image" href="/images/hero.jpg" />
```

**Bloat vermeiden**

* Große Libraries nur dort laden, wo gebraucht (dynamic import).
* `experimental.optimizePackageImports` für Icon-/UI-Pakete.
* `@next/bundle-analyzer` einsetzen und große Chunks reduzieren.

---

## Accessibility (A11y)

**Semantische HTML-Elemente & ARIA**

* Überschriften-Hierarchie (`h1`–`h6`) korrekt.
* Interaktive Elemente mit `button`, `a` + `aria-label` wo nötig.

**Fokus & Kontrast**

* Sichtbare Fokuszustände, ausreichender Farbkontrast.
* `alt`-Texte für alle Bilder (`next/image` verlangt `alt`).

---

## Best Practices

**Sichere Origin-Richtlinien**

* `Content-Security-Policy` Header (über Middleware/Hosting) setzen.
* Nur notwendige Third-Party-Skripte laden; keine veralteten APIs.

**Responsive & CLS-frei**

* Immer `width/height` **oder** `fill` bei Bildern angeben.
* UI-Schriften via `next/font` (kein Layout-Shift).

---

## SEO

**Meta & strukturierte Daten**

```js
// app/blog/[slug]/page.tsx
export const metadata = {
  title: "Artikel-Titel",
  description: "Kurzbeschreibung für die SERPs",
};
```

* Saubere URLs (file-based routing), korrekte `lang`-Attribute, sinnvolle Link-Texte.
* Sitemaps/robots unter `/public` bereitstellen.

---

## Diagnose & Monitoring

**Messen statt raten**

* `npm run build` → Warnungen beachten.
* Lighthouse/Pagespeed lokal & in CI laufen lassen.
* Web Vitals im Client reporten (LCP/CLS/FID) und in Analytics auswerten.

---

**Zusammenfassung**

* **Performance:** `next/image`, `next/font`, `next/script`, Server Components, Caching (SSG/SSR/ISR), Dynamic Imports.
* **A11y/SEO:** Semantik, Alt-Texte, Metadaten, saubere Struktur.
* **Bloat reduzieren:** nur benötigte Skripte/Libs laden, Bundles analysieren.
  Offizielle Doku (Einstieg & relevante Features): [Next.js – Installation & Guides](https://nextjs.org/docs/app/getting-started/installation)

  **[⬆ Наверх](#top)**

71. ### <a name="71"></a> Wie funktioniert der eingebaute SWC-Compiler?

**Definition:**
Der **SWC-Compiler** ist der eingebaute **Rust-basierte Compiler** von Next.js, der Babel und Teile von Terser ersetzt. Er wurde entwickelt, um **JavaScript/TypeScript-Transpilation, Minifizierung und Bundling** deutlich schneller zu machen (bis zu 20× schneller als Babel).

---

## **1. Hauptaufgaben**

* **Transpilation:**

  * Konvertiert modernen JS/TS (inkl. JSX, ES202x) in Browser-kompatiblen Code.
  * Unterstützt auch Dekoratoren, Class Fields, etc.

* **Minifizierung:**

  * Komprimiert und optimiert den Code im Production-Build.
  * Weniger Bundle-Größe, schnellere Ladezeiten.

* **React-Optimierungen:**

  * Automatische Unterstützung für **JSX-Transform**.
  * Entfernt `propTypes`, fügt Development-Checks hinzu.

* **Integration mit Next.js:**

  * Standardmäßig aktiviert, keine zusätzliche Konfiguration nötig.
  * Unterstützt Features wie `styled-components`, Emotion, Relay, etc. über `compiler`-Optionen.

---

## **2. Beispiel – Konfiguration in `next.config.js`**

```js
// next.config.js
const nextConfig = {
  compiler: {
    styledComponents: true,  // Aktiviert styled-components Unterstützung
    emotion: true,           // Für Emotion (CSS-in-JS)
    removeConsole: { exclude: ["error"] }, // Entfernt console.log im Build
  },
};

module.exports = nextConfig;
```

---

## **3. Unterschiede zu Babel/Terser**

| Aufgabe                   | Früher (Babel/Terser) | Heute (SWC)                          |
| ------------------------- | --------------------- | ------------------------------------ |
| **Sprache transpilieren** | Babel (langsam in JS) | SWC (Rust, sehr schnell)             |
| **Minifizierung**         | Terser                | SWC integriert                       |
| **Konfiguration**         | `.babelrc` nötig      | Next.js-Optionen im `next.config.js` |
| **Geschwindigkeit**       | Langsamer             | 10–20× schneller                     |

---

## **4. Vorteile**

* Sehr schnelle Builds & Refresh-Zeiten.
* Weniger externe Abhängigkeiten (kein Babel/Terser notwendig).
* Optimiert für **Next.js App Router** und moderne Features.

---

## **5. Einschränkungen**

* Weniger flexibel als Babel (manche exotischen Plugins fehlen).
* Für spezielle Babel-Plugins → `next/babel` verwenden (Fallback).

---

**Zusammenfassung:**
Der eingebaute **SWC-Compiler** in Next.js ist ein extrem schneller **Rust-basierter Transpiler und Minifier**, der Babel und Terser ersetzt. Er sorgt für **schnelle Builds, kleinere Bundles** und unterstützt nativ moderne Features wie JSX, TypeScript und CSS-in-JS.

📖 Quelle: [Next.js Docs – SWC](https://nextjs.org/docs/app/building-your-application/configuring/swc)

---

  **[⬆ Наверх](#top)**

72. ### <a name="72"></a> Was sind Edge Functions und wie unterscheiden sie sich von Serverless Functions?

**Definition:**

* **Serverless Functions**: Kleine Funktionen, die „on demand“ in der Cloud ausgeführt werden. Sie laufen meist in einer isolierten **Container- oder VM-Umgebung** (z. B. AWS Lambda).
* **Edge Functions**: Werden am **Netzwerkrand (Edge)** auf speziellen **Edge-Runtimes (z. B. V8 Isolate)** ausgeführt. Sie starten extrem schnell und sind **näher am Nutzer**, haben aber eine eingeschränkte Umgebung.

---

## **1. Serverless Functions**

* **Ort**: laufen in Rechenzentren (Regionen).
* **Startzeit**: Cold Starts können mehrere 100 ms dauern.
* **Umgebung**: volle Node.js-APIs (z. B. `fs`, größere Libraries).
* **Einsatz**: komplexe Business-Logik, längere Berechnungen, Datenbank-Queries.

**Beispiel in Next.js (Pages Router):**

```js
// pages/api/hello.js
export default function handler(req, res) {
  res.status(200).json({ message: "Hallo von Serverless Function" });
}
```

---

## **2. Edge Functions**

* **Ort**: laufen direkt auf **CDN-Knoten (Edge)** weltweit.
* **Startzeit**: nahezu **kein Cold Start** (ms-Bereich).
* **Umgebung**: Web-Standard-APIs wie `fetch`, `Request`, `Response`; **kein Node.js-API** (`fs`, `net`, etc. nicht verfügbar).
* **Einsatz**: Authentifizierung, Geolocation, Header-Manipulation, AB-Tests, Middleware.

**Beispiel in Next.js (App Router – Edge Runtime):**

```ts
// app/api/edge/route.ts
export const runtime = "edge";

export async function GET() {
  return new Response(JSON.stringify({ message: "Hallo von Edge Function" }), {
    headers: { "Content-Type": "application/json" },
  });
}
```

---

## **3. Vergleich**

| Merkmal            | **Serverless Functions**                   | **Edge Functions**                 |
| ------------------ | ------------------------------------------ | ---------------------------------- |
| **Ausführungsort** | Regionale Rechenzentren (z. B. AWS Lambda) | CDN Edge-Nodes, nahe beim Nutzer   |
| **Cold Start**     | bis zu mehrere 100 ms                      | wenige Millisekunden               |
| **Umgebung**       | Node.js (voller Zugriff)                   | Web-APIs (kein Node.js)            |
| **Laufzeit**       | Sekunden bis Minuten                       | sehr kurz (ms – Sekunden)          |
| **Use Cases**      | komplexe Logik, DB-Queries, APIs           | Auth, Caching, Routing, Middleware |

---

**Zusammenfassung:**

* **Serverless Functions**: flexibler, mehr APIs, aber langsamer (Cold Starts, zentrale Regionen).
* **Edge Functions**: extrem schnell, global verteilt, aber eingeschränkt (nur Web-APIs, keine Node.js-Funktionen).
  👉 Empfehlung: **Edge für leichtgewichtige, globale Aufgaben** (Auth, Routing, Headers), **Serverless für komplexe Backends**.

📖 Quelle: [Next.js Docs – Edge & Serverless Functions](https://nextjs.org/docs/app/building-your-application/rendering/edge-and-serverless)

---

  **[⬆ Наверх](#top)**

73. ### <a name="73"></a> Welche Sicherheitsrisiken gibt es in Next.js-Projekten?

**Häufige Sicherheitsrisiken in Next.js-Projekten**

---

## **1. Cross-Site Scripting (XSS)**

* **Gefahr**: Einschleusen von schädlichem JS durch unsichere Eingaben oder `dangerouslySetInnerHTML`.
* **Beispiel:**

```jsx
// ❌ unsicher
<div dangerouslySetInnerHTML={{ __html: req.query.content }} />
```

* **Best Practice:** niemals ungefiltertes HTML rendern → Escape oder Libraries wie `dompurify` nutzen.

---

## **2. Cross-Site Request Forgery (CSRF)**

* **Gefahr**: Nutzer führt ungewollte Aktionen (z. B. Formular-Submit) in eingeloggtem Zustand aus.
* **Abwehr:**

  * CSRF-Tokens (z. B. `next-auth` integriert dies).
  * Nur `POST` für zustandsverändernde Requests, SameSite-Cookies.

---

## **3. SQL Injection / NoSQL Injection**

* **Gefahr**: Unsichere Query-Strings führen zu manipulierten Datenbankabfragen.
* **Abwehr:**

  * Parameterisierte Queries nutzen (`prisma`, `mongoose`, `pg`).
  * Niemals Benutzereingaben direkt in Queries einfügen.

---

## **4. Unsichere API Routes**

* **Gefahr:** Unauthentifizierte Zugriffe auf `/api/...`.
* **Abwehr:**

  * Authentifizierung & Autorisierung implementieren.
  * Tokens, Sessions oder Middleware nutzen.

```ts
// Beispiel Middleware
import { NextResponse } from "next/server";
export function middleware(req) {
  const token = req.cookies.get("auth_token");
  if (!token) return NextResponse.redirect("/login");
}
```

---

## **5. Datenlecks über `getServerSideProps` oder `getStaticProps`**

* **Gefahr:** sensible Daten im JSON-Response an den Client.
* **Abwehr:** Nur benötigte, nicht sensible Daten weitergeben.

---

## **6. Clickjacking**

* **Gefahr:** App wird in fremdem `<iframe>` geladen → User klickt ungewollt.
* **Abwehr:** HTTP-Header `X-Frame-Options: DENY` oder `Content-Security-Policy: frame-ancestors 'none'`.

---

## **7. Unsichere Drittanbieter-Skripte**

* **Gefahr:** Externe JS-Libraries können kompromittiert sein.
* **Abwehr:**

  * `next/script` mit Strategie (`afterInteractive`, `lazyOnload`).
  * CSP (Content Security Policy) einsetzen.

---

## **8. Session Handling & Cookies**

* **Risiken:**

  * Session Hijacking bei unsicherem Cookie-Setup.
* **Abwehr:**

  * Cookies mit `HttpOnly`, `Secure`, `SameSite=strict`.
  * Keine sensiblen Daten im LocalStorage.

---

## **9. Directory Traversal & Public Folder**

* **Gefahr:** Über `/public` versehentlich sensible Dateien zugänglich machen.
* **Abwehr:** nur statische Assets dort speichern.

---

## **10. Denial of Service (DoS)**

* **Gefahr:** Teure SSR/DB-Queries blockieren Server.
* **Abwehr:**

  * **Caching (ISR, CDN)** nutzen.
  * **Rate Limiting** bei API Routes einbauen.

---

**Zusammenfassung:**
Die größten Risiken in Next.js sind **XSS**, **unsichere API Routes**, **CSRF**, **Injection-Angriffe**, **sensible Daten im Client**, sowie **unsichere externe Skripte**. Schutz durch: **Escape & Validierung, sichere Cookies, Auth in API Routes, CSP, Rate Limiting, Caching**.

📖 Quelle: [Next.js Security Best Practices](https://nextjs.org/docs/app/building-your-application/securing)

---

  **[⬆ Наверх](#top)**

74. ### <a name="74"></a> Wie schützt man API Routes?

**Ziele:**
API-Routen vor **unauthorisiertem Zugriff**, **Missbrauch** (Rate-Limiting), **Injection/XSS**, **CSRF** und **CORS-Problemen** schützen.

---

## 1) Authentifizieren & Autorisieren

**App Router – Route Handler:**

```js
// app/api/secret/route.ts
import { cookies } from "next/headers";

export async function GET() {
  const session = (await cookies()).get("session"); // HttpOnly-Token
  if (!session) return new Response("Unauthorized", { status: 401 });

  // Optional: Rollen/Scopes prüfen (RBAC/ABAC)
  return Response.json({ ok: true });
}
```

* Zugriff auf Cookies/Headers direkt im Handler; Tokens serverseitig prüfen. ([Next.js][1])

**Pages Router – API Route:**

```js
// pages/api/secret.ts
export default function handler(req, res) {
  const token = req.cookies.auth;
  if (!token) return res.status(401).json({ error: "Unauthorized" });
  return res.status(200).json({ ok: true });
}
```

* Für komplexe Auth: z. B. NextAuth.js (`getToken()` / `getSession()`). ([next-auth.js.org][2])

---

## 2) Globale Schutzschicht mit Middleware (Edge)

```js
// middleware.ts – vor allen /api/* prüfen
import { NextResponse } from "next/server";
import type { NextRequest } from "next/server";

export function middleware(req: NextRequest) {
  if (req.nextUrl.pathname.startsWith("/api/")) {
    const auth = req.cookies.get("session")?.value;
    if (!auth) return NextResponse.json({ error: "Unauthorized" }, { status: 401 });
  }
  return NextResponse.next();
}
```

* Läuft vor Routes (auch vor Cache); ideal für Auth-Gates, Geofencing, Header-Policies. ([Next.js][3])

---

## 3) Rate Limiting (einfaches Beispiel)

```js
// app/api/data/route.ts
export const runtime = "edge"; // schnelle Startzeiten

const WINDOW = 60_000; // 1 min
const LIMIT = 60;      // 60 req/min
const store = new Map<string, { count: number; ts: number }>();

export async function GET(req: Request) {
  const ip = req.headers.get("x-forwarded-for") ?? "unknown";
  const now = Date.now();
  const item = store.get(ip) ?? { count: 0, ts: now };
  if (now - item.ts > WINDOW) { item.count = 0; item.ts = now; }
  if (++item.count > LIMIT) return new Response("Too Many Requests", { status: 429 });
  store.set(ip, item);
  return Response.json({ ok: true });
}
```

> In Produktion: **persistente Stores** (Redis) statt In-Memory, sonst skaliert nicht horizontal. *(Best Practice)*

---

## 4) Eingaben validieren & ausgehende Daten härten

```js
// Beispiel mit Zod (Schema-Validierung vor DB-Operationen)
import { z } from "zod";
const Body = z.object({ email: z.string().email(), name: z.string().min(1) });

export async function POST(req: Request) {
  const data = Body.parse(await req.json()); // wirft bei Invalid
  // … sichere DB-Query (parametrisiert/ORM)
  return Response.json({ ok: true });
}
```

* Verhindert Injection/Deserialization-Probleme; immer **parametrisierte Queries**/ORM nutzen. *(Best Practice)*

---

## 5) CORS strikt konfigurieren (nur wenn nötig)

```js
// app/api/public/route.ts
export async function GET() {
  return new Response("ok", {
    headers: {
      "Access-Control-Allow-Origin": "https://your-frontend.example",
      "Access-Control-Allow-Methods": "GET,POST",
      "Access-Control-Allow-Headers": "content-type, authorization",
    },
  });
}
```

* CORS nur öffnen, wenn die API **von externen Origins** konsumiert wird. *(Best Practice)*

---

## 6) CSRF berücksichtigen (Pages Router/Form-POSTs)

* Zustandsänderungen **nicht** per GET; CSRF-Token prüfen; Cookies `SameSite=Strict/Lax`, `HttpOnly`, `Secure`. *(Best Practice)*
* Im App Router bei **reinen Fetch-APIs** mit Token-Auth (Bearer/JWT) oft ausreichend. *(Best Practice)*

---

## 7) Security-Header & Cookies

* Cookies: `HttpOnly`, `Secure`, `SameSite=Strict`, `Path`/`Domain` bewusst setzen. In Middleware/Route Handler setz-/lesbar. ([Next.js][4])
* Header: `Content-Security-Policy`, `X-Frame-Options`/`frame-ancestors`, `Referrer-Policy` über Middleware/Hosting setzen. *(Best Practice)*

---

## 8) Monitoring & Hardening

* **Logs/Audit** auf API-Ebenen; 4xx/5xx beobachten.
* **Production-Checkliste** von Next.js prüfen; nur notwendige Third-Party-Skripte laden. *(Best Practice)*

---

**Zusammenfassung**

* **Auth & RBAC** direkt im Route Handler prüfen; **Middleware** als globales Gate.
* **Rate Limiting, CORS, CSRF, Input-Validierung** konsequent einsetzen.
* **Sichere Cookies/Headers** und **parametrisierte DB-Zugriffe** verwenden; Monitoring aktiv halten.
  Quellen: **Installation/Grundlagen**, **Route Handlers**, **Middleware**, **Cookies/Headers**, **Auth-Guide**. ([Next.js][5])

[1]: https://nextjs.org/docs/app/api-reference/functions/cookies?utm_source=chatgpt.com "Functions: cookies"
[2]: https://next-auth.js.org/tutorials/securing-pages-and-api-routes?utm_source=chatgpt.com "Securing pages and API routes"
[3]: https://nextjs.org/docs/14/app/building-your-application/routing/middleware?utm_source=chatgpt.com "Middleware - Routing"
[4]: https://nextjs.org/docs/app/api-reference/functions/next-request?utm_source=chatgpt.com "Functions: NextRequest"
[5]: https://nextjs.org/docs/app?utm_source=chatgpt.com "Next.js Docs: App Router"

  **[⬆ Наверх](#top)**

75. ### <a name="75"></a> Wie implementiert man Authentifizierung in Next.js?

**Kurzübersicht:**
In Next.js (App Router) gibt es zwei gängige Wege:

1. **Auth.js (NextAuth v5)** – fertige Lösung mit OAuth, Sessions, Middleware-Integration.
2. **Custom Auth** – eigene Route Handlers + Cookies + Middleware.
   Next.js empfiehlt für die meisten Apps eine Auth-Library und zeigt zusätzlich ein „from scratch“-Muster mit Server Actions, Cookies und Middleware. ([Next.js][1])

---

## 1) Empfohlen: Auth.js (NextAuth v5) im App Router

**Installieren & Grundsetup**

```bash
npm install next-auth@beta
```

```js
// auth.ts (Projektroot)
import NextAuth from "next-auth";
import GitHub from "next-auth/providers/github";

export const { handlers, auth, signIn, signOut } = NextAuth({
  providers: [GitHub],
  session: { strategy: "jwt" },
});
```

```js
// app/api/auth/[...nextauth]/route.ts
import { handlers } from "@/auth";
export const { GET, POST } = handlers;
```

```js
// middleware.ts – optional: Session frisch halten / schützen
export { auth as middleware } from "@/auth";
```

```js
// app/dashboard/page.tsx – Schutz im Server Component
import { auth } from "@/auth";
import { redirect } from "next/navigation";

export default async function Dashboard() {
  const session = await auth();
  if (!session) redirect("/login");
  return <h1>Hi {session.user?.name}</h1>;
}
```

* `auth()` liefert die Session in Server Components; `handlers` stellt die `/api/auth`-Routen bereit; Middleware kann global schützen. ([authjs.dev][2])

---

## 2) Custom Auth: Cookies, Route Handlers, Middleware

**Login-Endpoint (setzt HttpOnly-Cookie)**

```js
// app/api/login/route.ts
import { cookies } from "next/headers";

export async function POST(request) {
  const { email, password } = await request.json();
  // TODO: Prüfen gegen eigene User-DB/Provider
  const token = "signed.jwt.token";
  cookies().set("session", token, {
    httpOnly: true, secure: true, sameSite: "lax", path: "/", maxAge: 60 * 60 * 24,
  });
  return Response.json({ ok: true });
}
```

**Middleware – nur eingeloggte Nutzer zu /app/**

```js
// middleware.ts
import { NextResponse } from "next/server";
import type { NextRequest } from "next/server";

export function middleware(req: NextRequest) {
  if (req.nextUrl.pathname.startsWith("/app/")) {
    const hasSession = req.cookies.get("session")?.value;
    if (!hasSession) return NextResponse.redirect(new URL("/login", req.url));
  }
  return NextResponse.next();
}

export const config = { matcher: ["/app/:path*"] };
```

**Server-seitige Prüfung in einer Seite**

```js
// app/app/page.tsx
import { cookies } from "next/headers";
import { redirect } from "next/navigation";

export default async function AppHome() {
  const token = (await cookies()).get("session")?.value;
  if (!token) redirect("/login");
  // TODO: Token verifizieren, User laden
  return <p>Willkommen!</p>;
}
```

* Next.js zeigt im Guide genau dieses Muster (Form → Server Action/Handler → Cookie setzen → Middleware/Server-Check). Wichtige Cookie-Flags: `HttpOnly`, `Secure`, `SameSite`. ([Next.js][1])

---

## 3) Hinweise & Best Practices

* **Middleware** schützt früh (vor Rendering/Cache) → gut für Auth-Gates/Geofencing. ([Next.js][3])
* **Route Handlers** sind die App-Router-Entsprechung zu API Routes. ([Next.js][4])
* **Auth-Flows & Sessions**: Auth-Library (z. B. Auth.js) vereinfacht Sign-In/Out, Session-Refresh und Route-Protection. ([authjs.dev][5])
* **Startpunkt / Setup**: offizielle Next.js-Installation & Projektstruktur. ([Next.js][1])

---

**Zusammenfassung**

* **Schnell & sicher:** Auth.js (NextAuth v5) – `auth.ts`, `handlers`, `auth()`, Middleware.
* **Flexibel:** Eigene Route Handlers + `cookies()` + Middleware + (optional) Server Actions.
* **Immer:** HttpOnly-Cookies, minimale Rechte, Prüfungen serverseitig/Middleware.

**Weiterlesen:**

* Next.js **Authentication Guide** (App Router) ([Next.js][1])
* Auth.js **Installation & Setup** (v5) ([authjs.dev][2])
* Next.js **Route Handlers & Middleware** ([Next.js][4])
* Einstieg/Setup: **Installation** ([Next.js][1])

[1]: https://nextjs.org/docs/app/guides/authentication "Guides: Authentication | Next.js"
[2]: https://authjs.dev/getting-started/installation "Auth.js | Installation"
[3]: https://nextjs.org/docs/14/app/building-your-application/routing/middleware?utm_source=chatgpt.com "Middleware - Routing"
[4]: https://nextjs.org/docs/app/getting-started/route-handlers-and-middleware?utm_source=chatgpt.com "Getting Started: Route Handlers and Middleware"
[5]: https://authjs.dev/getting-started/session-management/login?utm_source=chatgpt.com "Handling Signin and Signout"

  **[⬆ Наверх](#top)**

76. ### <a name="76"></a> Was ist NextAuth.js und wie funktioniert es?

**Definition**
**NextAuth.js** (heute **Auth.js** für Next.js) ist eine **vollständige Authentifizierungs-Lösung** für Next.js mit Support für **OAuth-Provider (Google, GitHub …)**, **Credentials**, **Sessions (JWT/DB)**, **Middleware-Schutz** und **App Router-Integration** über Route Handlers. ([authjs.dev][1])

---

### Kernprinzipien

* **Provider-basiert:** Fertige OAuth-Provider + eigene Provider/Anmeldelogik. ([next-auth.js.org][2])
* **Sessions:** JWT (stateless) oder persistente Session via Adapter/DB. ([authjs.dev][1])
* **App Router-Flow (v5):** zentrale `auth.ts` Datei → exportiert `handlers` (API), `auth()` (Session serverseitig), `signIn`/`signOut` (Server Actions). ([authjs.dev][1])
* **Route-Schutz:** per **Middleware** (früher Zugriff) oder **serverseitiger Check** in Pages/Layouts. ([Next.js][3])

---

### Minimal-Setup (App Router, v5)

```js
// auth.ts (Projektroot)
import NextAuth from "next-auth";
import GitHub from "next-auth/providers/github";

export const {
  handlers: { GET, POST },
  auth,
  signIn,
  signOut,
} = NextAuth({
  providers: [
    GitHub({
      clientId: process.env.GITHUB_ID,
      clientSecret: process.env.GITHUB_SECRET,
    }),
  ],
  session: { strategy: "jwt" },
});
```

```js
// app/api/auth/[...nextauth]/route.js
export { GET, POST } from "@/auth";
```

* Route Handlers sind der empfohlene Weg im App Router. ([next-auth.js.org][4])

---

### Route schützen (Server Component)

```js
// app/dashboard/page.js
import { auth } from "@/auth";
import { redirect } from "next/navigation";

export default async function Dashboard() {
  const session = await auth();
  if (!session) redirect("/login");
  return <h1>Hi {session.user?.name}</h1>;
}
```

* Serverseitiger Zugriff auf die Session in Routen/Layouts. ([Next.js][3])

---

### Sign-in / Sign-out (Server Actions)

```js
// app/login/page.js
import { signIn, signOut } from "@/auth";

export default function Login() {
  return (
    <main>
      {/* OAuth-Login per Server Action */}
      <form action={async () => { "use server"; await signIn("github"); }}>
        <button>Mit GitHub anmelden</button>
      </form>

      <form action={async () => { "use server"; await signOut(); }}>
        <button>Abmelden</button>
      </form>
    </main>
  );
}
```

* `signIn`/`signOut` werden aus `auth.ts` bereitgestellt und in Server Actions genutzt. ([authjs.dev][5])

---

### Middleware-Schutz (optional, Edge)

```js
// middleware.js
export { auth as middleware } from "@/auth";
```

* Einheitlicher Gatekeeper vor Seiten & API-Routen. **`NEXTAUTH_SECRET`** konfigurieren. ([next-auth.js.org][6])

---

### Pages Router (v4) – nur der Vollständigkeit halber

```js
// pages/api/auth/[...nextauth].js
import NextAuth from "next-auth";
import GithubProvider from "next-auth/providers/github";
export default NextAuth({ providers: [GithubProvider({ clientId: "...", clientSecret: "..." })] });
```

* V4 setzt API Route ein; App Router nutzt Route Handlers. ([next-auth.js.org][7])

---

### Typische Erweiterungen

* **Adapter** (Prisma, MongoDB, etc.) für persistente User/Sessions.
* **Callbacks** zum Anpassen von JWT/Session und Autorisierung. ([authjs.dev][1])

---

**Zusammenfassung**
NextAuth.js/**Auth.js** liefert eine **schnell integrierbare, flexible Auth** für Next.js: Provider konfigurieren, `auth.ts` anlegen, **handlers** für `/api/auth`, **`auth()`** für serverseitige Session, **`signIn`/`signOut`** in Server Actions und optional **Middleware** für Schutz. Ideal für App Router-Apps mit OAuth oder Credentials.
Quellen: Next.js **Authentication Guide**, **Route Handlers** & **Installation**, Auth.js **Installation/Quickstart**, **OAuth-Provider**, **v5-Migration**. ([Next.js][3])

**Zusatz — Projektbasis**: Einstieg & Grundgerüst mit Next.js: Installation/Struktur. ([Next.js][8])

[1]: https://authjs.dev/getting-started/installation?utm_source=chatgpt.com "Auth.js | Installation"
[2]: https://next-auth.js.org/configuration/providers/oauth?utm_source=chatgpt.com "OAuth"
[3]: https://nextjs.org/docs/app/guides/authentication?utm_source=chatgpt.com "Guides: Authentication"
[4]: https://next-auth.js.org/configuration/initialization?utm_source=chatgpt.com "Initialization | NextAuth.js"
[5]: https://authjs.dev/getting-started/session-management/login?utm_source=chatgpt.com "Handling Signin and Signout"
[6]: https://next-auth.js.org/configuration/nextjs?utm_source=chatgpt.com "Next.js"
[7]: https://next-auth.js.org/getting-started/example?utm_source=chatgpt.com "Getting Started | NextAuth.js"
[8]: https://nextjs.org/docs/pages/guides/authentication?utm_source=chatgpt.com "Guides: Authentication"

  **[⬆ Наверх](#top)**

77. ### <a name="77"></a> Wie speichert man Sessions in Next.js?

**Kurzüberblick**
Sessions in Next.js werden typischerweise als **JWT oder Session-ID im HttpOnly-Cookie** gespeichert. Lesen/Schreiben erfolgt im **App Router** über **Route Handlers** (und **Server Actions**); in **Server Components** darfst du **nur lesen**. Für „batteries-included“ nutzt man **Auth.js (NextAuth)**, ansonsten eine **Custom-Lösung** mit Cookies + optionalem Store (DB/Redis). ([Next.js][1])

---

## 1) Custom-Session mit HttpOnly-Cookie (App Router)

**Login → Cookie setzen (Route Handler)**

```js
// app/api/login/route.js
import { cookies } from "next/headers";

export async function POST(request) {
  const { email, password } = await request.json();
  // TODO: Benutzer prüfen, Token bauen/signieren
  const token = "signed.jwt.token";

  (await cookies()).set("session", token, {
    httpOnly: true, secure: true, sameSite: "lax", path: "/", maxAge: 60 * 60 * 24
  });

  return Response.json({ ok: true });
}
```

* **Route Handlers** sind die App-Router-Variante für API-Logik; hier kannst du Cookies **setzen/löschen**. ([Next.js][2])

**Zugriff serverseitig (lesen in Server Component)**

```js
// app/app/page.js
import { cookies } from "next/headers";
import { redirect } from "next/navigation";

export default async function AppHome() {
  const session = (await cookies()).get("session")?.value; // nur lesen
  if (!session) redirect("/login");
  // TODO: JWT verifizieren / User laden
  return <p>Willkommen!</p>;
}
```

* In **Server Components**: `cookies()` → **lesen erlaubt**, Schreiben nur in **Route Handlers/Server Actions**. ([Next.js][1])

**Optional: globaler Schutz via Middleware**

```js
// middleware.js
import { NextResponse } from "next/server";

export function middleware(req) {
  if (req.nextUrl.pathname.startsWith("/app/") && !req.cookies.get("session")) {
    return NextResponse.redirect(new URL("/login", req.url));
  }
  return NextResponse.next();
}

export const config = { matcher: ["/app/:path*"] };
```

* Middleware läuft **vor** den Routen (gut für Auth-Gates/Caching-Bypass). ([Next.js][3])

> Hinweis: Für **stateful Sessions** speicherst du statt JWT eine **Session-ID** im Cookie und legst Sitzungsdaten in **DB/Redis** ab.

---

## 2) Sessions mit Auth.js (NextAuth) – „fertige“ Lösung

**Setup (v5, App Router)**

```js
// auth.js
import NextAuth from "next-auth";
import GitHub from "next-auth/providers/github";

export const { handlers, auth, signIn, signOut } = NextAuth({
  providers: [GitHub({ clientId: process.env.GITHUB_ID, clientSecret: process.env.GITHUB_SECRET })],
  session: { strategy: "jwt" } // alternativ: DB-Session via Adapter
});
```

```js
// app/api/auth/[...nextauth]/route.js
export const { GET, POST } = handlers;
```

```js
// app/dashboard/page.js  – serverseitiger Session-Check
import { auth } from "@/auth";
import { redirect } from "next/navigation";

export default async function Dashboard() {
  const session = await auth();
  if (!session) redirect("/login");
  return <h1>Hi {session.user?.name}</h1>;
}
```

* v5 stellt **Route Handlers**, **`auth()`** (Session in Server Components) sowie **Sign-In/Out** bereit. **JWT oder DB-Session** wählbar. ([authjs.dev][4])

---

## 3) Best Practices

* **Cookies sicher setzen:** `HttpOnly`, `Secure`, `SameSite` passend wählen. ([Next.js][5])
* **Früh prüfen:** Zugriff mit **Middleware** schützen, um unnötiges Rendering zu vermeiden. ([Next.js][3])
* **Trennung beachten:** **Lesen** in Server Components, **Schreiben** in Route Handlers/Server Actions. ([Next.js][1])

---

**Zusammenfassung**

* **Custom:** HttpOnly-Cookie (JWT oder Session-ID) in **Route Handler** setzen; in **Server Components** aus `cookies()` lesen; optional **Middleware** als Gate.
* **Auth.js:** schnelle Integration mit **providers**, **`auth()`**, **handlers**, wahlweise **JWT-** oder **DB-Sessions**.
  Weiterlesen: **Installation/Setup** · **Authentication-Guide** · **Cookies** · **Route Handlers**. ([Next.js][6])

[1]: https://nextjs.org/docs/app/api-reference/functions/cookies?utm_source=chatgpt.com "Functions: cookies"
[2]: https://nextjs.org/docs/app/api-reference/file-conventions/route?utm_source=chatgpt.com "File-system conventions: route.js"
[3]: https://nextjs.org/docs/app/api-reference/file-conventions/middleware?utm_source=chatgpt.com "File-system conventions: middleware.js"
[4]: https://authjs.dev/getting-started/installation?utm_source=chatgpt.com "Auth.js | Installation"
[5]: https://nextjs.org/docs/app/guides/authentication?utm_source=chatgpt.com "Guides: Authentication"
[6]: https://nextjs.org/docs/app?utm_source=chatgpt.com "Next.js Docs: App Router"

  **[⬆ Наверх](#top)**

78. ### <a name="78"></a> Wie schützt man Seiten vor unautorisiertem Zugriff?

**Seiten vor unautorisiertem Zugriff schützen (App Router & Pages Router)**

---

## App Router (empfohlen)

**A) Globales Gate mit Middleware (Edge)**

```js
// middleware.ts
import { NextResponse } from "next/server";
import type { NextRequest } from "next/server";

export function middleware(req: NextRequest) {
  const isProtected = req.nextUrl.pathname.startsWith("/app");
  const hasSession = req.cookies.get("session")?.value; // oder Auth.js-Middleware
  if (isProtected && !hasSession) {
    return NextResponse.redirect(new URL("/login", req.url));
  }
  return NextResponse.next();
}
export const config = { matcher: ["/app/:path*"] };
```

*Läuft vor jeder Route, ideal für Auth-Gates, i18n, Geofencing.*

**B) Serverseitiger Check in Seiten/Layouts**

```js
// app/app/page.tsx
import { cookies } from "next/headers";
import { redirect } from "next/navigation";

export default async function AppHome() {
  const token = (await cookies()).get("session")?.value; // Lesen macht die Route automatisch dynamisch
  if (!token) redirect("/login");
  return <h1>Dashboard</h1>;
}
```

*`cookies()`/`headers()` → Route wird dynamisch (keine SSG/Caches), `redirect()` stoppt Rendering früh.*

**C) Mit Auth.js (NextAuth v5)**

```js
// middleware.ts
export { auth as middleware } from "@/auth"; // schützt gem. deiner Auth-Konfig
export const config = { matcher: ["/app/:path*"] };
```

```js
// app/app/page.tsx
import { auth } from "@/auth";
import { redirect } from "next/navigation";

export default async function Page() {
  const session = await auth();
  if (!session) redirect("/login");
  return <h1>Hi {session.user?.name}</h1>;
}
```

---

## Pages Router (klassisch)

**SSR-Weiterleitung per `getServerSideProps`**

```js
// pages/protected.tsx
export default function Protected() { return <h1>Secret</h1>; }

export async function getServerSideProps({ req }) {
  const session = req.cookies.session; // oder NextAuth getSession()
  if (!session) {
    return { redirect: { destination: "/login", permanent: false } };
  }
  return { props: {} };
}
```

---

## Best Practices

* **Nie nur Client-seitig prüfen** (z. B. in `useEffect`) – immer serverseitig/middlewarebasiert gate-keeping.
* **HttpOnly-Cookies** für Sessions (`Secure`, `SameSite`).
* **Geschützte Routen dynamisch halten** (App Router: `cookies()`/`headers()` lesen oder `cache: "no-store"`/`export const dynamic = "force-dynamic"`).
* **APIs ebenfalls schützen** (Route Handlers/Middleware), sonst kann man Seitenchecks umgehen.

---

**Zusammenfassung**

* **App Router:** Schutz per **Middleware** (früh, global) + **serverseitigem Redirect** in Seiten/Layouts.
* **Pages Router:** Schutz per **`getServerSideProps`** mit Redirect.
* **Immer serverseitig prüfen**, Cookies sicher setzen, geschützte Routen nicht statisch cachen.

**Quellen / Weiterlesen:**

* Installation & Projektstruktur: [https://nextjs.org/docs/app/getting-started/installation](https://nextjs.org/docs/app/getting-started/installation)
* Authentication (App Router): [https://nextjs.org/docs/app/building-your-application/authentication](https://nextjs.org/docs/app/building-your-application/authentication)
* Middleware: [https://nextjs.org/docs/app/building-your-application/routing/middleware](https://nextjs.org/docs/app/building-your-application/routing/middleware)
* `cookies()` API: [https://nextjs.org/docs/app/api-reference/functions/cookies](https://nextjs.org/docs/app/api-reference/functions/cookies)
* `redirect()` (next/navigation): [https://nextjs.org/docs/app/api-reference/functions/redirect](https://nextjs.org/docs/app/api-reference/functions/redirect)

  **[⬆ Наверх](#top)**

79. ### <a name="79"></a> Wie arbeitet man mit Environment Variablen (.env.local)?

**Arbeiten mit Environment Variablen in Next.js (.env.local):**

* **Dateien:**

  * `.env.local` → für lokale Entwicklung (nicht ins Git einchecken)
  * `.env.development`, `.env.production`, `.env.test` → für verschiedene Umgebungen

* **Namenskonvention:**

  * Variablen für **Server only**: `DATABASE_URL=...`
  * Variablen für **Client & Server**: müssen mit `NEXT_PUBLIC_` beginnen, z. B. `NEXT_PUBLIC_API_URL=...`

* **Beispiel `.env.local`:**

  ```env
  DATABASE_URL=postgres://user:pass@localhost:5432/db
  NEXT_PUBLIC_API_URL=https://api.example.com
  ```

* **Nutzung im Code (Server-Seite):**

  ```js
  // app/api/route.js
  export async function GET() {
    const dbUrl = process.env.DATABASE_URL; 
    // Nur auf dem Server verfügbar
    return Response.json({ dbUrl });
  }
  ```

* **Nutzung im Code (Client-Seite):**

  ```js
  // app/page.js
  export default function Page() {
    const apiUrl = process.env.NEXT_PUBLIC_API_URL; 
    // Kann im Browser verwendet werden
    return <p>API: {apiUrl}</p>;
  }
  ```

* **Wichtig:**

  * Änderungen in `.env.local` erfordern **Neustart des Dev-Servers** (`npm run dev`).
  * Keine sensiblen Daten mit `NEXT_PUBLIC_` versehen – diese landen im Frontend-Bundle.

🔗 [Next.js – Environment Variables](https://nextjs.org/docs/app/building-your-application/configuring/environment-variables)

---

**Zusammenfassung:**
Environment Variablen werden in `.env.*`-Dateien definiert. Für den Client müssen sie mit `NEXT_PUBLIC_` beginnen, serverseitig sind sie direkt über `process.env` verfügbar. Änderungen erfordern einen Neustart des Servers.

  **[⬆ Наверх](#top)**

80. ### <a name="80"></a> Wo kann man Next.js-Anwendungen deployen?

**Deployment-Optionen für Next.js-Anwendungen:**

* **Vercel** (von den Next.js-Machern, empfohlen)

  * Zero-Config-Deployment: automatisches Build, Preview Deployments bei jedem Git-Push
  * Unterstützt Edge Functions, ISR, Middleware out-of-the-box

* **Netlify**

  * Einfaches Hosting für statische & serverseitige Next.js-Anwendungen
  * Funktionen wie Serverless Functions und Edge Middleware verfügbar

* **AWS (z. B. Amplify, Lambda, ECS, S3 + CloudFront)**

  * Flexibel, aber mehr Konfigurationsaufwand
  * Gut für skalierbare Production-Umgebungen

* **Azure (z. B. Azure Static Web Apps, App Service)**

  * Deployment über GitHub Actions oder Azure Pipelines
  * Serverless Functions Integration möglich

* **Google Cloud (z. B. App Engine, Cloud Run, Firebase Hosting)**

  * Firebase Hosting: für statische Export-Projekte (`next export`)
  * Cloud Run: Container-basierte Deployments

* **Docker + eigener Server / Kubernetes**

  * Maximale Kontrolle über Infrastruktur
  * Typisch bei Enterprise- oder On-Premise-Setups

* **Andere Anbieter:** Render, Railway, Heroku (eingeschränkt), Cloudflare Pages (Edge-optimiert)

🔗 [Next.js – Deployment](https://nextjs.org/docs/app/building-your-application/deploying)

---

**Zusammenfassung:**
Next.js kann auf vielen Plattformen deployed werden, bevorzugt jedoch **Vercel** (native Integration). Alternativen wie Netlify, AWS, Azure, Google Cloud oder Docker sind ebenfalls möglich – Auswahl hängt von den Projektanforderungen ab.

  **[⬆ Наверх](#top)**  

81. ### <a name="81"></a> Worin unterscheidet sich Vercel von Netlify?

**Unterschiede zwischen Vercel und Netlify (für Next.js-Deployments):**

| Kriterium             | **Vercel**                                                                                               | **Netlify**                                                                                          |
| --------------------- | -------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| **Integration**       | Von den Next.js-Machern → beste native Unterstützung (ISR, Middleware, Edge Functions sofort verfügbar). | Generell gutes Next.js-Support, aber manche Features (z. B. ISR) benötigen Workarounds oder Plugins. |
| **Build & Deploy**    | Zero-Config für Next.js, automatische Optimierungen.                                                     | Benötigt oft zusätzliche Konfiguration (`next-on-netlify` Plugin).                                   |
| **Serverless / Edge** | Edge Functions und Middleware sind direkt integriert.                                                    | Bietet Serverless Functions, Edge Middleware – aber weniger tief integriert.                         |
| **Performance**       | Sehr optimiert für Next.js (Caching, Images, Routing).                                                   | Gut für JAMstack, aber nicht so tief auf Next.js zugeschnitten.                                      |
| **Previews**          | Preview Deployments bei jedem Git-Push (besonders stark integriert).                                     | Bietet ebenfalls Previews, aber weniger eng mit Next.js verbunden.                                   |
| **Ökosystem**         | Fokus stark auf Next.js und React-Ökosystem.                                                             | Breiter Fokus auf JAMstack (Gatsby, Hugo, Vue, Svelte usw.).                                         |
| **Kosten**            | Free-Tier + skalierbare Pläne; für Next.js oft effizienter.                                              | Ähnliche Preismodelle, aber manche Limits (Build-Minuten, Functions).                                |

🔗 [Next.js – Vercel Deployment](https://nextjs.org/docs/app/building-your-application/deploying/vercel)
🔗 [Netlify – Next.js Support](https://docs.netlify.com/integrations/frameworks/next-js/)

---

**Zusammenfassung:**
Vercel ist die **native Plattform für Next.js** und unterstützt alle Features ohne Zusatzkonfiguration. Netlify bietet zwar ebenfalls Hosting für Next.js, ist aber eher auf JAMstack allgemein ausgelegt und erfordert oft zusätzliche Anpassungen.

  **[⬆ Наверх](#top)**

82. ### <a name="82"></a> Wie deployt man Next.js auf Vercel?

**Next.js auf Vercel deployen (App Router):**

1. **Repo vorbereiten**

   * `package.json` enthält:

     ```js
     {
       "scripts": {
         "dev": "next dev",
         "build": "next build",
         "start": "next start"
       }
     }
     ```
   * Code nach GitHub/GitLab/Bitbucket pushen.

2. **Projekt importieren**

   * Auf **vercel.com → New Project → Import** und das Repo wählen.
   * Framework-Preset **Next.js** wird automatisch erkannt; Build-Command `next build`, Output `Next.js`.
   * Optional: **Environment Variables** im Projekt unter *Settings → Environment Variables* setzen (z. B. `NEXT_PUBLIC_API_URL`, `DATABASE_URL`).

3. **Erster Deploy**

   * Vercel baut automatisch und erstellt **Preview Deployments** für Branches/PRs.
   * Merge nach `main` → **Production Deployment**.

4. **CLI (Alternative ohne Dashboard)**

   ```bash
   npm i -g vercel
   vercel           # erstes Deployment (Preview)
   vercel --prod    # Production-Deploy
   ```

   * Beim ersten Lauf Projekt verlinken und ggf. Variablen setzen.

5. **Domäne & Routing**

   * *Settings → Domains* eigene Domain hinzufügen; DNS nach Anleitung konfigurieren.
   * Next.js-Routing (App Router) funktioniert ohne Zusatzkonfiguration; Middleware/Edge Functions werden automatisch unterstützt.

6. **Bilder & externe Hosts**

   * Falls externe Bilder: in `next.config.js` freigeben.

     ```js
     // next.config.js
     export default {
       images: {
         remotePatterns: [{ protocol: 'https', hostname: 'images.example.com' }]
       }
     }
     ```
   * `next/image` funktioniert auf Vercel ohne zusätzliche Infrastruktur.

7. **Rebuilds & ISR**

   * Incremental Static Regeneration (ISR) und On-Demand Revalidation sind **out of the box** verfügbar; bei Deploys werden Caches/CDN aktualisiert.

**Quellen:**

* Next.js – *Deploying* (App Router): ([nextjs.org][1])
* Vercel – *Next.js on Vercel* (Framework-Integration): ([Vercel][2])
* Vercel – *Git-Integration (GitHub)*: ([Vercel][3])
* Next.js – *next.config.js* (Konfiguration, `images`): ([nextjs.org][4])
* Next.js – *Installation* (Grundlage): ([nextjs.org][5])
* Vercel – *Domains hinzufügen*: ([Vercel][6])

---

**Zusammenfassung:**
Repo pushen → in Vercel importieren → Build läuft automatisch (Next.js-Preset) → Preview/Production-Deploys sind bereit. Optional per CLI deployen, Env-Variablen und Domain im Dashboard konfigurieren; `next/image`, ISR, Middleware/Edge laufen nativ auf Vercel.

[1]: https://nextjs.org/docs/14/app/building-your-application/deploying?utm_source=chatgpt.com "Building Your Application: Deploying"
[2]: https://vercel.com/docs/frameworks/full-stack/nextjs?utm_source=chatgpt.com "Next.js on Vercel"
[3]: https://vercel.com/docs/git/vercel-for-github?utm_source=chatgpt.com "Deploying GitHub Projects with Vercel"
[4]: https://nextjs.org/docs/app/api-reference/config/next-config-js?utm_source=chatgpt.com "Configuration: next.config.js"
[5]: https://nextjs.org/docs/pages/getting-started/deploying?utm_source=chatgpt.com "Getting Started: Deploying"
[6]: https://vercel.com/docs/domains/working-with-domains/add-a-domain?utm_source=chatgpt.com "Adding & Configuring a Custom Domain"

  **[⬆ Наверх](#top)**

83. ### <a name="83"></a> Kann man Next.js mit Docker deployen?

**Ja — Next.js kann mit Docker deployt werden. Vorgehensweise (App Router, produktionsfähig):**

1. **Next.js auf „standalone“ bauen (kleineres Image)**

   ```js
   // next.config.js (ESM)
   export default {
     output: 'standalone', // erzeugt .next/standalone + minimal node_modules
   }
   ```

   Quelle: Next.js Deploying → Docker/Standalone. ([nextjs.org][1])

2. **Multi-Stage-Dockerfile (Build → Runtime)**

   ```js
   # Dockerfile
   # --- Build Stage ---
   FROM node:18-alpine AS builder
   WORKDIR /app
   COPY package.json package-lock.json* pnpm-lock.yaml* yarn.lock* ./  # lockfile optional
   RUN npm ci --no-audit --no-fund
   COPY . .
   RUN npm run build  # erzeugt .next/standalone und .next/static

   # --- Runtime Stage ---
   FROM node:18-alpine AS runner
   WORKDIR /app
   ENV NODE_ENV=production
   # Optionale Port-Angabe für Plattformen, die sie auslesen:
   ENV PORT=3000
   # Dateien aus dem Build übernehmen
   COPY --from=builder /app/public ./public
   COPY --from=builder /app/.next/standalone ./
   COPY --from=builder /app/.next/static ./.next/static
   # Nicht-root Nutzer ist Best Practice
   RUN addgroup -S nextjs && adduser -S nextjs -G nextjs
   USER nextjs
   EXPOSE 3000
   # Next.js-Standalone bringt den Server bereits mit:
   CMD ["node", "server.js"]
   ```

   Hinweise:

   * `CMD ["node", "server.js"]` ist im Standalone-Bundle vorhanden.
   * Für eigene Startskripte ggf. `-r dotenv/config` etc. ergänzen, wenn `.env` zur Laufzeit geladen werden soll.
     Quellen: Next.js Deploying (Docker Image, App Router) und offizielles Beispiel `with-docker`. ([nextjs.org][1])

3. **Build & Run**

   ```js
   # Image bauen
   docker build -t my-nextjs-app .

   # Container starten (Prod)
   docker run -p 3000:3000 --env-file .env.production my-nextjs-app
   ```

   Tipp: Runtime-Env-Vars per `--env`/`--env-file` injizieren; der App Router kann sie serverseitig zur **Request-Zeit** lesen (z. B. in Server Components, RSC Actions). ([nextjs.org][2])

4. **Orchestrierung (optional)**

   * **Kubernetes/Cloud Run/ECS**: Container wie üblich deployen; Health-Checks auf `/` oder eigene Route.
   * **Wichtig**: Vercel **akzeptiert keine** Docker-Images direkt; für Docker nutze selbst-gehostete Plattformen (K8s, Render, Railway, Cloud Run, ECS). ([nextjs.org][1])

5. **Performance/Größe**

   * `node:18-alpine`, Multi-Stage, `output: 'standalone'` → kleine Images, schnelle Starts.
   * Assets (`public`, `.next/static`) separat kopieren, sonst fehlen Images/Fonts.
     Quellen & Best Practices: Next.js Docs (Deploying/Docker) + offizielles Repo-Beispiel. ([nextjs.org][1])

**Weiterlesen (offizielle Doku):**

* Next.js → *Deploying* (Docker, App Router): [https://nextjs.org/docs/app/building-your-application/deploying](https://nextjs.org/docs/app/building-your-application/deploying)
* Einstieg/Installation: [https://nextjs.org/docs/app/getting-started/installation](https://nextjs.org/docs/app/getting-started/installation) ([nextjs.org][1])

---

**Zusammenfassung:**
Ja, Deployment mit Docker ist möglich: `output: 'standalone'` aktivieren, Multi-Stage-Dockerfile nutzen, Image bauen und mit Runtime-Env-Vars starten. Für das Hosting nutze Plattformen, die Container ausführen (Kubernetes, Cloud Run, ECS, Render); Vercel nimmt keine Docker-Images direkt an. ([nextjs.org][1])

[1]: https://nextjs.org/docs/app/getting-started/deploying?utm_source=chatgpt.com "Getting Started: Deploying"
[2]: https://nextjs.org/docs/14/app/building-your-application/deploying?utm_source=chatgpt.com "Building Your Application: Deploying"

  **[⬆ Наверх](#top)**

84. ### <a name="84"></a> Wie deployt man Next.js auf AWS?

**Optionen & Schritte: Next.js auf AWS deployen (App Router)**

### 1) AWS Amplify Hosting (managed, SSR-Unterstützung)

* **Vorgehen**

  ```js
  // Build Settings werden automatisch erkannt
  // package.json
  {
    "scripts": { "build": "next build", "start": "next start" }
  }
  // In der Amplify Console: App anlegen → Repo/Branch verbinden → Deploy
  // Env-Vars in Amplify: Settings → Environment variables
  ```
* **Features:** SSR/ISR, Image-Optimierung, Previews, einfache Git-Integration.
  Quelle: AWS Amplify Next.js (SSR) & Quickstart. ([docs.amplify.aws][1])

---

### 2) OpenNext/SST (Vercel-ähnliche Architektur auf AWS: CloudFront + S3 + Lambda)

* **Setup (minimal)**

  ```js
  // sst.config.ts
  import { sst } from "sst";
  export default {
    app(input) {
      return { name: "my-next-app", home: "aws" };
    },
    stacks(app) {
      app.stack(function Site({ stack }) {
        new sst.aws.Nextjs("Web"); // nutzt OpenNext unter der Haube
      });
    },
  };
  ```
* **Konzept:** OpenNext transformiert den Next.js-Build für AWS-Services (Lambda, S3, CloudFront).
  Quellen: OpenNext & SST Docs. ([opennext.js.org][2])

---

### 3) Containerisiert (Docker) auf App Runner / ECS / EKS

* **Docker-Build (empfohlen: `output: 'standalone'`)**

  ```js
  // next.config.js
  export default { output: "standalone" };
  ```

  ```js
  // Dockerfile (schematisch)
  // 1) Build-Stage → next build
  // 2) Runtime-Stage kopiert .next/standalone + .next/static + public
  // CMD ["node","server.js"]
  ```
* **App Runner Tipp**

  ```js
  // Wichtige Env-Var in App Runner setzen:
  // HOSTNAME=0.0.0.0  // sonst bindet Next.js ggf. nicht korrekt
  ```
* **Alternativen:** ECS/Fargate (ECR-Image), EKS (K8s).
  Quellen: Next.js Deploying (Docker) + App Runner Hinweise. ([nextjs.org][3])

---

### 4) Statisches Hosting (ohne SSR): S3 + CloudFront

* **Nur für `next export`/statische Routen**

  ```js
  // Build
  // npm run build && npx next export  // erzeugt /out
  // Upload /out nach S3, über CloudFront ausliefern
  ```
* **Hinweis:** keine SSR-/Middleware-Features.
  Quellen: Next.js Static Export + S3/CloudFront Guides. ([nextjs.org][4])

---

### 5) Klassischer Node-Server: Elastic Beanstalk

* **Einsatzfall:** Monolithischer Node-Prozess (z. B. `next start`) mit Auto-Scaling durch EB.

  ```js
  // package.json (Production start)
  {
    "scripts": { "build": "next build", "start": "next start" }
  }
  // In EB als Node.js-App deployen
  ```

  Quellen: EB Node.js Doku & Quickstart. ([Документация AWS][5])

---

**Weiterführende Next.js-Doku:**

* Getting Started / Deploying: [https://nextjs.org/docs/app/getting-started/deploying](https://nextjs.org/docs/app/getting-started/deploying)
* Installation/Grundlagen: [https://nextjs.org/docs/app/getting-started/installation](https://nextjs.org/docs/app/getting-started/installation) ([nextjs.org][3])

---

**Zusammenfassung:**
Für **managed SSR**: Amplify Hosting. Für **AWS-native, Vercel-ähnlich**: OpenNext/SST (CloudFront+S3+Lambda). Für **Container-Workflows**: App Runner/ECS mit Docker (`output: 'standalone'`, ggf. `HOSTNAME=0.0.0.0`). Für **statische Sites**: S3+CloudFront via `next export`. Elastic Beanstalk eignet sich für klassische Node-Deployments. ([docs.amplify.aws][1])

[1]: https://docs.amplify.aws/gen1/javascript/deploy-and-host/frameworks/deploy-nextjs-app/?utm_source=chatgpt.com "Deploy a Next.js app - JavaScript - AWS Amplify Gen 1 ..."
[2]: https://opennext.js.org/aws?utm_source=chatgpt.com "AWS"
[3]: https://nextjs.org/docs/app/getting-started/deploying?utm_source=chatgpt.com "Getting Started: Deploying"
[4]: https://nextjs.org/docs/pages/getting-started/deploying?utm_source=chatgpt.com "Getting Started: Deploying"
[5]: https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_nodejs.html?utm_source=chatgpt.com "Deploying Node.js applications with Elastic Beanstalk"

  **[⬆ Наверх](#top)**

85. ### <a name="85"></a> Was ist der Unterschied zwischen Serverless-Deployment und Edge-Deployment?

**Unterschied: Serverless vs. Edge Deployment in Next.js**

| Kriterium                  | **Serverless Deployment**                                                           | **Edge Deployment**                                                                        |
| -------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| **Laufzeit-Umgebung**      | Node.js-basierte Serverless Functions (z. B. AWS Lambda, Vercel Functions).         | Edge-Runtime (V8 Isolate, ähnlich wie Cloudflare Workers, kein voller Node.js).            |
| **Startzeit (Cold Start)** | Höher (ms–sekundenabhängig von Provider, bei Inaktivität Neustart nötig).           | Extrem gering (ms), da global verteilt und ohne Cold-Starts wie bei klassischen Lambdas.   |
| **Node-API**               | Voller Zugriff auf Node.js APIs, z. B. `fs`, `crypto`, native Module.               | Kein voller Node.js-Support; eingeschränkte APIs, Fokus auf Web-APIs (`fetch`, `Request`). |
| **Globalität**             | Läuft in spezifischen Rechenzentren/Regionen → höherer Latenz für entfernte Nutzer. | Wird auf Edge-Netzwerk repliziert → sehr niedrige Latenz weltweit.                         |
| **Use Cases**              | Schwergewichtigere Logik: Auth, Datenbankzugriffe, Bildbearbeitung.                 | Leichte Middleware: Auth-Checks, Redirects, A/B-Testing, Geo-basierte Anpassungen.         |
| **Beispiele in Next.js**   | API Routes (`pages/api/*` oder App Router `app/api/*`), ISR-Revalidierung.          | Middleware (`middleware.js`), Edge Functions (`export const runtime = 'edge'`).            |

---

**Codebeispiel:**

*Serverless Function (Node.js Umgebung):*

```js
// app/api/hello/route.js
export async function GET() {
  const secret = process.env.SECRET_KEY; // Zugriff auf Node.js env
  return Response.json({ message: "Hello from Serverless" });
}
```

*Edge Function (Edge-Runtime):*

```js
// app/api/edge/route.js
export const runtime = 'edge'; // explizit Edge
export async function GET() {
  // Nur Web-APIs verfügbar (kein Node.js fs)
  return new Response(JSON.stringify({ message: "Hello from Edge" }), {
    headers: { "content-type": "application/json" }
  });
}
```

---

🔗 [Next.js – Middleware & Edge Functions](https://nextjs.org/docs/app/building-your-application/routing/middleware)
🔗 [Next.js – API Routes / Serverless Functions](https://nextjs.org/docs/pages/building-your-application/routing/api-routes)

---

**Zusammenfassung:**
Serverless läuft in Node.js-Umgebungen (flexibel, aber langsamer), Edge läuft in leichtgewichtigen V8-Isolates direkt am CDN-Edge (schneller, global, aber eingeschränkte APIs). Edge ist optimal für **leichte, globale Middleware**, Serverless für **vollwertige Backend-Logik**.

  **[⬆ Наверх](#top)**

86. ### <a name="86"></a> Welche Probleme können beim Deployment von Next.js auftreten?

**Häufige Probleme beim Deployment von Next.js und ihre Ursachen:**

* **Falsche Umgebungskonfiguration**

  * `process.env` Variablen fehlen oder sind falsch gesetzt → Fehler beim Build oder Runtime.
  * Lösung: `.env.*` richtig pflegen, Secrets nicht ins Client-Bundle ohne `NEXT_PUBLIC_`.

* **Node.js-Version inkompatibel**

  * Next.js erfordert bestimmte Node-Version (z. B. ≥ 18).
  * Lösung: In Deployment-Umgebung exakt gleiche Node-Version wie lokal nutzen.

* **Image-Optimierung fehlschlägt**

  * Externe Domains nicht freigegeben → `next/image` lädt nicht.
  * Lösung: `next.config.js → images.remotePatterns` konfigurieren.

* **Fehlerhafte Routing-Struktur**

  * Unterschied App Router (`app/`) vs. Pages Router (`pages/`).
  * Mögliche 404 bei Deployments, wenn Dateien nicht am richtigen Ort.

* **Build schlägt fehl**

  * Abhängigkeiten fehlen, lockfile nicht im Repo, falsches Install-Command.
  * Lösung: Lockfile committen, `npm ci` oder `pnpm install --frozen-lockfile` im CI/CD.

* **Serverless- vs. Edge-Limits**

  * Edge Functions → eingeschränkte Node-APIs (kein `fs`, kein `crypto.randomBytes`).
  * Serverless Functions → Cold Starts, Timeout-Limits (z. B. 10s auf Vercel/Hobby-Plan).

* **Statisches Export-Limit (`next export`)**

  * Funktioniert nicht mit Features wie SSR, Middleware oder API-Routes.
  * Lösung: Nur für rein statische Sites nutzen; sonst SSR-Deployment wählen.

* **Cache-/ISR-Probleme**

  * Incremental Static Regeneration funktioniert nicht, wenn Plattform keine Revalidierung unterstützt.
  * Lösung: Plattform wählen, die ISR/On-Demand Revalidation zulässt (z. B. Vercel, Netlify mit Plugin).

* **Fehlende Dateisystemrechte**

  * Bei Docker/Server-Deployments: `public` oder `.next/static` nicht kopiert → Assets fehlen.
  * Lösung: im Dockerfile oder CI/CD sicherstellen, dass statische Ressourcen enthalten sind.

---

🔗 [Next.js – Deployment](https://nextjs.org/docs/app/building-your-application/deploying)
🔗 [Next.js – Troubleshooting](https://nextjs.org/docs/messages)

---

**Zusammenfassung:**
Typische Probleme: falsche Environment-Variablen, inkompatible Node-Version, nicht konfigurierte Images, Routing-Fehler, fehlende Abhängigkeiten, Einschränkungen bei Serverless/Edge, sowie Cache-/ISR-Probleme. Lösung: Dokumentation prüfen, Build-/Runtime-Umgebung anpassen und Plattform-spezifische Limits beachten.

  **[⬆ Наверх](#top)**

87. ### <a name="87"></a> Wie aktiviert man die integrierte i18n-Unterstützung in Next.js?

**i18n in Next.js aktivieren (App Router und Pages Router):**

### 1. Konfiguration in `next.config.js`

```js
// next.config.js
export default {
  i18n: {
    locales: ["en", "de", "fr"], // unterstützte Sprachen
    defaultLocale: "en",         // Standardsprache
  },
};
```

* `locales`: Liste der Sprachen (z. B. `["en", "de"]`).
* `defaultLocale`: Fallback-Sprache.
* Next.js generiert automatisch sprachspezifische Routen (`/de/about`, `/fr/about`).

---

### 2. Nutzung im App Router

* Routen wie `app/[locale]/page.js` anlegen.
* `params.locale` in Server-Komponenten oder Layouts verwenden:

```js
// app/[locale]/page.js
export default function Page({ params }) {
  return <h1>Sprache: {params.locale}</h1>;
}
```

* Dynamische Inhalte (z. B. Übersetzungen) über JSON-Dateien oder externe Libraries (z. B. `next-intl`, `next-i18next`).

---

### 3. Nutzung im Pages Router (älter)

* Pfade automatisch `/en/...`, `/de/...`.
* Zugriff auf Locale über `useRouter`:

```js
import { useRouter } from "next/router";

export default function Home() {
  const { locale, locales, defaultLocale } = useRouter();
  return <p>Aktuelle Sprache: {locale}</p>;
}
```

---

### 4. Einschränkungen

* Die integrierte i18n-Unterstützung regelt **nur Routing & Locale-Erkennung**.
* Für echte Übersetzungen (Text, Pluralisierung) benötigt man zusätzliche Packages (`next-intl`, `next-i18next`).

---

🔗 [Next.js – Internationalized Routing](https://nextjs.org/docs/app/building-your-application/routing/internationalization)

---

**Zusammenfassung:**
Die integrierte i18n-Unterstützung aktiviert man in `next.config.js` über die `i18n`-Option. Sie sorgt für sprachbasierte Routen (`/de/...`), aber nicht für Übersetzungen selbst – dafür nutzt man zusätzliche Libraries.

  **[⬆ Наверх](#top)**

88. ### <a name="88"></a> Wie implementiert man Mehrsprachigkeit im App Router?

**Mehrsprachigkeit im App Router implementieren (Best Practice mit `next-intl`)**

> Im App Router gibt es **keine eingebaute i18n-Routing-Konfiguration** mehr; du setzt sie selbst via `[locale]`-Segment und optionaler Middleware um. ([nextjs.org][1])

### 1) Locale-Segment & Messages

```js
// app/[locale]/layout.js
import {NextIntlClientProvider} from 'next-intl';
import {notFound} from 'next/navigation';
import en from '@/messages/en.json';
import de from '@/messages/de.json';

const messagesMap = {en, de};
export const locales = ['en', 'de'];

export default function RootLayout({children, params}) {
  const {locale} = params;
  if (!locales.includes(locale)) notFound();

  // <html lang> pro Sprache setzen
  return (
    <html lang={locale}>
      <body>
        <NextIntlClientProvider locale={locale} messages={messagesMap[locale]}>
          {children}
        </NextIntlClientProvider>
      </body>
    </html>
  );
}
```

### 2) Routen statisch vorab generieren (optional, besseres SSG/ISR)

```js
// app/[locale]/page.js
export function generateStaticParams() {
  return [{locale: 'en'}, {locale: 'de'}]; // plus weitere Locales
}

export default function Page({params}) {
  return <h1>Home ({params.locale})</h1>;
}
```

### 3) Locale-Erkennung & Redirect aus `/` (Middleware)

```js
// middleware.js
import {NextResponse} from 'next/server';
import {locales} from './app/[locale]/layout.js';

function detectLocale(req) {
  // sehr einfach: Accept-Language → erstes unterstütztes Locale
  const header = req.headers.get('accept-language') || '';
  const preferred = header.split(',')[0]?.split('-')[0];
  return locales.includes(preferred) ? preferred : 'en';
}

export function middleware(req) {
  const {pathname} = req.nextUrl;
  // Wenn bereits /en/... oder /de/..., nichts tun
  if (locales.some(l => pathname.startsWith(`/${l}/`) || pathname === `/${l}`)) {
    return NextResponse.next();
  }
  // Root oder andere Pfade → auf ermitteltes Locale umschreiben
  if (pathname === '/' || pathname.split('/').filter(Boolean).length === 0) {
    const locale = detectLocale(req);
    return NextResponse.redirect(new URL(`/${locale}`, req.url));
  }
  return NextResponse.next();
}

export const config = {matcher: ['/((?!_next|.*\\..*).*)']};
```

Hinweis: Du kannst die Middleware auch mit `next-intl`’s Routing-Helpers umsetzen (Domain-/Cookie-basiert). ([next-intl.dev][2])

### 4) Übersetzungen im Code verwenden

```js
// app/[locale]/about/page.js
'use client';
import {useTranslations} from 'next-intl';

export default function About() {
  const t = useTranslations('about');
  return <p>{t('headline')}</p>; // messages/en.json → { "about": { "headline": "About us" } }
}
```

([next-intl.dev][3])

### 5) SEO: `alternates.languages` & Sitemaps

```js
// app/[locale]/layout.js
export async function generateMetadata({params}) {
  const {locale} = params;
  const base = 'https://example.com';
  return {
    alternates: {
      languages: {
        en: `${base}/en`,
        de: `${base}/de`
      }
    }
  };
}
```

Optional zusätzlich eine lokalisierte `sitemap.ts` erzeugen. ([nextjs.org][4])

### 6) Alternativen zu `next-intl`

* **i18next / react-i18next** direkt im App Router (ohne `next-i18next`) oder mit `next-i18n-router` für komfortables Routing & Detection. ([GitHub][5])

**Weiterlesen (offiziell & aktuell):**

* Next.js App Router – Internationalization (Guide & Patterns). ([nextjs.org][1])
* Middleware (App Router). ([nextjs.org][6])
* Installation/Grundlagen (Referenzlink). ([locize.com][7])
* next-intl (App Router Setup & Routing/SEO). ([next-intl.dev][3])

---

**Zusammenfassung:**
Im App Router realisierst du i18n über ein `[locale]`-Segment, Middleware für Locale-Erkennung/Redirects, einen Provider (z. B. `next-intl`) zum Laden der Messages und SEO-Metadaten mit `alternates.languages`. `generateStaticParams` verbessert das Prerendering; `next-intl` oder i18next liefern Übersetzungs-APIs, `next-i18n-router` ergänzt bequemes Routing. ([nextjs.org][1])

[1]: https://nextjs.org/docs/app/guides/internationalization?utm_source=chatgpt.com "Guides: Internationalization"
[2]: https://next-intl.dev/docs/routing/middleware?utm_source=chatgpt.com "Middleware – Internationalization (i18n) for Next.js"
[3]: https://next-intl.dev/docs?utm_source=chatgpt.com "Internationalization (i18n) for Next.js"
[4]: https://nextjs.org/docs/app/api-reference/functions/generate-metadata?utm_source=chatgpt.com "generateMetadata function"
[5]: https://github.com/i18next/next-i18next?utm_source=chatgpt.com "i18next/next-i18next: The easiest way to translate your ..."
[6]: https://nextjs.org/docs/app/api-reference/file-conventions/middleware?utm_source=chatgpt.com "File-system conventions: middleware.js"
[7]: https://www.locize.com/blog/i18n-next-app-router?utm_source=chatgpt.com "Simplifying i18next Setup in Next.js App Router"

  **[⬆ Наверх](#top)**

89. ### <a name="89"></a> Welche i18n-Bibliotheken werden am häufigsten mit Next.js verwendet?

**Häufig genutzte i18n-Bibliotheken mit Next.js:**

* **[next-i18next](https://github.com/i18next/next-i18next)**

  * Offizielles Next.js-Plugin für [i18next](https://www.i18next.com/).
  * Bietet automatische Integration mit dem Next.js-Routing (Pages Router), Namespaces, Pluralisierung.
  * Sehr etabliert in der Community, viel Dokumentation.
  * Einschränkung: Anpassung für den neuen **App Router** ist komplexer.

* **[next-intl](https://next-intl-docs.vercel.app/)**

  * Moderne Lösung speziell für den **App Router**.
  * Nutzt native Intl-APIs, kleine API-Oberfläche, optimiert für SSR/SSG.
  * Bietet `useTranslations` Hook, Middleware-Integration, SEO (hreflang/alternates).
  * Ideal für Projekte, die auf App Router setzen.

* **[react-intl](https://formatjs.io/docs/react-intl/)**

  * Teil von *FormatJS*.
  * Starke Unterstützung für ICU-Messageformat, komplexe Pluralisierung & Datums-/Zahlenformatierung.
  * Muss manuell in Next.js integriert werden, kein spezifisches Routing-Plugin.

* **[i18next + react-i18next](https://react.i18next.com/)** (ohne next-i18next)

  * Voll flexibel, direkte Verwendung in Next.js möglich.
  * Benötigt etwas mehr Boilerplate, Middleware oder Routing-Lösungen wie [next-i18n-router](https://github.com/QuiiBz/next-i18n-router).

* **[LinguiJS](https://lingui.dev/)**

  * Fokussiert auf Developer Experience.
  * Translation Keys als Code, unterstützt ICU-Format.
  * Gut für kleine Projekte oder wenn man lieber Messages statt Namespaces benutzt.

---

🔗 Offizielle Next.js Docs: [Internationalization](https://nextjs.org/docs/app/building-your-application/routing/internationalization)

---

**Zusammenfassung:**
Die **häufigsten Libraries** sind `next-i18next` (klassisch, stark im Pages Router), `next-intl` (empfohlen für App Router), sowie `react-intl` und `LinguiJS` für komplexere Übersetzungslogik. Für neue Projekte im **App Router** ist **next-intl** meist die beste Wahl.

  **[⬆ Наверх](#top)**

90. ### <a name="90"></a> Wie funktioniert automatisches Redirect nach Browsersprache?

**Automatisches Redirect nach Browsersprache in Next.js (App Router):**

### 1) Erkennung der Sprache

* Standard: HTTP-Header `Accept-Language` → enthält Präferenz des Browsers.
* Fallback: Cookie, Domain oder Default-Locale.

### 2) Middleware einsetzen

Middleware wird beim Request am Edge ausgeführt und kann Redirects setzen.

```js
// middleware.js
import {NextResponse} from 'next/server';

const locales = ['en', 'de', 'fr'];
const defaultLocale = 'en';

function getLocale(request) {
  const header = request.headers.get('accept-language') || '';
  const preferred = header.split(',')[0]?.split('-')[0]; 
  return locales.includes(preferred) ? preferred : defaultLocale;
}

export function middleware(request) {
  const {pathname} = request.nextUrl;

  // Prüfen: hat die URL bereits ein Locale?
  const pathnameIsMissingLocale = locales.every(
    (locale) => !pathname.startsWith(`/${locale}/`) && pathname !== `/${locale}`
  );

  if (pathnameIsMissingLocale) {
    const locale = getLocale(request);
    return NextResponse.redirect(new URL(`/${locale}${pathname}`, request.url));
  }
}

export const config = {
  matcher: ['/((?!_next|.*\\..*).*)'], // nur eigene Routen, keine Assets
};
```

### 3) Routing-Struktur anlegen

* `app/[locale]/page.js` → dynamisches Segment für Sprachen.
* Übersetzungen über `next-intl`, `next-i18next` oder eigenes System laden.

### 4) Best Practices

* User-Präferenz merken (z. B. mit Cookie `NEXT_LOCALE`) und bei erneutem Besuch verwenden.
* Fallback immer auf `defaultLocale`.
* SEO: `alternates.languages` in `generateMetadata` setzen.

---

🔗 [Next.js – Middleware](https://nextjs.org/docs/app/building-your-application/routing/middleware)
🔗 [next-intl – Locale Detection](https://next-intl-docs.vercel.app/docs/routing/middleware)

---

**Zusammenfassung:**
Automatische Locale-Redirects realisiert man in Next.js per **Middleware**: Sprache aus `Accept-Language` ermitteln, prüfen ob URL ein Locale enthält, andernfalls Redirect auf passende Sprachroute durchführen. Cookies + SEO-Alternates sorgen für bessere User-Experience und Suchmaschinenoptimierung.

  **[⬆ Наверх](#top)**  

91. ### <a name="91"></a> Was ist Middleware und wie wird sie verwendet?

**Middleware in Next.js (App Router):**

* **Definition:**
  Middleware ist Code, der **vor der Ausführung einer Route** (Page, API) am **Edge** läuft.
  Damit können Anfragen abgefangen, verändert oder umgeleitet werden.

* **Einsatzbereiche:**

  * Authentifizierung / Zugriffskontrolle
  * Lokalisierung (Redirect nach Browsersprache)
  * A/B-Testing oder Feature Flags
  * URL-Rewrites & Weiterleitungen
  * Logging, Header-Manipulation

---

### **Beispiel 1: Auth-Check**

```js
// middleware.js
import {NextResponse} from 'next/server';

export function middleware(request) {
  const isLoggedIn = request.cookies.get('token');
  if (!isLoggedIn && request.nextUrl.pathname.startsWith('/dashboard')) {
    return NextResponse.redirect(new URL('/login', request.url));
  }
  return NextResponse.next();
}

export const config = {
  matcher: ['/dashboard/:path*'], // nur auf /dashboard anwenden
};
```

---

### **Beispiel 2: Locale-Redirect**

```js
// middleware.js
import {NextResponse} from 'next/server';

export function middleware(request) {
  const locale = request.headers.get('accept-language')?.split(',')[0] || 'en';
  return NextResponse.rewrite(new URL(`/${locale}${request.nextUrl.pathname}`, request.url));
}

export const config = {matcher: ['/((?!_next|.*\\..*).*)']};
```

---

### **Technische Details**

* Läuft in einer **Edge-Runtime** (kein voller Node.js-Support).
* Zugriff nur auf Web APIs (`Request`, `Response`, `fetch`).
* Kann Response-Header ändern, Redirects oder Rewrites zurückgeben.

---

🔗 [Next.js – Middleware](https://nextjs.org/docs/app/building-your-application/routing/middleware)

---

**Zusammenfassung:**
Middleware ist ein Edge-Layer zwischen Anfrage und Antwort. Sie erlaubt Redirects, Auth-Checks, Internationalisierung und Header-Manipulation – läuft vor der Route und nutzt Web APIs statt Node.js.

  **[⬆ Наверх](#top)**

92. ### <a name="92"></a> Was ist Edge Runtime?

**Edge Runtime in Next.js**

* **Definition:**
  Die Edge Runtime ist eine **leichtgewichtige Ausführungsumgebung**, die auf **V8-Isolates** basiert (ähnlich wie Cloudflare Workers). Sie läuft **am Rand des CDN-Netzwerks** („Edge“) und nicht in zentralen Rechenzentren.

* **Eigenschaften:**

  * Extrem schnelle Antwortzeiten (kein klassischer „Cold Start“ wie bei Serverless Lambdas).
  * Weltweite Verteilung → niedrige Latenz für User.
  * Eingeschränkte APIs: keine Node.js-Module (`fs`, `net`, `crypto.randomBytes`), sondern **Web APIs** (`fetch`, `Request`, `Response`, `URL`).
  * Perfekt für leichte Middleware-Logik (Auth, Redirects, Geo-basiertes Routing).

---

### **Beispiel: Edge API Route**

```js
// app/api/hello/route.js
export const runtime = 'edge'; // explizit Edge Runtime aktivieren

export async function GET() {
  // Nur Web APIs verfügbar
  return new Response(JSON.stringify({msg: "Hello from Edge"}), {
    headers: {"Content-Type": "application/json"},
  });
}
```

---

### **Beispiele für Einsatz in Next.js**

* `middleware.js` → automatisch in Edge Runtime
* Edge API Routes (`export const runtime = 'edge'`)
* A/B-Testing, Geo-Redirects, schnelle Auth-Checks

---

🔗 [Next.js – Edge Runtime](https://nextjs.org/docs/app/building-your-application/rendering/edge-and-nodejs-runtimes)

---

**Zusammenfassung:**
Die Edge Runtime ist eine V8-basierte, global verteilte Laufzeitumgebung mit sehr niedriger Latenz. Sie bietet nur Web APIs, eignet sich aber hervorragend für Middleware, Edge-API-Routes und Geo-nahe Optimierungen.

  **[⬆ Наверх](#top)**

93. ### <a name="93"></a> Wie funktionieren Streaming und Suspense in Next.js 13?

**Streaming & Suspense in Next.js 13 (App Router):**

---

### 1. **Grundidee:**

* **Streaming:** Server-Rendering schickt HTML **schrittweise** zum Client → erste Teile sind sofort sichtbar, während andere noch nachgeladen werden.
* **Suspense:** React-Mechanismus, um UI zu „pausieren“, bis Daten oder Komponenten verfügbar sind. Im App Router direkt integriert.

---

### 2. **Server Components + Streaming**

* Next.js 13 rendert **Server Components** und streamt sie inkrementell an den Client.
* Kein Warten, bis die gesamte Seite fertig ist → **Time-to-First-Byte (TTFB)** sinkt, Nutzer sieht sofort Inhalte.

**Beispiel:**

```js
// app/page.js
import UserInfo from './UserInfo';

export default function Page() {
  return (
    <div>
      <h1>Dashboard</h1>
      {/* UserInfo braucht Daten und streamt separat */}
      <UserInfo />
    </div>
  );
}
```

---

### 3. **Suspense für Datenabhängigkeiten**

* `Suspense` zeigt Fallback, während eine Komponente lädt.
* Ideal für **langsamen Teil des UIs** (z. B. API-Aufruf).

**Beispiel:**

```js
// app/page.js
import {Suspense} from 'react';
import SlowPosts from './SlowPosts';

export default function Page() {
  return (
    <div>
      <h1>Blog</h1>
      <Suspense fallback={<p>Lade Beiträge...</p>}>
        <SlowPosts />
      </Suspense>
    </div>
  );
}
```

```js
// app/SlowPosts.js
export default async function SlowPosts() {
  const res = await fetch('https://jsonplaceholder.typicode.com/posts', {
    cache: 'no-store'
  });
  const posts = await res.json();
  return (
    <ul>
      {posts.slice(0, 5).map(p => <li key={p.id}>{p.title}</li>)}
    </ul>
  );
}
```

➡️ `Suspense` rendert erst das Fallback, bis `fetch` abgeschlossen ist; anschließend wird der Inhalt **gestreamt**.

---

### 4. **Nested Suspense & Parallel Routes**

* Mehrere Suspense-„Inseln“ ermöglichen **progressives Rendering** unterschiedlicher UI-Teile.
* Mit **Parallel Routes** können Bereiche unabhängig geladen werden.

---

🔗 [Next.js – Streaming & Suspense](https://nextjs.org/docs/app/building-your-application/routing/loading-ui-and-streaming)

---

**Zusammenfassung:**
Streaming erlaubt inkrementelles Ausliefern von Server-rendered Content; Suspense steuert, welche UI-Teile Fallbacks anzeigen, bis Daten da sind. Zusammen verbessern sie **Performance und User Experience**, weil Nutzer sofort etwas sehen, auch wenn andere Teile noch laden.

  **[⬆ Наверх](#top)**

94. ### <a name="94"></a> Wie funktionieren Parallel Routes?

**Parallel Routes in Next.js (App Router, ab v13):**

---

### 1. **Definition**

* Parallel Routes erlauben, **mehrere UI-Bereiche gleichzeitig** und unabhängig voneinander zu rendern.
* Jeder Bereich hat seinen eigenen „Slot“ (`@slotName`) im Layout.
* Ideal für Dashboards, Sidebars oder Overlays, die **parallel** geladen werden sollen.

---

### 2. **Grundstruktur**

```
app/
 ├─ layout.js
 ├─ page.js
 ├─ @analytics/page.js
 └─ @team/page.js
```

* `@analytics` und `@team` sind **benannte Slots**.
* In `layout.js` definierst du, wie diese Slots angezeigt werden.

```js
// app/layout.js
export default function RootLayout({ children, analytics, team }) {
  return (
    <div>
      <aside>{analytics}</aside>
      <main>{children}</main>
      <section>{team}</section>
    </div>
  );
}
```

* `children` → Standardroute
* `analytics` & `team` → Inhalte aus den entsprechenden `@slot`-Ordnern

---

### 3. **Vorteile**

* **Unabhängiges Laden**: Jeder Slot wird separat gestreamt (mit Suspense kombinierbar).
* **Flexibles UI**: Seitenabschnitte können **unterschiedliche Routing-Logik** haben.
* **Bessere UX**: Hauptinhalt kann sofort erscheinen, während Sidebar/Extras noch laden.

---

### 4. **Advanced: Default und Error UI**

* Jeder Slot kann eine **`default.js`** enthalten → Fallback, wenn kein Inhalt aktiv ist.
* Slots können eigene `error.js`, `loading.js` und `not-found.js` haben.

```js
// app/@analytics/default.js
export default function DefaultAnalytics() {
  return <p>No Analytics Data</p>;
}
```

---

🔗 [Next.js – Parallel Routes](https://nextjs.org/docs/app/building-your-application/routing/parallel-routes)

---

**Zusammenfassung:**
Parallel Routes teilen die UI in mehrere **benannte Slots** (`@slot`), die unabhängig voneinander geladen und gestreamt werden. Sie ermöglichen **gleichzeitiges Laden verschiedener UI-Bereiche**, was besonders in Dashboards oder komplexen Apps nützlich ist.

  **[⬆ Наверх](#top)**

95. ### <a name="95"></a> Was sind Intercepting Routes?

**Intercepting Routes in Next.js (App Router, ab v13.3):**

---

### 1. **Definition**

* Intercepting Routes erlauben, eine Route **abzufangen** und **in einem anderen Kontext darzustellen**, ohne die aktuelle Seite vollständig zu verlassen.
* Typisches Beispiel: Ein Modal-Fenster für Detailansichten, statt einen neuen Tab oder eine neue Seite zu laden.

---

### 2. **Syntax**

* In `app/`-Struktur nutzt man den Präfix **`(..)`**, um eine Route an anderer Stelle abzufangen.

**Beispiel-Projektstruktur:**

```
app/
 ├─ feed/page.js
 ├─ feed/[id]/page.js        // normale Detailseite
 └─ feed/(..)photo/[id]/page.js // Intercepting Route für Modal
```

---

### 3. **Verhalten**

* Besuchst du `/feed/123` direkt → normale Detailseite (`feed/[id]/page.js`).
* Klickst du innerhalb von `/feed` auf ein Foto → dieselbe Route wird **abgefangen** und im Modal (`(..)photo/[id]`) angezeigt, während der Feed sichtbar bleibt.

---

### 4. **Codebeispiel Modal-Intercept**

```js
// app/feed/(..)photo/[id]/page.js
'use client';

import {useRouter} from 'next/navigation';

export default function PhotoModal({params}) {
  const router = useRouter();
  return (
    <div className="modal">
      <img src={`/photos/${params.id}.jpg`} alt="Photo" />
      <button onClick={() => router.back()}>Schließen</button>
    </div>
  );
}
```

* `(..)` sagt: „Intercepte die Route `[id]` von `feed/`, aber rendere sie hier im Kontext.“

---

### 5. **Use Cases**

* Modale (Bildergalerien, Detail-Overlays)
* Previews (z. B. Artikelvorschau, ohne die Hauptseite zu verlassen)
* Nested Navigation mit gleichem Content in unterschiedlichen UI-Kontexten

---

🔗 [Next.js – Intercepting Routes](https://nextjs.org/docs/app/building-your-application/routing/intercepting-routes)

---

**Zusammenfassung:**
Intercepting Routes ermöglichen es, **eine Route an einer anderen Stelle darzustellen**, z. B. als Modal oder Overlay, ohne die aktuelle Seite zu verlassen. Sie nutzen den `(..)`-Präfix in der `app/`-Struktur und verbessern so UX bei Detailansichten.

  **[⬆ Наверх](#top)**

96. ### <a name="96"></a> Wie bindet man eine GraphQL-API in Next.js ein?

**GraphQL in Next.js (App Router) einbinden – drei etablierte Wege**

### 1) Direkt per `fetch` (Server Component, leicht & ohne Client-Library)

```js
// app/users/page.js  (Server Component)
const GQL = `#graphql
  query Users($limit:Int!) { users(limit:$limit) { id name email } }
`;

export default async function UsersPage() {
  const res = await fetch(process.env.GRAPHQL_URL, {
    method: 'POST',
    headers: { 'content-type': 'application/json', authorization: `Bearer ${process.env.API_TOKEN}` },
    body: JSON.stringify({ query: GQL, variables: { limit: 5 } }),
    // Caching/ISR nach Bedarf:
    next: { revalidate: 60 } // oder { tags: ['users'] }
  });
  const { data, errors } = await res.json();
  if (errors) throw new Error(errors[0].message);
  return <ul>{data.users.map(u => <li key={u.id}>{u.name}</li>)}</ul>;
}
```

* Vorteil: minimal, nutzt Next.js-Server-Fetch inkl. Cache/Revalidate.
* Passend für SSR/ISR ohne zusätzliche Runtime auf dem Client.
  Quelle: Next.js Data Fetching & Caching im App Router. ([nextjs.org][1])

---

### 2) Apollo Client (Client- oder hybride Nutzung, Typ-Safety & Cache)

**Provider einrichten (App Router)**

```js
// app/providers.jsx  (Client Component)
'use client';
import { ApolloClient, InMemoryCache, ApolloProvider, HttpLink } from '@apollo/client';

const client = new ApolloClient({
  link: new HttpLink({ uri: process.env.NEXT_PUBLIC_GRAPHQL_URL, fetch }),
  cache: new InMemoryCache()
});

export default function Providers({ children }) {
  return <ApolloProvider client={client}>{children}</ApolloProvider>;
}
```

```js
// app/layout.js  (Server Component)
import Providers from './providers.jsx';

export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body><Providers>{children}</Providers></body>
    </html>
  );
}
```

**Query im Client**

```js
// app/users/ClientUsers.jsx  (Client Component)
'use client';
import { gql, useQuery } from '@apollo/client';

const USERS = gql`query { users { id name } }`;

export default function ClientUsers() {
  const { data, loading, error } = useQuery(USERS);
  if (loading) return <p>Lade…</p>;
  if (error) return <p>Fehler: {error.message}</p>;
  return <ul>{data.users.map(u => <li key={u.id}>{u.name}</li>)}</ul>;
}
```

* Vorteil: Normalisierte Caches, React-Hooks, starke Ökosystem-Unterstützung.
* Für App Router existiert eine offizielle Integration von Apollo. ([GitHub][2])

---

### 3) `urql` (leichtgewichtig, gut für App Router)

```js
// app/providers.jsx  (Client Component)
'use client';
import { Provider, createClient } from 'urql';

const client = createClient({ url: process.env.NEXT_PUBLIC_GRAPHQL_URL });

export default function Providers({ children }) {
  return <Provider value={client}>{children}</Provider>;
}
```

```js
// app/users/ClientUsers.jsx  (Client Component)
'use client';
import { useQuery } from 'urql';

const Users = `
  query { users { id name } }
`;

export default function ClientUsers() {
  const [{ data, fetching, error }] = useQuery({ query: Users });
  if (fetching) return <p>Lade…</p>;
  if (error) return <p>Fehler: {error.message}</p>;
  return <ul>{data.users.map(u => <li key={u.id}>{u.name}</li>)}</ul>;
}
```

* Vorteil: kleiner Footprint, gute SSR-Story (next-urql/SSR-Guides). ([nearform.com][3])

---

### Praxis-Hinweise

* **Env-Vars:** Server-seitig `process.env.GRAPHQL_URL`; im Browser nur `NEXT_PUBLIC_…`.
* **Caching/Revalidate:** Bei `fetch` per `next: { revalidate }`/`cache` steuern; bei Apollo/urql über deren Cache. ([nextjs.org][1])
* **Type-Safety:** GraphQL Code Generator für Typen/Hooks. ([Webkul Software][4])
* **Security:** Keine Secrets im Client; Auth-Header in Server Components oder per Route Handler injizieren.

**Weiterlesen (offiziell):**

* Next.js App Router – Data Fetching/Caching/Revalidate & `fetch` API. ([nextjs.org][1])
* Apollo Client – Getting Started & App-Router-Integration. ([apollographql.com][5])
* urql – SSR/Next.js Leitfaden. ([nearform.com][3])
* Next.js – Installation/Grundlagen. ([nextjs.org][6])

---

**Zusammenfassung:**
Für Next.js (App Router) sind drei Wege üblich: **(1)** reines `fetch` in Server Components (einfach, SSR/ISR-freundlich), **(2)** **Apollo Client** mit Provider für komfortable Hooks & Cache, **(3)** **urql** als leichtgewichtige Alternative. Caching/ISR über Next.js steuern (bei `fetch`) oder über den Client-Cache; Env-Vars sauber trennen (Server vs. `NEXT_PUBLIC_`). ([nextjs.org][1])

[1]: https://nextjs.org/docs/14/app/building-your-application/data-fetching/fetching-caching-and-revalidating?utm_source=chatgpt.com "Data Fetching, Caching, and Revalidating"
[2]: https://github.com/apollographql/apollo-client-integrations?utm_source=chatgpt.com "Apollo Client support for the Next.js App Router"
[3]: https://nearform.com/open-source/urql/docs/advanced/server-side-rendering/?utm_source=chatgpt.com "Server-side Rendering | urql Documentation"
[4]: https://webkul.com/blog/nextjs-graphql-codegen/?utm_source=chatgpt.com "GraphQL CodeGen with Next.js"
[5]: https://www.apollographql.com/docs/react/get-started?utm_source=chatgpt.com "Get started with Apollo Client"
[6]: https://nextjs.org/docs/app/getting-started/fetching-data?utm_source=chatgpt.com "Getting Started: Fetching Data"

  **[⬆ Наверх](#top)**

97. ### <a name="97"></a> Wie integriert man Redux Toolkit mit Next.js?

**Redux Toolkit im Next.js App Router integrieren (empfohlener Ansatz)**

### 1) Store & Slice anlegen

```js
// lib/store.js
import { configureStore, createSlice } from '@reduxjs/toolkit';

const counterSlice = createSlice({
  name: 'counter',
  initialState: { value: 0 },
  reducers: {
    inc: (state) => { state.value += 1; },
    add: (state, action) => { state.value += action.payload; }
  }
});

export const { inc, add } = counterSlice.actions;

export const makeStore = () =>
  configureStore({
    reducer: { counter: counterSlice.reducer },
    // optional: middleware, devTools etc.
  });

export const store = makeStore();
```

### 2) Provider als **Client Component**

> Hooks wie `useSelector` / `useDispatch` funktionieren nur in **Client Components**.

```js
// app/providers.jsx
'use client';
import { Provider } from 'react-redux';
import { store } from '@/lib/store';

export default function Providers({ children }) {
  return <Provider store={store}>{children}</Provider>;
}
```

### 3) Provider im Root-Layout einhängen

```js
// app/layout.js
import Providers from './providers.jsx';

export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body>
        <Providers>{children}</Providers>
      </body>
    </html>
  );
}
```

### 4) Nutzung in Client Components

```js
// app/example/Counter.jsx
'use client';
import { useDispatch, useSelector } from 'react-redux';
import { inc, add } from '@/lib/store';

export default function Counter() {
  const value = useSelector((s) => s.counter.value);
  const dispatch = useDispatch();

  return (
    <div>
      <p>Count: {value}</p>
      <button onClick={() => dispatch(inc())}>+1</button>
      <button onClick={() => dispatch(add(5))}>+5</button>
    </div>
  );
}
```

### 5) Server Components beachten

* Server Components **dürfen keine Redux-Hooks** nutzen.
* Muster: Daten in Server Components laden, per Props an Client Components mit Redux übergeben **oder** State ausschließlich im Client verwalten. ([redux-toolkit.js.org][1])

### 6) RTK Query (optional)

* Client-seitig: normal über Hooks (`useGetXQuery`).
* Klassisches SSR mit Pages Router nutzt `next-redux-wrapper` zur Rehydration; im App Router setzt man eher auf **Client-Fetching** oder serverseitiges `fetch` + Props. ([redux-toolkit.js.org][2])

**Quellen:**

* Redux Toolkit – *Setup mit Next.js (App Router)*. ([redux-toolkit.js.org][1])
* Redux Toolkit – *Quick Start* / *Usage Guide*. ([redux-toolkit.js.org][3])
* Next.js – *Getting Started (App Router Grundlagen)*. ([nextjs.org][4])
* Next.js – *Installation* (Referenzlink). ([nextjs.org][4])

---

**Zusammenfassung:**
Store mit RTK erstellen → `Provider` als **Client Component** definieren → im `app/layout.js` einbinden → Hooks nur in Client Components verwenden. Für RTK Query im App Router bevorzugt Client-Hooks oder serverseitiges `fetch` + Props; SSR-Rehydration ist primär ein Pages-Router-Pattern. ([redux-toolkit.js.org][1])

[1]: https://redux-toolkit.js.org/usage/nextjs?utm_source=chatgpt.com "Redux Toolkit Setup with Next.js"
[2]: https://redux-toolkit.js.org/rtk-query/usage/server-side-rendering?utm_source=chatgpt.com "Server Side Rendering"
[3]: https://redux-toolkit.js.org/tutorials/quick-start?utm_source=chatgpt.com "Redux Toolkit Quick Start"
[4]: https://nextjs.org/docs/app/getting-started?utm_source=chatgpt.com "App Router: Getting Started"

  **[⬆ Наверх](#top)**

98. ### <a name="98"></a> Wie integriert man Zustand mit Next.js?

**Zustand mit Next.js (App Router) integrieren — schlank & SSR-sicher**

### 1) Basis-Store (ohne Provider)

```js
// lib/store.js
import {create} from 'zustand';

export const useCounter = create((set) => ({
  value: 0,
  inc: () => set((s) => ({ value: s.value + 1 })),
  add: (n) => set((s) => ({ value: s.value + n })),
}));
```

```js
// app/example/Counter.jsx
'use client';
import {useCounter} from '@/lib/store';

export default function Counter() {
  const value = useCounter((s) => s.value);         // selektiver Zugriff
  const inc = useCounter((s) => s.inc);
  return (
    <div>
      <p>Value: {value}</p>
      <button onClick={inc}>+1</button>
    </div>
  );
}
```

* Hooks nur in **Client Components** verwenden. Server/Client-Komponenten: siehe Next.js App-Router-Grundlagen. ([nextjs.org][1])

---

### 2) SSR-sicherer Store mit Initialzustand vom Server

Wenn der anfängliche Zustand **vom Server** kommt (z. B. Session, DB), pro Request einen Store erstellen und in einem **Client-Provider** einmalig initialisieren.

```js
// lib/makeStore.js
import {createStore} from 'zustand';
export function initCounterStore(preloaded = { value: 0 }) {
  return createStore(() => ({ ...preloaded, inc: () => {} })); // Platzhalter; s. unten
}
```

```js
// app/providers.jsx
'use client';
import {useRef} from 'react';
import {create} from 'zustand';
import {initCounterStore} from '@/lib/makeStore';

export function CounterProvider({ children, initialState }) {
  // Store nur einmal pro Client instanziieren
  const storeRef = useRef();
  if (!storeRef.current) {
    const base = initCounterStore(initialState).getState();
    storeRef.current = create((set) => ({
      ...base,
      inc: () => set((s) => ({ value: s.value + 1 })),
    }));
  }
  return <ZustandContext.Provider value={storeRef.current}>{children}</ZustandContext.Provider>;
}
```

```js
// app/layout.js  (Server Component)
import {CounterProvider} from './providers.jsx';

export default async function RootLayout({ children }) {
  const initial = { value: 5 }; // z. B. aus DB/Session
  return (
    <html lang="de">
      <body>
        <CounterProvider initialState={initial}>{children}</CounterProvider>
      </body>
    </html>
  );
}
```

> Hintergrund: Next.js rendert Server- und Client-Seite separat; der Zustand darf nicht zwischen Requests „leaken“. Der offizielle Leitfaden empfiehlt pro Request/Client eine **eigene Store-Instanz** zu benutzen. ([zustand.docs.pmnd.rs][2])

---

### 3) Persistenz (optional) mit Middleware

```js
// lib/themeStore.js
import {create} from 'zustand';
import {persist} from 'zustand/middleware';

export const useTheme = create(persist(
  (set) => ({ theme: 'light', toggle: () => set((s) => ({ theme: s.theme === 'light' ? 'dark' : 'light' })) }),
  { name: 'theme-store' } // localStorage-Key (nur Client)
));
```

* Persist nur **im Browser** aktiv; auf dem Server existiert `localStorage` nicht. Bei Hydration-Meldungen ggf. erst nach `useEffect` rendern oder selektiv lesen. ([zustand.docs.pmnd.rs][3])

---

### 4) Best Practices

* **Client only:** Zustand-Consumer-Komponenten mit `'use client'` markieren. ([nextjs.org][1])
* **Selektoren & `shallow`:** immer selektiv subscriben, um Re-Renders zu minimieren.
* **Hydration-Fallen:** Bei Persist/Browser-APIs auf **Mismatch** achten und mit „hasMounted“-Guard oder lazy init umgehen (siehe Community-Guides). ([Medium][4])
* **Kein globaler Singleton bei Server-Initialzustand:** pro Request initialisieren (siehe Zustand-Next.js-Guide). ([zustand.docs.pmnd.rs][2])

---

**Weiterlesen:**

* Zustand – *Setup with Next.js (SSR-Hinweise, per-request Stores)*. ([zustand.docs.pmnd.rs][2])
* Zustand – *Persist middleware*. ([zustand.docs.pmnd.rs][3])
* Next.js – *Server und Client Components (App Router)*. ([nextjs.org][1])
* Next.js – *Installation (Referenzlink, wie gefordert)*. ([nextjs.org][5])

---

**Zusammenfassung:**
Zustand im App Router: Store definieren, in **Client Components** nutzen; wenn Serverdaten den Initialzustand bestimmen, den Store **pro Request** erstellen und im Client-Provider einmalig hydrieren. Persistenz per `persist` (nur Client) und auf Hydration achten. Quellen: Zustand-Next.js-Guide, Persist-Doku, Next.js App-Router-Docs. ([zustand.docs.pmnd.rs][2])

[1]: https://nextjs.org/docs/app/getting-started/server-and-client-components?utm_source=chatgpt.com "Getting Started: Server and Client Components"
[2]: https://zustand.docs.pmnd.rs/guides/nextjs?utm_source=chatgpt.com "Setup with Next.js - Zustand"
[3]: https://zustand.docs.pmnd.rs/integrations/persisting-store-data?utm_source=chatgpt.com "Persisting store data - Zustand"
[4]: https://medium.com/%40koalamango/fix-next-js-hydration-error-with-zustand-state-management-0ce51a0176ad?utm_source=chatgpt.com "Fix Next.js 14 hydration error with Zustand state management"
[5]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"

  **[⬆ Наверх](#top)**

99. ### <a name="99"></a> Wie integriert man React Query mit Next.js?

**React Query (TanStack Query) im Next.js App Router integrieren (inkl. SSR/Hydration)**

### 1) Provider als **Client Component**

```js
// app/providers.jsx
'use client';
import { useState } from 'react';
import { QueryClient, QueryClientProvider } from '@tanstack/react-query';

export default function Providers({ children }) {
  // pro Browser-Session EIN QueryClient (verhindert Leaks/Neuerstellung)
  const [client] = useState(() => new QueryClient());
  return <QueryClientProvider client={client}>{children}</QueryClientProvider>;
}
```

```js
// app/layout.js (Server Component)
import Providers from './providers.jsx';

export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body><Providers>{children}</Providers></body>
    </html>
  );
}
```

### 2) SSR/Streaming mit **HydrationBoundary** (empfohlen)

```js
// app/users/page.js  (Server Component)
import { dehydrate, HydrationBoundary, QueryClient } from '@tanstack/react-query';
import UsersClient from './UsersClient.jsx';

async function prefetchUsers(qc) {
  await qc.prefetchQuery({
    queryKey: ['users', { limit: 5 }],
    queryFn: async () => {
      const res = await fetch(process.env.API_URL + '/users?limit=5', { cache: 'no-store' });
      if (!res.ok) throw new Error('Failed to fetch users');
      return res.json();
    },
  });
}

export default async function UsersPage() {
  const qc = new QueryClient();
  await prefetchUsers(qc);     // Server holt Daten vorab
  const state = dehydrate(qc); // dehydrieren → an Client übergeben

  return (
    // Teile der UI können gestreamt werden; Query-Daten sind sofort da
    <HydrationBoundary state={state}>
      <UsersClient />
    </HydrationBoundary>
  );
}
```

```js
// app/users/UsersClient.jsx  (Client Component)
'use client';
import { useQuery } from '@tanstack/react-query';

export default function UsersClient() {
  const { data, isLoading, error } = useQuery({
    queryKey: ['users', { limit: 5 }],
    queryFn: async () => {
      const res = await fetch(process.env.NEXT_PUBLIC_API_URL + '/users?limit=5');
      if (!res.ok) throw new Error('Failed');
      return res.json();
    },
    staleTime: 30_000, // Beispiel: Cache-Einstellung
  });

  if (isLoading) return <p>Lade…</p>;
  if (error) return <p>Fehler: {error.message}</p>;
  return <ul>{data?.map(u => <li key={u.id}>{u.name}</li>)}</ul>;
}
```

**Wichtig**

* **Provider muss clientseitig** sein; `useState(() => new QueryClient())` verhindert, dass pro Render ein neuer Client entsteht.
* **HydrationBoundary+dehydrate**: Server-prefetch → sofort nutzbare Daten ohne FOUC; kompatibel mit **Streaming/Suspense** im App Router.
* **Env-Vars:** Server: `API_URL`; Client: `NEXT_PUBLIC_API_URL`.
* **Alternative:** rein serverseitig mit `fetch` (ohne React Query) für einfache SSR/ISR-Fälle; React Query lohnt sich für clientseitiges Re-Fetching, Caching, Mutations.

**Quellen (aktuell):**

* TanStack Query – *Advanced Server Rendering* (App Router, Streaming, HydrationBoundary). ([tanstack.com][1])
* TanStack Query – *Server Rendering & Hydration* (dehydrate/hydrate). ([tanstack.com][2])
* (Referenzlink gefordert) Next.js – *Installation / Getting Started*. ([nextjs.org][3])

---

**Zusammenfassung:**
`QueryClientProvider` als **Client Component**, pro Browser einen `QueryClient`. Für SSR: im **Server Component** Queries per `prefetchQuery` laden, `dehydrate` aufrufen und mit **HydrationBoundary** an den Client übergeben. So kombinierst du Next.js-Streaming mit React-Query-Caching und bekommst sofort gerenderte, reaktive Daten. ([tanstack.com][1])

[1]: https://tanstack.com/query/v5/docs/react/guides/advanced-ssr?utm_source=chatgpt.com "Advanced Server Rendering | TanStack Query React Docs"
[2]: https://tanstack.com/query/v5/docs/react/guides/ssr?utm_source=chatgpt.com "Server Rendering & Hydration | TanStack Query React Docs"
[3]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"

  **[⬆ Наверх](#top)**

100. ### <a name="100"></a> Wie implementiert man SSR mit Redux in Next.js?

**SSR mit Redux in Next.js (App Router & Pages Router)**

### App Router (empfohlen ab Next 13)

**Ziel:** pro Request einen frischen Store, Daten serverseitig laden und beim ersten Render ohne Flicker anzeigen.

1. **Store pro Request + Provider (Client Component)**

```js
// lib/store.js
import { configureStore, createSlice } from '@reduxjs/toolkit';

const counter = createSlice({
  name: 'counter',
  initialState: { value: 0 },
  reducers: { set: (s, a) => { s.value = a.payload; } }
});
export const { set } = counter.actions;

export const makeStore = () =>
  configureStore({ reducer: { counter: counter.reducer } });
```

```js
// app/StoreProvider.jsx
'use client';
import { useRef } from 'react';
import { Provider } from 'react-redux';
import { makeStore } from '@/lib/store';
import { set } from '@/lib/store';

export default function StoreProvider({ children, initialCount = 0 }) {
  const storeRef = useRef();
  if (!storeRef.current) {
    storeRef.current = makeStore();
    // Wichtig: beim ersten Render initialisieren (nicht in useEffect!)
    storeRef.current.dispatch(set(initialCount));
  }
  return <Provider store={storeRef.current}>{children}</Provider>;
}
```

2. **Serverseitig Daten laden und als Prop übergeben**

```js
// app/page.js  (Server Component)
import StoreProvider from './StoreProvider';

export default async function Page() {
  const countFromServer = 5; // z. B. DB/Fetch
  return (
    <html lang="de">
      <body>
        <StoreProvider initialCount={countFromServer}>
          {/* Client-UI, die Redux nutzt */}
          <Counter />
        </StoreProvider>
      </body>
    </html>
  );
}
```

```js
// app/Counter.jsx  (Client Component)
'use client';
import { useSelector } from 'react-redux';

export default function Counter() {
  const value = useSelector(s => s.counter.value);
  return <p>SSR-Wert: {value}</p>;
}
```

**Hinweise:**

* RSCs (Server Components) lesen/schreiben **nicht** direkt den Redux-Store; Initialdaten per Props an einen **Client-Provider** übergeben und dort dispatchen.
* Vermeide Initialisierung in `useEffect` → sonst Hydration-Differenzen. ([Redux][1])

---

### Pages Router (klassisch)

**Pattern:** `next-redux-wrapper` + `getServerSideProps`/`getStaticProps` → Server-Store wird befüllt und per HYDRATE an den Client übergeben.

```js
// store.ts
import { configureStore } from '@reduxjs/toolkit';
export const makeStore = () => configureStore({ reducer: {/* ... */} });
export const wrapper = createWrapper(makeStore); // aus next-redux-wrapper
```

```js
// pages/index.tsx
import { wrapper } from '@/store';
import { set } from '@/features/counter';

export const getServerSideProps = wrapper.getServerSideProps(
  store => async () => {
    store.dispatch(set(5)); // Server-State
    return { props: {} };
  }
);

export default function Home() { /* ... */ }
```

**Hinweis:** `next-redux-wrapper` kapselt HYDRATE und synchronisiert Server-→Client-State. ([GitHub][2])

---

### Typische Stolpersteine (SSR + Redux)

* **Hydration-Fehler**: Unterschiedlicher HTML-Baum Server/Client (z. B. wenn State erst im `useEffect` gesetzt wird). Initialisierung **während** des ersten Renders im Provider durchführen. ([nextjs.org][3])
* **Globaler Singleton-Store** im App Router → Request-Leaks. Immer **per Request** erzeugen. ([Redux][1])

**Weiterlesen (offiziell/aktuell):**

* Redux Toolkit – *Setup with Next.js* (Fokus **App Router**, per-Request Store, Initialdaten) ([Redux][1])
* `next-redux-wrapper` (Pages Router + SSR/HYDRATE) ([GitHub][2])
* RTK Query SSR mit Next.js (Pages Router) ([redux-toolkit.js.org][4])
* Next.js – *Installation* (Referenzlink) ([nextjs.org][5])

---

**Zusammenfassung:**
App Router: Store **pro Request** erzeugen, Daten in einer **Server Component** laden und als Props an einen **Client-Provider** geben, der beim ersten Render dispatcht (keine `useEffect`-Init). Pages Router: **`next-redux-wrapper`** nutzen und in `getServerSideProps`/`getStaticProps` befüllen (HYDRATE synchronisiert). Dies verhindert Hydration-Fehler und ermöglicht echtes SSR mit Redux. ([Redux][1])

[1]: https://redux.js.org/usage/nextjs "Redux Toolkit Setup with Next.js | Redux"
[2]: https://github.com/kirill-konshin/next-redux-wrapper?utm_source=chatgpt.com "kirill-konshin/next-redux-wrapper: Redux wrapper for Next.js"
[3]: https://nextjs.org/docs/messages/react-hydration-error?utm_source=chatgpt.com "Text content does not match server-rendered HTML"
[4]: https://redux-toolkit.js.org/rtk-query/usage/server-side-rendering?utm_source=chatgpt.com "Server Side Rendering"
[5]: https://nextjs.org/docs/app/getting-started/fetching-data?utm_source=chatgpt.com "Getting Started: Fetching Data"

  **[⬆ Наверх](#top)**    

101. ### <a name="101"></a> Wie richtet man eine PWA in Next.js ein?

**PWA in Next.js (App Router) einrichten – ohne Zusatz-Plugin**

### 1) Web App Manifest anlegen

`app/manifest.json` (oder `app/manifest.webmanifest`)

```js
{
  "name": "My App",
  "short_name": "MyApp",
  "start_url": "/",
  "display": "standalone",
  "background_color": "#ffffff",
  "theme_color": "#111111",
  "icons": [
    { "src": "/icons/icon-192.png", "sizes": "192x192", "type": "image/png" },
    { "src": "/icons/icon-512.png", "sizes": "512x512", "type": "image/png" }
  ]
}
```

Icons nach `public/icons` legen. In Next.js wird das Manifest automatisch erkannt. ([nextjs.org][1])

### 2) `<link rel="manifest">` & Meta (optional, falls nicht automatisch gesetzt)

```js
// app/layout.js
export const metadata = {
  title: 'My App',
  themeColor: '#111111',
  manifest: '/manifest.json'
};
export default function RootLayout({ children }) {
  return <html lang="de"><body>{children}</body></html>;
}
```

([nextjs.org][2])

### 3) Service Worker erstellen und registrieren

`public/sw.js` (ein einfaches Cache-First-Beispiel)

```js
// public/sw.js
const CACHE = 'app-cache-v1';
self.addEventListener('install', (e) => {
  e.waitUntil(caches.open(CACHE).then((c) => c.addAll(['/'])));
});
self.addEventListener('fetch', (e) => {
  e.respondWith(
    caches.match(e.request).then((res) => res || fetch(e.request))
  );
});
```

Client-Registrierung (nur im Browser):

```js
// app/sw-register.jsx
'use client';
import { useEffect } from 'react';

export default function SWRegister() {
  useEffect(() => {
    if ('serviceWorker' in navigator) {
      navigator.serviceWorker.register('/sw.js');
    }
  }, []);
  return null;
}
```

Im Root-Layout einbinden:

```js
// app/layout.js
import SWRegister from './sw-register.jsx';
export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body>
        <SWRegister />
        {children}
      </body>
    </html>
  );
}
```

Grundlagen zu Service Workern und Offline-Caching siehe Guides. ([nextjs.org][2])

### 4) Installierbarkeit testen

* Via **Lighthouse** oder Chrome „Application → Manifest/Service Workers“.
* HTTPS ist Pflicht; lokal mit `next dev`, produktiv über TLS hosten. ([nextjs.org][2])

### 5) Optional: `next-pwa` verwenden

Wenn du Workbox-Features (Precache, Runtime-Caching-Strategien) komfortabel willst:

```js
// next.config.js
import withPWA from 'next-pwa';
export default withPWA({
  dest: 'public',
  // weitere Optionen…
});
```

Dokumentation und App-Router-Hinweise beachten. ([ducanh-next-pwa.vercel.app][3])

**Weiterlesen (offiziell):**

* Next.js – **PWAs Guide** (Manifest, SW, A2HS, Tests). ([nextjs.org][2])
* Next.js – **Manifest Datei** (File Convention). ([nextjs.org][1])
* Next.js – **Installation (Referenzlink)**. ([nextjs.org][4])

---

**Zusammenfassung:**
Manifest unter `app/manifest.json` + Icons in `public/`, Service Worker in `public/sw.js` schreiben und in einer Client-Komponente registrieren, optional Workbox/`next-pwa` für komfortables Caching. Installierbarkeit/Offline-Funktion via Lighthouse prüfen; HTTPS ist erforderlich. ([nextjs.org][2])

[1]: https://nextjs.org/docs/app/api-reference/file-conventions/metadata/manifest?utm_source=chatgpt.com "Metadata Files: manifest.json"
[2]: https://nextjs.org/docs/app/guides/progressive-web-apps?utm_source=chatgpt.com "Guides: PWAs"
[3]: https://ducanh-next-pwa.vercel.app/docs/next-pwa/getting-started?utm_source=chatgpt.com "Getting started - next-pwa"
[4]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"

  **[⬆ Наверх](#top)**

102. ### <a name="102"></a> Wie implementiert man dynamische Meta-Informationen (head)?

**Dynamische Meta-Informationen (SEO) im Next.js App Router**

---

### 1) **Statische Meta-Infos** (Basis)

Im App Router nutzt man `export const metadata` in `layout.js` oder `page.js`.

```js
// app/page.js
export const metadata = {
  title: 'Startseite',
  description: 'Meine Next.js App',
};
```

---

### 2) **Dynamische Meta-Infos mit `generateMetadata`**

Mit `generateMetadata` kannst du die Meta-Daten **pro Request** dynamisch setzen (z. B. via `params` oder `fetch`).

```js
// app/blog/[slug]/page.js
export async function generateMetadata({ params }) {
  const post = await fetch(`https://api.example.com/posts/${params.slug}`)
    .then((res) => res.json());

  return {
    title: post.title,
    description: post.excerpt,
    openGraph: {
      title: post.title,
      description: post.excerpt,
      url: `https://example.com/blog/${params.slug}`,
      images: [{ url: post.image }],
    },
  };
}

export default function BlogPost({ params }) {
  return <h1>{params.slug}</h1>;
}
```

➡️ `generateMetadata` läuft **auf dem Server** und unterstützt asynchrone Datenquellen.

---

### 3) **Nested Metadata (Layouts + Pages)**

* `layout.js` → setzt Basis-SEO für einen Bereich.
* `page.js` → überschreibt oder ergänzt.
* Next.js **merged** die Metadata automatisch.

---

### 4) **Beispiele für weitere Felder**

```js
// app/product/[id]/page.js
export async function generateMetadata({ params }) {
  return {
    title: `Produkt ${params.id} | Shop`,
    description: `Details zum Produkt ${params.id}`,
    alternates: {
      canonical: `/product/${params.id}`,
      languages: {
        'en': `/en/product/${params.id}`,
        'de': `/de/product/${params.id}`,
      },
    },
    robots: { index: true, follow: true },
  };
}
```

---

### 5) **Pages Router (ältere Version)**

* Dort verwendet man `next/head`:

```js
// pages/blog/[slug].js
import Head from 'next/head';

export default function Blog({ post }) {
  return (
    <>
      <Head>
        <title>{post.title}</title>
        <meta name="description" content={post.excerpt} />
      </Head>
      <h1>{post.title}</h1>
    </>
  );
}
```

---

🔗 [Next.js – Metadata API](https://nextjs.org/docs/app/building-your-application/optimizing/metadata)

---

**Zusammenfassung:**
Im App Router setzt man dynamische Meta-Infos mit `generateMetadata` (async möglich, Datenabhängig). Statische Werte mit `metadata` in `layout.js`/`page.js`. Im Pages Router nutzt man `<Head>`. So lassen sich Titel, Open Graph, Canonical, Robots etc. flexibel steuern.

  **[⬆ Наверх](#top)**

103. ### <a name="103"></a> Wie funktioniert die metadata API im App Router?

**Metadata API im Next.js App Router**

---

### 1) **Definition**

* Die **Metadata API** ist das zentrale Feature im App Router für **SEO, Open Graph, Robots, Favicons, Manifest usw.**
* Statt `<Head>`-Komponenten wie im Pages Router nutzt man strukturierte Objekte (`metadata`) oder die Funktion `generateMetadata`.

---

### 2) **Statische Metadata**

Einfaches Objekt in `page.js` oder `layout.js`:

```js
// app/page.js
export const metadata = {
  title: 'Home',
  description: 'Startseite meiner Next.js-App',
  keywords: ['Next.js', 'SEO', 'App Router'],
};
```

➡️ Wird beim Build gesetzt, **nicht dynamisch**.

---

### 3) **Dynamische Metadata**

Mit `generateMetadata` (async möglich, z. B. für API-Daten oder URL-Parameter):

```js
// app/blog/[slug]/page.js
export async function generateMetadata({ params }) {
  const post = await fetch(`https://api.example.com/posts/${params.slug}`).then(r => r.json());

  return {
    title: post.title,
    description: post.excerpt,
    openGraph: {
      title: post.title,
      description: post.excerpt,
      url: `https://example.com/blog/${params.slug}`,
      images: [{ url: post.image }],
    },
  };
}

export default function BlogPost({ params }) {
  return <h1>{params.slug}</h1>;
}
```

➡️ `generateMetadata` läuft auf dem **Server**, daher sicher für Secrets.

---

### 4) **Merge von Layout & Page**

* `layout.js`-Metadata liefert Standardwerte.
* `page.js`-Metadata überschreibt oder ergänzt diese.
* Ergebnis = **kombinierte SEO-Infos pro Route**.

---

### 5) **Unterstützte Felder**

* **SEO**: `title`, `description`, `keywords`
* **Open Graph / Twitter**: `openGraph`, `twitter`
* **Internationalisierung**: `alternates.languages`
* **Technisch**: `robots`, `icons`, `manifest`
* **Weitere**: `metadataBase` (für absolute URLs)

---

### 6) **Unterschied zu Pages Router**

* Pages Router: `<Head>`-Komponente (`next/head`).
* App Router: **strukturierte Objekte + API** → sicherer, standardisierter, asynchron möglich.

---

🔗 [Next.js – Metadata API](https://nextjs.org/docs/app/building-your-application/optimizing/metadata)

---

**Zusammenfassung:**
Die Metadata API ersetzt `<Head>` im App Router. Statische Daten setzt man mit `export const metadata`, dynamische mit `generateMetadata`. Layouts liefern Defaults, Pages überschreiben. Unterstützt SEO, Social Media, Robots, Favicons und Internationalisierung.

  **[⬆ Наверх](#top)**

104. ### <a name="104"></a> Wie fügt man eine Sitemap in Next.js hinzu?

**Sitemap in Next.js (App Router, ab v13.3+)**

---

### 1) **Dateikonvention nutzen**

Next.js bietet eine eingebaute **Sitemap API** über den App Router.

* Lege `app/sitemap.js` oder `app/sitemap.ts` an.
* Die Datei muss eine Funktion exportieren, die Routen zurückgibt.

---

### 2) **Statische Sitemap**

```js
// app/sitemap.js
export default function sitemap() {
  return [
    {
      url: 'https://example.com',
      lastModified: new Date(),
      changeFrequency: 'daily',
      priority: 1.0,
    },
    {
      url: 'https://example.com/about',
      lastModified: new Date(),
      changeFrequency: 'monthly',
      priority: 0.8,
    },
  ];
}
```

➡️ Next.js generiert daraus automatisch `https://example.com/sitemap.xml`.

---

### 3) **Dynamische Sitemap (z. B. Blog)**

```js
// app/sitemap.js
export default async function sitemap() {
  const posts = await fetch('https://api.example.com/posts').then(r => r.json());

  const postUrls = posts.map((post) => ({
    url: `https://example.com/blog/${post.slug}`,
    lastModified: new Date(post.updatedAt),
  }));

  return [
    { url: 'https://example.com', lastModified: new Date() },
    ...postUrls,
  ];
}
```

➡️ Ideal für dynamische Inhalte wie Produkte, Blogs, Userseiten.

---

### 4) **Metadata + Alternates für Sprachen**

In Kombination mit der **Metadata API** kannst du `alternates.languages` definieren, damit Suchmaschinen Lokalisierung verstehen.

```js
// app/[locale]/layout.js
export async function generateMetadata({ params }) {
  return {
    alternates: {
      languages: {
        en: `https://example.com/en`,
        de: `https://example.com/de`,
      },
    },
  };
}
```

---

### 5) **Sitemap & robots.txt zusammen**

* `app/robots.js` anlegen für `robots.txt`.

```js
// app/robots.js
export default function robots() {
  return {
    rules: [{ userAgent: '*', allow: '/' }],
    sitemap: 'https://example.com/sitemap.xml',
  };
}
```

---

🔗 [Next.js – Sitemaps](https://nextjs.org/docs/app/api-reference/file-conventions/metadata/sitemap)

---

**Zusammenfassung:**
Eine Sitemap implementiert man im App Router über die Datei `app/sitemap.js`. Dort gibt man statische oder dynamisch generierte Routen zurück. Next.js erstellt daraus automatisch `sitemap.xml`, optional kombiniert mit `robots.js` für `robots.txt`.

  **[⬆ Наверх](#top)**

105. ### <a name="105"></a> Wie fügt man eine robots.txt in Next.js hinzu?

**robots.txt in Next.js (App Router, ab v13.3)**

---

### 1) **File Convention nutzen**

Next.js generiert `robots.txt` automatisch, wenn du eine Datei `app/robots.js` oder `app/robots.ts` erstellst.

---

### 2) **Statisches Beispiel**

```js
// app/robots.js
export default function robots() {
  return {
    rules: [
      {
        userAgent: '*',
        allow: '/',
      },
    ],
    sitemap: 'https://example.com/sitemap.xml',
  };
}
```

➡️ Ausgabe:

```
User-agent: *
Allow: /
Sitemap: https://example.com/sitemap.xml
```

---

### 3) **Komplexere Regeln**

```js
// app/robots.js
export default function robots() {
  return {
    rules: [
      { userAgent: '*', allow: '/' },
      { userAgent: 'Googlebot', disallow: ['/private'] },
    ],
    host: 'https://example.com',
    sitemap: [
      'https://example.com/sitemap.xml',
      'https://example.com/sitemap-blog.xml',
    ],
  };
}
```

➡️ Mehrere `Sitemap`-Einträge und Botspezifische Regeln.

---

### 4) **Dynamisch (optional)**

* Da es ein normaler Server-Export ist, kannst du Datenbank/API-Aufrufe nutzen, um dynamische Regeln zu erzeugen.
* Beispiel: einzelne Bereiche für bestimmte User-Agents sperren.

---

🔗 [Next.js – robots.txt](https://nextjs.org/docs/app/api-reference/file-conventions/metadata/robots)

---

**Zusammenfassung:**
Eine `robots.txt` legst du in Next.js einfach über `app/robots.js` an. Du gibst `rules`, `sitemap` und optional `host` zurück; Next.js erstellt daraus automatisch die `robots.txt`. Dynamische Inhalte sind ebenfalls möglich.

  **[⬆ Наверх](#top)**

106. ### <a name="106"></a> Wie integriert man WebSockets in Next.js?

**WebSockets in Next.js integrieren (App Router)**

### 1) Eigenen WebSocket-Server neben Next.js betreiben (empfohlen bei klassischem WS)

**Server (Node, `ws` oder Socket.IO) läuft als separater Prozess/Container; Next.js bleibt „rein“ für HTTP/SSR.**

```js
// server/ws-server.mjs  (Node-Prozess, ESM)
import { WebSocketServer } from 'ws';

const wss = new WebSocketServer({ port: 4000 });
wss.on('connection', (socket) => {
  socket.send(JSON.stringify({ type: 'hello', ts: Date.now() }));
  socket.on('message', (msg) => {
    // Echo an alle
    for (const client of wss.clients) client.send(msg);
  });
});

console.log('WS listening on ws://localhost:4000');
```

```js
// app/ws-client/Client.jsx  (Client Component)
'use client';
import { useEffect, useState } from 'react';

export default function WSClient() {
  const [msgs, setMsgs] = useState([]);
  useEffect(() => {
    const ws = new WebSocket(process.env.NEXT_PUBLIC_WS_URL); // z. B. ws://localhost:4000
    ws.onmessage = (e) => setMsgs((m) => [...m, e.data]);
    return () => ws.close();
  }, []);
  return <ul>{msgs.map((m, i) => <li key={i}>{m}</li>)}</ul>;
}
```

**Warum so?** Route Handlers/Middleware sind HTTP-orientiert; ein stabiler WS-Server läuft am besten als separater Dienst oder auf einer Plattform, die echte WebSocket-Upgrades unterstützt. Auf Vercel sind **WebSockets in Functions** nicht unterstützt; nutze dort z. B. einen externen WS-Dienst oder Realtime-Anbieter. ([nextjs.org][1])

---

### 2) Socket.IO verwenden (gleiche Architektur, komfortabler Client/Rooms)

```js
// server/socket-server.mjs
import { createServer } from 'node:http';
import { Server } from 'socket.io';

const httpServer = createServer();
const io = new Server(httpServer, { cors: { origin: '*' } });

io.on('connection', (socket) => {
  socket.emit('hello', { ts: Date.now() });
  socket.on('msg', (data) => io.emit('msg', data));
});

httpServer.listen(4001);
```

```js
// app/socket/Client.jsx
'use client';
import { useEffect, useState } from 'react';
import { io } from 'socket.io-client';

export default function SocketClient() {
  const [list, setList] = useState([]);
  useEffect(() => {
    const socket = io(process.env.NEXT_PUBLIC_SOCKET_URL);
    socket.on('hello', (p) => setList((arr) => [...arr, `hello ${p.ts}`]));
    socket.on('msg', (m) => setList((arr) => [...arr, m]));
    return () => socket.disconnect();
  }, []);
  return <ul>{list.map((m, i) => <li key={i}>{m}</li>)}</ul>;
}
```

**Hinweis Deployment:** Die **offizielle Socket.IO-Doku** weist darauf hin, dass Vercel-Functions **keine** WebSocket-Verbindungen unterstützen; betreibe Socket.IO woanders (z. B. AWS/ECS, Fly.io, Railway) oder nutze einen Realtime-Service. ([socket.io][2])

---

### 3) Managed Realtime-Services (kein eigener WS-Server)

Wenn du auf Vercel bleibst oder Serverbetrieb vermeiden willst: nutze **Ably/Pusher/Supabase Realtime** – diese liefern persistenten WS-Transport, während Next.js nur HTTP/SSR macht.

* Beispiel/Guide (Next.js + Vercel + Ably): Realtime-Features über externen Dienst. ([Ably Realtime][3])

---

### 4) Alternative bei Einweg-Updates: **SSE** (Server-Sent Events) in Route Handlers

Für reines Downstream-Streaming reicht oft SSE (keine bidirektionale WS-Verbindung nötig).

```js
// app/api/sse/route.js   (Route Handler → Text/Event-Stream)
export async function GET() {
  const stream = new ReadableStream({
    start(controller) {
      const enc = new TextEncoder();
      let i = 0;
      const id = setInterval(() => {
        controller.enqueue(enc.encode(`data: ${JSON.stringify({ tick: ++i })}\n\n`));
      }, 1000);
      return () => clearInterval(id);
    }
  });
  return new Response(stream, {
    headers: { 'Content-Type': 'text/event-stream', 'Cache-Control': 'no-cache' }
  });
}
```

```js
// app/sse/Client.jsx
'use client';
import { useEffect, useState } from 'react';

export default function SSEClient() {
  const [v, setV] = useState(0);
  useEffect(() => {
    const es = new EventSource('/api/sse');
    es.onmessage = (e) => setV(JSON.parse(e.data).tick);
    return () => es.close();
  }, []);
  return <p>Tick: {v}</p>;
}
```

Route Handlers eignen sich gut für SSE und integrieren sich mit dem App-Router. ([nextjs.org][1])

---

### Platform-/Deploy-Hinweise

* **Vercel Functions**: keine WebSocket-Upgrades → WS separat hosten oder Managed Realtime. ([Vercel][4])
* **Eigenes Hosting / Docker**: Next.js + WS-Server in Compose/K8s deployen; Frontend verbindet über `NEXT_PUBLIC_WS_URL`.
* **Sicherheit**: Auth-Token **nicht** im Client speichern; WS-Auth z. B. via signierten Kurz-Tokens oder Upstream-Auth-Endpoint.

**Weiterlesen:**

* Next.js App Router – Route Handlers & Middleware (Architektur/HTTP-Handling). ([nextjs.org][1])
* Vercel – Support-Artikel zu WebSockets in Functions. ([Vercel][4])
* Socket.IO – „How to use with Next.js“. ([socket.io][2])
* **Referenzlink (gewünscht):** Getting Started / Installation. ([nextjs.org][1])

---

**Zusammenfassung:**
Für echte WebSockets: **separaten WS-Server** (z. B. `ws`/Socket.IO) neben Next.js betreiben oder **Managed Realtime** nutzen; Vercel-Functions unterstützen keine WS-Upgrades. Für Einweg-Events reicht **SSE** in Route Handlers. Frontend verbindet sich über `NEXT_PUBLIC_WS_URL`, State/Rooms/Authentifizierung übernimmt der WS-Dienst. ([Vercel][4])

[1]: https://nextjs.org/docs/app/getting-started/route-handlers-and-middleware?utm_source=chatgpt.com "Getting Started: Route Handlers and Middleware"
[2]: https://socket.io/how-to/use-with-nextjs?utm_source=chatgpt.com "How to use with Next.js"
[3]: https://ably.com/blog/next-js-vercel-link-sharing-serverless-websockets?utm_source=chatgpt.com "Next.js + Vercel: Building a live app with serverless ..."
[4]: https://vercel.com/guides/do-vercel-serverless-functions-support-websocket-connections?utm_source=chatgpt.com "Do Vercel Serverless Functions support WebSocket ..."

  **[⬆ Наверх](#top)**

107. ### <a name="107"></a> Wie verwendet man Next.js in einem Monorepo (z. B. Turborepo)?

**Next.js im Monorepo (z. B. mit Turborepo) – Setup & Best Practices**

### 1) Workspace-Struktur

```
repo/
├─ apps/
│  └─ web/                  # Next.js-App
├─ packages/
│  ├─ ui/                   # gemeinsame UI-Komponenten
│  └─ config/               # eslint, tsconfig, tailwind o. ä.
├─ package.json
├─ turbo.json
└─ pnpm-workspace.yaml      # oder npm/yarn workspaces
```

**Workspaces aktivieren**

```js
// package.json (Root)
{
  "private": true,
  "workspaces": ["apps/*", "packages/*"],     // npm/yarn
  // pnpm: in pnpm-workspace.yaml definieren
  "devDependencies": { "turbo": "^2" },
  "scripts": { "dev": "turbo run dev", "build": "turbo run build" }
}
```

Quellen: Turborepo – Next.js Guide & Repo-Struktur. ([Turborepo][1])

---

### 2) Next.js-App hinzufügen

```bash
pnpm dlx create-next-app@latest apps/web
# oder
npm create next-app@latest apps/web
```

Quellen: Next.js Installation (App Router). ([nextjs.org][2])

---

### 3) Gemeinsames Paket („ui“) erstellen

```js
// packages/ui/package.json
{
  "name": "@repo/ui",
  "version": "1.0.0",
  "main": "src/index.ts",
  "types": "src/index.ts",
  "exports": { ".": "./src/index.ts" }
}
```

```js
// packages/ui/src/Button.tsx
export function Button({children}) { return <button>{children}</button>; }
export default Button;
```

In der App verwenden:

```js
// apps/web/app/page.js
import Button from '@repo/ui/src/Button';
export default function Page(){ return <Button>Hi</Button>; }
```

---

### 4) `transpilePackages` für gemeinsame Pakete

Damit Next.js Code aus `packages/*` transpiliert (TS/JSX):

```js
// apps/web/next.config.js (ESM)
export default {
  transpilePackages: ['@repo/ui']  // ersetzt next-transpile-modules
};
```

Quelle: Next.js `transpilePackages`. ([nextjs.org][3])

---

### 5) Pfad-Aliase (optional)

```js
// apps/web/tsconfig.json (oder jsconfig.json)
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": { "@/*": ["./app/*"] }
  }
}
```

Quelle: Absolute Imports & Module Aliases. ([nextjs.org][4])

---

### 6) Turborepo-Pipeline

```js
// turbo.json
{
  "$schema": "https://turbo.build/schema.json",
  "pipeline": {
    "dev": { "cache": false, "persistent": true },
    "build": {
      "dependsOn": ["^build"],
      "outputs": [".next/**", "dist/**"]
    },
    "lint": {}
  }
}
```

Quellen: Turborepo – Package Configurations & Beispiele. ([Turborepo][5])

---

### 7) Dev/Build starten

```bash
# root
pnpm install
pnpm dev          # startet alle dev-Tasks (z. B. apps/web)
pnpm build        # inkrementelle Builds via Turborepo
```

---

### 8) Häufige Stolpersteine

* **Nicht transpiliertes Shared-Package** → `transpilePackages` setzen. ([nextjs.org][3])
* **Unklare Aliase** → Pfade pro Paket definieren; Kollisionen vermeiden. ([nextjs.org][4])
* **CI/Deployment**: auf Vercel das **Monorepo**-Root verbinden, Projektpfad auf `apps/web` setzen; Template/Starter vorhanden. ([Vercel][6])

---

### Minimalbeispiel (Next-App + Turborepo)

```js
// apps/web/package.json
{
  "name": "web",
  "scripts": { "dev": "next dev", "build": "next build", "start": "next start" },
  "dependencies": { "next": "latest", "react": "latest", "react-dom": "latest", "@repo/ui": "*" }
}
```

```js
// pnpm-workspace.yaml (falls pnpm)
packages:
  - "apps/*"
  - "packages/*"
```

Quellen: Next.js Installation; pnpm Workspaces. ([nextjs.org][2])

---

**Weiterlesen**

* Next.js – Getting Started / Installation. ([nextjs.org][2])
* Next.js – `transpilePackages`. ([nextjs.org][3])
* Turborepo – Next.js Guide, Struktur, Beispiele. ([Turborepo][1])
* Vercel Template: „Monorepo with Turborepo“. ([Vercel][6])

---

**Zusammenfassung:**
Monorepo per Workspaces + Turborepo strukturieren, Next-App in `apps/*` anlegen, Shared-Code in `packages/*` auslagern. In Next.js **`transpilePackages`** für lokale Pakete aktivieren und optional Pfad-Aliase setzen. Builds/Devs über `turbo.json` orchestrieren; auf Vercel Monorepo-Projektpfad konfigurieren. ([nextjs.org][2])

[1]: https://turborepo.com/docs/guides/frameworks/nextjs?utm_source=chatgpt.com "Next.js"
[2]: https://nextjs.org/docs/app/getting-started/installation?utm_source=chatgpt.com "Getting Started: Installation"
[3]: https://nextjs.org/docs/app/api-reference/config/next-config-js/transpilePackages?utm_source=chatgpt.com "next.config.js: transpilePackages"
[4]: https://nextjs.org/docs/14/app/building-your-application/configuring/absolute-imports-and-module-aliases?utm_source=chatgpt.com "Configuring: Absolute Imports and Module Path Aliases"
[5]: https://turborepo.com/docs/reference/package-configurations?utm_source=chatgpt.com "Package Configurations"
[6]: https://vercel.com/templates/next.js/monorepo-turborepo?utm_source=chatgpt.com "Monorepo with Turborepo"

  **[⬆ Наверх](#top)**

108. ### <a name="108"></a> Wie funktioniert Hot Reloading in Next.js?

**Hot Reloading in Next.js**

---

### 1) **Definition**

Hot Reloading = Änderungen am Code werden im Dev-Server erkannt und **automatisch im Browser aktualisiert**, ohne dass ein manueller Reload nötig ist. Next.js verwendet dabei **Fast Refresh**, eine React-Technologie für zuverlässiges State-Preserving Reloading.

---

### 2) **Ablauf im Detail**

* Du startest den Dev-Server:

  ```bash
  npm run dev
  ```
* Webpack (oder Turbopack, seit Next.js 13 als neuer Dev-Bundler) überwacht Dateien.
* Sobald eine Datei geändert wird:

  * **Nur betroffene Module** werden neu kompiliert.
  * Browser erhält Update über **Hot Module Replacement (HMR)**.
  * React Fast Refresh rendert die Komponente neu **mit Erhalt des States**, sofern möglich.

---

### 3) **Fast Refresh Verhalten**

* Änderungen in **Komponenten/JSX** → direkt sichtbar, State bleibt erhalten.
* Änderungen in **Hooks oder Business-Logic** → Komponenten werden neu gemountet (State Reset).
* Änderungen an **Server Components** → Seite wird serverseitig neu gerendert und gestreamt.
* Änderungen in **next.config.js** oder `.env` → Dev-Server muss neu gestartet werden.

---

### 4) **Unterschiede App Router vs. Pages Router**

* **Pages Router**: HMR + Fast Refresh wie in React.
* **App Router**: Streaming + React Server Components → Updates können **teilweise** kommen (Client Components sofort, Server Components per Refresh/Stream).

---

### 5) **Beispiel**

```js
// app/page.js
export default function Page() {
  return <h1>Hallo {new Date().toLocaleTimeString()}</h1>;
}
```

➡️ Im Dev-Server: jede Codeänderung wird sofort sichtbar; beim Aktualisieren bleibt der State von Kind-Komponenten erhalten.

---

### 6) **Troubleshooting**

* Hot Reloading funktioniert nicht?

  * Prüfen: läuft `npm run dev` oder `next dev`?
  * Keine manuelle Browser-Caching-Probleme?
  * `node_modules` löschen und neu installieren.
  * Bei **Docker**: Volumes und `CHOKIDAR_USEPOLLING=true` setzen, damit File-Watcher funktioniert.

---

🔗 [Next.js – Fast Refresh](https://nextjs.org/docs/app/building-your-application/optimizing/fast-refresh)

---

**Zusammenfassung:**
Hot Reloading in Next.js basiert auf **HMR + React Fast Refresh**. Änderungen im Code werden ohne kompletten Reload übernommen, wobei der State erhalten bleibt (sofern möglich). Im App Router kommen Server- und Client-Komponenten hinzu → Updates werden gestreamt oder komplett neu gerendert.

  **[⬆ Наверх](#top)**

109. ### <a name="109"></a> Was sind App Router Layouts?

**App Router Layouts in Next.js**

---

### 1) **Definition**

* Layouts sind **React-Komponenten**, die in der App-Router-Struktur (`app/`) auf einer bestimmten Ebene platziert werden.
* Sie dienen als **Wrapper** für darunterliegende Seiten und Routen und ermöglichen gemeinsame UI-Strukturen (z. B. Navigation, Footer, Sidebar).
* Layouts sind **persistent** → sie bleiben zwischen Navigationswechseln erhalten (kein vollständiger Reload).

---

### 2) **Dateikonvention**

* Jede Route kann eine Datei `layout.js` (oder `.tsx`) enthalten.
* `children` wird automatisch an die darunterliegenden Seiten weitergegeben.

**Beispielstruktur:**

```
app/
 ├─ layout.js        // Root Layout (für gesamte App)
 ├─ page.js
 └─ dashboard/
     ├─ layout.js    // Layout nur für Dashboard
     ├─ page.js
     └─ settings/
         └─ page.js
```

---

### 3) **Codebeispiel Root-Layout**

```js
// app/layout.js
export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body>
        <header>Navigation</header>
        <main>{children}</main>
        <footer>© 2025</footer>
      </body>
    </html>
  );
}
```

➡️ `children` = jeweilige Page/Route.

---

### 4) **Verschachtelte Layouts**

```js
// app/dashboard/layout.js
export default function DashboardLayout({ children }) {
  return (
    <section>
      <aside>Sidebar</aside>
      <div>{children}</div>
    </section>
  );
}
```

➡️ Öffnet man `/dashboard/settings`, so wird `DashboardLayout` **+** `RootLayout` gerendert.

---

### 5) **Besonderheiten**

* Layouts können **Server Components** sein (empfohlen).
* Können **async** sein → Datenfetching direkt im Layout möglich.
* Bleiben beim Client-Routing **persistent**, d. h. nur der Inhalt im `children`-Bereich wird neu geladen.
* Neben `layout.js` existieren verwandte Konventionen: `error.js`, `loading.js`, `not-found.js`.

---

🔗 [Next.js – Layouts im App Router](https://nextjs.org/docs/app/building-your-application/routing/pages-and-layouts#layouts)

---

**Zusammenfassung:**
App Router Layouts sind **persistent Wrapper-Komponenten**, die gemeinsame UI-Strukturen definieren. Sie können verschachtelt sein, async-Daten laden und bleiben beim Navigieren erhalten – nur `children`-Inhalte wechseln.

  **[⬆ Наверх](#top)**

110. ### <a name="110"></a> Was ist der Unterschied zwischen Root Layout und Nested Layout?

**Unterschied: Root Layout vs. Nested Layout (Next.js App Router)**

---

### **Root Layout**

* Datei: `app/layout.js` (Pflicht).
* Umschließt die **gesamte Anwendung**.
* Wird nur **einmal** pro App definiert.
* Enthält globale Strukturen: `<html>`, `<body>`, globale CSS, Fonts, Provider (Redux, React Query, Theme).
* Beispiel:

```js
// app/layout.js
export default function RootLayout({ children }) {
  return (
    <html lang="de">
      <body>
        <header>Global Nav</header>
        {children}
        <footer>© 2025</footer>
      </body>
    </html>
  );
}
```

---

### **Nested Layout**

* Datei: `layout.js` in einem Unterordner (z. B. `app/dashboard/layout.js`).
* Umschließt nur den **Teilbaum der Route**, unter der sie liegt.
* Kann **mehrfach** pro App existieren.
* Typisch für spezifische Bereiche: Dashboard, Admin-Bereich, Shop.
* Beispiel:

```js
// app/dashboard/layout.js
export default function DashboardLayout({ children }) {
  return (
    <section>
      <aside>Sidebar</aside>
      <main>{children}</main>
    </section>
  );
}
```

---

### **Verhalten beim Navigieren**

* Root Layout bleibt **immer gleich** (persistiert).
* Nested Layouts bleiben erhalten, solange man innerhalb ihres Routenbereichs navigiert.
* Nur der `children`-Bereich wird neu gerendert.

---

🔗 [Next.js – Layouts](https://nextjs.org/docs/app/building-your-application/routing/pages-and-layouts#layouts)

---

**Zusammenfassung:**

* **Root Layout** = global, nur einmal definiert, enthält `<html>` & `<body>`.
* **Nested Layout** = beliebig oft, pro Teilbereich, erweitert oder überschreibt Root Layout für Unterrouten.

  **[⬆ Наверх](#top)**

111. ### <a name="111"></a> 



  **[⬆ Наверх](#top)**

112. ### <a name="112"></a> 



  **[⬆ Наверх](#top)**

113. ### <a name="113"></a> 



  **[⬆ Наверх](#top)**

114. ### <a name="114"></a> 



  **[⬆ Наверх](#top)**

115. ### <a name="115"></a> 



  **[⬆ Наверх](#top)**

116. ### <a name="116"></a> 



  **[⬆ Наверх](#top)**

117. ### <a name="117"></a> 



  **[⬆ Наверх](#top)**

118. ### <a name="118"></a> 



  **[⬆ Наверх](#top)**

119. ### <a name="119"></a> 



  **[⬆ Наверх](#top)**

120. ### <a name="120"></a> 



  **[⬆ Наверх](#top)**

121. ### <a name="121"></a> 



  **[⬆ Наверх](#top)**

122. ### <a name="122"></a> 



  **[⬆ Наверх](#top)**

123. ### <a name="123"></a> 



  **[⬆ Наверх](#top)**

124. ### <a name="124"></a> 



  **[⬆ Наверх](#top)**

125. ### <a name="125"></a> 



  **[⬆ Наверх](#top)**

126. ### <a name="126"></a> 



  **[⬆ Наверх](#top)**

127. ### <a name="127"></a> 



  **[⬆ Наверх](#top)**

128. ### <a name="128"></a> 



  **[⬆ Наверх](#top)**

129. ### <a name="129"></a> 



  **[⬆ Наверх](#top)**

130. ### <a name="130"></a> 



  **[⬆ Наверх](#top)**  

131. ### <a name="131"></a> 



  **[⬆ Наверх](#top)**

132. ### <a name="132"></a> 



  **[⬆ Наверх](#top)**

133. ### <a name="133"></a> 



  **[⬆ Наверх](#top)**

134. ### <a name="134"></a> 



  **[⬆ Наверх](#top)**

135. ### <a name="135"></a> 



  **[⬆ Наверх](#top)**

136. ### <a name="136"></a> 



  **[⬆ Наверх](#top)**

137. ### <a name="137"></a> 



  **[⬆ Наверх](#top)**

138. ### <a name="138"></a> 



  **[⬆ Наверх](#top)**

139. ### <a name="139"></a> 



  **[⬆ Наверх](#top)**

140. ### <a name="140"></a> 



  **[⬆ Наверх](#top)**  

141. ### <a name="141"></a> 



  **[⬆ Наверх](#top)**

142. ### <a name="142"></a> 



  **[⬆ Наверх](#top)**

143. ### <a name="143"></a> 



  **[⬆ Наверх](#top)**

144. ### <a name="144"></a> 



  **[⬆ Наверх](#top)**

145. ### <a name="145"></a> 



  **[⬆ Наверх](#top)**

146. ### <a name="146"></a> 



  **[⬆ Наверх](#top)**

147. ### <a name="147"></a> 



  **[⬆ Наверх](#top)**

148. ### <a name="148"></a> 



  **[⬆ Наверх](#top)**

149. ### <a name="149"></a> 



  **[⬆ Наверх](#top)**

150. ### <a name="150"></a> 



  **[⬆ Наверх](#top)**  

151. ### <a name="151"></a> 



  **[⬆ Наверх](#top)**

152. ### <a name="152"></a> 



  **[⬆ Наверх](#top)**

153. ### <a name="153"></a> 



  **[⬆ Наверх](#top)**

154. ### <a name="154"></a> 



  **[⬆ Наверх](#top)**

155. ### <a name="155"></a> 



  **[⬆ Наверх](#top)**

156. ### <a name="156"></a> 



  **[⬆ Наверх](#top)**

157. ### <a name="157"></a> 



  **[⬆ Наверх](#top)**

158. ### <a name="158"></a> 



  **[⬆ Наверх](#top)**

159. ### <a name="159"></a> 



  **[⬆ Наверх](#top)**

160. ### <a name="160"></a> 



  **[⬆ Наверх](#top)**

161. ### <a name="161"></a> 



  **[⬆ Наверх](#top)**

162. ### <a name="162"></a> 



  **[⬆ Наверх](#top)**

163. ### <a name="163"></a> 



  **[⬆ Наверх](#top)**

164. ### <a name="164"></a> 



  **[⬆ Наверх](#top)**

165. ### <a name="165"></a> 



  **[⬆ Наверх](#top)**

166. ### <a name="166"></a> 



  **[⬆ Наверх](#top)**

167. ### <a name="167"></a> 



  **[⬆ Наверх](#top)**

168. ### <a name="168"></a> 



  **[⬆ Наверх](#top)**

169. ### <a name="169"></a> 



  **[⬆ Наверх](#top)**

170. ### <a name="170"></a> 



  **[⬆ Наверх](#top)**

171. ### <a name="171"></a> 



  **[⬆ Наверх](#top)**

172. ### <a name="172"></a> 



  **[⬆ Наверх](#top)**

173. ### <a name="173"></a> 



  **[⬆ Наверх](#top)**

174. ### <a name="174"></a> 



  **[⬆ Наверх](#top)**

175. ### <a name="175"></a> 



  **[⬆ Наверх](#top)**

176. ### <a name="176"></a> 



  **[⬆ Наверх](#top)**

177. ### <a name="177"></a> 



  **[⬆ Наверх](#top)**

178. ### <a name="178"></a> 



  **[⬆ Наверх](#top)**

179. ### <a name="179"></a> 



  **[⬆ Наверх](#top)**

180. ### <a name="180"></a> 



  **[⬆ Наверх](#top)**  

181. ### <a name="181"></a> 



  **[⬆ Наверх](#top)**

182. ### <a name="182"></a> 



  **[⬆ Наверх](#top)**

183. ### <a name="183"></a> 



  **[⬆ Наверх](#top)**

184. ### <a name="184"></a> 



  **[⬆ Наверх](#top)**

185. ### <a name="185"></a> 



  **[⬆ Наверх](#top)**

186. ### <a name="186"></a> 



  **[⬆ Наверх](#top)**

187. ### <a name="187"></a> 



  **[⬆ Наверх](#top)**

188. ### <a name="188"></a> 



  **[⬆ Наверх](#top)**

189. ### <a name="189"></a> 



  **[⬆ Наверх](#top)**

190. ### <a name="190"></a> 



  **[⬆ Наверх](#top)**  

191. ### <a name="191"></a> 



  **[⬆ Наверх](#top)**

192. ### <a name="192"></a> 



  **[⬆ Наверх](#top)**

193. ### <a name="193"></a> 



  **[⬆ Наверх](#top)**

194. ### <a name="194"></a> 



  **[⬆ Наверх](#top)**

195. ### <a name="195"></a> 



  **[⬆ Наверх](#top)**

196. ### <a name="196"></a> 



  **[⬆ Наверх](#top)**

197. ### <a name="197"></a> 



  **[⬆ Наверх](#top)**

198. ### <a name="198"></a> 



  **[⬆ Наверх](#top)**

199. ### <a name="199"></a> 



  **[⬆ Наверх](#top)**

200. ### <a name="200"></a> 



  **[⬆ Наверх](#top)**      
