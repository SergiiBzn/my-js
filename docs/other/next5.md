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



  **[⬆ Наверх](#top)**

20. ### <a name="20"></a> 



  **[⬆ Наверх](#top)**

21. ### <a name="21"></a> 



  **[⬆ Наверх](#top)**

22. ### <a name="22"></a> 



  **[⬆ Наверх](#top)**

23. ### <a name="23"></a> 



  **[⬆ Наверх](#top)**

24. ### <a name="24"></a> 



  **[⬆ Наверх](#top)**

25. ### <a name="25"></a> 



  **[⬆ Наверх](#top)**

26. ### <a name="26"></a> 



  **[⬆ Наверх](#top)**

27. ### <a name="27"></a> 



  **[⬆ Наверх](#top)**

28. ### <a name="28"></a> 



  **[⬆ Наверх](#top)**

29. ### <a name="29"></a> 



  **[⬆ Наверх](#top)**

30. ### <a name="30"></a> 



  **[⬆ Наверх](#top)**  

31. ### <a name="31"></a> 



  **[⬆ Наверх](#top)**

32. ### <a name="32"></a> 



  **[⬆ Наверх](#top)**

33. ### <a name="33"></a> 



  **[⬆ Наверх](#top)**

34. ### <a name="34"></a> 



  **[⬆ Наверх](#top)**

35. ### <a name="35"></a> 



  **[⬆ Наверх](#top)**

36. ### <a name="36"></a> 



  **[⬆ Наверх](#top)**

37. ### <a name="37"></a> 



  **[⬆ Наверх](#top)**

38. ### <a name="38"></a> 



  **[⬆ Наверх](#top)**

39. ### <a name="39"></a> 



  **[⬆ Наверх](#top)**

40. ### <a name="40"></a> 



  **[⬆ Наверх](#top)**  

41. ### <a name="41"></a> 



  **[⬆ Наверх](#top)**

42. ### <a name="42"></a> 



  **[⬆ Наверх](#top)**

43. ### <a name="43"></a> 



  **[⬆ Наверх](#top)**

44. ### <a name="44"></a> 



  **[⬆ Наверх](#top)**

45. ### <a name="45"></a> 



  **[⬆ Наверх](#top)**

46. ### <a name="46"></a> 



  **[⬆ Наверх](#top)**

47. ### <a name="47"></a> 



  **[⬆ Наверх](#top)**

48. ### <a name="48"></a> 



  **[⬆ Наверх](#top)**

49. ### <a name="49"></a> 



  **[⬆ Наверх](#top)**

50. ### <a name="50"></a> 



  **[⬆ Наверх](#top)**  

51. ### <a name="51"></a> 



  **[⬆ Наверх](#top)**

52. ### <a name="52"></a> 



  **[⬆ Наверх](#top)**

53. ### <a name="53"></a> 



  **[⬆ Наверх](#top)**

54. ### <a name="54"></a> 



  **[⬆ Наверх](#top)**

55. ### <a name="55"></a> 



  **[⬆ Наверх](#top)**

56. ### <a name="56"></a> 



  **[⬆ Наверх](#top)**

57. ### <a name="57"></a> 



  **[⬆ Наверх](#top)**

58. ### <a name="58"></a> 



  **[⬆ Наверх](#top)**

59. ### <a name="59"></a> 



  **[⬆ Наверх](#top)**

60. ### <a name="60"></a> 



  **[⬆ Наверх](#top)**

61. ### <a name="61"></a> 



  **[⬆ Наверх](#top)**

62. ### <a name="62"></a> 



  **[⬆ Наверх](#top)**

63. ### <a name="63"></a> 



  **[⬆ Наверх](#top)**

64. ### <a name="64"></a> 



  **[⬆ Наверх](#top)**

65. ### <a name="65"></a> 



  **[⬆ Наверх](#top)**

66. ### <a name="66"></a> 



  **[⬆ Наверх](#top)**

67. ### <a name="67"></a> 



  **[⬆ Наверх](#top)**

68. ### <a name="68"></a> 



  **[⬆ Наверх](#top)**

69. ### <a name="69"></a> 



  **[⬆ Наверх](#top)**

70. ### <a name="70"></a> 



  **[⬆ Наверх](#top)**

71. ### <a name="71"></a> 



  **[⬆ Наверх](#top)**

72. ### <a name="72"></a> 



  **[⬆ Наверх](#top)**

73. ### <a name="73"></a> 



  **[⬆ Наверх](#top)**

74. ### <a name="74"></a> 



  **[⬆ Наверх](#top)**

75. ### <a name="75"></a> 



  **[⬆ Наверх](#top)**

76. ### <a name="76"></a> 



  **[⬆ Наверх](#top)**

77. ### <a name="77"></a> 



  **[⬆ Наверх](#top)**

78. ### <a name="78"></a> 



  **[⬆ Наверх](#top)**

79. ### <a name="79"></a> 



  **[⬆ Наверх](#top)**

80. ### <a name="80"></a> 



  **[⬆ Наверх](#top)**  

81. ### <a name="81"></a> 



  **[⬆ Наверх](#top)**

82. ### <a name="82"></a> 



  **[⬆ Наверх](#top)**

83. ### <a name="83"></a> 



  **[⬆ Наверх](#top)**

84. ### <a name="84"></a> 



  **[⬆ Наверх](#top)**

85. ### <a name="85"></a> 



  **[⬆ Наверх](#top)**

86. ### <a name="86"></a> 



  **[⬆ Наверх](#top)**

87. ### <a name="87"></a> 



  **[⬆ Наверх](#top)**

88. ### <a name="88"></a> 



  **[⬆ Наверх](#top)**

89. ### <a name="89"></a> 



  **[⬆ Наверх](#top)**

90. ### <a name="90"></a> 



  **[⬆ Наверх](#top)**  

91. ### <a name="91"></a> 



  **[⬆ Наверх](#top)**

92. ### <a name="92"></a> 



  **[⬆ Наверх](#top)**

93. ### <a name="93"></a> 



  **[⬆ Наверх](#top)**

94. ### <a name="94"></a> 



  **[⬆ Наверх](#top)**

95. ### <a name="95"></a> 



  **[⬆ Наверх](#top)**

96. ### <a name="96"></a> 



  **[⬆ Наверх](#top)**

97. ### <a name="97"></a> 



  **[⬆ Наверх](#top)**

98. ### <a name="98"></a> 



  **[⬆ Наверх](#top)**

99. ### <a name="99"></a> 



  **[⬆ Наверх](#top)**

100. ### <a name="100"></a> 



  **[⬆ Наверх](#top)**    

101. ### <a name="101"></a> 



  **[⬆ Наверх](#top)**

102. ### <a name="102"></a> 



  **[⬆ Наверх](#top)**

103. ### <a name="103"></a> 



  **[⬆ Наверх](#top)**

104. ### <a name="104"></a> 



  **[⬆ Наверх](#top)**

105. ### <a name="105"></a> 



  **[⬆ Наверх](#top)**

106. ### <a name="106"></a> 



  **[⬆ Наверх](#top)**

107. ### <a name="107"></a> 



  **[⬆ Наверх](#top)**

108. ### <a name="108"></a> 



  **[⬆ Наверх](#top)**

109. ### <a name="109"></a> 



  **[⬆ Наверх](#top)**

110. ### <a name="110"></a> 



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
