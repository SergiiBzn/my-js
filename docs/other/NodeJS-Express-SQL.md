<a name="top"></a>

[На главную](../README.md)

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
|   | Grundlagen Express.js |
|1 | [Was ist Express.js und warum wird es verwendet?](#1) |
|2 | [Welche Vorteile bietet Express.js im Vergleich zu reinem Node.js?](#2) |
|3 | [Wie installiert man Express.js in einem Projekt?](#3) |
|4 | [Wie startet man einen einfachen Express-Server?](#4) |
|5 | [Was ist app.listen() und wie funktioniert es?](#5) |
|6 | [Wie kann man statische Dateien in Express bereitstellen?](#6) |
|7 | [Wie arbeitet Express intern mit dem Node.js HTTP-Modul?](#7) |
|8 | [Was ist der Unterschied zwischen Express.js und anderen Frameworks wie Koa oder Fastify?](#8) |
|9 | [Welche Rolle spielt package.json in einem Express-Projekt?](#9) |
|10 | [Was bedeutet „Middleware-basiertes Framework“ bei Express?](#10) |
|   | Routing |
|11 | [Wie funktioniert Routing in Express.js?](#11) |
|12 | [Was ist der Unterschied zwischen app.get() und app.post()?](#12) |
|13 | [Was macht app.use() im Zusammenhang mit Routing?](#13) |
|14 | [Wie definiert man Routenparameter in Express?](#14) |
|15 | [Wie greift man in einer Route auf Query-Parameter zu?](#15) |
|16 | [Wie erstellt man verschachtelte Router (express.Router)?](#16) |
|17 | [Wie kann man eine Route auf mehrere HTTP-Methoden gleichzeitig reagieren lassen?](#17) |
|18 | [Was ist der Unterschied zwischen app.all() und spezifischen Methoden wie app.get()?](#18) |
|19 | [Wie kann man Wildcard-Routen erstellen?](#19) |
|20 | [Was passiert, wenn keine Route im Express-Server passt?](#20) |
|   | Middleware |
|21 | [Was ist Middleware in Express.js?](#21) |
|22 | [Welche Arten von Middleware gibt es?](#22) |
|23 | [Wie unterscheidet sich globale Middleware von Router-spezifischer Middleware?](#23) |
|24 | [Wie erstellt man eine eigene Middleware-Funktion?](#24) |
|25 | [Was sind Third-Party-Middleware-Beispiele in Express?](#25) |
|26 | [Wie wird next() in Middleware verwendet?](#26) |
|27 | [Wie kann man Reihenfolge von Middleware steuern?](#27) |
|28 | [Wie kann man Middleware nur auf bestimmte Routen anwenden?](#28) |
|29 | [Wie funktioniert express.json() und wofür wird es genutzt?](#29) |
|30 | [Wie funktioniert express.urlencoded()?](#30) |
|   | Request & Response |
|31 | [Welche Objekte sind in Express.js für HTTP-Anfragen und -Antworten zuständig?](#31) |
|32 | [Wie greift man auf Request-Header zu?](#32) |
|33 | [Wie greift man auf Body-Daten zu?](#33) |
|34 | [Wie sendet man JSON als Antwort?](#34) |
|35 | [Wie funktioniert res.send()?](#35) |
|36 | [Unterschied zwischen res.json() und res.send()?](#36) |
|37 | [Wie setzt man einen HTTP-Statuscode?](#37) |
|38 | [Wie werden Cookies gesetzt und gelesen?](#38) |
|39 | [Unterschied zwischen synchronem und asynchronem Request-Handling?](#39) |
|40 | [Wie behandelt man Datei-Uploads in Express?](#40) |
|   | Fehlerbehandlung |
|41 | [Wie implementiert man Error-Handling in Express?](#41) |
|42 | [Warum braucht man spezielle Error-Middleware?](#42) |
|43 | [Unterschied zwischen synchronem und asynchronem Fehlerhandling?](#43) |
|44 | [Wie gibt man unterschiedliche Statuscodes im Fehlerfall zurück?](#44) |
|45 | [Wie verhindert man, dass nicht abgefangene Fehler den Server crashen?](#45) |
|   | Security |
|46 | [Wie schützt man Express-Anwendungen vor XSS?](#46) |
|47 | [Welche Middleware nutzt man für Security (z. B. Helmet)?](#47) |
|48 | [Was ist CORS und wie aktiviert man es in Express?](#48) |
|49 | [Wie funktioniert Rate-Limiting in Express?](#49) |
|50 | [Wie speichert man Passwörter sicher in Kombination mit Express?](#50) |
|51 | [Wie verhindert man SQL-Injections in Express?](#51) |
|52 | [Was ist CSRF und wie schützt man sich dagegen?](#52) |
|53 | [Wie kann man HTTPS in Express konfigurieren?](#53) |
|54 | [Was ist express-session und wofür wird es verwendet?](#54) |
|55 | [Wie implementiert man JWT-Authentifizierung in Express?](#55) |
|   | REST APIs |
|56 | [Wie baut man eine REST-API mit Express?](#56) |
|57 | [Unterschied zwischen REST und GraphQL im Kontext von Express?](#57) |
|58 | [Wie validiert man Daten in einer REST-API?](#58) |
|59 | [Welche Best Practices gibt es für RESTful Routes?](#59) |
|60 | [Was ist HATEOAS?](#60) |
|61 | [Wie baut man eine Versionierung für APIs in Express ein?](#61) |
|62 | [Wie verarbeitet man große Datenmengen in einer API?](#62) |
|63 | [Wie integriert man Swagger oder OpenAPI mit Express?](#63) |
|64 | [Was ist ein DTO (Data Transfer Object) und wie nutzt man es in Express?](#64) |
|65 | [Wie testet man eine Express REST API?](#65) |
|   | Datenbanken & Integration |
|66 | [Wie verbindet man Express mit einer Datenbank (z. B. MongoDB oder PostgreSQL)?](#66) |
|67 | [Was ist Mongoose und wie wird es in Express verwendet?](#67) |
|68 | [Wie implementiert man ein Repository Pattern mit Express?](#68) |
|69 | [Unterschied zwischen SQL- und NoSQL-Integration in Express?](#69) |
|70 | [Wie arbeitet man mit ORMs (z. B. Sequelize, Prisma) in Express?](#70) |
|71 | [Wie behandelt man Transaktionen in Express?](#71) |
|72 | [Wie implementiert man ein Logging-System in Express?](#72) |
|73 | [Wie integriert man Caching (z. B. Redis) in Express?](#73) |
|74 | [Wie geht man mit Verbindungen zu externen APIs um?](#74) |
|75 | [Wie baut man eine WebSocket-Verbindung mit Express?](#75) |
|   | Architektur & Best Practices |
|76 | [Welche Projektstruktur ist für Express empfehlenswert?](#76) |
|77 | [Was sind Controller in einer Express-App?](#77) |
|78 | [Was ist der Unterschied zwischen MVC und einer service-basierten Architektur in Express?](#78) |
|79 | [Wie trennt man Business-Logik von Routing?](#79) |
|80 | [Warum sollte man .env-Dateien in Express verwenden?](#80) |
|81 | [Wie implementiert man Dependency Injection in Express?](#81) |
|82 | [Wie geht man mit Konfigurationen in verschiedenen Umgebungen (Dev/Prod) um?](#82) |
|83 | [Was sind Best Practices für Error Logging in Express?](#83) |
|84 | [Warum sollte man asynchrone Fehler immer mit try/catch oder asyncHandler behandeln?](#84) |
|85 | [Wie implementiert man eine saubere API-Dokumentation?](#85) |
|   | Testing |
|86 | [Welche Tools nutzt man zum Testen einer Express-App?](#86) |
|87 | [Wie testet man einzelne Endpoints?](#87) |
|88 | [Was ist Supertest und wie wird es in Express eingesetzt?](#88) |
|89 | [Wie simuliert man Requests im Unit-Test?](#89) |
|90 | [Wie testet man Middleware?](#90) |
|91 | [Was ist der Unterschied zwischen Unit-Tests und Integrationstests in Express?](#91) |
|92 | [Wie implementiert man Mocking im Express-Test?](#92) |
|93 | [Wie kann man CI/CD mit Tests für Express automatisieren?](#93) |
|94 | [Was ist Test Coverage und wie misst man sie in Express?](#94) |
|95 | [Was sind gängige Fehler beim Testen von Express-Apps?](#95) |
|   | Performance & Deployment |
|96 | [Wie optimiert man Performance in Express?](#96) |
|97 | [Welche Möglichkeiten gibt es zum Caching von Responses?](#97) |
|98 | [Wie kann man eine Express-App in Docker deployen?](#98) |
|99 | [Wie deployt man eine Express-Anwendung auf Heroku oder Vercel?](#99) |
|100 | [Wie geht man mit Skalierung von Express-Servern um?](#100) |
|101 | [Unterschied zwischen Cluster-Mode und Single-Threaded Mode in Node/Express?](#101) |
|102 | [Wie funktioniert Load Balancing bei Express?](#102) |
|103 | [Wie überwacht man eine Express-App im Betrieb?](#103) |
|104 | [Was sind typische Bottlenecks in Express-Anwendungen?](#104) |
|105 | [Wie misst man Response-Zeiten in Express?](#105) |
|   | Erweiterte Themen |
|106 | [Wie integriert man GraphQL in Express?](#106) |
|107 | [Unterschied zwischen REST- und gRPC-Integration mit Express?](#107) |
|108 | [Wie nutzt man EventEmitter in Express?](#108) |
|109 | [Wie integriert man Message Queues (z. B. RabbitMQ, Kafka) mit Express?](#109) |
|110 | [Wie baut man eine Multitenant-Anwendung mit Express?](#110) |
|111 | [Was ist ein Proxy in Express und wie implementiert man ihn?](#111) |
|112 | [Wie konfiguriert man Middleware global und dynamisch?](#112) |
|113 | [Wie geht man mit Dateistreams in Express um?](#113) |
|114 | [Wie implementiert man Soft-Delete in Express mit einer DB?](#114) |
|115 | [Welche Patterns gibt es für saubere Express-Architekturen?](#115) |
|116 | [](#116) |
|117 | [](#117) |
|118 | [](#118) |
|119 | [](#119) |
|120 | [](#120) |
|   | Node.js Grundlagen |
|121 | [Was ist Node.js und wofür wird es verwendet?](#121) |
|122 | [Wie funktioniert die V8 Engine?](#122) |
|123 | [Was ist Event Loop und wie funktioniert er?](#123) |
|124 | [Unterschied zwischen Call Stack, Callback Queue und Event Loop?](#124) |
|125 | [Unterschied zwischen asynchronem und synchronem Code in Node.js?](#125) |
|126 | [Unterschied zwischen process.nextTick(), setImmediate() und setTimeout()?](#126) |
|127 | [Was sind Streams in Node.js und welche Typen gibt es?](#127) |
|128 | [Unterschied zwischen Buffer und Stream?](#128) |
|129 | [Wie arbeitet Node.js intern mit Non-Blocking I/O?](#129) |
|130 | [Wie funktioniert das Modul-System in Node.js (CommonJS vs. ES Modules)?](#130) |
|131 | [Was ist require und was ist import?](#131) |
|132 | [Unterschied zwischen module.exports und exports?](#132) |
|133 | [Wie setzt man Umgebungsvariablen in Node.js (process.env)?](#133) |
|134 | [Was ist package-lock.json und warum wichtig?](#134) |
|135 | [Unterschied zwischen global und lokaler Installation von npm-Paketen?](#135) |
|136 | [Was sind Worker Threads in Node.js?](#136) |
|137 | [Unterschied zwischen cluster und child_process?](#137) |
|138 | [Wie behandelt man Exceptions (try/catch vs. process.on('uncaughtException'))?](#138) |
|139 | [Was ist Garbage Collection in Node.js?](#139) |
|140 | [Welche Nachteile hat Node.js bei CPU-intensiven Aufgaben?](#140) |
|   | Node.js Asynchronität |
|141 | [Unterschied zwischen Callbacks, Promises und async/await?](#141) |
|142 | [Typische Callback-Hell-Beispiele und wie man sie vermeidet?](#142) |
|143 | [Wie funktioniert Promise.all()?](#143) |
|144 | [Unterschied zwischen Promise.allSettled() und Promise.race()?](#144) |
|145 | [Wie funktioniert async/await intern?](#145) |
|146 | [Warum ist Error-Handling bei async/await kritisch?](#146) |
|147 | [Unterschied zwischen for...of und forEach in async Code?](#147) |
|148 | [Was sind EventEmitter in Node.js?](#148) |
|149 | [Wie implementiert man Custom Events mit EventEmitter?](#149) |
|150 | [Unterschied zwischen once und on bei Events?](#150) |
|   | Datenbanken (SQL / NoSQL) |
|151 | [Unterschied zwischen SQL und NoSQL?](#151) |
|152 | [Wann verwendet man relationale DB vs. dokumentbasierte DB?](#152) |
|153 | [Unterschiede zwischen PostgreSQL, MySQL und SQLite?](#153) |
|154 | [Unterschiede zwischen MongoDB und PostgreSQL?](#154) |
|155 | [Wie baut man eine DB-Verbindung in Express auf?](#155) |
|156 | [Was sind Migrations in SQL-Datenbanken?](#156) |
|157 | [Unterschied zwischen INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN?](#157) |
|158 | [Was sind Normalformen in relationalen Datenbanken?](#158) |
|159 | [Unterschied zwischen 1NF, 2NF, 3NF?](#159) |
|160 | [Wie funktioniert Indexierung in SQL-Datenbanken?](#160) |
|161 | [Was ist ein Primärschlüssel und ein Fremdschlüssel?](#161) |
|162 | [Unterschied zwischen UNIQUE und PRIMARY KEY?](#162) |
|163 | [Unterschied zwischen HAVING und WHERE in SQL?](#163) |
|164 | [Was sind Aggregate-Funktionen in SQL (z. B. COUNT, SUM, AVG)?](#164) |
|165 | [Wie baut man Many-to-Many Beziehungen in SQL?](#165) |
|166 | [Wie arbeitet man mit Transaktionen in PostgreSQL?](#166) |
|167 | [Was ist ACID in Datenbanken?](#167) |
|168 | [Unterschied zwischen ACID und BASE Prinzipien?](#168) |
|169 | [Was ist ein Deadlock und wie vermeidet man ihn?](#169) |
|170 | [Was ist Sharding und Partitionierung in Datenbanken?](#170) |
|171 | [Unterschied zwischen vertikaler und horizontaler Skalierung?](#171) |
|172 | [Wie funktioniert Replikation in SQL-DBs?](#172) |
|173 | [Wie schützt man DB-Verbindungen in einer Express-App?](#173) |
|174 | [Was sind ORM-Tools (z. B. Sequelize, Prisma, TypeORM)?](#174) |
|175 | [Vorteile und Nachteile von ORM vs. Plain SQL?](#175) |
|176 | [Wie implementiert man Soft Delete in einer Datenbank?](#176) |
|177 | [Unterschied zwischen NoSQL-Typen: Key-Value, Document, Graph, Column?](#177) |
|178 | [Wie funktioniert Indexierung in MongoDB?](#178) |
|179 | [Was ist Aggregation Pipeline in MongoDB?](#179) |
|180 | [Unterschied zwischen Embedded Documents und Referenzen in MongoDB?](#180) |
|   | Deployment & Betrieb |
|181 | [Wie deployt man eine Node/Express-App auf AWS/Heroku/Vercel?](#181) |
|182 | [Was ist der Unterschied zwischen Development- und Production-Umgebung?](#182) |
|183 | [Wie nutzt man .env-Dateien für Konfigurationen?](#183) |
|184 | [Wie optimiert man Node.js Apps für Production?](#184) |
|185 | [Unterschied zwischen PM2 und Nodemon?](#185) |
|186 | [Wie funktioniert Logging in Express/Node.js?](#186) |
|187 | [Welche Tools für Monitoring von Node.js Apps (z. B. NewRelic, PM2, Grafana)?](#187) |
|188 | [Was ist CI/CD und wie implementiert man es mit Node.js?](#188) |
|189 | [Wie baut man ein Docker-Image für eine Node/Express-App?](#189) |
|190 | [Unterschied zwischen Skalierung mit Clustering und Load Balancing?](#190) |
|   | Testing |
|191 | [Welche Testing-Frameworks nutzt man mit Node.js/Express (Mocha, Jest, Supertest)?](#191) |
|192 | [Unterschied zwischen Unit-Test, Integrationstest und End-to-End-Test?](#192) |
|193 | [Wie testet man REST APIs mit Supertest?](#193) |
|194 | [Was sind Mocks und Stubs im Testing?](#194) |
|195 | [Wie testet man asynchronen Code in Jest?](#195) |
|196 | [Unterschied zwischen beforeAll, beforeEach, afterAll, afterEach?](#196) |
|197 | [Was bedeutet Test Coverage?](#197) |
|198 | [Was sind Best Practices für Test-Driven Development (TDD)?](#198) |
|199 | [Unterschied zwischen TDD und BDD (Behavior Driven Development)?](#199) |
|200 | [Welche Rolle spielt Continuous Testing in CI/CD?](#200) |
|   | Security (Node + Express) |
|201 | [Was ist SQL Injection und wie verhindert man sie?](#201) |
|202 | [Was ist NoSQL Injection?](#202) |
|203 | [Unterschied zwischen XSS und CSRF?](#203) |
|204 | [Wie schützt man REST-APIs mit JWT?](#204) |
|205 | [Unterschied zwischen JWT und OAuth2?](#205) |
|206 | [Unterschied zwischen Session-basiertem und Token-basiertem Auth?](#206) |
|207 | [Wie konfiguriert man sichere CORS-Regeln?](#207) |
|208 | [Was ist HTTPS und wie implementiert man es in Node.js?](#208) |
|209 | [Welche Sicherheits-Header kann man mit Helmet setzen?](#209) |
|210 | [Wie schützt man API-Keys in einer Node.js App?](#210) |
|   | Authentifizierung & Autorisierung (Node.js + Express |
|211 | [Was ist der Unterschied zwischen Authentifizierung und Autorisierung?](#211) |
|212 | [Welche Möglichkeiten gibt es, Authentifizierung in Express zu implementieren?](#212) |
|213 | [Unterschied zwischen Session-basiertem und Token-basiertem Login?](#213) |
|214 | [Wie funktioniert express-session und wann sollte man es nutzen?](#214) |
|215 | [Was ist der Unterschied zwischen Cookies und Tokens?](#215) |
|216 | [Was ist JWT (JSON Web Token) und wie funktioniert es?](#216) |
|217 | [Welche Vorteile und Nachteile hat JWT gegenüber Sessions?](#217) |
|218 | [Wie speichert man ein JWT sicher im Browser (LocalStorage vs. HttpOnly-Cookie)?](#218) |
|219 | [Wie verhindert man JWT-Manipulation?](#219) |
|220 | [Was sind die Bestandteile eines JWT (Header, Payload, Signature)?](#220) |
|221 | [Wie setzt man Token-Expiration (Refresh Token vs. Access Token)?](#221) |
|222 | [Wie implementiert man Refresh Tokens in einer Express-App?](#222) |
|223 | [Was ist OAuth2 und wie unterscheidet es sich von JWT?](#223) |
|224 | [Unterschied zwischen OAuth2 und OpenID Connect?](#224) |
|225 | [Wie integriert man Social Logins (Google, Facebook, GitHub) in Express?](#225) |
|226 | [Wie implementiert man eine Middleware zum Schutz von privaten Routen?](#226) |
|227 | [Wie prüft man Benutzerrollen (Role-Based Access Control, RBAC) in Express?](#227) |
|228 | [Was ist Policy-Based Access Control (PBAC)?](#228) |
|229 | [Wie schützt man REST-Endpunkte vor unautorisierten Zugriffen?](#229) |
|230 | [Wie kann man Public Routes von Private Routes in Express trennen?](#230) |
|231 | [Was ist CSRF und wie hängt es mit Session-Authentifizierung zusammen?](#231) |
|232 | [Wie verhindert man Session Fixation?](#232) |
|233 | [Welche Best Practices gibt es für Passwort-Hashing (bcrypt, argon2)?](#233) |
|234 | [Warum sollte man niemals Passwörter im Klartext speichern?](#234) |
|235 | [Wie implementiert man Zwei-Faktor-Authentifizierung (2FA) in einer Node.js-App?](#235) |
|236 | [Was ist der Unterschied zwischen Single Sign-On (SSO) und klassischem Login?](#236) |
|237 | [Wie funktioniert Authentifizierung mit Passport.js?](#237) |
|238 | [Welche Vorteile bietet Passport.js in Express?](#238) |
|239 | [Unterschied zwischen lokaler Strategie und OAuth-Strategie in Passport.js?](#239) |
|240 | [Wie testet man Authentifizierungs- und Autorisierungslogik in einer Express-App?](#240) |
|241 | [](#241) |
|242 | [](#242) |
|243 | [](#243) |
|244 | [](#244) |
|245 | [](#245) |
|246 | [](#246) |
|247 | [](#247) |
|248 | [](#248) |
|249 | [](#249) |
|250 | [](#250) |



<a name="questions"></a>

## Grundlagen Express.js 

  **[⬆ Наверх](#top)**
  
1. ### <a name="1"></a> Was ist Express.js und warum wird es verwendet?

## Was ist Express.js und warum wird es verwendet?

**Definition:**
Express.js ist ein minimalistisches und flexibles Web-Framework für Node.js, das Funktionen zur Erstellung von Webanwendungen und APIs bereitstellt. Es baut auf den nativen HTTP-Modulen von Node.js auf und vereinfacht typische Aufgaben wie Routing, Middleware-Handling und Request-/Response-Verarbeitung.

**Warum wird es verwendet?**

* **Routing:** Ermöglicht das einfache Definieren von Routen (`GET`, `POST`, `PUT`, `DELETE` usw.).
* **Middleware:** Unterstützt Middleware-Funktionen, die Requests vor der endgültigen Antwort verarbeiten (z. B. Logging, Authentifizierung, Body-Parsing).
* **Schnelle Entwicklung:** Abstraktionen für wiederkehrende Aufgaben reduzieren Boilerplate-Code.
* **Integration:** Einfach kombinierbar mit Datenbanken (z. B. PostgreSQL via Sequelize) und Frontend-Frameworks.
* **Community & Ökosystem:** Große Anzahl an Plugins und Middleware-Paketen.

**Beispiel:**

```js
// Import von Express
const express = require('express');
const app = express();

// Middleware zum Parsen von JSON
app.use(express.json());

// GET-Route
app.get('/hello', (req, res) => {
  res.send('Hallo, Express!');
});

// Serverstart
app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

### Zusammenfassung

Express.js ist ein leichtgewichtiges Framework für Node.js, das die Erstellung von Webservern und APIs stark vereinfacht, indem es Routing, Middleware und HTTP-Verarbeitung handhabbarer macht.

**Quellen:**

* [Express.js Offizielle Dokumentation](https://expressjs.com/de/)
* [Node.js Dokumentation](https://nodejs.org/docs)

---

  **[⬆ Наверх](#top)**

2. ### <a name="2"></a> Welche Vorteile bietet Express.js im Vergleich zu reinem Node.js?

## Vorteile von Express.js im Vergleich zu reinem Node.js

**1. Vereinfachtes Routing**

* In reinem Node.js muss man mit dem `http`-Modul Routen manuell über `req.url` und `req.method` abfangen.
* Express.js bietet eine klare und lesbare Routing-API: `app.get()`, `app.post()`, `app.put()`, `app.delete()`.

```js
// Node.js (ohne Express)
const http = require('http');

const server = http.createServer((req, res) => {
  if (req.url === '/hello' && req.method === 'GET') {
    res.writeHead(200, { 'Content-Type': 'text/plain' });
    res.end('Hallo von Node.js!');
  }
});

server.listen(3000);
```

```js
// Express.js
const express = require('express');
const app = express();

app.get('/hello', (req, res) => {
  res.send('Hallo von Express!');
});

app.listen(3000);
```

**2. Middleware-Unterstützung**

* In Node.js muss man selbst Lösungen für Logging, Body-Parsing oder Authentifizierung implementieren.
* Express.js erlaubt die einfache Integration von Middleware (`app.use()`), z. B. für JSON-Parsing (`express.json()`), Cookies, Sessions oder Authentifizierung.

**3. Strukturierte und modulare Anwendungen**

* Express.js bietet ein klares Konzept, um Code in Routen, Controller und Middleware zu strukturieren.
* In reinem Node.js tendiert man zu unübersichtlichem, monolithischem Code.

**4. Große Community und Ökosystem**

* Viele vorgefertigte Middleware-Pakete existieren für Express.js (z. B. `cors`, `helmet`, `morgan`).
* Spart Zeit und Aufwand bei der Entwicklung.

**5. Weniger Boilerplate-Code**

* Express abstrahiert wiederkehrende Aufgaben wie Header-Handling, Statuscodes und Fehlerbehandlung.
* In Node.js muss man diese Details selbst schreiben.

### Zusammenfassung

Express.js bietet gegenüber reinem Node.js klare Vorteile: einfacheres Routing, Middleware-Support, bessere Strukturierung, großes Ökosystem und deutlich weniger Boilerplate-Code. Dadurch ist Express die bevorzugte Wahl für die Entwicklung von Webanwendungen und APIs.

**Quellen:**

* [Express.js Offizielle Dokumentation](https://expressjs.com/de/)
* [Node.js Dokumentation](https://nodejs.org/docs)

---

  **[⬆ Наверх](#top)**

3. ### <a name="3"></a> Wie installiert man Express.js in einem Projekt?

## Installation von Express.js in einem Projekt

**Schritte:**

1. **Neues Node.js Projekt initialisieren**

```bash
mkdir mein-projekt
cd mein-projekt
npm init -y   # erstellt package.json
```

2. **Express.js installieren**

```bash
npm install express
```

3. **Einfache Anwendung erstellen**
   Datei `index.js`:

```js
// Import von Express
const express = require('express');
const app = express();

// Route definieren
app.get('/', (req, res) => {
  res.send('Hallo Welt mit Express!');
});

// Server starten
app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

4. **Server starten**

```bash
node index.js
```

5. **Test im Browser oder mit curl**
   [http://localhost:3000](http://localhost:3000)

---

### Zusammenfassung

Zur Installation von Express.js:

1. Node.js-Projekt mit `npm init` starten.
2. Express mit `npm install express` hinzufügen.
3. Eine `index.js` schreiben und den Server starten.

**Quellen:**

* [Express.js – Installation](https://expressjs.com/de/starter/installing.html)
* [Node.js Dokumentation](https://nodejs.org/docs)

---

  **[⬆ Наверх](#top)**

4. ### <a name="4"></a> Wie startet man einen einfachen Express-Server?

## Einfachen Express-Server starten

**Schritte:**

1. **Projekt vorbereiten**

```bash
mkdir express-server
cd express-server
npm init -y
npm install express
```

2. **Datei `server.js` erstellen**

```js
// Import von Express
const express = require('express');
const app = express();

// Einfache Route
app.get('/', (req, res) => {
  res.send('Hallo, Express-Server läuft!');
});

// Server starten
app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

3. **Server starten**

```bash
node server.js
```

4. **Im Browser öffnen**
   [http://localhost:3000](http://localhost:3000) → Ausgabe: *Hallo, Express-Server läuft!*

---

### Zusammenfassung

Ein Express-Server wird erstellt, indem man `express` importiert, eine App-Instanz anlegt, mindestens eine Route definiert und den Server mit `app.listen(port)` startet.

**Quellen:**

* [Express.js – Hello World Beispiel](https://expressjs.com/de/starter/hello-world.html)

---

  **[⬆ Наверх](#top)**

5. ### <a name="5"></a> Was ist app.listen() und wie funktioniert es?

## Was ist `app.listen()` und wie funktioniert es?

**Definition:**
`app.listen()` ist eine Methode in Express.js, die den HTTP-Server startet und ihn an einen bestimmten Port bindet. Dadurch kann die Anwendung eingehende HTTP-Anfragen empfangen und beantworten.

**Funktionsweise:**

* `app.listen(port, callback)` erstellt intern einen HTTP-Server mit dem Node.js-`http`-Modul.
* `port` bestimmt, auf welchem Port der Server lauscht (z. B. `3000`).
* `callback` ist eine optionale Funktion, die ausgeführt wird, sobald der Server erfolgreich gestartet wurde.

**Beispiel:**

```js
const express = require('express');
const app = express();

// Route
app.get('/', (req, res) => {
  res.send('Hallo Welt');
});

// Server starten
app.listen(3000, () => {
  console.log('Server läuft auf http://localhost:3000');
});
```

**Technischer Hintergrund:**
`app.listen()` ist ein Shortcut für:

```js
const http = require('http');
const server = http.createServer(app);
server.listen(3000);
```

Das bedeutet: Express verwendet intern Node.js’ `http`-Server, man ruft nur die vereinfachte Methode `app.listen()` auf.

---

### Zusammenfassung

`app.listen()` startet den Express-Server, bindet ihn an einen Port und macht die Anwendung über HTTP erreichbar. Es ist eine Abkürzung für die direkte Verwendung des Node.js-`http`-Moduls.

**Quellen:**

* [Express.js – app.listen()](https://expressjs.com/de/4x/api.html#app.listen)
* [Node.js http.Server.listen()](https://nodejs.org/docs/latest/api/http.html#serverlisten)

---

  **[⬆ Наверх](#top)**

6. ### <a name="6"></a> Wie kann man statische Dateien in Express bereitstellen?

## Statische Dateien in Express bereitstellen

**Definition:**
Mit Express.js können statische Dateien (z. B. HTML, CSS, JavaScript, Bilder) über die eingebaute Middleware `express.static()` ausgeliefert werden.

**Verwendung:**

* Man legt die Dateien in einem Ordner ab (z. B. `public`).
* Mit `app.use(express.static('public'))` macht man diesen Ordner für Clients zugänglich.

**Beispielprojektstruktur:**

```
projekt/
│── server.js
│── public/
│     ├── index.html
│     ├── style.css
│     └── script.js
```

**server.js**

```js
const express = require('express');
const app = express();

// "public"-Ordner als statisch bereitstellen
app.use(express.static('public'));

app.listen(3000, () => {
  console.log('Server läuft auf http://localhost:3000');
});
```

**Zugriff:**

* `http://localhost:3000/index.html`
* `http://localhost:3000/style.css`
* `http://localhost:3000/script.js`

**Optional – eigener Pfadpräfix:**

```js
app.use('/static', express.static('public'));
```

→ Dateien sind dann unter `http://localhost:3000/static/...` erreichbar.

---

### Zusammenfassung

Mit `express.static()` kann man Ordner für statische Dateien freigeben. Typische Anwendung: Ausliefern von HTML, CSS, Bildern oder Frontend-JS.

**Quellen:**

* [Express.js – Statische Dateien](https://expressjs.com/de/starter/static-files.html)

---

  **[⬆ Наверх](#top)**

7. ### <a name="7"></a> Wie arbeitet Express intern mit dem Node.js HTTP-Modul?

## Wie arbeitet Express intern mit dem Node.js HTTP-Modul?

**Grundidee:**
Express ist kein eigener Webserver, sondern baut auf dem nativen `http`-Modul von Node.js auf. Intern erstellt Express einen HTTP-Server mit `http.createServer()` und verwendet seine eigene Middleware- und Routing-Logik, um Requests zu verarbeiten.

**Technischer Ablauf:**

1. Express erstellt eine Funktion `app`, die kompatibel mit der Signatur von `http.createServer()` ist:

   ```js
   (req, res) => { /* Request-Verarbeitung */ }
   ```
2. Bei `app.listen(port)` ruft Express intern `http.createServer(app)` auf.
3. Das `http`-Modul nimmt eingehende Anfragen entgegen und leitet sie an die `app`-Funktion von Express weiter.
4. Express durchläuft seine Middleware-Kette und Routing-Mechanismen, bevor eine Antwort über `res.end()` (aus dem HTTP-Modul) gesendet wird.

**Vergleich:**

```js
// Node.js ohne Express
const http = require('http');

const server = http.createServer((req, res) => {
  if (req.url === '/' && req.method === 'GET') {
    res.writeHead(200, { 'Content-Type': 'text/plain' });
    res.end('Hallo von Node.js');
  }
});

server.listen(3000);
```

```js
// Express.js – nutzt intern auch http.createServer()
const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hallo von Express');
});

app.listen(3000);
```

**Interner Mechanismus von Express:**

* Express fügt eine Abstraktionsschicht hinzu, die das Arbeiten mit `req` und `res` vereinfacht.
* Methoden wie `res.send()`, `res.json()`, `req.params`, `req.body` sind Wrapper um das native `http`-Objekt.
* Am Ende ruft Express immer `res.end()` vom `http`-Modul auf.

---

### Zusammenfassung

Express basiert auf Node.js’ `http`-Modul. Es abstrahiert das Erstellen des Servers, Middleware-Handling und Routing, nutzt aber intern die gleichen Mechanismen (`http.createServer`, `req`, `res`).

**Quellen:**

* [Express.js API – app.listen()](https://expressjs.com/de/4x/api.html#app.listen)
* [Node.js http.createServer()](https://nodejs.org/docs/latest/api/http.html#httpcreateserveroptions-requestlistener)

---

  **[⬆ Наверх](#top)**

8. ### <a name="8"></a> Was ist der Unterschied zwischen Express.js und anderen Frameworks wie Koa oder Fastify?

## Unterschied zwischen Express.js, Koa und Fastify

**1. Express.js**

* **Architektur:** Minimalistisch, basiert direkt auf dem Node.js `http`-Modul.
* **Middleware:** Callback-basiert, Middleware-Kette (`app.use()`).
* **Ökosystem:** Sehr verbreitet, viele Tutorials und Third-Party-Middleware verfügbar.
* **Performance:** Stabil und zuverlässig, aber nicht das schnellste.
* **API-Stil:** Klassisch, leichtgewichtig, aber teilweise „veraltet“ im Vergleich zu moderneren Frameworks.

```js
const express = require('express');
const app = express();

app.get('/', (req, res) => {
  res.send('Hallo von Express');
});

app.listen(3000);
```

---

**2. Koa.js**

* **Entwickler:** Von den gleichen Machern wie Express entwickelt.
* **Architektur:** Moderner, setzt stark auf **async/await** statt Callbacks.
* **Middleware:** Sehr schlank, Middleware folgt einem **Onion-Pattern** (jede Middleware kann vor und nach `next()` Code ausführen).
* **Flexibilität:** Kein eingebautes Routing → separate Pakete notwendig (z. B. `koa-router`).
* **Performance:** Etwas leichter und flexibler als Express.

```js
const Koa = require('koa');
const app = new Koa();

app.use(async (ctx) => {
  ctx.body = 'Hallo von Koa';
});

app.listen(3000);
```

---

**3. Fastify**

* **Architektur:** Fokus auf **Performance** und geringe Overhead.
* **Middleware:** Unterstützt Express-Middleware teilweise, bietet aber auch eigenes Plugin-System.
* **Routing:** Eingebaut, mit Schema-basierten Validierungen (z. B. JSON-Schema für Requests).
* **Performance:** Eines der schnellsten Node.js-Frameworks (Benchmark höher als Express und Koa).
* **Features:** Eingebaute Unterstützung für JSON-Schema, automatische Swagger-Generierung, bessere TypScript-Integration.

```js
const fastify = require('fastify')();

fastify.get('/', async (request, reply) => {
  return { message: 'Hallo von Fastify' };
});

fastify.listen({ port: 3000 });
```

---

### Zusammenfassung

* **Express.js:** Einfach, stabil, große Community, aber älter und weniger modern.
* **Koa:** Moderner mit async/await und Onion-Middleware, benötigt aber zusätzliche Pakete.
* **Fastify:** Sehr performant, moderne Features, starkes Ökosystem, besonders geeignet für APIs.

**Quellen:**

* [Express.js Dokumentation](https://expressjs.com/de/)
* [Koa Dokumentation](https://koajs.com/)
* [Fastify Dokumentation](https://fastify.dev/)

---

  **[⬆ Наверх](#top)**

9. ### <a name="9"></a> Welche Rolle spielt package.json in einem Express-Projekt?

## Rolle von `package.json` in einem Express-Projekt

**Definition:**
Die Datei `package.json` ist die zentrale Konfigurationsdatei eines Node.js-/Express-Projekts. Sie beschreibt das Projekt, listet Abhängigkeiten auf und steuert Skripte sowie Metadaten.

**Wichtige Inhalte:**

* **Metadaten:** Name, Version, Beschreibung, Autor, Lizenz.
* **Abhängigkeiten:** Enthält installierte Pakete wie `express`, `pg`, `sequelize`.
* **Scripts:** Definiert Befehle, z. B. `npm start`, `npm run dev`.
* **Konfiguration:** Einstellungen für Tools (z. B. ESLint, Jest).
* **Type-Flag:** `"type": "module"` → ermöglicht die Verwendung von ES Modules (`import/export`).

**Beispiel einer `package.json` für ein Express-Projekt:**

```json
{
  "name": "mein-express-projekt",
  "version": "1.0.0",
  "description": "Ein einfaches Express-Projekt",
  "main": "server.js",
  "type": "module",
  "scripts": {
    "start": "node server.js",
    "dev": "nodemon server.js"
  },
  "dependencies": {
    "express": "^4.19.2"
  },
  "devDependencies": {
    "nodemon": "^3.0.2"
  },
  "author": "Sergii",
  "license": "MIT"
}
```

**Verwendung im Projekt:**

```bash
npm install        # liest Abhängigkeiten aus package.json
npm start          # führt Script "start" aus
```

---

### Zusammenfassung

`package.json` steuert Express-Projekte, indem sie Metadaten, Abhängigkeiten, Scripts und Konfigurationen verwaltet. Sie ist notwendig, um ein Projekt reproduzierbar und wartbar zu machen.

**Quellen:**

* [npm – package.json Dokumentation](https://docs.npmjs.com/cli/v10/configuring-npm/package-json)
* [Node.js Dokumentation](https://nodejs.org/docs/latest/api/packages.html)

---

  **[⬆ Наверх](#top)**

10. ### <a name="10"></a> Was bedeutet „Middleware-basiertes Framework“ bei Express?

## Was bedeutet „Middleware-basiertes Framework“ bei Express?

**Definition:**
Ein *Middleware-basiertes Framework* bedeutet, dass die gesamte Request-/Response-Verarbeitung in Express über eine **Kette von Middleware-Funktionen** läuft. Jede Middleware erhält Zugriff auf das `req`- (Request) und `res`- (Response) Objekt und entscheidet, ob sie die Anfrage verarbeitet oder an die nächste Middleware weitergibt.

**Merkmale von Middleware in Express:**

* **Signatur:** `(req, res, next)`
* **Funktion:**

  * Request-Daten analysieren oder verändern
  * zusätzliche Informationen an `req` anhängen
  * Antwort über `res` senden
  * mit `next()` die Kontrolle an die nächste Middleware geben

**Beispiel:**

```js
import express from 'express';

const app = express();

// 1. Middleware – Logging
app.use((req, res, next) => {
  console.log(`${req.method} ${req.url}`);
  next(); // geht weiter zur nächsten Middleware
});

// 2. Middleware – JSON-Parser
app.use(express.json());

// 3. Route als Middleware
app.get('/', (req, res) => {
  res.send('Hallo Middleware-Welt!');
});

// 4. Fehlerbehandlung (spezielle Middleware mit 4 Parametern)
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).send('Etwas ist schiefgelaufen!');
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

**Vorteile des Middleware-Ansatzes:**

* **Flexibel:** Beliebig viele Schritte im Request-Lifecycle einbaubar.
* **Wiederverwendbar:** Viele Drittanbieter-Middleware (z. B. `cors`, `helmet`, `morgan`).
* **Trennung der Logik:** Authentifizierung, Validierung, Logging, Error-Handling sind klar trennbar.

---

### Zusammenfassung

„Middleware-basiert“ heißt: Express verarbeitet HTTP-Anfragen, indem sie durch eine Kette von Funktionen (Middleware) laufen, die den Request/Response verändern, darauf reagieren oder weiterreichen.

**Quellen:**

* [Express.js – Using Middleware](https://expressjs.com/de/guide/using-middleware.html)

---

  **[⬆ Наверх](#top)**

11. ### <a name="11"></a> Wie funktioniert Routing in Express.js?

## Wie funktioniert Routing in Express.js?

**Definition:**
Routing in Express.js bedeutet, dass HTTP-Anfragen (basierend auf URL und HTTP-Methode) bestimmten Handler-Funktionen zugeordnet werden. Jeder Handler bestimmt, wie auf eine Anfrage reagiert wird.

**Wichtige Aspekte:**

* **Methoden:** `app.get()`, `app.post()`, `app.put()`, `app.delete()`, usw.
* **Pfade:** können statisch (`/about`) oder dynamisch (`/users/:id`) sein.
* **Middleware-Prinzip:** Routen sind selbst Middleware-Funktionen.
* **Router-Objekte:** Express erlaubt die Modularisierung von Routen mit `express.Router()`.

---

**Einfaches Beispiel:**

```js
import express from 'express';

const app = express();

// GET-Route
app.get('/', (req, res) => {
  res.send('Startseite');
});

// POST-Route
app.post('/submit', (req, res) => {
  res.send('Formular abgeschickt');
});

// Route mit Parameter
app.get('/users/:id', (req, res) => {
  res.send(`Benutzer-ID: ${req.params.id}`);
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

---

**Router-Modularisierung:**

```js
// routes/users.js
import { Router } from 'express';

const router = Router();

router.get('/', (req, res) => {
  res.send('Alle Benutzer');
});

router.get('/:id', (req, res) => {
  res.send(`Benutzer mit ID ${req.params.id}`);
});

export default router;
```

```js
// server.js
import express from 'express';
import userRoutes from './routes/users.js';

const app = express();
app.use('/users', userRoutes);

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

---

### Zusammenfassung

Routing in Express ordnet Anfragen (Methode + Pfad) spezifischen Handlern zu. Es unterstützt statische und dynamische Routen sowie Modularisierung über `express.Router()`.

**Quellen:**

* [Express.js – Routing](https://expressjs.com/de/guide/routing.html)


  **[⬆ Наверх](#top)**

12. ### <a name="12"></a> Was ist der Unterschied zwischen app.get() und app.post()?

## Unterschied zwischen `app.get()` und `app.post()`

**1. app.get()**

* Wird für **HTTP-GET-Anfragen** verwendet.
* Dient hauptsächlich zum **Abrufen von Daten**.
* Daten werden in der Regel über **Query-Parameter** oder **Route-Parameter** übergeben.
* GET-Anfragen sind **idempotent** (mehrfaches Aufrufen hat keine Seiteneffekte).

```js
import express from 'express';
const app = express();

app.get('/users/:id', (req, res) => {
  const userId = req.params.id; // Route-Parameter
  const filter = req.query.filter; // Query-Parameter
  res.send(`GET-Anfrage für Benutzer ${userId}, Filter: ${filter}`);
});

app.listen(3000);
```

---

**2. app.post()**

* Wird für **HTTP-POST-Anfragen** verwendet.
* Dient zum **Senden von Daten an den Server** (z. B. Formulardaten, JSON).
* Die Daten stehen im **Request-Body** (daher oft `express.json()` als Middleware nötig).
* POST-Anfragen sind **nicht idempotent** (mehrfaches Senden kann neue Ressourcen erzeugen oder Zustand ändern).

```js
import express from 'express';
const app = express();

app.use(express.json()); // Middleware für JSON-Body

app.post('/users', (req, res) => {
  const newUser = req.body; // Daten aus dem Request-Body
  res.status(201).send(`Benutzer erstellt: ${JSON.stringify(newUser)}`);
});

app.listen(3000);
```

---

### Zusammenfassung

* **`app.get()`**: Daten abrufen, Parameter kommen aus **URL** (Query/Route).
* **`app.post()`**: Daten senden, Inhalt kommt aus dem **Request-Body**.
* GET ist idempotent, POST nicht.

**Quellen:**

* [Express.js – Routing](https://expressjs.com/de/guide/routing.html)
* [MDN Web Docs – HTTP-Methoden](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods)


  **[⬆ Наверх](#top)**

13. ### <a name="13"></a> Was macht app.use() im Zusammenhang mit Routing?

## Was macht `app.use()` im Zusammenhang mit Routing?

**Definition:**
`app.use()` registriert Middleware in Express. Im Zusammenhang mit Routing bedeutet das, dass man entweder **Middleware-Funktionen** oder **Router-Objekte** an bestimmte Pfade binden kann.

---

**1. Globale Middleware (ohne Pfad):**
Wird für **alle Anfragen** ausgeführt, unabhängig von der Route oder HTTP-Methode.

```js
import express from 'express';
const app = express();

// Logging-Middleware für alle Routen
app.use((req, res, next) => {
  console.log(`${req.method} ${req.url}`);
  next(); // zur nächsten Middleware oder Route
});
```

---

**2. Middleware für einen bestimmten Pfad:**
Nur Anfragen, die mit diesem Pfad beginnen, durchlaufen die Middleware.

```js
app.use('/api', (req, res, next) => {
  console.log('Middleware für /api');
  next();
});

app.get('/api/test', (req, res) => {
  res.send('API-Route erreicht');
});
```

---

**3. Router einbinden:**
Mit `app.use()` können Router-Module modular integriert werden.

```js
// routes/users.js
import { Router } from 'express';
const router = Router();

router.get('/', (req, res) => {
  res.send('Alle Benutzer');
});

router.get('/:id', (req, res) => {
  res.send(`Benutzer mit ID ${req.params.id}`);
});

export default router;

// server.js
import express from 'express';
import userRoutes from './routes/users.js';

const app = express();

// Mount des Routers unter /users
app.use('/users', userRoutes);

app.listen(3000);
```

→ Aufruf: `http://localhost:3000/users` oder `http://localhost:3000/users/5`

---

### Zusammenfassung

* `app.use()` bindet Middleware oder Router ein.
* Ohne Pfad: gilt für alle Anfragen.
* Mit Pfad: gilt für Routen unterhalb dieses Pfads.
* Häufig verwendet, um Router-Module (`express.Router()`) einzubinden.

**Quellen:**

* [Express.js – app.use()](https://expressjs.com/de/4x/api.html#app.use)
* [Express.js – Router](https://expressjs.com/de/guide/routing.html#express-router)


  **[⬆ Наверх](#top)**

14. ### <a name="14"></a> Wie definiert man Routenparameter in Express?

## Routenparameter in Express

**Definition:**
Routenparameter sind Platzhalter in der URL, die mit `:` definiert werden. Sie dienen dazu, Werte aus der URL zu extrahieren (z. B. IDs oder Namen). Der Zugriff erfolgt über `req.params`.

---

**Einfaches Beispiel:**

```js
import express from 'express';
const app = express();

// Route mit Parameter ":id"
app.get('/users/:id', (req, res) => {
  const userId = req.params.id; // Zugriff auf den Wert von :id
  res.send(`Benutzer mit ID: ${userId}`);
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

→ Aufruf: `http://localhost:3000/users/42`
Antwort: `Benutzer mit ID: 42`

---

**Mehrere Parameter:**

```js
app.get('/users/:userId/books/:bookId', (req, res) => {
  const { userId, bookId } = req.params;
  res.send(`User: ${userId}, Buch: ${bookId}`);
});
```

→ Aufruf: `http://localhost:3000/users/7/books/15`

---

**Optionale Parameter:**

```js
app.get('/products/:id?', (req, res) => {
  const productId = req.params.id || 'keine ID angegeben';
  res.send(`Produkt-ID: ${productId}`);
});
```

→ `http://localhost:3000/products` → `Produkt-ID: keine ID angegeben`
→ `http://localhost:3000/products/99` → `Produkt-ID: 99`

---

### Zusammenfassung

* Routenparameter werden mit `:` definiert (`/users/:id`).
* Zugriff auf Werte über `req.params`.
* Unterstützung für mehrere und optionale Parameter.

**Quellen:**

* [Express.js – Routing](https://expressjs.com/de/guide/routing.html#route-parameter)


  **[⬆ Наверх](#top)**

15. ### <a name="15"></a> Wie greift man in einer Route auf Query-Parameter zu?

## Zugriff auf Query-Parameter in Express

**Definition:**
Query-Parameter sind Schlüssel-Wert-Paare in der URL nach einem `?`. In Express stehen sie im Objekt `req.query` als Properties zur Verfügung.

---

**Einfaches Beispiel:**

```js
import express from 'express';
const app = express();

app.get('/search', (req, res) => {
  const query = req.query.q;      // Zugriff auf Parameter "q"
  const limit = req.query.limit;  // Zugriff auf Parameter "limit"
  res.send(`Suche: ${query}, Limit: ${limit}`);
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

**Aufruf:**
`http://localhost:3000/search?q=Node.js&limit=10`
Antwort: `Suche: Node.js, Limit: 10`

---

**Mehrere Parameter (automatisch als Objekt):**

```js
app.get('/filter', (req, res) => {
  res.json(req.query); // gibt alle Query-Parameter zurück
});
```

`http://localhost:3000/filter?category=books&sort=asc`
Antwort:

```json
{
  "category": "books",
  "sort": "asc"
}
```

---

**Wichtige Hinweise:**

* Query-Parameter sind **immer Strings** (z. B. `"10"` statt `10`). → ggf. konvertieren mit `parseInt()`.
* Sie sind **optional** – wenn nicht vorhanden, ist der Wert `undefined`.

---

### Zusammenfassung

* Zugriff über `req.query`.
* Alle Query-Parameter werden als Objekt gespeichert.
* Typen sind Strings und müssen ggf. konvertiert werden.

**Quellen:**

* [Express.js – req.query](https://expressjs.com/de/4x/api.html#req.query)
* [MDN – Query-Strings](https://developer.mozilla.org/ru/docs/Learn/Common_questions/What_is_a_URL#Параметры_запроса)


  **[⬆ Наверх](#top)**

16. ### <a name="16"></a> Wie erstellt man verschachtelte Router (express.Router)?

## Verschachtelte Router in Express mit `express.Router`

**Definition:**
`express.Router()` erlaubt es, Routen modular aufzubauen. Verschachtelte Router helfen, Routen logisch zu strukturieren, z. B. `/users/:id/posts/:postId`.

---

**Beispiel – Einfacher Router:**

```js
// routes/users.js
import { Router } from 'express';
const router = Router();

router.get('/', (req, res) => {
  res.send('Alle Benutzer');
});

router.get('/:id', (req, res) => {
  res.send(`Benutzer mit ID ${req.params.id}`);
});

export default router;
```

```js
// server.js
import express from 'express';
import userRoutes from './routes/users.js';

const app = express();
app.use('/users', userRoutes);

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

→ `/users` und `/users/42`

---

**Beispiel – Verschachtelung:**

```js
// routes/posts.js
import { Router } from 'express';
const router = Router({ mergeParams: true });

// Zugriff auf :userId aus dem Eltern-Router
router.get('/', (req, res) => {
  res.send(`Alle Posts von User ${req.params.userId}`);
});

router.get('/:postId', (req, res) => {
  res.send(`Post ${req.params.postId} von User ${req.params.userId}`);
});

export default router;
```

```js
// routes/users.js
import { Router } from 'express';
import postRoutes from './posts.js';

const router = Router();

router.get('/', (req, res) => {
  res.send('Alle Benutzer');
});

// Verschachtelter Router für /users/:userId/posts
router.use('/:userId/posts', postRoutes);

export default router;
```

```js
// server.js
import express from 'express';
import userRoutes from './routes/users.js';

const app = express();
app.use('/users', userRoutes);

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

**Aufrufe:**

* `http://localhost:3000/users/5/posts` → *Alle Posts von User 5*
* `http://localhost:3000/users/5/posts/10` → *Post 10 von User 5*

---

### Zusammenfassung

* `express.Router()` ermöglicht modulare und verschachtelte Routen.
* Mit `mergeParams: true` kann ein Kind-Router Parameter des Eltern-Routers nutzen.
* Praktisch für REST-Strukturen wie `/users/:id/posts/:postId`.

**Quellen:**

* [Express.js – Router](https://expressjs.com/de/guide/routing.html#express-router)

  **[⬆ Наверх](#top)**

17. ### <a name="17"></a> Wie kann man eine Route auf mehrere HTTP-Methoden gleichzeitig reagieren lassen?

## Route auf mehrere HTTP-Methoden reagieren lassen

**In Express gibt es zwei Hauptwege:**

---

**1. Mit `app.route()` – Ketten von Methoden für denselben Pfad**

```js
import express from 'express';
const app = express();

app.route('/users')
  .get((req, res) => {
    res.send('GET /users – Liste aller Benutzer');
  })
  .post((req, res) => {
    res.send('POST /users – Neuen Benutzer anlegen');
  })
  .put((req, res) => {
    res.send('PUT /users – Benutzer aktualisieren');
  });

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

→ Vorteil: Saubere Gruppierung mehrerer Methoden für denselben Pfad.

---

**2. Mit `app.all()` – alle Methoden auf einer Route abfangen**

```js
app.all('/test', (req, res) => {
  res.send(`Route /test reagiert auf ${req.method}`);
});
```

→ Wird für **alle HTTP-Methoden** (`GET`, `POST`, `PUT`, `DELETE` …) ausgeführt.

---

**3. Kombination mit Middleware (optional)**

```js
app.use('/items', (req, res, next) => {
  console.log(`Items-Route wurde mit ${req.method} aufgerufen`);
  next();
});

app.get('/items', (req, res) => res.send('GET /items'));
app.post('/items', (req, res) => res.send('POST /items'));
```

---

### Zusammenfassung

* **`app.route(path)`**: mehrere HTTP-Methoden für denselben Pfad gruppieren.
* **`app.all(path)`**: alle Methoden für eine Route behandeln.
* Praktisch für REST-Endpunkte oder gemeinsame Logik.

**Quellen:**

* [Express.js – app.route()](https://expressjs.com/de/4x/api.html#app.route)
* [Express.js – app.all()](https://expressjs.com/de/4x/api.html#app.all)

  **[⬆ Наверх](#top)**

18. ### <a name="18"></a> Was ist der Unterschied zwischen app.all() und spezifischen Methoden wie app.get()?

## Unterschied zwischen `app.all()` und spezifischen Methoden wie `app.get()`

**1. `app.get()`, `app.post()`, `app.put()`, `app.delete()`**

* Reagieren **nur auf eine bestimmte HTTP-Methode**.
* Typisch für **REST-APIs**, wo jede Methode eine eigene Bedeutung hat.
* Beispiel:

```js
import express from 'express';
const app = express();

app.get('/users', (req, res) => {
  res.send('GET /users – alle Benutzer abrufen');
});

app.post('/users', (req, res) => {
  res.send('POST /users – neuen Benutzer erstellen');
});
```

---

**2. `app.all()`**

* Reagiert auf **alle HTTP-Methoden** (`GET`, `POST`, `PUT`, `DELETE`, `PATCH`, …) für den angegebenen Pfad.
* Nützlich für:

  * Middleware-artige Funktionen für eine Route
  * Fehlerseiten oder Catch-All-Routen
  * Logging oder spezielle Regeln, bevor die spezifischen Methoden verarbeitet werden

```js
app.all('/test', (req, res) => {
  res.send(`Route /test reagiert auf ${req.method}`);
});
```

---

**Vergleich in der Praxis:**

* `app.get('/route')` → nur GET-Anfragen
* `app.post('/route')` → nur POST-Anfragen
* `app.all('/route')` → jede HTTP-Anfrage wird abgefangen

---

### Zusammenfassung

* **`app.get()` (und ähnliche):** für spezifische HTTP-Methoden, REST-konform.
* **`app.all()`:** für alle Methoden, oft für Middleware, Logging oder Fallback-Routen genutzt.

**Quellen:**

* [Express.js – app.get()](https://expressjs.com/de/4x/api.html#app.METHOD)
* [Express.js – app.all()](https://expressjs.com/de/4x/api.html#app.all)

  **[⬆ Наверх](#top)**

19. ### <a name="19"></a> Wie kann man Wildcard-Routen erstellen?

## Wildcard-Routen in Express

**Definition:**
Wildcard-Routen (Platzhalter-Routen) fangen mehrere oder alle möglichen Pfade ab. Sie werden mit `*` oder regulären Ausdrücken definiert. Nützlich für **Fallbacks, 404-Seiten oder Catch-All-Logik**.

---

**1. Catch-All-Route mit `*`:**

```js
import express from 'express';
const app = express();

app.get('*', (req, res) => {
  res.status(404).send('Seite nicht gefunden');
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

→ Fängt alle GET-Anfragen ab, die keiner spezifischen Route entsprechen.

---

**2. Wildcard in Pfaden:**

```js
app.get('/files/*', (req, res) => {
  res.send(`Dateipfad: ${req.originalUrl}`);
});
```

→ `/files/docs/readme.txt` → Antwort: *Dateipfad: /files/docs/readme.txt*

---

**3. Reguläre Ausdrücke für flexible Routen:**

```js
// Alle Routen, die mit "api" beginnen
app.get(/^\/api\/.*/, (req, res) => {
  res.send('API-Wildcard-Route');
});
```

---

**4. Typische 404-Route (am Ende der Route-Definitionen):**

```js
// Muss ganz am Ende stehen
app.use((req, res) => {
  res.status(404).send('404 – Route nicht gefunden');
});
```

---

### Zusammenfassung

* Wildcard-Routen (`*`) dienen als Fallback oder Catch-All.
* Nützlich für 404-Seiten, Logging oder das Abfangen von unbekannten Pfaden.
* Auch reguläre Ausdrücke können in Express für flexible Wildcards genutzt werden.

**Quellen:**

* [Express.js – Routing](https://expressjs.com/de/guide/routing.html)

  **[⬆ Наверх](#top)**

20. ### <a name="20"></a> Was passiert, wenn keine Route im Express-Server passt?

## Was passiert, wenn keine Route im Express-Server passt?

### Standardverhalten

* Wenn keine definierte Route mit der Anfrage übereinstimmt, geht Express die Middleware-Kette durch.
* Wird keine passende Middleware/Route gefunden, endet der Request ohne Antwort.
* In diesem Fall sendet Express automatisch einen **404-Statuscode (Not Found)** zurück.

---

### Eigene 404-Fehlerseite definieren

Um bessere Kontrolle zu haben, legt man am Ende aller Routen eine Middleware ohne Pfad an:

```js
import express from 'express';
const app = express();

app.get('/', (req, res) => {
  res.send('Startseite');
});

// 404-Catch-All (immer am Ende platzieren!)
app.use((req, res) => {
  res.status(404).send('404 – Seite nicht gefunden');
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

---

### 404 + Error-Handling kombinieren

```js
// 404-Handler
app.use((req, res, next) => {
  res.status(404).json({ error: 'Route nicht gefunden' });
});

// Globaler Fehler-Handler (für Exceptions)
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).send('500 – Interner Serverfehler');
});
```

---

### Zusammenfassung

* Ohne passende Route gibt Express **automatisch 404 Not Found** zurück.
* **Best Practice:** Eigene 404-Middleware am Ende definieren.
* Zusätzlich sollte man einen globalen **500-Fehler-Handler** für Serverfehler einbauen.

**Quellen:**

* [Express.js – Fehlerbehandlung](https://expressjs.com/de/guide/error-handling.html)

  **[⬆ Наверх](#top)**

21. ### <a name="21"></a> Was ist Middleware in Express.js?

## Was ist Middleware in Express.js?

**Definition:**
Middleware in Express.js sind Funktionen, die Zugriff auf die Objekte `req` (Request), `res` (Response) und die Funktion `next` haben. Sie werden in der Reihenfolge ausgeführt, wie sie mit `app.use()` oder an einer Route registriert wurden.

**Aufgaben von Middleware:**

* Anfragen vorverarbeiten (z. B. Body-Parser, Logging, Authentifizierung).
* Daten an `req` anhängen oder verändern.
* Antworten mit `res` senden.
* Mit `next()` die Verarbeitung an die nächste Middleware oder Route weitergeben.

---

**Typen von Middleware:**

1. **Built-in Middleware:**

   * `express.json()` → JSON-Body parsen
   * `express.urlencoded()` → Formulardaten parsen
   * `express.static()` → statische Dateien bereitstellen

2. **Third-Party Middleware:**

   * `morgan` (Logging)
   * `cors` (Cross-Origin Resource Sharing)
   * `helmet` (Sicherheits-Header)

3. **Custom Middleware:**

   * Eigene Logik definieren

---

**Beispiele:**

```js
import express from 'express';
const app = express();

// Built-in Middleware
app.use(express.json());

// Custom Middleware (Logger)
app.use((req, res, next) => {
  console.log(`${req.method} ${req.url}`);
  next(); // wichtig: geht weiter zur nächsten Middleware/Route
});

// Route
app.get('/', (req, res) => {
  res.send('Hallo Middleware!');
});

// Error-Handling Middleware
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).send('Interner Serverfehler');
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

---

### Zusammenfassung

* Middleware sind Funktionen, die den Request-Response-Zyklus in Express steuern.
* Sie können Anfragen verarbeiten, Daten anreichern, Antworten senden oder an die nächste Funktion weitergeben.
* Es gibt **eingebaute**, **Third-Party-** und **eigene** Middleware.

**Quellen:**

* [Express.js – Using Middleware](https://expressjs.com/de/guide/using-middleware.html)


  **[⬆ Наверх](#top)**

22. ### <a name="22"></a> Welche Arten von Middleware gibt es?

## Arten von Middleware in Express.js

**1. Built-in Middleware (eingebaute Middleware)**
Von Express direkt bereitgestellt:

* `express.json()` – parst JSON-Daten im Request-Body.
* `express.urlencoded()` – parst Formulardaten (`application/x-www-form-urlencoded`).
* `express.static()` – liefert statische Dateien wie HTML, CSS, JS, Bilder aus.

```js
app.use(express.json());
app.use(express.urlencoded({ extended: true }));
app.use(express.static('public'));
```

---

**2. Third-Party Middleware (externe Middleware)**
Von der Community entwickelt, via npm installierbar:

* `morgan` – Logging von Requests.
* `cors` – Cross-Origin Resource Sharing aktivieren.
* `helmet` – Security-Header setzen.

```js
import morgan from 'morgan';
import cors from 'cors';
import helmet from 'helmet';

app.use(morgan('dev'));
app.use(cors());
app.use(helmet());
```

---

**3. Application-Level Middleware**
Direkt mit `app.use()` oder `app.METHOD()` definiert.

```js
app.use((req, res, next) => {
  console.log('Application-Level Middleware');
  next();
});
```

---

**4. Router-Level Middleware**
Nur für bestimmte Router gültig.

```js
import { Router } from 'express';
const router = Router();

router.use((req, res, next) => {
  console.log('Router-Level Middleware');
  next();
});

router.get('/', (req, res) => res.send('Hallo vom Router'));
app.use('/users', router);
```

---

**5. Error-Handling Middleware**
Besonderheit: **vier Parameter** `(err, req, res, next)`.

```js
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).send('Interner Serverfehler');
});
```

---

**6. Custom Middleware**
Eigene Funktionen für spezielle Aufgaben, z. B. Authentifizierung:

```js
function authMiddleware(req, res, next) {
  if (req.headers.authorization === 'secret') {
    next();
  } else {
    res.status(403).send('Zugriff verweigert');
  }
}

app.use('/admin', authMiddleware);
```

---

### Zusammenfassung

* **Built-in** (express.json, express.static)
* **Third-Party** (morgan, cors, helmet)
* **Application-Level** (app.use)
* **Router-Level** (express.Router)
* **Error-Handling** (mit `err`-Parameter)
* **Custom** (eigene Logik, z. B. Auth)

**Quellen:**

* [Express.js – Using Middleware](https://expressjs.com/de/guide/using-middleware.html)


  **[⬆ Наверх](#top)**

23. ### <a name="23"></a> Wie unterscheidet sich globale Middleware von Router-spezifischer Middleware?

## Unterschied zwischen globaler Middleware und Router-spezifischer Middleware in Express.js

**1. Globale Middleware**

* Wird mit `app.use()` registriert.
* Gilt für **alle Routen** und **alle HTTP-Methoden**, die nach der Registrierung folgen.
* Typisch für Logging, Body-Parsing oder Sicherheitsfunktionen.

```js
import express from 'express';
const app = express();

// Globale Middleware – läuft bei jeder Anfrage
app.use((req, res, next) => {
  console.log(`Globale Middleware: ${req.method} ${req.url}`);
  next();
});

app.get('/', (req, res) => res.send('Startseite'));
app.get('/about', (req, res) => res.send('Über uns'));

app.listen(3000);
```

---

**2. Router-spezifische Middleware**

* Wird nur für einen bestimmten **Router** oder **Pfad** ausgeführt.
* Mit `router.use()` oder beim Mounten eines Routers (`app.use('/path', router)`).
* Typisch für Authentifizierung, Validierung oder spezielle Logik pro Router.

```js
import { Router } from 'express';
const app = express();
const router = Router();

// Router-spezifische Middleware
router.use((req, res, next) => {
  console.log(`Router-Middleware für /users: ${req.method} ${req.url}`);
  next();
});

router.get('/', (req, res) => res.send('Alle Benutzer'));
router.get('/:id', (req, res) => res.send(`Benutzer mit ID ${req.params.id}`));

// Router wird unter /users gemountet
app.use('/users', router);

app.listen(3000);
```

---

### Zusammenfassung

* **Globale Middleware:** wirkt auf alle Routen und Methoden im gesamten Express-App-Kontext.
* **Router-spezifische Middleware:** wirkt nur innerhalb eines bestimmten Routers oder Pfads.

**Quellen:**

* [Express.js – Using Middleware](https://expressjs.com/de/guide/using-middleware.html)


  **[⬆ Наверх](#top)**

24. ### <a name="24"></a> Wie erstellt man eine eigene Middleware-Funktion?

## Eigene Middleware in Express erstellen

**Definition:**
Eine eigene Middleware ist eine Funktion mit den Parametern `(req, res, next)`.

* `req` → enthält die Request-Daten
* `res` → ermöglicht das Senden einer Antwort
* `next` → ruft die nächste Middleware oder Route auf

---

**Beispiel – einfache Logging-Middleware:**

```js
import express from 'express';
const app = express();

// Eigene Middleware
function logger(req, res, next) {
  console.log(`${req.method} ${req.url}`);
  next(); // wichtig: geht weiter zur nächsten Middleware/Route
}

app.use(logger);

app.get('/', (req, res) => {
  res.send('Startseite');
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

---

**Beispiel – Middleware für Authentifizierung:**

```js
function auth(req, res, next) {
  if (req.headers.authorization === 'secret') {
    next(); // Zugriff erlaubt
  } else {
    res.status(403).send('Zugriff verweigert');
  }
}

app.get('/admin', auth, (req, res) => {
  res.send('Adminbereich');
});
```

---

**Beispiel – Error-Handling Middleware:**
Besonderheit: hat **vier Parameter** `(err, req, res, next)`.

```js
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).send('Interner Serverfehler');
});
```

---

### Zusammenfassung

* Eigene Middleware wird als Funktion `(req, res, next)` definiert.
* Typische Aufgaben: Logging, Validierung, Authentifizierung, Fehlerbehandlung.
* Mit `next()` wird der Request weitergereicht.
* Fehler-Middleware benötigt **vier Parameter**.

**Quellen:**

* [Express.js – Using Middleware](https://expressjs.com/de/guide/using-middleware.html)


  **[⬆ Наверх](#top)**

25. ### <a name="25"></a> Was sind Third-Party-Middleware-Beispiele in Express?

## Third-Party-Middleware in Express – Beispiele

**Definition:**
Third-Party-Middleware sind externe Pakete, die man per **npm** installiert und in Express integriert. Sie erweitern die Funktionalität der Anwendung, z. B. für Logging, Sicherheit oder CORS.

---

**1. morgan – HTTP-Request-Logger**
Hilft beim Loggen von Anfragen im Terminal.

```js
import express from 'express';
import morgan from 'morgan';

const app = express();
app.use(morgan('dev')); // Loggt Methode, Pfad, Statuscode

app.get('/', (req, res) => res.send('Hallo Morgan!'));
app.listen(3000);
```

---

**2. cors – Cross-Origin Resource Sharing**
Erlaubt Requests von anderen Domains (z. B. React-Frontend → Express-API).

```js
import express from 'express';
import cors from 'cors';

const app = express();
app.use(cors()); // Alle Domains erlaubt
// oder app.use(cors({ origin: 'http://localhost:5173' }));

app.get('/data', (req, res) => res.json({ message: 'CORS aktiviert' }));
app.listen(3000);
```

---

**3. helmet – Sicherheits-Header**
Setzt HTTP-Header, um die App sicherer zu machen.

```js
import express from 'express';
import helmet from 'helmet';

const app = express();
app.use(helmet());

app.get('/', (req, res) => res.send('Mit Sicherheits-Headern'));
app.listen(3000);
```

---

**4. cookie-parser – Cookies auslesen**

```js
import express from 'express';
import cookieParser from 'cookie-parser';

const app = express();
app.use(cookieParser());

app.get('/cookies', (req, res) => {
  res.send(req.cookies); // zeigt alle Cookies
});
app.listen(3000);
```

---

**5. express-session – Session-Management**

```js
import express from 'express';
import session from 'express-session';

const app = express();
app.use(session({
  secret: 'meinSecret',
  resave: false,
  saveUninitialized: true
}));

app.get('/', (req, res) => {
  req.session.views = (req.session.views || 0) + 1;
  res.send(`Seite besucht: ${req.session.views} mal`);
});
app.listen(3000);
```

---

### Zusammenfassung

Typische Third-Party-Middleware in Express:

* **morgan** (Logging)
* **cors** (CORS-Unterstützung)
* **helmet** (Sicherheit)
* **cookie-parser** (Cookies auslesen)
* **express-session** (Sessions)

**Quellen:**

* [morgan](https://www.npmjs.com/package/morgan)
* [cors](https://www.npmjs.com/package/cors)
* [helmet](https://www.npmjs.com/package/helmet)
* [cookie-parser](https://www.npmjs.com/package/cookie-parser)
* [express-session](https://www.npmjs.com/package/express-session)


  **[⬆ Наверх](#top)**

26. ### <a name="26"></a> Wie wird next() in Middleware verwendet?

## Verwendung von `next()` in Middleware

**Definition:**
`next()` ist eine Funktion, die in Express-Middleware aufgerufen wird, um den Request an die **nächste Middleware oder Route** weiterzugeben.

* Ohne `next()` bleibt der Request hängen (Timeout).
* Mit `next(err)` wird stattdessen die **Error-Handling-Middleware** ausgelöst.

---

**1. Normaler Ablauf mit `next()`**

```js
import express from 'express';
const app = express();

// Logging-Middleware
app.use((req, res, next) => {
  console.log(`${req.method} ${req.url}`);
  next(); // geht weiter zur nächsten Middleware oder Route
});

app.get('/', (req, res) => {
  res.send('Startseite');
});

app.listen(3000);
```

---

**2. Bedingungen prüfen und weiterleiten**

```js
function checkAuth(req, res, next) {
  if (req.headers.authorization === 'secret') {
    next(); // Zugriff erlaubt → geht zur Route
  } else {
    res.status(403).send('Zugriff verweigert'); // bricht ab, kein next()
  }
}

app.get('/admin', checkAuth, (req, res) => {
  res.send('Adminbereich');
});
```

---

**3. Fehler weitergeben mit `next(err)`**

```js
app.use((req, res, next) => {
  const error = new Error('Etwas ist schiefgelaufen');
  next(error); // Springt zur Error-Handling-Middleware
});

// Error-Handler
app.use((err, req, res, next) => {
  console.error(err.message);
  res.status(500).send('Interner Serverfehler');
});
```

---

### Zusammenfassung

* `next()` leitet den Request an die nächste Middleware/Route weiter.
* Ohne Aufruf bleibt der Request hängen.
* `next(err)` ruft die Error-Handling-Middleware auf.

**Quellen:**

* [Express.js – Using Middleware](https://expressjs.com/de/guide/using-middleware.html)


  **[⬆ Наверх](#top)**

27. ### <a name="27"></a> Wie kann man Reihenfolge von Middleware steuern?

## Reihenfolge von Middleware in Express steuern

**Prinzip:**

* Express führt Middleware in **genau der Reihenfolge** aus, in der sie mit `app.use()` oder `app.METHOD()` registriert wurde.
* Reihenfolge = Kontrolle über den Request-Response-Flow.

---

**1. Globale Reihenfolge**

```js
import express from 'express';
const app = express();

// 1. Logger
app.use((req, res, next) => {
  console.log('Logger');
  next();
});

// 2. Parser
app.use(express.json());

// 3. Route
app.get('/', (req, res) => {
  res.send('Antwort von der Route');
});

// 4. 404-Middleware (immer am Ende)
app.use((req, res) => {
  res.status(404).send('Nicht gefunden');
});

app.listen(3000);
```

→ Die Middleware wird strikt in dieser Reihenfolge abgearbeitet.

---

**2. Reihenfolge pro Route**
Middleware kann **direkt bei einer Route** definiert werden.

```js
function mw1(req, res, next) {
  console.log('mw1');
  next();
}

function mw2(req, res, next) {
  console.log('mw2');
  next();
}

app.get('/test', mw1, mw2, (req, res) => {
  res.send('Fertig');
});
```

→ Reihenfolge: `mw1 → mw2 → Route`.

---

**3. Router-Reihenfolge**

* Router selbst werden in der Reihenfolge eingebunden, in der `app.use()` sie registriert.

```js
import { Router } from 'express';
const router1 = Router();
const router2 = Router();

router1.get('/', (req, res) => res.send('Router1'));
router2.get('/', (req, res) => res.send('Router2'));

app.use('/r1', router1); // wird vor router2 ausgeführt
app.use('/r2', router2);
```

---

**Best Practices:**

* **Globale Middleware (Logger, Parser)** zuerst.
* **Routen** in der Mitte.
* **404-Handler** am Ende.
* **Error-Handler** ganz am Schluss.

---

### Zusammenfassung

* Middleware wird in der Reihenfolge der Registrierung ausgeführt.
* Reihenfolge gilt sowohl global (`app.use`) als auch pro Route.
* 404- und Error-Handler immer am Ende platzieren.

**Quellen:**

* [Express.js – Middleware](https://expressjs.com/de/guide/using-middleware.html)


  **[⬆ Наверх](#top)**

28. ### <a name="28"></a> Wie kann man Middleware nur auf bestimmte Routen anwenden?

## Middleware nur auf bestimmte Routen anwenden

**1. Direkt bei der Route definieren**
Man hängt die Middleware als zusätzlichen Parameter vor den Route-Handler.

```js
import express from 'express';
const app = express();

function checkAuth(req, res, next) {
  if (req.headers.authorization === 'secret') {
    next();
  } else {
    res.status(403).send('Zugriff verweigert');
  }
}

// Nur für /admin angewendet
app.get('/admin', checkAuth, (req, res) => {
  res.send('Adminbereich');
});

app.get('/', (req, res) => {
  res.send('Öffentliche Seite');
});

app.listen(3000);
```

---

**2. Mehrere Middleware-Funktionen in einer Route**

```js
function mw1(req, res, next) {
  console.log('mw1');
  next();
}

function mw2(req, res, next) {
  console.log('mw2');
  next();
}

app.get('/test', mw1, mw2, (req, res) => {
  res.send('Route mit zwei Middleware-Funktionen');
});
```

---

**3. Router-spezifische Middleware**
Mit `express.Router()` kann Middleware für bestimmte Router gelten.

```js
import { Router } from 'express';
const app = express();
const userRouter = Router();

function logUserRoute(req, res, next) {
  console.log(`Benutzer-Route aufgerufen: ${req.method} ${req.url}`);
  next();
}

// Middleware nur für userRouter
userRouter.use(logUserRoute);

userRouter.get('/', (req, res) => res.send('Alle Benutzer'));
userRouter.get('/:id', (req, res) => res.send(`Benutzer ${req.params.id}`));

app.use('/users', userRouter);

app.listen(3000);
```

→ Middleware `logUserRoute` gilt **nur für `/users`**.

---

### Zusammenfassung

* Middleware kann direkt bei einer Route definiert werden.
* Mehrere Middleware-Funktionen sind möglich (Kette).
* Mit `express.Router()` lässt sich Middleware nur auf bestimmte Routenbereiche anwenden.

**Quellen:**

* [Express.js – Router Middleware](https://expressjs.com/de/guide/using-middleware.html)


  **[⬆ Наверх](#top)**

29. ### <a name="29"></a> Wie funktioniert express.json() und wofür wird es genutzt?

## Wie funktioniert `express.json()` und wofür wird es genutzt?

**Definition:**
`express.json()` ist eine **eingebaute Middleware** in Express.

* Sie parst den Request-Body, wenn der **Content-Type `application/json`** ist.
* Danach stehen die Daten im Objekt `req.body` zur Verfügung.

Ohne diese Middleware wäre `req.body` standardmäßig `undefined`.

---

**Funktionsweise:**

* Bei einer Anfrage mit JSON-Body liest `express.json()` den Body-Stream.
* Die Daten werden in ein JavaScript-Objekt geparst.
* Dieses Objekt wird an `req.body` gehängt, sodass es in Routen-Handlern verfügbar ist.

---

**Beispiel – JSON-Parsing aktivieren:**

```js
import express from 'express';
const app = express();

// Middleware aktivieren
app.use(express.json());

app.post('/data', (req, res) => {
  console.log(req.body); // enthält geparstes JSON
  res.send(`Empfangene Daten: ${JSON.stringify(req.body)}`);
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

**Aufruf mit POST-Request (z. B. via curl oder Postman):**

```bash
curl -X POST http://localhost:3000/data \
  -H "Content-Type: application/json" \
  -d '{"name":"Sergii","age":30}'
```

**Antwort:**

```
Empfangene Daten: {"name":"Sergii","age":30}
```

---

**Typische Anwendungsfälle:**

* REST-APIs, die JSON-Daten empfangen (z. B. Benutzer-Registrierung, Formulardaten).
* Kommunikation mit Frontends wie React, Angular oder Vue, die Daten als JSON senden.

---

### Zusammenfassung

* `express.json()` ist Middleware zum automatischen Parsen von JSON-Bodys.
* Ergebnis ist als `req.body` im Route-Handler verfügbar.
* Unerlässlich für APIs, die JSON empfangen.

**Quellen:**

* [Express.js – express.json()](https://expressjs.com/de/api.html#express.json)


  **[⬆ Наверх](#top)**

30. ### <a name="30"></a> Wie funktioniert express.urlencoded()?

## Wie funktioniert `express.urlencoded()`?

**Definition:**
`express.urlencoded()` ist eine **eingebaute Middleware** in Express.

* Sie parst **URL-encoded Daten** (Content-Type: `application/x-www-form-urlencoded`).
* Solche Daten entstehen typischerweise, wenn man ein HTML-Formular abschickt.
* Die geparsten Werte stehen anschließend in `req.body` zur Verfügung.

---

**Funktionsweise:**

* Liest den Body der Anfrage ein.
* Wandelt die `key=value&key2=value2`-Notation in ein JavaScript-Objekt um.
* Beispiel: `name=Sergii&age=30` → `{ name: 'Sergii', age: '30' }`.

---

**Beispiel – Formulardaten verarbeiten:**

```js
import express from 'express';
const app = express();

// Middleware aktivieren
app.use(express.urlencoded({ extended: true }));

app.post('/form', (req, res) => {
  console.log(req.body); // enthält geparste Formulardaten
  res.send(`Empfangene Daten: ${JSON.stringify(req.body)}`);
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

**HTML-Formular:**

```html
<form action="/form" method="post">
  <input type="text" name="name" value="Sergii" />
  <input type="number" name="age" value="30" />
  <button type="submit">Absenden</button>
</form>
```

**Resultat:**

```json
{
  "name": "Sergii",
  "age": "30"
}
```

---

**Option `extended`:**

* `extended: false` → verwendet den Node.js-Standardparser (`querystring`), kann nur einfache Schlüssel-Wert-Paare parsen.
* `extended: true` → verwendet das `qs`-Paket, unterstützt auch verschachtelte Objekte und Arrays.

Beispiel:

```
user[name]=Sergii&user[age]=30
```

→ `{ user: { name: 'Sergii', age: '30' } }` (nur bei `extended: true`)

---

### Zusammenfassung

* `express.urlencoded()` parst **Formulardaten (x-www-form-urlencoded)** in `req.body`.
* Mit `extended: true` lassen sich auch verschachtelte Datenstrukturen parsen.
* Typisch für klassische HTML-Formulare.

**Quellen:**

* [Express.js – express.urlencoded()](https://expressjs.com/de/api.html#express.urlencoded)


  **[⬆ Наверх](#top)**  

31. ### <a name="31"></a> Welche Objekte sind in Express.js für HTTP-Anfragen und -Antworten zuständig?

## Objekte für HTTP-Anfragen und -Antworten in Express.js

**1. `req` (Request-Objekt)**

* Repräsentiert die eingehende HTTP-Anfrage.
* Enthält Daten über die Anfrage: Methode, URL, Header, Parameter, Body.
* Wichtige Eigenschaften und Methoden:

  * `req.method` → HTTP-Methode (`GET`, `POST`, …)
  * `req.url` → angeforderte URL
  * `req.params` → Routen-Parameter (`/users/:id`)
  * `req.query` → Query-Parameter (`?sort=asc`)
  * `req.body` → Body-Daten (mit Middleware wie `express.json()` oder `express.urlencoded()`)
  * `req.headers` → Header-Informationen

---

**2. `res` (Response-Objekt)**

* Repräsentiert die ausgehende Antwort an den Client.
* Wird verwendet, um Daten zurückzugeben, Header zu setzen oder den Statuscode festzulegen.
* Wichtige Methoden:

  * `res.send()` → Antwort als String/Buffer/Objekt senden
  * `res.json()` → JSON-Daten senden
  * `res.status(code)` → HTTP-Status setzen
  * `res.redirect(url)` → Umleitung an eine andere URL
  * `res.end()` → Antwort beenden (niedriger Level, selten direkt genutzt)

---

**Beispiel:**

```js
import express from 'express';
const app = express();

app.use(express.json());

app.get('/users/:id', (req, res) => {
  console.log(req.params.id);     // Zugriff auf Route-Parameter
  console.log(req.query.filter);  // Zugriff auf Query-Parameter

  res.status(200).json({
    message: 'Benutzerdaten',
    id: req.params.id,
    filter: req.query.filter || 'none'
  });
});

app.post('/users', (req, res) => {
  console.log(req.body); // JSON-Body
  res.status(201).send(`Neuer Benutzer erstellt: ${req.body.name}`);
});

app.listen(3000, () => {
  console.log('Server läuft auf Port 3000');
});
```

---

### Zusammenfassung

* **`req`**: Eingehende Anfrage (enthält Methode, URL, Header, Parameter, Body).
* **`res`**: Antwort an den Client (enthält Methoden wie `send()`, `json()`, `status()`).
* Beide Objekte sind Wrapper um Node.js’ `http.IncomingMessage` und `http.ServerResponse`.

**Quellen:**

* [Express.js – Request-Objekt](https://expressjs.com/de/4x/api.html#req)
* [Express.js – Response-Objekt](https://expressjs.com/de/4x/api.html#res)


  **[⬆ Наверх](#top)**

32. ### <a name="32"></a> Wie greift man auf Request-Header zu?

## Zugriff auf Request-Header in Express.js

**Definition:**
Request-Header enthalten zusätzliche Informationen über die HTTP-Anfrage (z. B. `Content-Type`, `Authorization`, `User-Agent`).
In Express kann man mit `req.headers` oder `req.get()` darauf zugreifen.

---

**1. Zugriff auf alle Header:**

```js
app.get('/info', (req, res) => {
  console.log(req.headers); // alle Header als Objekt
  res.send(req.headers);
});
```

---

**2. Zugriff auf einen bestimmten Header:**

```js
app.get('/auth', (req, res) => {
  const authHeader = req.get('Authorization'); // oder req.headers['authorization']
  res.send(`Authorization-Header: ${authHeader}`);
});
```

---

**3. Beispiel mit Content-Type:**

```js
app.post('/data', (req, res) => {
  const contentType = req.get('Content-Type');
  res.send(`Content-Type ist: ${contentType}`);
});
```

---

**Wichtige Hinweise:**

* Header-Namen sind **case-insensitive** (`Authorization` = `authorization`).
* Viele Header werden von Browsern automatisch gesetzt (`Host`, `User-Agent`, `Accept`).

---

### Zusammenfassung

* Mit `req.headers` bekommt man ein Objekt aller Header.
* Mit `req.get('Header-Name')` liest man einen bestimmten Header aus.
* Header sind wichtig für Authentifizierung, Content-Type, CORS usw.

**Quellen:**

* [Express.js – req.get()](https://expressjs.com/de/4x/api.html#req.get)
* [MDN – HTTP-Header](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers)


  **[⬆ Наверх](#top)**

33. ### <a name="33"></a> Wie greift man auf Body-Daten zu?

## Zugriff auf Body-Daten in Express.js

**Definition:**
Der Request-Body enthält Daten, die vom Client (z. B. Browser oder API-Client) im Rahmen einer Anfrage gesendet werden – oft bei **POST**, **PUT** oder **PATCH**.
In Express sind Body-Daten standardmäßig **nicht verfügbar** → man benötigt Middleware wie `express.json()` oder `express.urlencoded()`.

---

**1. JSON-Body auslesen**

```js
import express from 'express';
const app = express();

// JSON-Body-Parser aktivieren
app.use(express.json());

app.post('/user', (req, res) => {
  console.log(req.body); // enthält geparstes JSON
  res.send(`Empfangen: ${JSON.stringify(req.body)}`);
});

app.listen(3000);
```

**Beispiel-Request (POST mit JSON):**

```bash
curl -X POST http://localhost:3000/user \
  -H "Content-Type: application/json" \
  -d '{"name":"Sergii","age":30}'
```

---

**2. URL-encoded Body (Formulardaten)**

```js
app.use(express.urlencoded({ extended: true }));

app.post('/form', (req, res) => {
  console.log(req.body); // enthält Formulardaten
  res.send(req.body);
});
```

**Beispiel-Request:**

```
name=Sergii&age=30
```

→ `{ name: 'Sergii', age: '30' }`

---

**3. Zugriff auf Dateien (mit Multer als Third-Party-Middleware)**
Wenn der Body Dateien enthält (Multipart-Formular), wird **Multer** benötigt:

```js
import multer from 'multer';
const upload = multer({ dest: 'uploads/' });

app.post('/upload', upload.single('file'), (req, res) => {
  console.log(req.file); // Datei-Infos
  console.log(req.body); // zusätzliche Felder
  res.send('Upload erfolgreich');
});
```

---

### Zusammenfassung

* **JSON-Daten:** mit `express.json()` → Zugriff über `req.body`.
* **Formulardaten:** mit `express.urlencoded()` → Zugriff über `req.body`.
* **Dateien:** mit Middleware wie `multer` → Zugriff über `req.file` / `req.files`.

**Quellen:**

* [Express.js – express.json()](https://expressjs.com/de/api.html#express.json)
* [Express.js – express.urlencoded()](https://expressjs.com/de/api.html#express.urlencoded)
* [Multer – npm](https://www.npmjs.com/package/multer)


  **[⬆ Наверх](#top)**

34. ### <a name="34"></a> Wie sendet man JSON als Antwort?

## JSON als Antwort in Express senden

**1. Mit `res.json()`**

* Wandelt automatisch ein JavaScript-Objekt in JSON um.
* Setzt den Header `Content-Type: application/json`.

```js
import express from 'express';
const app = express();

app.get('/user', (req, res) => {
  res.json({ name: 'Sergii', age: 30 });
});

app.listen(3000);
```

→ Antwort:

```json
{
  "name": "Sergii",
  "age": 30
}
```

---

**2. Mit `res.send()` (funktioniert auch, aber weniger spezifisch)**

* Erkennt Objekte und konvertiert sie ebenfalls in JSON.
* Setzt aber nicht immer explizit den richtigen Header.

```js
app.get('/info', (req, res) => {
  res.send({ status: 'ok', version: '1.0' });
});
```

---

**3. Statuscode und JSON kombinieren**

```js
app.post('/login', (req, res) => {
  res.status(201).json({ message: 'User erstellt', id: 123 });
});
```

---

### Zusammenfassung

* **Empfohlene Methode:** `res.json(obj)` → sendet JSON + richtigen Content-Type.
* `res.send(obj)` geht auch, ist aber weniger eindeutig.
* Mit `res.status(code)` lässt sich ein Statuscode hinzufügen.

**Quellen:**

* [Express.js – res.json()](https://expressjs.com/de/4x/api.html#res.json)
* [Express.js – res.send()](https://expressjs.com/de/4x/api.html#res.send)


  **[⬆ Наверх](#top)**

35. ### <a name="35"></a> Wie funktioniert res.send()?

## Wie funktioniert `res.send()` in Express?

**Definition:**
`res.send()` ist eine Methode des Response-Objekts in Express, mit der man eine Antwort an den Client schickt. Sie beendet automatisch den Request-Response-Zyklus.

---

**Eigenschaften von `res.send()`:**

* Kann **Strings, Buffer, Objekte oder Arrays** senden.
* Setzt automatisch den passenden `Content-Type`-Header:

  * String → `text/html` oder `text/plain`
  * Objekt/Array → `application/json`
  * Buffer → `application/octet-stream`
* Schließt die Verbindung nach dem Senden der Antwort.

---

**Beispiele:**

```js
import express from 'express';
const app = express();

// String senden
app.get('/text', (req, res) => {
  res.send('Hallo Welt');
});

// HTML senden
app.get('/html', (req, res) => {
  res.send('<h1>Hallo Express</h1>');
});

// JSON senden (automatisch)
app.get('/json', (req, res) => {
  res.send({ user: 'Sergii', role: 'admin' });
});

// Buffer senden
app.get('/buffer', (req, res) => {
  res.send(Buffer.from('Binärdaten'));
});

app.listen(3000);
```

---

**Mit Statuscode kombinieren:**

```js
app.post('/login', (req, res) => {
  res.status(201).send('Benutzer erstellt');
});
```

---

### Zusammenfassung

* `res.send()` sendet eine Antwort an den Client und beendet den Zyklus.
* Automatisch wird der passende `Content-Type` gesetzt.
* Kann Strings, HTML, JSON, Arrays und Buffer verarbeiten.

**Quellen:**

* [Express.js – res.send()](https://expressjs.com/de/4x/api.html#res.send)


  **[⬆ Наверх](#top)**

36. ### <a name="36"></a> Unterschied zwischen res.json() und res.send()?

## Unterschied zwischen `res.json()` und `res.send()` in Express

**1. `res.json()`**

* Speziell für das Senden von JSON-Antworten gedacht.
* Wandelt ein JavaScript-Objekt oder Array automatisch in JSON um.
* Setzt den Header `Content-Type: application/json` immer korrekt.

```js
app.get('/user', (req, res) => {
  res.json({ name: 'Sergii', age: 30 });
});
```

Antwort:

```json
{
  "name": "Sergii",
  "age": 30
}
```

---

**2. `res.send()`**

* Allgemeiner, kann Strings, Buffer, Objekte oder Arrays senden.
* Wenn ein Objekt/Array übergeben wird, konvertiert Express es ebenfalls in JSON.
* Setzt `Content-Type` automatisch anhand des Datentyps:

  * String → `text/html` oder `text/plain`
  * Objekt/Array → `application/json`
  * Buffer → `application/octet-stream`

```js
app.get('/info', (req, res) => {
  res.send({ status: 'ok', version: '1.0' });
});
```

Antwort (ähnlich wie bei `res.json()`):

```json
{
  "status": "ok",
  "version": "1.0"
}
```

---

**3. Hauptunterschiede:**

* `res.json()` ist **explizit** für JSON → sicherer und klarer bei APIs.
* `res.send()` ist **flexibel** und erkennt den Datentyp selbst.
* Best Practice:

  * **API-Responses:** `res.json()`
  * **Einfache Texte/HTML/sonstiges:** `res.send()`

---

### Zusammenfassung

* `res.json()` → nur für JSON, setzt immer `application/json`.
* `res.send()` → flexibel, erkennt Typ automatisch (String, Buffer, Objekt, Array).
* Empfehlung: Bei **APIs** `res.json()`, bei **Textrückgaben/HTML** `res.send()`.

**Quellen:**

* [Express.js – res.json()](https://expressjs.com/de/4x/api.html#res.json)
* [Express.js – res.send()](https://expressjs.com/de/4x/api.html#res.send)


  **[⬆ Наверх](#top)**

37. ### <a name="37"></a> Wie setzt man einen HTTP-Statuscode?

## HTTP-Statuscode in Express setzen

**Definition:**
In Express wird der HTTP-Statuscode mit der Methode `res.status(code)` gesetzt. Anschließend kann man die Antwort mit `res.send()`, `res.json()` oder anderen Methoden abschicken.

---

**1. Statuscode mit `res.status()` setzen**

```js
app.get('/ok', (req, res) => {
  res.status(200).send('Alles in Ordnung');
});

app.get('/notfound', (req, res) => {
  res.status(404).send('Seite nicht gefunden');
});

app.get('/error', (req, res) => {
  res.status(500).json({ error: 'Interner Serverfehler' });
});
```

---

**2. Methoden-Ketten (Chaining)**

```js
app.post('/user', (req, res) => {
  res.status(201).json({ message: 'Benutzer erstellt' });
});
```

---

**3. Shortcut für häufige Fehler (optional)**
Manchmal wird `res.sendStatus(code)` genutzt:

```js
app.get('/unauthorized', (req, res) => {
  res.sendStatus(401); // setzt Status und sendet den Code als Text
});
```

→ Antwort: `401 Unauthorized`

---

### Zusammenfassung

* Mit `res.status(code)` den HTTP-Status setzen.
* Danach mit `res.send()` oder `res.json()` Antwort senden.
* Alternative: `res.sendStatus(code)` (setzt + sendet direkt).

**Quellen:**

* [Express.js – res.status()](https://expressjs.com/de/4x/api.html#res.status)
* [Express.js – res.sendStatus()](https://expressjs.com/de/4x/api.html#res.sendStatus)


  **[⬆ Наверх](#top)**

38. ### <a name="38"></a> Wie werden Cookies gesetzt und gelesen?

## Cookies in Express setzen und lesen

Express selbst hat keine eingebaute Cookie-Verwaltung. Man nutzt dafür meist die **Third-Party-Middleware `cookie-parser`**.

---

**1. Installation von `cookie-parser`**

```bash
npm install cookie-parser
```

---

**2. Setup in Express**

```js
import express from 'express';
import cookieParser from 'cookie-parser';

const app = express();
app.use(cookieParser()); // Middleware aktivieren
```

---

**3. Cookie setzen**

```js
app.get('/set-cookie', (req, res) => {
  res.cookie('username', 'Sergii', { maxAge: 60000, httpOnly: true });
  res.send('Cookie gesetzt');
});
```

* `username=Sergii` wird als Cookie im Browser gespeichert.
* `maxAge: 60000` → Ablaufzeit (1 Minute).
* `httpOnly: true` → Cookie ist nur für Server sichtbar, nicht für JavaScript im Browser.

---

**4. Cookies auslesen**

```js
app.get('/get-cookie', (req, res) => {
  const username = req.cookies.username; // Zugriff auf Cookies
  res.send(`Gespeicherter Benutzer: ${username}`);
});
```

---

**5. Cookie löschen**

```js
app.get('/clear-cookie', (req, res) => {
  res.clearCookie('username');
  res.send('Cookie gelöscht');
});
```

---

### Zusammenfassung

* Cookies in Express über `cookie-parser` verwalten.
* `res.cookie(name, value, options)` → Cookie setzen.
* `req.cookies` → Cookies lesen.
* `res.clearCookie(name)` → Cookie löschen.

**Quellen:**

* [cookie-parser – npm](https://www.npmjs.com/package/cookie-parser)
* [MDN – HTTP Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)


  **[⬆ Наверх](#top)**

39. ### <a name="39"></a> Unterschied zwischen synchronem und asynchronem Request-Handling?

## Unterschied zwischen synchronem und asynchronem Request-Handling in Express

**1. Synchrones Request-Handling**

* Die Route oder Middleware führt eine Aufgabe **direkt und vollständig** aus.
* Der Code blockiert nicht, da die Aufgabe sofort erledigt wird.
* Typisch für einfache Berechnungen oder Antworten.

```js
app.get('/sync', (req, res) => {
  const result = 2 + 2; // sofort verfügbar
  res.send(`Ergebnis: ${result}`);
});
```

→ Antwort erfolgt sofort, kein Warten auf externe Ressourcen.

---

**2. Asynchrones Request-Handling**

* Wird genutzt, wenn Aufgaben **Zeit benötigen** (z. B. Datenbank, externe API, Dateisystem).
* Express unterstützt asynchrone Funktionen (`Promise`, `async/await`).
* Die Route wartet auf die Aufgabe, blockiert aber nicht den gesamten Server.

```js
app.get('/async', async (req, res) => {
  const user = await getUserFromDB(); // simuliert DB-Abfrage
  res.json(user);
});

// Beispiel: Fake-Datenbankfunktion
function getUserFromDB() {
  return new Promise(resolve => {
    setTimeout(() => resolve({ id: 1, name: 'Sergii' }), 1000);
  });
}
```

→ Anfrage wird erst beantwortet, wenn die Datenbank-Antwort da ist.

---

**3. Vergleich**

* **Synchron:** Direkt berechenbar, kein Warten → schnell, aber nur für einfache Logik sinnvoll.
* **Asynchron:** Notwendig bei externen Operationen (DB, API, Filesystem). Verhindert, dass der Server blockiert.

---

### Zusammenfassung

* **Synchron:** sofortige Antwort, kein Warten (geeignet für einfache Logik).
* **Asynchron:** arbeitet mit `Promises`/`async/await`, wichtig für externe Ressourcen.
* Vorteil: Node.js kann mehrere Requests parallel abarbeiten, ohne blockiert zu werden.

**Quellen:**

* [Express.js – Routing (mit async)](https://expressjs.com/de/guide/routing.html)
* [MDN – async/await](https://developer.mozilla.org/ru/docs/Learn/JavaScript/Asynchronous/Promises)


  **[⬆ Наверх](#top)**

40. ### <a name="40"></a> Wie behandelt man Datei-Uploads in Express?

## Datei-Uploads in Express behandeln

Express selbst hat keine eingebaute Unterstützung für Datei-Uploads. Dafür wird häufig die **Third-Party-Middleware [`multer`](https://www.npmjs.com/package/multer)** verwendet.

---

**1. Installation von Multer**

```bash
npm install multer
```

---

**2. Setup in Express**

```js
import express from 'express';
import multer from 'multer';

const app = express();

// Speicherort und Dateinamen festlegen
const upload = multer({ dest: 'uploads/' });
```

---

**3. Einzelne Datei hochladen**

```js
app.post('/upload', upload.single('file'), (req, res) => {
  console.log(req.file);  // Informationen zur hochgeladenen Datei
  res.send(`Datei ${req.file.originalname} hochgeladen`);
});
```

* `upload.single('file')` → erwartet ein Feld mit dem Namen `file`.
* Datei wird automatisch im Ordner `uploads/` gespeichert.

---

**4. Mehrere Dateien hochladen**

```js
app.post('/uploads', upload.array('files', 5), (req, res) => {
  console.log(req.files); // Array mit Dateien
  res.send(`${req.files.length} Dateien hochgeladen`);
});
```

* `upload.array('files', 5)` → maximal 5 Dateien erlaubt.

---

**5. Kombination aus Feldern und Dateien**

```js
app.post('/profile', upload.fields([
  { name: 'avatar', maxCount: 1 },
  { name: 'gallery', maxCount: 5 }
]), (req, res) => {
  console.log(req.files); // avatar + gallery
  console.log(req.body);  // zusätzliche Formulardaten
  res.send('Profil gespeichert');
});
```

---

### Zusammenfassung

* Datei-Uploads in Express mit **Multer**.
* `upload.single()` → eine Datei.
* `upload.array()` → mehrere Dateien.
* `upload.fields()` → Kombination von Feldern + Dateien.
* Standardmäßig werden Dateien lokal gespeichert, man kann aber auch **Cloud-Speicher** (AWS S3, Cloudinary) konfigurieren.

**Quellen:**

* [Multer – npm](https://www.npmjs.com/package/multer)
* [Express.js – Working with forms](https://expressjs.com/en/resources/middleware/multer.html)


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

201. ### <a name="201"></a> 



  **[⬆ Наверх](#top)**      

202. ### <a name="202"></a> 



  **[⬆ Наверх](#top)**      

203. ### <a name="203"></a> 



  **[⬆ Наверх](#top)**      

204. ### <a name="204"></a> 



  **[⬆ Наверх](#top)**      

205. ### <a name="205"></a> 



  **[⬆ Наверх](#top)**      

206. ### <a name="206"></a> 



  **[⬆ Наверх](#top)**      

207. ### <a name="207"></a> 



  **[⬆ Наверх](#top)**      

208. ### <a name="208"></a> 



  **[⬆ Наверх](#top)**      

209. ### <a name="209"></a> 



  **[⬆ Наверх](#top)**      

210. ### <a name="210"></a> 



  **[⬆ Наверх](#top)**      

211. ### <a name="211"></a> 



  **[⬆ Наверх](#top)**      

212. ### <a name="212"></a> 



  **[⬆ Наверх](#top)**      

213. ### <a name="213"></a> 



  **[⬆ Наверх](#top)**      

214. ### <a name="214"></a> 



  **[⬆ Наверх](#top)**      

215. ### <a name="215"></a> 



  **[⬆ Наверх](#top)**      

216. ### <a name="216"></a> 



  **[⬆ Наверх](#top)**      

217. ### <a name="217"></a> 



  **[⬆ Наверх](#top)**      

218. ### <a name="218"></a> 



  **[⬆ Наверх](#top)**      

219. ### <a name="219"></a> 



  **[⬆ Наверх](#top)**      

220. ### <a name="220"></a> 



  **[⬆ Наверх](#top)**      

221. ### <a name="221"></a> 



  **[⬆ Наверх](#top)**      

222. ### <a name="222"></a> 



  **[⬆ Наверх](#top)**      

223. ### <a name="223"></a> 



  **[⬆ Наверх](#top)**      

224. ### <a name="224"></a> 



  **[⬆ Наверх](#top)**      

225. ### <a name="225"></a> 



  **[⬆ Наверх](#top)**      

226. ### <a name="226"></a> 



  **[⬆ Наверх](#top)**      

227. ### <a name="227"></a> 



  **[⬆ Наверх](#top)**      

228. ### <a name="228"></a> 



  **[⬆ Наверх](#top)**      

229. ### <a name="229"></a> 



  **[⬆ Наверх](#top)**      

230. ### <a name="230"></a>


  **[⬆ Наверх](#top)**      

231. ### <a name="231"></a> 



  **[⬆ Наверх](#top)**      

232. ### <a name="232"></a> 



  **[⬆ Наверх](#top)**      

233. ### <a name="233"></a> 



  **[⬆ Наверх](#top)**      

234. ### <a name="234"></a> 



  **[⬆ Наверх](#top)**      

235. ### <a name="235"></a> 



  **[⬆ Наверх](#top)**      

236. ### <a name="236"></a> 



  **[⬆ Наверх](#top)**      

237. ### <a name="237"></a> 



  **[⬆ Наверх](#top)**      

238. ### <a name="238"></a> 



  **[⬆ Наверх](#top)**      

239. ### <a name="239"></a> 



  **[⬆ Наверх](#top)**      

240. ### <a name="240"></a>


  **[⬆ Наверх](#top)**      

241. ### <a name="241"></a> 



  **[⬆ Наверх](#top)**      

242. ### <a name="242"></a> 



  **[⬆ Наверх](#top)**      

243. ### <a name="243"></a> 



  **[⬆ Наверх](#top)**      

244. ### <a name="244"></a> 



  **[⬆ Наверх](#top)**      

245. ### <a name="245"></a> 



  **[⬆ Наверх](#top)**      

246. ### <a name="246"></a> 



  **[⬆ Наверх](#top)**      

247. ### <a name="247"></a> 



  **[⬆ Наверх](#top)**      

248. ### <a name="248"></a> 



  **[⬆ Наверх](#top)**      

249. ### <a name="249"></a> 



  **[⬆ Наверх](#top)**      

250. ### <a name="250"></a>


  **[⬆ Наверх](#top)**     
