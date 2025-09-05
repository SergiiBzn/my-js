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

41. ### <a name="41"></a> Wie implementiert man Error-Handling in Express?

## Error-Handling in Express – zentral und korrekt

Grundprinzipien

* Fehler-Middleware hat **vier Parameter**: `(err, req, res, next)`.
* Reihenfolge: **Routen → 404-Handler → Error-Handler (ganz am Ende)**.
* Fehler weiterreichen mit `next(err)` oder in `async`-Routen per `try/catch`.

Zentrale Error-Handling-Middleware

```js
import express from 'express';
const app = express();

app.use(express.json());

// Beispielroute mit bewusstem Fehler
app.get('/boom', (req, res, next) => {
  const err = new Error('Boom!');
  err.status = 400; // optional: eigener Status
  next(err);
});

// 404 – muss vor dem Error-Handler stehen
app.use((req, res, next) => {
  res.status(404).json({ error: 'Route nicht gefunden' });
});

// Globaler Error-Handler (immer zuletzt)
app.use((err, req, res, next) => {
  const status = err.status || err.statusCode || 500;
  // Beispiel: keine Stacktraces in Produktion ausgeben
  const payload = {
    error: err.message || 'Interner Serverfehler',
    ...(process.env.NODE_ENV !== 'production' && { stack: err.stack })
  };
  res.status(status).json(payload);
});

app.listen(3000, () => console.log('Server läuft auf 3000'));
```

Async/await: Fehler abfangen

```js
// Variante A: try/catch in async-Routen
app.get('/user/:id', async (req, res, next) => {
  try {
    const user = await loadUser(req.params.id); // z. B. DB-Call
    if (!user) {
      const err = new Error('User nicht gefunden');
      err.status = 404;
      throw err;
    }
    res.json(user);
  } catch (err) {
    next(err); // an zentralen Handler weitergeben
  }
});

// Variante B: Wrapper-Helfer, um try/catch zu sparen
const asyncHandler = (fn) => (req, res, next) => Promise.resolve(fn(req, res, next)).catch(next);

app.get('/orders', asyncHandler(async (req, res) => {
  const orders = await loadOrders();
  res.json(orders);
}));
```

Validierungsfehler konsistent behandeln (Beispiel)

```js
function validateBody(schema) {
  return (req, res, next) => {
    const { error, value } = schema.validate(req.body, { abortEarly: false });
    if (error) {
      const err = new Error('Validierungsfehler');
      err.status = 422; // Unprocessable Entity
      err.details = error.details;
      return next(err);
    }
    req.body = value;
    next();
  };
}
```

Best Practices

* **Eine** zentrale Fehler-Middleware, überall `next(err)` nutzen.
* Konsistente Statuscodes (400/401/403/404/409/422/500).
* Keine sensiblen Infos/Stacktraces in Produktion.
* 404-Handler **vor** dem Error-Handler platzieren.
* Für `async`-Routen Wrapper wie `asyncHandler` verwenden.

Zusammenfassung

* Fehler laufen über eine **zentrale Error-Middleware** `(err, req, res, next)`.
* `next(err)` bzw. `asyncHandler` sorgt für sauberes Weiterreichen.
* 404-Handler vor dem globalen Error-Handler, konsistente Statuscodes + sichere Fehlermeldungen.

Quellen

* Express.js – Fehlerbehandlung: [https://expressjs.com/de/guide/error-handling.html](https://expressjs.com/de/guide/error-handling.html)
* Express.js – API (`res.status`, `app.use`): [https://expressjs.com/de/4x/api.html](https://expressjs.com/de/4x/api.html)
* MDN – HTTP-Statuscodes: [https://developer.mozilla.org/ru/docs/Web/HTTP/Status](https://developer.mozilla.org/ru/docs/Web/HTTP/Status)

  **[⬆ Наверх](#top)**

42. ### <a name="42"></a> Warum braucht man spezielle Error-Middleware?

## Warum braucht man spezielle Error-Middleware in Express?

**1. Unterschied zur normalen Middleware**

* Normale Middleware hat die Signatur `(req, res, next)`.
* Fehler-Middleware hat **vier Parameter** `(err, req, res, next)`.
* Express erkennt nur an dieser Signatur, dass es sich um einen Fehler-Handler handelt.

---

**2. Zweck von Error-Middleware**

* Einheitliche Behandlung von Fehlern (statt in jeder Route manuell).
* Verhindert, dass Requests ohne Antwort hängen bleiben.
* Ermöglicht Logging und Monitoring von Fehlern an einer zentralen Stelle.
* Ermöglicht sichere Antworten für Clients (z. B. keine internen Stacktraces in Produktion).

---

**3. Beispiel**

```js
import express from 'express';
const app = express();

app.get('/fail', (req, res, next) => {
  const err = new Error('Etwas ist schiefgelaufen');
  err.status = 400;
  next(err); // Fehler weiterleiten
});

// Spezielle Error-Middleware (4 Parameter!)
app.use((err, req, res, next) => {
  console.error(err.message); // Logging
  res.status(err.status || 500).json({ error: err.message });
});

app.listen(3000, () => console.log('Server läuft'));
```

---

**4. Warum nicht nur try/catch in jeder Route?**

* Würde zu viel **doppeltem Code** führen.
* Fehler könnten vergessen werden → Gefahr von offenen Requests.
* Mit zentraler Error-Middleware: **einheitliche Struktur + weniger Code**.

---

### Zusammenfassung

* Spezielle Error-Middleware (`(err, req, res, next)`) ist notwendig, weil Express nur so Fehler erkennt.
* Sie sorgt für einheitliches Fehler-Handling, Logging und saubere Antworten.
* Best Practice: **eine zentrale Error-Middleware am Ende** aller Middleware und Routen.

**Quellen:**

* [Express.js – Error Handling](https://expressjs.com/de/guide/error-handling.html)

---

  **[⬆ Наверх](#top)**

43. ### <a name="43"></a> Unterschied zwischen synchronem und asynchronem Fehlerhandling?

## Unterschied zwischen synchronem und asynchronem Fehlerhandling in Express

**1. Synchrones Fehlerhandling**

* Tritt ein Fehler direkt im Code der Route oder Middleware auf.
* Lösung: `throw` oder `next(err)` aufrufen.
* Express fängt den Fehler automatisch ab und leitet ihn an die Error-Middleware weiter.

```js
app.get('/sync', (req, res, next) => {
  try {
    throw new Error('Synchroner Fehler');
  } catch (err) {
    next(err); // an Error-Middleware weitergeben
  }
});
```

---

**2. Asynchrones Fehlerhandling (z. B. Promises, async/await)**

* Fehler treten zeitversetzt auf (DB-Abfragen, externe APIs, Filesystem).
* Express fängt diese Fehler **nicht automatisch** ab.
* Man muss sie entweder in `try/catch` behandeln oder `next(err)` nutzen.

```js
// Mit async/await und try/catch
app.get('/async', async (req, res, next) => {
  try {
    const user = await getUserFromDB(); // wirft evtl. Fehler
    res.json(user);
  } catch (err) {
    next(err); // Fehler weiterreichen
  }
});
```

Alternative: **Wrapper-Helfer**, um try/catch zu sparen:

```js
const asyncHandler = (fn) => (req, res, next) =>
  Promise.resolve(fn(req, res, next)).catch(next);

app.get('/wrapped', asyncHandler(async (req, res) => {
  const orders = await getOrders(); // Fehler → automatisch an next(err)
  res.json(orders);
}));
```

---

**3. Vergleich**

* **Synchron:** Fehler können mit `throw` oder `next(err)` abgefangen werden.
* **Asynchron:** Fehler müssen in `try/catch` oder mit `catch(next)` weitergeleitet werden, sonst stürzt die App ab oder der Request hängt.

---

### Zusammenfassung

* **Synchron:** `throw` oder `next(err)` reicht.
* **Asynchron:** Fehler manuell mit `try/catch` oder Wrapper an Error-Middleware weiterleiten.
* Best Practice: `asyncHandler` oder ähnliche Wrapper nutzen, um Code sauber zu halten.

**Quellen:**

* [Express.js – Fehlerbehandlung](https://expressjs.com/de/guide/error-handling.html)
* [MDN – async/await Fehler](https://developer.mozilla.org/ru/docs/Learn/JavaScript/Asynchronous/Promises#обработка_ошибок)

---

  **[⬆ Наверх](#top)**

44. ### <a name="44"></a> Wie gibt man unterschiedliche Statuscodes im Fehlerfall zurück?

## Unterschiedliche Statuscodes im Fehlerfall zurückgeben in Express

**Grundidee:**

* Fehlerobjekte können mit einem **eigenen Statuscode** versehen werden (`err.status` oder `err.statusCode`).
* Die zentrale Error-Middleware liest diesen Wert aus und gibt den passenden HTTP-Status zurück.

---

**1. Beispiel mit synchronem Fehler**

```js
import express from 'express';
const app = express();

app.get('/bad-request', (req, res, next) => {
  const err = new Error('Ungültige Anfrage');
  err.status = 400; // Bad Request
  next(err);
});
```

---

**2. Beispiel mit asynchronem Fehler (z. B. DB-Abfrage)**

```js
app.get('/user/:id', async (req, res, next) => {
  try {
    const user = null; // simuliert: User nicht gefunden
    if (!user) {
      const err = new Error('User nicht gefunden');
      err.status = 404;
      throw err;
    }
    res.json(user);
  } catch (err) {
    next(err); // an Error-Middleware weiterreichen
  }
});
```

---

**3. Zentrale Error-Middleware für unterschiedliche Statuscodes**

```js
app.use((err, req, res, next) => {
  const status = err.status || 500;
  res.status(status).json({
    error: err.message || 'Interner Serverfehler'
  });
});
```

---

**4. Typische Statuscodes im Fehlerfall**

* **400 Bad Request** → ungültige Eingaben (Validation Errors)
* **401 Unauthorized** → Benutzer nicht authentifiziert
* **403 Forbidden** → keine Berechtigung
* **404 Not Found** → Ressource nicht gefunden
* **409 Conflict** → Konflikt (z. B. Duplikat)
* **422 Unprocessable Entity** → Validierungsfehler bei korrektem Request-Format
* **500 Internal Server Error** → allgemeiner Serverfehler

---

### Zusammenfassung

* Statuscodes werden im Fehlerobjekt (`err.status`) gesetzt.
* Die zentrale Error-Middleware verwendet diesen Code (`res.status(err.status || 500)`).
* Damit können unterschiedliche Fehlerarten (400, 401, 403, 404, 500 …) konsistent abgebildet werden.

**Quellen:**

* [Express.js – Fehlerbehandlung](https://expressjs.com/de/guide/error-handling.html)
* [MDN – HTTP Statuscodes](https://developer.mozilla.org/ru/docs/Web/HTTP/Status)

---

  **[⬆ Наверх](#top)**

45. ### <a name="45"></a> Wie verhindert man, dass nicht abgefangene Fehler den Server crashen?

## Wie verhindert man, dass nicht abgefangene Fehler den Server crashen?

**Problem:**
In Node.js führen **nicht abgefangene Fehler** (`uncaughtException`, `unhandledRejection`) oft dazu, dass der Prozess abstürzt. Das ist gefährlich für Produktionssysteme.

---

**1. Zentrales Error-Handling in Express**

* Fehler mit `next(err)` weitergeben.
* Am Ende eine **globale Error-Middleware** definieren:

```js
import express from 'express';
const app = express();

app.get('/fail', (req, res, next) => {
  try {
    throw new Error('Boom!');
  } catch (err) {
    next(err); // an Error-Middleware weiterreichen
  }
});

app.use((err, req, res, next) => {
  console.error('Fehler:', err.message);
  res.status(err.status || 500).json({ error: 'Interner Serverfehler' });
});

app.listen(3000, () => console.log('Server läuft'));
```

---

**2. Asynchrone Fehler abfangen**

* In `async`-Routen mit `try/catch` arbeiten oder einen **Wrapper** nutzen:

```js
const asyncHandler = (fn) => (req, res, next) =>
  Promise.resolve(fn(req, res, next)).catch(next);

app.get('/async', asyncHandler(async (req, res) => {
  throw new Error('Async-Fehler'); // wird an Error-Middleware weitergegeben
}));
```

---

**3. Prozessweite Fehler abfangen (Sicherheitsnetz)**

* Für wirklich unerwartete Fehler kann man Listener auf Prozessebene registrieren:

```js
process.on('uncaughtException', (err) => {
  console.error('Uncaught Exception:', err);
  // Hier besser: Logging + kontrolliertes Beenden mit Neustart durch PM2/Docker
});

process.on('unhandledRejection', (reason, promise) => {
  console.error('Unhandled Rejection:', reason);
});
```

👉 Achtung: Diese sollten nur als **letzte Absicherung** dienen – Best Practice ist, Fehler sauber mit `next(err)` an Middleware weiterzugeben.

---

**4. Produktions-Setup (Best Practices)**

* **PM2, Docker oder systemd** verwenden, um Node.js-Prozesse automatisch neu zu starten, falls sie doch abstürzen.
* Logging (z. B. mit `winston`, `pino`) nutzen, um Fehler zu protokollieren.

---

### Zusammenfassung

* Nicht abgefangene Fehler verhindern durch:

  * zentrale Error-Middleware in Express,
  * sauberes Handling von async-Fehlern (`try/catch`, Wrapper),
  * Prozess-Events (`uncaughtException`, `unhandledRejection`) nur als Fallback.
* In Produktion Prozessmanager wie **PM2/Docker** einsetzen.

**Quellen:**

* [Express.js – Fehlerbehandlung](https://expressjs.com/de/guide/error-handling.html)
* [Node.js – Prozess-Events](https://nodejs.org/docs/latest/api/process.html)

---

  **[⬆ Наверх](#top)**

46. ### <a name="46"></a> Wie schützt man Express-Anwendungen vor XSS?

## Schutz vor XSS (Cross-Site Scripting) in Express

**Maßnahmen-Überblick**

* **Content Security Policy (CSP)** setzen → verhindert Inline-Skripte und fremde Skriptquellen.
* **Output Encoding/Escaping** im Template-Engine verwenden (keine ungeprüften Werte ins HTML injizieren).
* **Eingaben validieren & ggf. säubern** (Whitelist, Schema-Validierung, serverseitiges Sanitizing nur gezielt).
* **Sichere Cookies** verwenden (`httpOnly`, `secure`, `sameSite`) → erschwert Session-Diebstahl.
* **Kein Inline-JS** und keine gefährlichen DOM-APIs (Client) wie `innerHTML` ohne Sanitizing.
* **Security-Header** mit `helmet` setzen (CSP, weitere Header).

**CSP mit Helmet**

```js
import express from 'express';
import helmet from 'helmet';

const app = express();

// strikte, aber praxistaugliche CSP (ohne inline Skripte)
app.use(
  helmet.contentSecurityPolicy({
    useDefaults: true,
    directives: {
      "default-src": ["'self'"],
      "script-src": ["'self'"],            // kein 'unsafe-inline', kein 'unsafe-eval'
      "style-src": ["'self'", "https:"],   // falls nötig: "'unsafe-inline'" vermeiden
      "img-src": ["'self'", "data:", "https:"],
      "object-src": ["'none'"],
      "base-uri": ["'self'"],
      "frame-ancestors": ["'self'"]
    }
  })
);

// weitere sinnvolle Header
app.use(helmet.referrerPolicy({ policy: 'no-referrer' }));
app.use(helmet.xssFilter?.()); // Hinweis: x-xss-protection ist in modernen Browsern obsolet
```

**Sichere Antwort- und Cookie-Settings**

```js
import cookieParser from 'cookie-parser';

app.use(cookieParser());

// JSON statt HTML, wenn möglich (vermeidet HTML-Einbettung)
app.get('/data', (req, res) => {
  res.json({ safe: true }); // res.json() setzt Content-Type korrekt
});

// Cookies schützen
app.get('/login', (req, res) => {
  res.cookie('session', 'token', {
    httpOnly: true,   // nicht per JS auslesbar
    secure: true,     // nur HTTPS
    sameSite: 'lax'   // reduziert CSRF-Risiko
  });
  res.send('ok');
});
```

**Validierung & Sanitizing (gezielt)**

```js
// Beispiel: Schema-Validierung (z. B. mit joi/zod)
// Danach: serverseitig nur in TEXTKONTEXT ausgeben oder escapen.
// Für seltene Fälle HTML-Sanitizing, z. B. sanitize-html oder DOMPurify (Server-Variante).
```

**Template-Engines**

* Engines mit **Auto-Escaping** nutzen (z. B. Pug standardmäßig; bei EJS `<%= %>` escapt, **nicht** `<%- %>`).
* Niemals ungeprüfte Eingaben als **unescaped/RAW** einfügen.

**Clientseitige Grundsätze (ergänzend)**

* Statt `element.innerHTML = userInput` → `textContent` verwenden.
* Falls HTML erforderlich: vorher **sanitizen**.

### Zusammenfassung

* Primärschutz: **CSP** + **konsequentes Escaping** im View.
* **Helmet** für Security-Header einsetzen.
* **Validierung/Sanitizing** nur gezielt, kein Blind-“Strippen”.
* **Sichere Cookies** konfigurieren; Inline-JS vermeiden.

**Quellen**

* Express (Helmet/Best Practices): [https://expressjs.com/de/advanced/best-practice-security.html](https://expressjs.com/de/advanced/best-practice-security.html)
* MDN – XSS Übersicht: [https://developer.mozilla.org/ru/docs/Glossary/Cross-site\_scripting](https://developer.mozilla.org/ru/docs/Glossary/Cross-site_scripting)
* MDN – Content Security Policy (CSP): [https://developer.mozilla.org/ru/docs/Web/HTTP/CSP](https://developer.mozilla.org/ru/docs/Web/HTTP/CSP)


  **[⬆ Наверх](#top)**

47. ### <a name="47"></a> Welche Middleware nutzt man für Security (z. B. Helmet)?

## Security-Middleware in Express (z. B. Helmet)

**1. Helmet**

* Setzt verschiedene HTTP-Header, um Angriffe wie **XSS**, **Clickjacking**, **MIME sniffing** zu erschweren.
* Enthält mehrere Module (z. B. `contentSecurityPolicy`, `xssFilter`, `frameguard`).

```js
import express from 'express';
import helmet from 'helmet';

const app = express();

// Standard-Sicherheits-Header
app.use(helmet());

// Beispiel: CSP aktivieren
app.use(
  helmet.contentSecurityPolicy({
    useDefaults: true,
    directives: {
      "default-src": ["'self'"],
      "script-src": ["'self'"]
    }
  })
);

app.get('/', (req, res) => res.send('Sicher mit Helmet!'));
app.listen(3000);
```

---

**2. cors**

* Erlaubt kontrollierten Zugriff von anderen Domains (Cross-Origin Resource Sharing).
* Wichtig für APIs, die von einem Frontend (z. B. React) konsumiert werden.

```js
import cors from 'cors';
app.use(cors({ origin: 'http://localhost:5173' })); // nur bestimmte Domain erlauben
```

---

**3. express-rate-limit**

* Schützt vor **Brute-Force-Angriffen** durch Begrenzung der Requests pro IP.

```js
import rateLimit from 'express-rate-limit';

const limiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 Minuten
  max: 100                  // max. 100 Anfragen pro IP
});

app.use(limiter);
```

---

**4. express-mongo-sanitize** (für MongoDB-Projekte)

* Entfernt gefährliche Zeichen aus Requests, die für **NoSQL-Injection** genutzt werden könnten.

```js
import mongoSanitize from 'express-mongo-sanitize';
app.use(mongoSanitize());
```

---

**5. xss-clean** (optional, für JSON-Bodies)

* Entfernt potenziell gefährliche XSS-Skripte aus Eingaben.

```js
import xss from 'xss-clean';
app.use(xss());
```

---

### Zusammenfassung

Wichtige Security-Middleware für Express:

* **helmet** → Security-Header (Grundschutz)
* **cors** → kontrollierter Cross-Origin-Zugriff
* **express-rate-limit** → Schutz vor Brute-Force
* **express-mongo-sanitize / xss-clean** → Eingabe-Sanitizing

**Quellen:**

* [Helmet – npm](https://www.npmjs.com/package/helmet)
* [CORS – npm](https://www.npmjs.com/package/cors)
* [express-rate-limit – npm](https://www.npmjs.com/package/express-rate-limit)

---

  **[⬆ Наверх](#top)**

48. ### <a name="48"></a> Was ist CORS und wie aktiviert man es in Express?

## Was ist CORS und wie aktiviert man es in Express?

**Definition:**
CORS (*Cross-Origin Resource Sharing*) ist ein Sicherheitsmechanismus im Browser.

* Standardmäßig blockieren Browser Anfragen von einer anderen Domain/Port (z. B. React-Frontend auf `http://localhost:5173` → Express-API auf `http://localhost:3000`).
* Mit CORS kann der Server explizit erlauben, welche Domains, Methoden und Header Zugriff haben dürfen.

---

**1. CORS in Express aktivieren (mit Middleware `cors`)**

```bash
npm install cors
```

```js
import express from 'express';
import cors from 'cors';

const app = express();

// Standardmäßig: alle Domains erlauben (nicht empfohlen für Produktion)
app.use(cors());

app.get('/data', (req, res) => {
  res.json({ msg: 'CORS aktiviert' });
});

app.listen(3000);
```

---

**2. Zugriff nur für bestimmte Domains erlauben**

```js
app.use(cors({ origin: 'http://localhost:5173' }));
```

→ Nur Requests vom React-Frontend `http://localhost:5173` sind erlaubt.

---

**3. Mehrere Optionen konfigurieren**

```js
app.use(cors({
  origin: ['http://localhost:5173', 'https://meine-app.de'],
  methods: ['GET', 'POST', 'PUT', 'DELETE'],
  allowedHeaders: ['Content-Type', 'Authorization'],
  credentials: true // Cookies/Authorization-Header zulassen
}));
```

---

**4. CORS nur für bestimmte Routen aktivieren**

```js
app.get('/public', cors(), (req, res) => {
  res.send('Öffentliche Route mit CORS');
});
```

---

### Zusammenfassung

* **CORS = Cross-Origin Resource Sharing**, notwendig für Frontend-Backend-Kommunikation.
* In Express über `cors`-Middleware aktivierbar.
* Konfiguration möglich: erlaubte Domains, Methoden, Header, Cookies.

**Quellen:**

* [CORS – npm](https://www.npmjs.com/package/cors)
* [MDN – Cross-Origin Resource Sharing](https://developer.mozilla.org/ru/docs/Web/HTTP/CORS)

---

  **[⬆ Наверх](#top)**

49. ### <a name="49"></a> Wie funktioniert Rate-Limiting in Express?

## Wie funktioniert Rate-Limiting in Express?

**Definition:**
Rate-Limiting begrenzt die Anzahl von Anfragen, die ein Client (z. B. pro IP) in einem bestimmten Zeitfenster an den Server senden darf.

* Schützt vor **Brute-Force-Angriffen** (z. B. Login-Versuche).
* Verhindert **Denial-of-Service (DoS)** durch zu viele Requests.

---

**1. Installation von `express-rate-limit`**

```bash
npm install express-rate-limit
```

---

**2. Einfaches Setup**

```js
import express from 'express';
import rateLimit from 'express-rate-limit';

const app = express();

// Limiter: max. 100 Anfragen pro 15 Minuten pro IP
const limiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 Minuten
  max: 100,                 // 100 Anfragen
  message: 'Zu viele Anfragen – bitte später erneut versuchen'
});

// Global anwenden
app.use(limiter);

app.get('/', (req, res) => {
  res.send('Willkommen! Rate-Limiting aktiv.');
});

app.listen(3000);
```

---

**3. Nur für bestimmte Routen anwenden**

```js
// Strengeres Limit nur für /login
const loginLimiter = rateLimit({
  windowMs: 60 * 1000, // 1 Minute
  max: 5,              // max. 5 Versuche pro Minute
  message: 'Zu viele Login-Versuche, bitte warte eine Minute'
});

app.post('/login', loginLimiter, (req, res) => {
  res.send('Login-Route mit Rate-Limit');
});
```

---

**4. Erweiterte Optionen**

* `keyGenerator`: definiert, wie der Client identifiziert wird (standard: IP).
* `skip`: bestimmte Anfragen ignorieren (z. B. interne Dienste).
* `handler`: eigene Antwortlogik für blockierte Requests.

```js
const apiLimiter = rateLimit({
  windowMs: 10 * 60 * 1000,
  max: 50,
  keyGenerator: (req, res) => req.ip, // Standard
  handler: (req, res) => {
    res.status(429).json({ error: 'Limit überschritten' });
  }
});

app.use('/api/', apiLimiter);
```

---

### Zusammenfassung

* Rate-Limiting in Express mit `express-rate-limit`.
* Begrenzung von Requests pro IP in einem Zeitfenster.
* Schützt vor Brute-Force und DoS.
* Kann global oder für bestimmte Routen eingesetzt werden.

**Quellen:**

* [express-rate-limit – npm](https://www.npmjs.com/package/express-rate-limit)
* [MDN – HTTP 429 Too Many Requests](https://developer.mozilla.org/ru/docs/Web/HTTP/Status/429)

---

  **[⬆ Наверх](#top)**

50. ### <a name="50"></a> Wie speichert man Passwörter sicher in Kombination mit Express?

## Sichere Passwortspeicherung mit Express (Best Practices)

Grundsätze

* Niemals Klartext-Passwörter speichern.
* Einen starken, bewährten **Passworthashing-Algorithmus** nutzen: **Argon2id** (empfohlen) oder **bcrypt**.
* **Salt** ist obligatorisch (bei Argon2/bcrypt integriert); optional zusätzlicher **Pepper** (geheimer Server-Key in `process.env`).
* Sichere Transportebene (HTTPS), Rate-Limiting auf Login, und timing-sichere Vergleiche.

### Variante A – mit **Argon2id**

```bash
npm i argon2
```

```js
// hashing.js
import argon2 from 'argon2';

const opts = {
  type: argon2.argon2id,
  memoryCost: 2 ** 16, // ~64 MB
  timeCost: 3,
  parallelism: 1
};

export async function hashPassword(plain, pepper = '') {
  return argon2.hash(plain + pepper, opts);
}

export async function verifyPassword(hash, plain, pepper = '') {
  return argon2.verify(hash, plain + pepper);
}
```

### Variante B – mit **bcrypt**

```bash
npm i bcrypt
```

```js
// hashing-bcrypt.js
import bcrypt from 'bcrypt';

const ROUNDS = Number(process.env.BCRYPT_ROUNDS ?? 12);

export async function hashPasswordBcrypt(plain, pepper = '') {
  const salt = await bcrypt.genSalt(ROUNDS);
  return bcrypt.hash(plain + pepper, salt);
}

export async function verifyPasswordBcrypt(hash, plain, pepper = '') {
  return bcrypt.compare(plain + pepper, hash); // timing-safe intern
}
```

### Express-Integration (Registrierung/Anmeldung)

```js
// auth.routes.js
import express from 'express';
import { hashPassword, verifyPassword } from './hashing.js'; // Argon2
import { z } from 'zod'; // optional für Validierung
import { User } from './models.js'; // Sequelize-Modell
const router = express.Router();

const PEPPER = process.env.PWD_PEPPER ?? '';
const schema = z.object({
  email: z.string().email(),
  password: z.string().min(8) // Richtlinie: min 8–12, Komplexität projektabhängig
});

router.post('/register', express.json(), async (req, res, next) => {
  try {
    const { email, password } = schema.parse(req.body);
    const passwordHash = await hashPassword(password, PEPPER);
    const user = await User.create({ email, passwordHash });
    res.status(201).json({ id: user.id, email: user.email });
  } catch (err) {
    // 409 falls E-Mail bereits existiert
    err.status ??= 400;
    next(err);
  }
});

router.post('/login', express.json(), async (req, res, next) => {
  try {
    const { email, password } = schema.pick({ email: true, password: true }).parse(req.body);
    const user = await User.findOne({ where: { email } });
    if (!user) return res.status(401).json({ error: 'Ungültige Anmeldedaten' });

    const ok = await verifyPassword(user.passwordHash, password, PEPPER);
    if (!ok) return res.status(401).json({ error: 'Ungültige Anmeldedaten' });

    // Session/JWT ausstellen …
    res.json({ message: 'Login ok' });
  } catch (err) {
    err.status ??= 400;
    next(err);
  }
});

export default router;
```

### Sequelize: Passwort-Hash im Modell/Hook

```js
// models.js
import { Sequelize, DataTypes, Model } from 'sequelize';
import { hashPassword } from './hashing.js';

const sequelize = new Sequelize(process.env.DATABASE_URL, {
  dialect: 'postgres',
  logging: false
});

export class User extends Model {}

User.init({
  email: { type: DataTypes.STRING, unique: true, allowNull: false },
  passwordHash: { type: DataTypes.STRING, allowNull: false }
}, { sequelize, modelName: 'User' });

// Optional: Hash bei create/update, wenn ein Plain-Field vorhanden wäre
// Hier: wir erwarten bereits passwordHash im create()-Call.
// Beispiel für ein virtuelles Feld "password":
User.addHook('beforeCreate', async (user) => {
  if (user.password) {
    const pepper = process.env.PWD_PEPPER ?? '';
    user.passwordHash = await hashPassword(user.password, pepper);
  }
});
```

### Zusätzliche Schutzmaßnahmen

* **Transport**: nur über **HTTPS** (secure Cookies, `secure: true`).
* **Rate-Limiting** auf `/login` (z. B. `express-rate-limit`).
* **Lockout/Backoff** nach X Fehlversuchen.
* **Session/JWT** sicher konfigurieren (Cookies: `httpOnly`, `sameSite`, `secure`).
* **Kein Passwort-„Reset“ per Klartext** senden; stattdessen **Token-basierte** Reset-Links.
* **Rotation/Parameter-Tuning**: Work-Factor (bcrypt rounds / Argon2 timeCost) projektabhängig an Hardware anpassen.
* **Kein eigenes Kryptodesign**; nur etablierte libs einsetzen.

### Zusammenfassung

* Passwörter nie im Klartext speichern; **Argon2id** oder **bcrypt** verwenden.
* Hashing in zentralen Helfern/Hooks kapseln; optional **Pepper** aus `process.env`.
* Express-Routen: Validierung, Hash bei Registrierung, Verify bei Login.
* Ergänzen durch HTTPS, Rate-Limiting, sichere Cookies, sauberes Reset-Verfahren.

Quellen

* Node.js (process/env, Security Best Practices): [https://nodejs.org/docs](https://nodejs.org/docs)
* Express – Security/Best Practices (Helmet, allgemeine Richtlinien): [https://expressjs.com/de/advanced/best-practice-security.html](https://expressjs.com/de/advanced/best-practice-security.html)
* Sequelize – Hooks/Modelle: [https://sequelize.org/](https://sequelize.org/)
* MDN – HTTPS/Passwörter/Hashing-Grundlagen: [https://developer.mozilla.org/ru/](https://developer.mozilla.org/ru/) (Allg. Sicherheitsressourcen)


  **[⬆ Наверх](#top)**  

51. ### <a name="51"></a> Wie verhindert man SQL-Injections in Express?

## Wie verhindert man SQL-Injection in Express?

Grundprinzipien

* **Keine String-Konkatenation** für SQL. Immer **parametrisierte Queries** / Prepared Statements.
* **ORM/Query-Builder** korrekt nutzen (Sequelize `where`, `bind`/`replacements`), kein Roh-SQL ohne Bindings.
* **Eingaben validieren/sanitizen** (Schema-Validierung).
* **Least Privilege** für DB-User, Logging/Monitoring von ungewöhnlichen Zugriffen.

Parametrisierte Queries mit `pg` (PostgreSQL)

```js
import express from 'express';
import pg from 'pg';

const app = express();
const pool = new pg.Pool({ connectionString: process.env.DATABASE_URL });

app.get('/users', async (req, res, next) => {
  try {
    const { email } = req.query;
    // $1 ist ein Placeholder – DB behandelt Wert getrennt vom SQL-Text
    const sql = 'SELECT id, email FROM users WHERE email = $1';
    const { rows } = await pool.query(sql, [email]);
    res.json(rows);
  } catch (err) { next(err); }
});

app.listen(3000);
```

Sequelize sicher einsetzen

```js
// 1) Bevorzugt: Model-API (automatisch gebundene Parameter)
import { User } from './models.js';

app.get('/user/:id', async (req, res, next) => {
  try {
    const user = await User.findByPk(req.params.id); // sicher
    res.json(user);
  } catch (e) { next(e); }
});
```

```js
// 2) Roh-SQL mit Bind/Replacements (niemals String-Templates mit User-Input)
import { sequelize, Sequelize } from './db.js';

const { QueryTypes } = Sequelize;

app.get('/search', async (req, res, next) => {
  try {
    const term = req.query.q ?? '';
    const rows = await sequelize.query(
      'SELECT id, name FROM products WHERE name ILIKE :term',
      { replacements: { term: `%${term}%` }, type: QueryTypes.SELECT }
    );
    res.json(rows);
  } catch (e) { next(e); }
});
```

Input-Validierung (Beispiel)

```js
import { z } from 'zod';

const searchSchema = z.object({ q: z.string().max(100) });

app.get('/safe-search', async (req, res, next) => {
  try {
    const { q } = searchSchema.parse(req.query);
    // ab hier garantiert Typ/Format
    // … parametrisierte Query wie oben
    res.json({ ok: true });
  } catch (e) { e.status = 400; next(e); }
});
```

Zusätzliche Hinweise

* Für `LIKE`/`ILIKE` Platzhalter (`%`, `_`) nicht selbst escapen, sondern **parameterisieren** und bei Bedarf `ESCAPE` verwenden.
* Keine dynamischen Spalten-/Tabellennamen aus User-Input. Wenn nötig, **Whitelist** (Mapping) verwenden.
* DB-User ohne `SUPERUSER`/DDL-Rechte; nur benötigte Schemas/Tabellen.
* Fehlerantworten ohne SQL-Details/Stacktraces in Produktion.

Zusammenfassung

* SQL-Injection vermeidet man durch **parametrisierte Queries** und **korrekte ORM-Nutzung**; nie String-Konkatenation.
* Ergänzend: **Validierung**, **Least Privilege**, und zurückhaltende Fehlermeldungen.

Quellen

* PostgreSQL Doku – Vorbereiten/Parameter & Sicherheit: [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)
* Sequelize – Queries/Bind/Replacements: [https://sequelize.org/](https://sequelize.org/)
* Express – Security Best Practices: [https://expressjs.com/de/advanced/best-practice-security.html](https://expressjs.com/de/advanced/best-practice-security.html)
* MDN (RU) – Обзор SQL-инъекций: [https://developer.mozilla.org/ru/docs/Glossary/SQL\_Injection](https://developer.mozilla.org/ru/docs/Glossary/SQL_Injection)


  **[⬆ Наверх](#top)**

52. ### <a name="52"></a> Was ist CSRF und wie schützt man sich dagegen?

## Was ist CSRF und wie schützt man sich dagegen?

**Definition:**
CSRF (*Cross-Site Request Forgery*) ist ein Angriff, bei dem ein Angreifer den Browser eines eingeloggten Nutzers dazu bringt, **unerwünschte Aktionen** auf einer anderen Website auszuführen – z. B. Geld überweisen oder Passwort ändern.
Da Cookies automatisch mitgesendet werden, könnte eine bösartige Seite Requests im Namen des Opfers auslösen.

---

## Schutzmaßnahmen gegen CSRF

### 1. CSRF-Token nutzen (Synchronizer Token Pattern)

* Bei Formularen oder API-Requests wird ein **zufälliges Token** generiert und im HTML oder JSON mitgegeben.
* Der Client sendet dieses Token bei der Anfrage zurück.
* Der Server prüft, ob das Token gültig ist.

```bash
npm install csurf
```

```js
import express from 'express';
import cookieParser from 'cookie-parser';
import csrf from 'csurf';

const app = express();
app.use(cookieParser());
app.use(express.urlencoded({ extended: true }));

// CSRF-Schutz aktivieren (Token in Cookies)
const csrfProtection = csrf({ cookie: true });

app.get('/form', csrfProtection, (req, res) => {
  res.send(`<form action="/process" method="POST">
              <input type="hidden" name="_csrf" value="${req.csrfToken()}">
              <button type="submit">Absenden</button>
            </form>`);
});

app.post('/process', csrfProtection, (req, res) => {
  res.send('Formular sicher abgeschickt');
});
```

---

### 2. SameSite-Cookies

* Cookies mit `SameSite=strict` oder `SameSite=lax` markieren, damit sie **nicht bei Cross-Site-Anfragen** automatisch gesendet werden.

```js
res.cookie('session', 'token', {
  httpOnly: true,
  secure: true,
  sameSite: 'lax'
});
```

---

### 3. Nur sichere Methoden ohne Token erlauben

* CSRF betrifft vor allem **zustandsändernde Methoden** (`POST`, `PUT`, `DELETE`).
* `GET` sollte niemals Änderungen durchführen.

---

### 4. Zusätzliche Schutzmaßnahmen

* **CORS restriktiv konfigurieren** (`cors`-Middleware).
* **Double Submit Cookie Pattern** (zusätzliches Anti-CSRF-Cookie mit Token).
* **CAPTCHA** bei besonders sensiblen Aktionen.

---

## Zusammenfassung

* **CSRF = Cross-Site Request Forgery**, Angriffe durch automatische Cookie-Weitergabe.
* Schutz:

  * CSRF-Token (`csurf`-Middleware in Express),
  * sichere Cookies (`httpOnly`, `secure`, `sameSite`),
  * keine Zustandsänderungen via GET.
* Best Practice: Kombination von **CSRF-Token + SameSite-Cookies**.

**Quellen:**

* [Express.js – Best Practice Security](https://expressjs.com/de/advanced/best-practice-security.html)
* [csurf Middleware – npm](https://www.npmjs.com/package/csurf)
* [MDN – CSRF](https://developer.mozilla.org/ru/docs/Glossary/CSRF)

---

  **[⬆ Наверх](#top)**

53. ### <a name="53"></a> Wie kann man HTTPS in Express konfigurieren?

## HTTPS in Express konfigurieren

**Grundidee:**
Express läuft über Node.js’ TLS-Server. Du übergibst Key/Cert an einen `https`-Server und mountest darauf deine Express-App. Optional leitest du Port 80 → 443 um, setzt HSTS und aktivierst `trust proxy`, wenn ein Upstream-Proxy (NGINX, Cloud) davor sitzt.

**1) Direktes HTTPS mit Key/Cert (Self-Signed oder CA/Let’s Encrypt)**

```js
import fs from 'node:fs';
import https from 'node:https';
import express from 'express';

const app = express();

// Beispielroute
app.get('/', (req, res) => {
  res.send('Hallo über HTTPS');
});

// Zertifikate (Pfad anpassen)
const key  = fs.readFileSync('/etc/ssl/private/privkey.pem');
const cert = fs.readFileSync('/etc/ssl/certs/fullchain.pem');

https.createServer({ key, cert }, app).listen(443, () => {
  console.log('HTTPS läuft auf :443');
});
```

**2) HTTP → HTTPS weiterleiten (Port 80)**

```js
import http from 'node:http';

http.createServer((req, res) => {
  const host = req.headers.host?.replace(/:\d+$/, ''); // Host ohne Port
  const location = `https://${host}${req.url}`;
  res.writeHead(301, { Location: location });
  res.end();
}).listen(80, () => console.log('HTTP-Redirect läuft auf :80'));
```

**3) Hinter Proxy/Load-Balancer (Heroku/NGINX, Railway, etc.)**

```js
import express from 'express';
const app = express();

app.enable('trust proxy'); // respektiert X-Forwarded-* Header

// Erzwinge HTTPS auf App-Ebene (nur wenn kein externer Redirect erfolgt)
app.use((req, res, next) => {
  if (req.secure) return next();
  return res.redirect(301, `https://${req.headers.host}${req.originalUrl}`);
});
```

**4) Security-Header (HSTS) & sichere Cookies**

```js
import helmet from 'helmet';
import express from 'express';

const app = express();

// HSTS: Erzwingt HTTPS bei Clients nach dem ersten Besuch
app.use(helmet.hsts({ maxAge: 15552000, includeSubDomains: true, preload: false }));

// Sichere Cookies
app.get('/login', (req, res) => {
  res.cookie('session', 'token', {
    httpOnly: true,
    secure: true,      // nur über HTTPS senden
    sameSite: 'lax'    // reduziert CSRF-Risiko
  });
  res.send('ok');
});
```

**5) Optional: HTTP/2 (TLS)**

```js
import fs from 'node:fs';
import { createSecureServer } from 'node:http2';
import express from 'express';

const app = express();
app.get('/', (req, res) => res.send('HTTP/2 über TLS'));

const server = createSecureServer({
  key:  fs.readFileSync('/etc/ssl/private/privkey.pem'),
  cert: fs.readFileSync('/etc/ssl/certs/fullchain.pem'),
  allowHTTP1: true // Fallback für Browser ohne HTTP/2
}, app);

server.listen(443, () => console.log('HTTP/2 TLS läuft auf :443'));
```

**Hinweise (ohne Code):**

* Zertifikate: in Produktion **öffentlich signierte** Certs (z. B. Let’s Encrypt) verwenden.
* Private Keys streng schützen (Dateirechte, kein Repo).
* In Containern/Cloud meist TLS am Proxy/Ingress terminieren; die App läuft intern auf HTTP, **mit `trust proxy`** und **HSTS**.
* Fehlerbehandlung: sinnvoll loggen, aber keine sensiblen Pfade/Keys ausgeben.

### Zusammenfassung

* HTTPS: `https.createServer({ key, cert }, app)` auf Port 443.
* Port 80 → 443 per 301 umleiten oder am Proxy terminieren.
* Hinter Proxy: `app.enable('trust proxy')` + optionaler HTTPS-Redirect.
* Sicherheit: **HSTS**, **secure/httpOnly/sameSite Cookies**, **Helmet**.

**Quellen**

* Express – Best Practices/Security: [https://expressjs.com/de/advanced/best-practice-security.html](https://expressjs.com/de/advanced/best-practice-security.html)
* Express – API (app.enable/use): [https://expressjs.com/de/4x/api.html](https://expressjs.com/de/4x/api.html)
* Node.js – HTTPS/TLS: [https://nodejs.org/docs/latest/api/https.html](https://nodejs.org/docs/latest/api/https.html)
* MDN (RU) – HSTS/Cookies/HTTPS: [https://developer.mozilla.org/ru/](https://developer.mozilla.org/ru/)


  **[⬆ Наверх](#top)**

54. ### <a name="54"></a> Was ist express-session und wofür wird es verwendet?

## Was ist `express-session` und wofür wird es verwendet?

**Definition:**
`express-session` ist eine Middleware für Express, die **Server-seitige Sitzungen (Sessions)** verwaltet.

* Jeder Client bekommt eine eindeutige **Session-ID** (im Cookie gespeichert).
* Die eigentlichen Sitzungsdaten liegen **auf dem Server** (Memory oder Datenbank).
* Dient häufig für **Login-/Authentifizierungs-Mechanismen**, Warenkörbe, oder temporäre Benutzerdaten.

---

**1. Installation**

```bash
npm install express-session
```

---

**2. Einfaches Setup**

```js
import express from 'express';
import session from 'express-session';

const app = express();

app.use(session({
  secret: 'meinGeheimerKey',   // zur Signierung des Cookies
  resave: false,               // Session nicht speichern, wenn sie nicht verändert wurde
  saveUninitialized: false,    // leere Sessions nicht speichern
  cookie: {
    httpOnly: true,            // nicht per JS auslesbar
    secure: false,             // true in Produktion (nur HTTPS!)
    maxAge: 1000 * 60 * 15     // 15 Minuten
  }
}));

app.get('/set', (req, res) => {
  req.session.username = 'Sergii';
  res.send('Session gesetzt');
});

app.get('/get', (req, res) => {
  res.send(`Hallo ${req.session.username || 'Gast'}`);
});

app.listen(3000, () => console.log('Server läuft auf 3000'));
```

---

**3. Ablauf**

1. Beim ersten Request: Session wird erstellt + Session-ID als Cookie `connect.sid` gesetzt.
2. Bei weiteren Requests: Browser sendet Cookie mit, Server erkennt Session und liest gespeicherte Daten.

---

**4. Storage-Optionen**

* Standard: **MemoryStore** (nicht für Produktion geeignet).
* Beliebte Stores:

  * `connect-pg-simple` (PostgreSQL)
  * `connect-mongo` (MongoDB)
  * `connect-redis` (Redis, oft in Produktion)

Beispiel Redis-Store:

```bash
npm install connect-redis ioredis
```

```js
import RedisStore from 'connect-redis';
import Redis from 'ioredis';

const redisClient = new Redis();

app.use(session({
  store: new RedisStore({ client: redisClient }),
  secret: 'meinGeheimerKey',
  resave: false,
  saveUninitialized: false
}));
```

---

### Zusammenfassung

* `express-session` verwaltet **serverseitige Sitzungen**.
* Session-ID wird im Cookie gespeichert, Daten bleiben auf dem Server.
* Typische Anwendungsfälle: **Login, Warenkorb, Benutzerstatus**.
* Für Produktion: **externer Store** (Redis, DB) statt Memory.

**Quellen:**

* [express-session – npm](https://www.npmjs.com/package/express-session)
* [Express.js – Best Practices Security](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**

55. ### <a name="55"></a> Wie implementiert man JWT-Authentifizierung in Express?

## JWT-Authentifizierung in Express (Access-/Refresh-Token)

**Ziel:** Nutzer nach Login ein **JWT** (Access-Token) ausstellen, bei geschützten Routen **verifizieren**, optional **Refresh-Token** für langlebige Sessions.

---

**1) Installation & Setup**

```bash
npm i jsonwebtoken
```

```js
// config/env.js
export const JWT_ACCESS_SECRET = process.env.JWT_ACCESS_SECRET;     // z. B. 32+ zufällige Bytes
export const JWT_REFRESH_SECRET = process.env.JWT_REFRESH_SECRET;   // separat zum Access-Secret
export const JWT_ACCESS_EXPIRES_IN = '15m';     // kurzlebig
export const JWT_REFRESH_EXPIRES_IN = '7d';     // langlebig
```

---

**2) Token helpers (sign/verify)**

```js
// auth/jwt.js
import jwt from 'jsonwebtoken';
import {
  JWT_ACCESS_SECRET, JWT_REFRESH_SECRET,
  JWT_ACCESS_EXPIRES_IN, JWT_REFRESH_EXPIRES_IN
} from '../config/env.js';

export function signAccessToken(payload) {
  return jwt.sign(payload, JWT_ACCESS_SECRET, { expiresIn: JWT_ACCESS_EXPIRES_IN });
}

export function signRefreshToken(payload) {
  return jwt.sign(payload, JWT_REFRESH_SECRET, { expiresIn: JWT_REFRESH_EXPIRES_IN });
}

export function verifyAccessToken(token) {
  return jwt.verify(token, JWT_ACCESS_SECRET);
}

export function verifyRefreshToken(token) {
  return jwt.verify(token, JWT_REFRESH_SECRET);
}
```

---

**3) Auth-Middleware (geschützte Routen)**

```js
// auth/requireAuth.js
import { verifyAccessToken } from './jwt.js';

export function requireAuth(req, res, next) {
  const auth = req.headers.authorization || '';
  const [, token] = auth.split(' ');
  if (!token) return res.status(401).json({ error: 'Unauthorized' });

  try {
    const payload = verifyAccessToken(token); // { sub, role, ... }
    req.user = payload;
    next();
  } catch {
    return res.status(401).json({ error: 'Invalid or expired token' });
  }
}
```

> Üblich ist `Authorization: Bearer <token>`. Alternativ: **httpOnly** Cookie (mit CORS `credentials: true`).

---

**4) Login/Refresh/Logout Routen**

```js
// auth/routes.js
import { Router } from 'express';
import { signAccessToken, signRefreshToken, verifyRefreshToken } from './jwt.js';
// Beispiel: User aus DB holen + Passwort prüfen (aus Platzgründen hier weggelassen)
const router = Router();

// Login – Tokens ausstellen
router.post('/login', async (req, res) => {
  const { userId, role } = { userId: 123, role: 'user' }; // aus DB nach Prüfung
  const accessToken = signAccessToken({ sub: userId, role });
  const refreshToken = signRefreshToken({ sub: userId });
  res.status(200).json({ accessToken, refreshToken });
});

// Geschützte Route
router.get('/me', (req, res) => {
  // in requireAuth wird req.user gesetzt; hier nur Beispiel ohne Middleware
  res.json({ message: 'OK – geschützter Inhalt' });
});

// Access-Token erneuern
router.post('/refresh', (req, res) => {
  const { refreshToken } = req.body || {};
  if (!refreshToken) return res.status(401).json({ error: 'Missing refresh token' });
  try {
    const { sub } = verifyRefreshToken(refreshToken);
    const newAccess = signAccessToken({ sub });
    return res.json({ accessToken: newAccess });
  } catch {
    return res.status(401).json({ error: 'Invalid refresh token' });
  }
});

export default router;
```

---

**5) Einbindung in Express-App**

```js
// server.js
import express from 'express';
import authRoutes from './auth/routes.js';
import { requireAuth } from './auth/requireAuth.js';

const app = express();
app.use(express.json());

app.use('/auth', authRoutes);

// Beispiel für geschützte API
app.get('/api/secret', requireAuth, (req, res) => {
  res.json({ user: req.user.sub, secret: 'top' });
});

app.listen(3000, () => console.log('API läuft auf :3000'));
```

---

**Sicherheits-Hinweise (kurz)**

* **Secrets** nur aus Umgebungsvariablen; getrennte Secrets für Access/Refresh.
* **Kurze TTL** für Access-Token (z. B. 15 min); Refresh-Token rotieren/speichern (z. B. DB/Redis) → bei Logout/Revoke invalidieren.
* Bei Cookies: `httpOnly`, `secure`, `sameSite=lax/strict`, CORS `credentials: true`.
* Payload minimal halten (z. B. nur `sub`, `role`), keine sensiblen Daten in JWT.
* Auf **Clock Skew** achten (Serverzeit), 401/403 sauber unterscheiden.

### Zusammenfassung

* JWTs mit `jsonwebtoken`: kurzlebiges **Access-Token** für Auth, **Refresh-Token** zum Erneuern.
* Middleware prüft `Authorization: Bearer <token>` und setzt `req.user`.
* Secrets/TTL korrekt konfigurieren, Refresh-Token sicher speichern/rotieren, Cookies optional mit `httpOnly/secure`.

**Quellen**

* Node.js – Prozess/Umgebung: [https://nodejs.org/docs](https://nodejs.org/docs)
* Express – Best Practices/Security: [https://expressjs.com/de/advanced/best-practice-security.html](https://expressjs.com/de/advanced/best-practice-security.html)
* MDN (RU) – JSON Web Token Überblick: [https://developer.mozilla.org/ru/docs/Web/HTTP/Authentication#json\_web\_token\_jwt](https://developer.mozilla.org/ru/docs/Web/HTTP/Authentication#json_web_token_jwt)
* jsonwebtoken – npm: [https://www.npmjs.com/package/jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken)


  **[⬆ Наверх](#top)**

56. ### <a name="56"></a> Wie baut man eine REST-API mit Express?

## REST-API mit Express: Vorgehen, Struktur, Beispiele

Ziele

* Klare **Routen** (Resources/CRUD), **Controller**-Logik, **Middleware** (Parsing, CORS, Auth, Fehler).
* **Statuscodes** und **JSON**-Antworten konsistent.
* Optional: **PostgreSQL** via **Sequelize**.

Projektstruktur (Beispiel)

```
src/
  app.js
  server.js
  routes/
    users.routes.js
  controllers/
    users.controller.js
  middlewares/
    error.middleware.js
    auth.middleware.js
  db/
    index.js
    models/
      user.model.js
  validators/
    users.schema.js
package.json
.env
```

package.json (ESM, Scripts)

```json
{
  "type": "module",
  "scripts": {
    "dev": "node --watch src/server.js",
    "start": "node src/server.js"
  },
  "dependencies": {
    "express": "^4.19.2",
    "cors": "^2.8.5",
    "helmet": "^7.1.0",
    "sequelize": "^6.37.0",
    "pg": "^8.11.5",
    "zod": "^3.23.0"
  }
}
```

App-Grundgerüst (Parsing, CORS, Security, Error-Handling)

```js
// src/app.js
import express from 'express';
import cors from 'cors';
import helmet from 'helmet';
import usersRouter from './routes/users.routes.js';
import { notFound } from './middlewares/error.middleware.js';
import { errorHandler } from './middlewares/error.middleware.js';

const app = express();

app.use(helmet());
app.use(cors({ origin: ['http://localhost:5173'], credentials: true }));
app.use(express.json());
app.use(express.urlencoded({ extended: true }));

app.get('/health', (req, res) => res.json({ status: 'ok' }));

app.use('/api/v1/users', usersRouter);

// 404 → Error-Handler
app.use(notFound);
app.use(errorHandler);

export default app;
```

Server starten

```js
// src/server.js
import app from './app.js';

const PORT = process.env.PORT ?? 3000;
app.listen(PORT, () => console.log(`API läuft auf :${PORT}`));
```

REST-Routen (CRUD)

```js
// src/routes/users.routes.js
import { Router } from 'express';
import * as ctrl from '../controllers/users.controller.js';

const r = Router();

r.get('/', ctrl.listUsers);      // GET /api/v1/users
r.get('/:id', ctrl.getUser);     // GET /api/v1/users/:id
r.post('/', ctrl.createUser);    // POST
r.put('/:id', ctrl.updateUser);  // PUT (vollständig)
r.patch('/:id', ctrl.patchUser); // PATCH (teilweise)
r.delete('/:id', ctrl.deleteUser);// DELETE

export default r;
```

Controller (Beispiel, mit Statuscodes)

```js
// src/controllers/users.controller.js
import { User } from '../db/models/user.model.js';
import { createUserSchema, updateUserSchema } from '../validators/users.schema.js';

export async function listUsers(req, res, next) {
  try {
    const { page = 1, limit = 10 } = req.query;
    const offset = (Number(page) - 1) * Number(limit);
    const { rows, count } = await User.findAndCountAll({ offset, limit: Number(limit), order: [['id', 'ASC']] });
    res.json({ data: rows, meta: { page: Number(page), limit: Number(limit), total: count } });
  } catch (e) { next(e); }
}

export async function getUser(req, res, next) {
  try {
    const user = await User.findByPk(req.params.id);
    if (!user) return res.status(404).json({ error: 'User nicht gefunden' });
    res.json(user);
  } catch (e) { next(e); }
}

export async function createUser(req, res, next) {
  try {
    const dto = createUserSchema.parse(req.body);
    const user = await User.create(dto);
    res.status(201).json(user);
  } catch (e) { e.status ??= 400; next(e); }
}

export async function updateUser(req, res, next) {
  try {
    const dto = updateUserSchema.parse(req.body);
    const user = await User.findByPk(req.params.id);
    if (!user) return res.status(404).json({ error: 'User nicht gefunden' });
    await user.update(dto);
    res.json(user);
  } catch (e) { e.status ??= 400; next(e); }
}

export async function patchUser(req, res, next) {
  try {
    const user = await User.findByPk(req.params.id);
    if (!user) return res.status(404).json({ error: 'User nicht gefunden' });
    await user.update(req.body);
    res.json(user);
  } catch (e) { e.status ??= 400; next(e); }
}

export async function deleteUser(req, res, next) {
  try {
    const user = await User.findByPk(req.params.id);
    if (!user) return res.status(404).json({ error: 'User nicht gefunden' });
    await user.destroy();
    res.status(204).send();
  } catch (e) { next(e); }
}
```

Validierung (zod)

```js
// src/validators/users.schema.js
import { z } from 'zod';

export const createUserSchema = z.object({
  email: z.string().email(),
  name: z.string().min(2),
  role: z.enum(['user', 'admin']).default('user')
});

export const updateUserSchema = createUserSchema.partial();
```

Error-Middleware (404 + zentraler Handler)

```js
// src/middlewares/error.middleware.js
export function notFound(req, res, next) {
  res.status(404).json({ error: 'Route nicht gefunden' });
}

export function errorHandler(err, req, res, next) {
  const status = err.status || err.statusCode || 500;
  const payload = {
    error: err.message || 'Interner Serverfehler'
  };
  if (process.env.NODE_ENV !== 'production') {
    payload.stack = err.stack;
  }
  res.status(status).json(payload);
}
```

Datenbank (PostgreSQL + Sequelize)

```js
// src/db/index.js
import { Sequelize } from 'sequelize';

export const sequelize = new Sequelize(process.env.DATABASE_URL, {
  dialect: 'postgres',
  logging: false
});

export async function initDb() {
  await sequelize.authenticate();
  await sequelize.sync(); // in Prod: Migrations verwenden!
}
```

```js
// src/db/models/user.model.js
import { DataTypes, Model } from 'sequelize';
import { sequelize } from '../index.js';

export class User extends Model {}

User.init({
  email: { type: DataTypes.STRING, unique: true, allowNull: false, validate: { isEmail: true } },
  name:  { type: DataTypes.STRING, allowNull: false },
  role:  { type: DataTypes.ENUM('user', 'admin'), allowNull: false, defaultValue: 'user' }
}, { sequelize, modelName: 'User', tableName: 'users' });
```

Server-Start inkl. DB-Init

```js
// src/server.js
import app from './app.js';
import { initDb } from './db/index.js';

const PORT = process.env.PORT ?? 3000;

initDb()
  .then(() => app.listen(PORT, () => console.log(`API läuft auf :${PORT}`)))
  .catch((e) => {
    console.error('DB-Start fehlgeschlagen:', e);
    process.exit(1);
  });
```

Best Practices (kurz)

* **Versionierung** von Routen: `/api/v1`.
* **Statuscodes** konsistent (201 bei Create, 204 bei Delete).
* **Pagination/Filter/Sort** anbieten.
* **Security**: `helmet`, `cors`, Rate-Limiting für sensible Endpunkte.
* **Auth**: Sessions oder **JWT** (Bearer) für geschützte Routen.
* **Validation** auf allen Eingaben.
* **Migrations** statt `sync()` in Produktion (z. B. Sequelize CLI).
* **Logs** (morgan/pino) und **Monitoring**.
* **E2E-/Integrationstests** (z. B. supertest, jest).

Zusammenfassung

* Express-REST-API = klare Schichten: **Routes → Controller → Services/DB**, plus **Middleware** (Parsing, Errors, Security).
* JSON-Antworten, korrekte **Statuscodes**, **Validierung** und **zentrales Fehlerhandling** sind Pflicht.
* Mit Sequelize/PostgreSQL schnell produktiv: Modelle, CRUD, Pagination.

Quellen

* Express.js – Starter/Guide/API: [https://expressjs.com/de/](https://expressjs.com/de/)
* Node.js Dokumentation: [https://nodejs.org/docs](https://nodejs.org/docs)
* PostgreSQL Dokumentation: [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)
* Sequelize Dokumentation: [https://sequelize.org/](https://sequelize.org/)
* MDN Web Docs (RU) – HTTP, REST-Grundlagen: [https://developer.mozilla.org/ru/](https://developer.mozilla.org/ru/)


  **[⬆ Наверх](#top)**

57. ### <a name="57"></a> Unterschied zwischen REST und GraphQL im Kontext von Express?

## Unterschied zwischen REST und GraphQL im Kontext von Express

**1. REST (Representational State Transfer)**

* Architekturstil für APIs, basiert auf **Ressourcen und HTTP-Methoden**.
* Jede Ressource hat eine eindeutige URL (`/api/v1/users/123`).
* Methoden definieren die Operation: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`.
* **Antwort:** gesamte Ressource oder eine Liste.
* **Nachteile:** Overfetching (zu viele Daten) oder Underfetching (zu wenige Daten → mehrere Requests nötig).

```js
// REST-Beispiel in Express
app.get('/api/v1/users/:id', (req, res) => {
  res.json({ id: req.params.id, name: 'Sergii', email: 'sergii@mail.de' });
});
```

---

**2. GraphQL**

* Query-Sprache für APIs, **ein einziger Endpunkt** (`/graphql`).
* Client bestimmt **selbst**, welche Felder er benötigt.
* **Antwort:** exakt die angeforderten Daten.
* **Vorteile:** kein Over-/Underfetching, flexible Queries.
* **Nachteile:** komplexere Implementierung, Caching schwieriger, Overhead bei kleinen Projekten.

```js
// GraphQL in Express mit express-graphql
import express from 'express';
import { graphqlHTTP } from 'express-graphql';
import { buildSchema } from 'graphql';

const schema = buildSchema(`
  type User { id: ID!, name: String!, email: String! }
  type Query { user(id: ID!): User }
`);

const root = {
  user: ({ id }) => ({ id, name: 'Sergii', email: 'sergii@mail.de' })
};

const app = express();
app.use('/graphql', graphqlHTTP({ schema, rootValue: root, graphiql: true }));
app.listen(3000);
```

---

**3. Vergleich REST vs. GraphQL**

| Kriterium     | REST                                | GraphQL                               |
| ------------- | ----------------------------------- | ------------------------------------- |
| Endpunkte     | Viele (`/users`, `/posts/:id`)      | Ein einziger (`/graphql`)             |
| Abfragen      | Vorgegebene Struktur (durch Server) | Client bestimmt Felder (flexibel)     |
| Overfetching  | möglich                             | vermieden                             |
| Versionierung | Oft `/api/v1`, `/api/v2`            | Schema-Änderungen statt Versionierung |
| Caching       | Einfach via HTTP-Cache              | komplexer, eigene Layer nötig         |
| Einstieg      | einfacher                           | höherer Lernaufwand                   |

---

### Zusammenfassung

* **REST:** bewährt, einfach, ressourcenorientiert, gute Integration mit HTTP-Standards.
* **GraphQL:** flexibel, clientgetrieben, löst Over-/Underfetching, aber komplexer in Setup und Betrieb.
* In Express: REST = klassische Routen, GraphQL = ein Endpunkt mit `express-graphql` oder Apollo Server.

**Quellen:**

* [Express.js – Routing](https://expressjs.com/de/guide/routing.html)
* [GraphQL Offizielle Seite](https://graphql.org/)
* [express-graphql – npm](https://www.npmjs.com/package/express-graphql)
* [MDN – REST](https://developer.mozilla.org/ru/docs/Glossary/REST)

---

  **[⬆ Наверх](#top)**

58. ### <a name="58"></a> Wie validiert man Daten in einer REST-API?

## Datenvalidierung in einer REST-API mit Express

**Warum wichtig?**

* Schutz vor fehlerhaften oder bösartigen Eingaben.
* Konsistente API → klar definierte Eingabe- und Ausgabestrukturen.
* Verhindert Sicherheitslücken (z. B. SQL Injection, XSS).

---

### 1. Manuelle Validierung

Einfach, aber fehleranfällig bei größeren Projekten.

```js
app.post('/users', (req, res) => {
  const { email, age } = req.body;
  if (!email || !email.includes('@')) {
    return res.status(400).json({ error: 'Ungültige E-Mail' });
  }
  if (!age || isNaN(age)) {
    return res.status(400).json({ error: 'Ungültiges Alter' });
  }
  res.status(201).json({ email, age });
});
```

---

### 2. Schema-basierte Validierung mit **Joi**

```bash
npm install joi
```

```js
import Joi from 'joi';

const userSchema = Joi.object({
  email: Joi.string().email().required(),
  age: Joi.number().integer().min(18).required()
});

app.post('/users', (req, res) => {
  const { error, value } = userSchema.validate(req.body);
  if (error) {
    return res.status(400).json({ error: error.details.map(d => d.message) });
  }
  res.status(201).json(value);
});
```

---

### 3. Validierung mit **Zod** (modern, TypeScript-freundlich)

```bash
npm install zod
```

```js
import { z } from 'zod';

const userSchema = z.object({
  email: z.string().email(),
  age: z.number().int().min(18)
});

app.post('/users', (req, res, next) => {
  try {
    const data = userSchema.parse(req.body); // validiert & typisiert
    res.status(201).json(data);
  } catch (err) {
    res.status(400).json({ error: err.errors });
  }
});
```

---

### 4. Middleware für Validierung

Best Practice: Validierung in Middleware auslagern.

```js
function validate(schema) {
  return (req, res, next) => {
    try {
      req.body = schema.parse(req.body);
      next();
    } catch (err) {
      res.status(400).json({ error: err.errors });
    }
  };
}

app.post('/users', validate(userSchema), (req, res) => {
  res.status(201).json(req.body);
});
```

---

### 5. Validierung auf Query-/Params-Ebene

```js
const querySchema = z.object({
  page: z.string().regex(/^\d+$/).transform(Number).default("1"),
  limit: z.string().regex(/^\d+$/).transform(Number).default("10")
});

app.get('/users', (req, res) => {
  const { page, limit } = querySchema.parse(req.query);
  res.json({ page, limit });
});
```

---

### Zusammenfassung

* **Manuell** → gut für kleine Checks.
* **Joi/Zod** → mächtig und konsistent für große APIs.
* **Middleware** nutzen, um Validierung zentral zu handhaben.
* Validierung nicht nur für `body`, sondern auch für `params` und `query`.

**Quellen:**

* [Express.js – Best Practices](https://expressjs.com/de/advanced/best-practice-performance.html)
* [Joi – npm](https://www.npmjs.com/package/joi)
* [Zod – npm](https://www.npmjs.com/package/zod)

---

  **[⬆ Наверх](#top)**

59. ### <a name="59"></a> Welche Best Practices gibt es für RESTful Routes?

## Best Practices für RESTful Routes in Express

**Ressourcen-Design**

* **Substantive, Plural**: `/users`, `/orders`, `/products`.
* **Eindeutige IDs**: `/users/:id` (keine Aktionswörter in Pfaden).
* **Nesting sparsam**: max. 1 Ebene – z. B. `/users/:id/orders`; tieferes Nesting via Filter (`/orders?userId=:id`).

**HTTP-Methoden semantisch nutzen**

* `GET /users` (lesen, idempotent)
* `GET /users/:id`
* `POST /users` (erstellen, `201 Created`)
* `PUT /users/:id` (vollständiges Update)
* `PATCH /users/:id` (teilweises Update)
* `DELETE /users/:id` (`204 No Content` bei Erfolg)

**Statuscodes & Header**

* `201` + `Location`-Header nach `POST`.
* `204` ohne Body bei `DELETE`/idempotenten Updates ohne Rückgabe.
* Konsistente Fehler: `400/401/403/404/409/422/500`.
* Caching-Header (`ETag`, `Last-Modified`, `Cache-Control`) wo sinnvoll.

**Query-Parameter für Abfragen**

* Filtering/Sorting/Pagination über Query: `GET /users?role=admin&sort=createdAt&order=desc&page=2&limit=20`.
* Einheitliche Paginierung (`page`, `limit`) und Metadaten im Response (`total`, `page`, `limit`).

**Versionierung**

* Präfix: `/api/v1/...`.
* Alternativ über Header (fortgeschritten), im Alltag meist Pfadversionierung.

**Konsistente JSON-Antworten**

* Einheitliches Format: `{ data, meta, error }`.
* Keine HTML-Antworten in einer JSON-API; `Content-Type: application/json`.

**Idempotenz & Sicherheit**

* `PUT`/`DELETE` idempotent gestalten.
* Eingaben validieren (Schema, z. B. Zod/Joi).
* AuthN/AuthZ zentral (Middleware), Rate-Limit, Helmet, CORS restriktiv.

**Fehler-Handling**

* Zentrale Error-Middleware; klare Fehlerobjekte (`{ error: '...', details: [...] }`).
* Keine internen Stacktraces in Produktion.

**Dateistruktur & Router**

* Trennung: **Routes → Controller → Service/DB**, Wiederverwendung durch `express.Router()`.
* Gruppierung nach Ressourcen, nicht nach HTTP-Methode.

**Beispiel (ESM, Express-Router)**

```js
// routes/users.routes.js
import { Router } from 'express';
import * as ctrl from '../controllers/users.controller.js';
import { validate } from '../middlewares/validate.js';
import { createUserSchema, updateUserSchema } from '../validators/users.schema.js';

const r = Router();

r.get('/', ctrl.list);                    // GET /api/v1/users
r.get('/:id', ctrl.getById);              // GET /api/v1/users/:id
r.post('/', validate(createUserSchema), ctrl.create);   // POST
r.put('/:id', validate(updateUserSchema), ctrl.replace); // PUT
r.patch('/:id', validate(updateUserSchema.partial()), ctrl.partial); // PATCH
r.delete('/:id', ctrl.remove);            // DELETE

export default r;
```

```js
// Beispiel-Response für List mit Meta
export async function list(req, res, next) {
  try {
    const page = Number(req.query.page ?? 1);
    const limit = Number(req.query.limit ?? 10);
    const offset = (page - 1) * limit;
    const { rows, count } = await User.findAndCountAll({ offset, limit, order: [['id','ASC']] });
    res.json({ data: rows, meta: { total: count, page, limit } });
  } catch (e) { next(e); }
}
```

**Weitere Hinweise**

* Ressourcen-URLs sind **ohne Verben**; Aktionen als Zustandswechsel per Methode modellieren.
* Batch-Operationen klar kennzeichnen (`POST /users/batch`).
* HATEOAS optional via Links (`self`, `next`, `prev`).
* Einheitliche Uhrzeit- und ID-Formate (ISO 8601, UUID).

### Zusammenfassung

* Klare Ressourcennamen, semantische Methoden, konsistente Statuscodes/JSON.
* Query-Parameter für Filter/Sort/Pagination, Versionierung via `/api/v1`.
* Validierung, Security-Middleware und zentrales Error-Handling sind Pflicht.
* Saubere Schichten-Trennung und Router-Struktur erhöhen Wartbarkeit.

**Quellen**

* Express.js – Guide & Routing: [https://expressjs.com/de/guide/routing.html](https://expressjs.com/de/guide/routing.html)
* Express.js – Best Practices (Security/Performance): [https://expressjs.com/de/advanced/best-practice-performance.html](https://expressjs.com/de/advanced/best-practice-performance.html)
* MDN (RU) – HTTP-Methoden/Status: [https://developer.mozilla.org/ru/docs/Web/HTTP/Methods](https://developer.mozilla.org/ru/docs/Web/HTTP/Methods) , [https://developer.mozilla.org/ru/docs/Web/HTTP/Status](https://developer.mozilla.org/ru/docs/Web/HTTP/Status)
* Node.js Dokumentation: [https://nodejs.org/docs](https://nodejs.org/docs)


  **[⬆ Наверх](#top)**

60. ### <a name="60"></a> Was ist HATEOAS?

## Was ist HATEOAS?

**Definition:**
HATEOAS steht für **Hypermedia as the Engine of Application State**.

* Es ist ein Prinzip von REST (aus Roy Fieldings Dissertation).
* Idee: Ein Client soll eine API **entdecken und navigieren können**, ohne deren Struktur im Voraus kennen zu müssen.
* Jede Ressource liefert **Hypermedia-Links**, die auf weitere mögliche Aktionen verweisen.

---

**Beispiel ohne HATEOAS (klassisches REST):**

```json
{
  "id": 42,
  "title": "REST API lernen",
  "author": "Sergii"
}
```

👉 Hier muss der Client die Endpunkte (z. B. `/posts/42/comments`) kennen.

---

**Beispiel mit HATEOAS:**

```json
{
  "id": 42,
  "title": "REST API lernen",
  "author": "Sergii",
  "_links": {
    "self": { "href": "/api/v1/posts/42" },
    "comments": { "href": "/api/v1/posts/42/comments" },
    "author": { "href": "/api/v1/users/7" }
  }
}
```

👉 Der Client kann anhand der Links automatisch sehen, welche nächsten Schritte möglich sind.

---

**Vorteile:**

* API ist **selbstbeschreibend**.
* Weniger harte Kopplung zwischen Client und Server.
* Einfachere Weiterentwicklung/Versionierung.

**Nachteile:**

* Höherer Implementierungsaufwand.
* Nicht alle Clients nutzen oder benötigen HATEOAS.
* In modernen REST-APIs oft weggelassen zugunsten von **OpenAPI/Swagger**.

---

### Zusammenfassung

* **HATEOAS = Hypermedia als Navigationshilfe in REST-APIs.**
* Jede Antwort enthält **Links zu weiteren möglichen Aktionen**.
* Stärkt die Selbstbeschreibung der API, aber heute oft durch **Swagger/OpenAPI** ersetzt.

**Quellen:**

* [MDN – HATEOAS](https://developer.mozilla.org/ru/docs/Glossary/HATEOAS)
* [REST Dissertation von Roy Fielding](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm)

---

  **[⬆ Наверх](#top)**

61. ### <a name="61"></a> Wie baut man eine Versionierung für APIs in Express ein?

## API-Versionierung in Express: Strategien und Umsetzung

**Hauptstrategien**

* **Pfadbasiert (empfohlen für Einfachheit):** `/api/v1/...`, später `/api/v2/...`.
* **Header-basiert (Content-Negotiation):** `Accept: application/vnd.myapp.v1+json`.
* **Query-Parameter (nicht empfohlen):** `?version=1` (leicht missbrauchbar, schwer zu cachen).

**Pfadbasierte Versionierung (einfach & klar)**

```js
// src/app.js
import express from 'express';
import v1Routes from './v1/index.js';
import v2Routes from './v2/index.js';

const app = express();
app.use(express.json());

// v1 – stabil
app.use('/api/v1', v1Routes);

// v2 – neue Breaking Changes
app.use('/api/v2', v2Routes);

export default app;
```

```js
// src/v1/index.js
import { Router } from 'express';
const r = Router();

r.get('/users/:id', (req, res) => {
  res.json({ id: req.params.id, fullName: 'V1-Name' });
});

export default r;
```

```js
// src/v2/index.js
import { Router } from 'express';
const r = Router();

r.get('/users/:id', (req, res) => {
  res.json({ id: req.params.id, name: { first: 'V2', last: 'Name' } });
});

export default r;
```

**Header-basierte Versionierung (fortgeschritten)**

```js
// src/middlewares/versioning.js
export function pickVersion(req, res, next) {
  const accept = req.headers.accept || '';
  if (accept.includes('vnd.myapp.v2+json')) req.apiVersion = 'v2';
  else if (accept.includes('vnd.myapp.v1+json')) req.apiVersion = 'v1';
  else req.apiVersion = 'v1'; // Default
  next();
}
```

```js
// src/app.js
import express from 'express';
import { pickVersion } from './middlewares/versioning.js';
import v1Routes from './v1/index.js';
import v2Routes from './v2/index.js';

const app = express();
app.use(express.json());
app.use(pickVersion);

// Multiplexer
app.use((req, res, next) => {
  if (req.apiVersion === 'v2') return v2Routes(req, res, next);
  return v1Routes(req, res, next);
});

export default app;
```

**Deprecation & Sunset (Kommunikation)**

```js
// Deprecation-Header für alte Versionen
app.use('/api/v1', (req, res, next) => {
  res.setHeader('Deprecation', 'true');            // RFC 8594
  res.setHeader('Sunset', 'Tue, 31 Mar 2026 23:59:59 GMT');
  res.setHeader('Link', '</api/v2>; rel="successor-version"');
  next();
});
```

**Best Practices**

* **Stabile Basis:** Business-Logik in Services kapseln, nur DTO/Mapper pro Version anpassen.
* **Konsistente Semantik:** 201/204/404/422 etc. beibehalten; nur **Schema** oder **Felder** zwischen Versionen ändern.
* **Dokumentation pro Version:** Separate OpenAPI-Spezifikationen (`openapi-v1.yaml`, `openapi-v2.yaml`).
* **Lebenszyklus definieren:** Support-Zeitraum, Deprecation-Ankündigung, Sunset-Datum.
* **Default-Version:** Klar kommunizieren (z. B. v1), Fallbacks dokumentieren.
* **Tests je Version:** Contract-Tests/Snapshot-Tests, um unbeabsichtigte Brüche zu vermeiden.
* **Caching berücksichtigen:** Pfadversionierung ist HTTP-Cache-freundlich; Header-Versionierung benötigt passende Vary-Header (`Vary: Accept`).

### Zusammenfassung

* **Pfadversionierung** ist am einfachsten (`/api/v1`), **Header-Versionierung** ist flexibler, aber komplexer.
* Versionen sauber trennen (eigene Router), Kernlogik teilen, nur **DTO/Antwortformate** pro Version variieren.
* Deprecation/Sunset-Header setzen, getrennte OpenAPI-Dokumente pflegen, Tests pro Version.

**Quellen**

* Express.js – Guide & Routing: [https://expressjs.com/de/guide/routing.html](https://expressjs.com/de/guide/routing.html)
* Express.js – Best Practices: [https://expressjs.com/de/advanced/best-practice-performance.html](https://expressjs.com/de/advanced/best-practice-performance.html)
* MDN (RU) – HTTP-Header (Vary/Content Negotiation): [https://developer.mozilla.org/ru/docs/Web/HTTP/Headers](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers)
* Node.js Dokumentation: [https://nodejs.org/docs](https://nodejs.org/docs)


  **[⬆ Наверх](#top)**

62. ### <a name="62"></a> Wie verarbeitet man große Datenmengen in einer API?

## Große Datenmengen in einer API verarbeiten (Express + Node.js)

Strategien (kurz)

* Pagination/Keyset-Cursor statt alles auf einmal laden.
* Streams & Backpressure: Daten stückweise verarbeiten/liefern.
* Komprimierung & Caching: weniger Bytes über die Leitung.
* “Projektion” (nur benötigte Felder), Filter/Sort am DB-Server.
* Hintergrundjobs für teure Tasks, asynchrone Verarbeitung.
* Zeit- & Größenlimits, Rate-Limiting, Schutz vor Memory-Spikes.

Pagination (Offset vs. Cursor/Keyset)

```js
// Sequelize – Offset-Pagination (einfach, bei großen Offsets langsam)
const page = Number(req.query.page ?? 1);
const limit = Number(req.query.limit ?? 50);
const offset = (page - 1) * limit;
const { rows, count } = await User.findAndCountAll({
  offset, limit, order: [['id','ASC']],
  attributes: ['id','email'] // Projektion
});
res.json({ data: rows, meta: { page, limit, total: count } });
```

```js
// Keyset/Cursor-Pagination – performanter bei großen Tabellen
// client übergibt lastId (cursor); kein COUNT(*) nötig
const limit = Number(req.query.limit ?? 50);
const lastId = req.query.lastId ? Number(req.query.lastId) : 0;
const rows = await User.findAll({
  where: lastId ? { id: { [Op.gt]: lastId } } : {},
  order: [['id','ASC']],
  limit,
  attributes: ['id','email']
});
const nextCursor = rows.length ? rows[rows.length - 1].id : null;
res.json({ data: rows, nextCursor });
```

Streaming aus der Datenbank

```js
// pg-Cursor: speichert nicht alles im RAM, verarbeitet Block-weise
import pg from 'pg';
import Cursor from 'pg-cursor';
const pool = new pg.Pool({ connectionString: process.env.DATABASE_URL });

app.get('/export-ndjson', async (req, res, next) => {
  const client = await pool.connect();
  try {
    res.setHeader('Content-Type', 'application/x-ndjson');
    const cursor = client.query(new Cursor('SELECT id, email FROM users ORDER BY id'));
    const readNext = () => {
      cursor.read(1000, (err, rows) => {
        if (err) return next(err);
        if (!rows.length) {
          cursor.close(() => client.release());
          return res.end();
        }
        for (const r of rows) {
          if (!res.write(JSON.stringify(r) + '\n')) {
            return res.once('drain', readNext); // Backpressure
          }
        }
        readNext();
      });
    };
    readNext();
  } catch (e) {
    client.release();
    next(e);
  }
});
```

HTTP-Streaming & Backpressure (Server → Client)

```js
// NDJSON streamen; res.write() + 'drain' beachten
app.get('/stream', async (req, res) => {
  res.setHeader('Content-Type', 'application/x-ndjson');
  for (let i = 0; i < 1e6; i++) {
    if (!res.write(JSON.stringify({ n: i }) + '\n')) {
      await new Promise(r => res.once('drain', r)); // Backpressure
    }
  }
  res.end();
});
```

Dateien/Exports als Stream senden

```js
import { createReadStream } from 'node:fs';
import { pipeline } from 'node:stream/promises';

app.get('/download', async (req, res, next) => {
  try {
    res.setHeader('Content-Type', 'application/octet-stream');
    res.setHeader('Content-Disposition', 'attachment; filename="dump.bin"');
    await pipeline(createReadStream('/data/dump.bin'), res); // zero-copy Stream
  } catch (e) { next(e); }
});
```

Komprimierung & Caching

```js
// Gzip/Brotli spart Bandbreite; bei großen JSON-Listen relevant
import compression from 'compression';
app.use(compression()); // automatisch nach Accept-Encoding

// ETag/Cache-Control für GET-Listen wenn möglich
app.get('/list', (req, res) => {
  res.set('Cache-Control', 'public, max-age=60'); // kurzzeitiges Caching
  res.json(/* ... */);
});
```

Limits & Schutz

```js
// Body-Size begrenzen, um RAM zu schützen
app.use(express.json({ limit: '1mb' }));
// Rate-Limiting für teure Endpunkte
import rateLimit from 'express-rate-limit';
app.use('/api/heavy', rateLimit({ windowMs: 60_000, max: 60 }));
// Request-Timeout (Upstream oder App)
```

DB-Performance (PostgreSQL)

* Indexe auf Filter-/Sort-Spalten (z. B. `id`, `created_at`).
* Projekte nur benötigte Spalten (`SELECT`-Liste; `attributes` in Sequelize).
* Keine N+1-Queries: sinnvolle `include`/Joins, Batch-Loading.
* Keyset-Pagination bei großen Offsets, kein `OFFSET 1000000`.
* Lange Jobs als Batch/Async (siehe unten), Ergebnis in Files/Tabellen persistieren.

Asynchrone Verarbeitung/Hintergrundjobs

* Für große Exports/Aggregationen: Job-Queue (z. B. BullMQ/Redis).
* API triggert Job → sofort `202 Accepted` + Status-Endpunkt → Client pollt/WS.
* Ergebnis als Download-Link bereitstellen (S3/Blob/Datei-Store) statt Inline-JSON.

Beispiel: “Accepted” + Job-ID

```js
app.post('/reports', async (req, res) => {
  const jobId = await queue.add('build-report', { filters: req.body });
  res.status(202).json({ jobId, statusUrl: `/reports/${jobId}/status` });
});
```

Front-freundliche Antworten

* Pagination-Meta mitsenden: `{ data, meta: { total, page, limit } }` oder `{ data, nextCursor }`.
* Optional serverseitiges ETag für idempotente GETs.

Zusammenfassung

* Für große Daten: **Cursor/Keyset-Pagination**, **Streams** (DB→Server→Client), **Komprimierung** und **Projektion**.
* **Indexe**, **keine N+1**, serverseitiges **Filtering/Sorting**.
* Teure Jobs **asynchron** verarbeiten; API gibt `202 Accepted` + Status zurück.
* Schütze RAM & Durchsatz mit **Backpressure**, **Limits**, **Rate-Limit** und **Caching**.

Quellen

* Node.js Streams & http/https: [https://nodejs.org/docs](https://nodejs.org/docs)
* Express – Performance/Security Best Practices: [https://expressjs.com/de/advanced/best-practice-performance.html](https://expressjs.com/de/advanced/best-practice-performance.html)
* PostgreSQL – Performance/Indexes: [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)
* Sequelize – Queries, Pagination, Attributes: [https://sequelize.org/](https://sequelize.org/)
* MDN Web Docs (RU) – HTTP Caching/Compression: [https://developer.mozilla.org/ru/](https://developer.mozilla.org/ru/)


  **[⬆ Наверх](#top)**

63. ### <a name="63"></a> Wie integriert man Swagger oder OpenAPI mit Express?

## Swagger / OpenAPI in Express integrieren

Ziele

* Interaktive API-Doku unter `/api-docs`.
* OpenAPI-Schema (JSON/YAML) pflegen; optional aus JSDoc generieren.

Variante A: OpenAPI aus JSDoc-Kommentaren (swagger-jsdoc) + Swagger UI

```bash
npm i swagger-ui-express swagger-jsdoc
```

```js
// src/app.js
import express from 'express';
import swaggerUi from 'swagger-ui-express';
import swaggerJSDoc from 'swagger-jsdoc';

const app = express();
app.use(express.json());

// OpenAPI-Definition (Basis)
const swaggerDefinition = {
  openapi: '3.0.3', // oder '3.1.0'
  info: {
    title: 'Meine REST API',
    version: '1.0.0',
    description: 'Beispiel-API mit Express + OpenAPI'
  },
  servers: [{ url: 'http://localhost:3000' }]
};

const options = {
  swaggerDefinition,
  apis: ['./src/routes/*.js'] // JSDoc-Quellen
};

const openapiSpec = swaggerJSDoc(options);

// UI unter /api-docs
app.use('/api-docs', swaggerUi.serve, swaggerUi.setup(openapiSpec));

// Beispielroute
app.get('/health', (req, res) => res.json({ status: 'ok' }));

export default app;
```

```js
// src/routes/users.routes.js
import { Router } from 'express';
const r = Router();

/**
 * @openapi
 * /users:
 *   get:
 *     summary: Liste aller Benutzer
 *     tags: [Users]
 *     parameters:
 *       - in: query
 *         name: page
 *         schema: { type: integer, minimum: 1, default: 1 }
 *     responses:
 *       200:
 *         description: Erfolgreich
 *         content:
 *           application/json:
 *             schema:
 *               type: object
 *               properties:
 *                 data:
 *                   type: array
 *                   items:
 *                     type: object
 *                     properties:
 *                       id:   { type: integer }
 *                       email:{ type: string, format: email }
 */
r.get('/users', (req, res) => {
  res.json({ data: [{ id: 1, email: 'user@example.com' }] });
});

export default r;
```

Variante B: Externe YAML/JSON-Spezifikation einbinden

```bash
npm i swagger-ui-express yaml
```

```js
// src/app.js
import express from 'express';
import swaggerUi from 'swagger-ui-express';
import { readFileSync } from 'node:fs';
import { parse as parseYaml } from 'yaml';

const app = express();
app.use(express.json());

const file = readFileSync('./openapi.yaml', 'utf8');
const openapiSpec = parseYaml(file);

app.use('/api-docs', swaggerUi.serve, swaggerUi.setup(openapiSpec));

export default app;
```

```yaml
# openapi.yaml (kurzer Ausschnitt)
openapi: 3.0.3
info:
  title: Meine REST API
  version: 1.0.0
servers:
  - url: http://localhost:3000
paths:
  /health:
    get:
      summary: Healthcheck
      responses:
        '200':
          description: OK
```

Tipps

* Security-Schemes definieren (z. B. Bearer JWT) und global referenzieren.
* Responses/Request-Bodies per `$ref` (Schemas) wiederverwenden.
* Für CI: OpenAPI mit Linter/Validator prüfen (z. B. `spectral`).
* In Produktion Basic-Auth für `/api-docs` erwägen oder nur nicht-prod aktivieren.

Zusammenfassung

* `swagger-ui-express` rendert die UI; Quelle ist ein OpenAPI-Schema.
* Schema entweder per **swagger-jsdoc** aus JSDoc-Kommentaren generieren (Variante A) oder als **YAML/JSON** pflegen (Variante B).
* UI unter `/api-docs`, Schema bei Bedarf auch roh unter `/openapi.json` ausliefern.

Quellen

* Express – Routing/Guide: [https://expressjs.com/de/](https://expressjs.com/de/)
* swagger-ui-express (npm): [https://www.npmjs.com/package/swagger-ui-express](https://www.npmjs.com/package/swagger-ui-express)
* swagger-jsdoc (npm): [https://www.npmjs.com/package/swagger-jsdoc](https://www.npmjs.com/package/swagger-jsdoc)
* OpenAPI-Spezifikation: [https://spec.openapis.org/](https://spec.openapis.org/)
* MDN (RU) – HTTP/Content types (allg. Grundlagen): [https://developer.mozilla.org/ru/](https://developer.mozilla.org/ru/)


  **[⬆ Наверх](#top)**

64. ### <a name="64"></a> Was ist ein DTO (Data Transfer Object) und wie nutzt man es in Express?

## DTO (Data Transfer Object) in Express

**Definition**
Ein **DTO (Data Transfer Object)** ist ein **Objekt, das Daten zwischen Schichten** einer Anwendung überträgt.

* Dient als **klar definierte Schnittstelle** für Eingaben/Ausgaben (z. B. zwischen Client ↔ API oder Controller ↔ Service).
* Schützt die interne Datenstruktur (z. B. DB-Modelle) vor direkter Exposition.
* Ermöglicht **Validierung, Transformation und Konsistenz** der Daten.

---

## Warum DTOs?

* **Trennung von Logik und Transport**: DB-Modelle ≠ API-Contracts.
* **Validierung**: z. B. mit Joi oder Zod.
* **Sicherheit**: Nur freigegebene Felder werden übertragen.
* **Flexibilität**: API kann sich entwickeln, ohne dass interne Models geändert werden müssen.

---

## Beispiel in Express mit Zod

### 1. DTO definieren

```js
// src/dto/user.dto.js
import { z } from 'zod';

export const CreateUserDto = z.object({
  email: z.string().email(),
  name: z.string().min(2),
  password: z.string().min(8)
});

export const UpdateUserDto = z.object({
  email: z.string().email().optional(),
  name: z.string().min(2).optional()
});
```

---

### 2. Middleware zur Validierung

```js
// src/middlewares/validate.js
export function validate(schema) {
  return (req, res, next) => {
    try {
      req.body = schema.parse(req.body);
      next();
    } catch (err) {
      return res.status(400).json({ error: err.errors });
    }
  };
}
```

---

### 3. Nutzung im Controller

```js
// src/routes/users.routes.js
import { Router } from 'express';
import { validate } from '../middlewares/validate.js';
import { CreateUserDto, UpdateUserDto } from '../dto/user.dto.js';

const r = Router();

r.post('/', validate(CreateUserDto), (req, res) => {
  const userDto = req.body; // validiertes DTO
  // DB-Insert hier, nur mit freigegebenen Feldern
  res.status(201).json({ message: 'User erstellt', user: userDto });
});

r.put('/:id', validate(UpdateUserDto), (req, res) => {
  const userDto = req.body; // validiertes Update-DTO
  // DB-Update hier
  res.json({ message: 'User aktualisiert', user: userDto });
});

export default r;
```

---

## Unterschied zu Modellen

* **Model (z. B. Sequelize, Mongoose):** beschreibt die Datenstruktur in der Datenbank.
* **DTO:** beschreibt, welche Daten **zwischen API und Client** fließen dürfen.

👉 Ein User-Model kann z. B. `passwordHash`, `createdAt` enthalten, aber das DTO nur `email` und `name`.

---

### Zusammenfassung

* **DTO = Datenobjekt für Transport zwischen Schichten.**
* In Express typischerweise für **Request-Validierung** und **Response-Formatierung** genutzt.
* Vorteil: Schutz der internen Models, Konsistenz der API, saubere Validierung.

**Quellen:**

* [Express.js – Best Practices](https://expressjs.com/de/advanced/best-practice-performance.html)
* [Zod – npm](https://www.npmjs.com/package/zod)
* [MDN – Datenvalidierung](https://developer.mozilla.org/ru/docs/Learn/Forms/Form_validation)

---

  **[⬆ Наверх](#top)**

65. ### <a name="65"></a> Wie testet man eine Express REST API?

## Wie testet man eine Express REST API?

**Ziele:** Routen/Controller testen (Statuscode, Header, Body), Fehlerfälle, Auth, Validierung, ohne echten Netzwerk-Port.
**Tools:** **Jest** (Test-Runner/Assertions) + **supertest** (HTTP gegen Express-App), Mocks für DB/Services.

---

### Projekt-Setup (ESM) – minimal

```js
// package.json (Ausschnitt)
{
  "type": "module",
  "scripts": { "test": "NODE_OPTIONS=--experimental-vm-modules jest --runInBand" },
  "devDependencies": { "jest": "^29.7.0", "supertest": "^6.3.4" }
}
```

```js
// jest.config.js
export default { testEnvironment: 'node', clearMocks: true };
```

```js
// src/app.js – App exportieren (nicht listen!)
import express from 'express';
import usersRouter from './routes/users.js';

const app = express();
app.use(express.json());
app.use('/api/v1/users', usersRouter);

// 404 + Error-Handler (gekürzt)
app.use((req, res) => res.status(404).json({ error: 'not found' }));
app.use((err, req, res, next) => res.status(err.status||500).json({ error: err.message }));

export default app;
```

---

### Beispiel-Router + Service (für Mocks)

```js
// src/routes/users.js
import { Router } from 'express';
import * as userService from '../services/user.service.js';
const r = Router();

r.get('/', async (req, res, next) => {
  try { res.json({ data: await userService.list() }); }
  catch (e) { next(e); }
});

r.post('/', async (req, res, next) => {
  try {
    const created = await userService.create(req.body);
    res.status(201).json(created);
  } catch (e) { e.status ??= 400; next(e); }
});

export default r;
```

---

### Integrationstests mit supertest (happy-path + Fehlerfälle)

```js
// test/users.test.js
import request from 'supertest';
import app from '../src/app.js';

// Service-Funktionen mocken (kein echter DB-Zugriff)
jest.unstable_mockModule('../src/services/user.service.js', () => ({
  list: jest.fn().mockResolvedValue([{ id: 1, email: 'a@b.de' }]),
  create: jest.fn(async (dto) => {
    if (!dto?.email) { const e = new Error('email required'); e.status = 422; throw e; }
    return { id: 2, ...dto };
  })
}));

// import NACH dem Mock
const userService = await import('../src/services/user.service.js');

describe('Users API', () => {
  test('GET /api/v1/users → 200 & data', async () => {
    const res = await request(app).get('/api/v1/users').expect(200);
    expect(res.body.data).toEqual([{ id: 1, email: 'a@b.de' }]);
    expect(userService.list).toHaveBeenCalled();
  });

  test('POST /api/v1/users → 201 bei validem Body', async () => {
    const res = await request(app)
      .post('/api/v1/users')
      .send({ email: 'x@y.de' })
      .expect(201);
    expect(res.body).toMatchObject({ id: 2, email: 'x@y.de' });
  });

  test('POST /api/v1/users → 422 bei Validierungsfehler', async () => {
    const res = await request(app).post('/api/v1/users').send({}).expect(422);
    expect(res.body.error).toMatch(/email/i);
  });

  test('GET unknown route → 404', async () => {
    await request(app).get('/nope').expect(404);
  });
});
```

---

### Auth/JWT testen (Header setzen)

```js
// Beispiel: geschützte Route
const token = 'Bearer eyJ...'; // ggf. Testtoken signen
await request(app)
  .get('/api/v1/secret')
  .set('Authorization', token)
  .expect(200);
```

---

### Performance & große Antworten (Streaming)

```js
// Chunked/NDJSON prüfen
const res = await request(app).get('/export-ndjson').expect(200);
expect(res.text.split('\n')[0]).toContain('{'); // grobe Prüfung erster Datensatz
```

---

### Best Practices

* **App von Server trennen** (exportierte `app` ohne `listen`) → supertest nutzt sie direkt.
* **DB/Externes** mocken (Service-/Repository-Schicht) → schnelle, deterministische Tests.
* **Error-Cases** abdecken: 400/401/403/404/409/422/500.
* **Validierung** separat testen (falsche/fehlende Felder).
* **Fixtures/Factory** für Testdaten, keine Zufallswerte ohne Seed.
* **runInBand** bei DB/Port-Konflikten, **Test-ENV** nutzen.
* **Coverage** für Controller/Middleware, aber nicht blind 100% erzwingen.

---

### Zusammenfassung

* Express-API testet man mit **Jest + supertest** ohne echten Port.
* **App exportieren**, **Services mocken**, **Happy- und Fehlerpfade** prüfen.
* Auth-Header, Streaming, Statuscodes/JSON-Formate gezielt testen.

**Quellen:**

* [Express.js – Testing-Hinweise](https://expressjs.com/de/advanced/best-practice-performance.html)
* [Node.js Dokumentation](https://nodejs.org/docs)
* [Jest Dokumentation](https://jestjs.io/)
* [supertest (npm)](https://www.npmjs.com/package/supertest)

---

  **[⬆ Наверх](#top)**

66. ### <a name="66"></a> Wie verbindet man Express mit einer Datenbank (z. B. MongoDB oder PostgreSQL)?

## Express mit Datenbanken verbinden (PostgreSQL & MongoDB)

### PostgreSQL – direkt mit `pg` (Connection Pool)

```js
// db/pg.js
import pg from 'pg';
export const pool = new pg.Pool({ connectionString: process.env.DATABASE_URL });

// Beispiel-Query (parametrisiert!)
export async function getUsers() {
  const { rows } = await pool.query('SELECT id, email FROM users ORDER BY id LIMIT $1', [50]);
  return rows;
}
```

```js
// app.js
import express from 'express';
import { getUsers } from './db/pg.js';

const app = express();
app.get('/users', async (req, res, next) => {
  try { res.json(await getUsers()); } catch (e) { next(e); }
});

export default app;
```

```js
// server.js
import app from './app.js';
import { pool } from './db/pg.js';

const PORT = process.env.PORT ?? 3000;
const server = app.listen(PORT, () => console.log(`API auf :${PORT}`));

// Graceful shutdown
for (const sig of ['SIGINT','SIGTERM']) {
  process.on(sig, async () => {
    await pool.end();
    server.close(() => process.exit(0));
  });
}
```

**Hinweise:** `.env` nutzen, Pool wiederverwenden, immer **parametrisierte Queries** (`$1, $2`).

---

### PostgreSQL – mit **Sequelize** (ORM)

```js
// db/sequelize.js
import { Sequelize, DataTypes, Model } from 'sequelize';

export const sequelize = new Sequelize(process.env.DATABASE_URL, {
  dialect: 'postgres', logging: false
});

export class User extends Model {}
User.init({
  email: { type: DataTypes.STRING, allowNull: false, unique: true, validate: { isEmail: true } },
  name:  { type: DataTypes.STRING, allowNull: false }
}, { sequelize, modelName: 'User', tableName: 'users' });

// Aufruf zum Start
export async function initDb() {
  await sequelize.authenticate();
  await sequelize.sync(); // in Prod: Migrations statt sync()
}
```

```js
// app.js (Ausschnitt)
import express from 'express';
import { User } from './db/sequelize.js';

const app = express();
app.use(express.json());

app.post('/users', async (req, res, next) => {
  try {
    const u = await User.create(req.body);
    res.status(201).json(u);
  } catch (e) { e.status ??= 400; next(e); }
});

export default app;
```

```js
// server.js
import app from './app.js';
import { initDb, sequelize } from './db/sequelize.js';

const PORT = process.env.PORT ?? 3000;
await initDb();
const server = app.listen(PORT, () => console.log(`API auf :${PORT}`));

for (const sig of ['SIGINT','SIGTERM']) {
  process.on(sig, async () => {
    await sequelize.close();
    server.close(() => process.exit(0));
  });
}
```

**Hinweise:** Models kapseln, DTO/Validierung vorschalten, Migrations nutzen (Sequelize CLI).

---

### MongoDB – mit **Mongoose**

```js
// db/mongoose.js
import mongoose from 'mongoose';

export async function connectMongo() {
  await mongoose.connect(process.env.MONGO_URI); // z. B. mongodb://localhost:27017/app
}

const userSchema = new mongoose.Schema({
  email: { type: String, required: true, unique: true, lowercase: true },
  name:  { type: String, required: true }
}, { timestamps: true });

export const UserModel = mongoose.model('User', userSchema);
```

```js
// app.js (Ausschnitt)
import express from 'express';
import { UserModel } from './db/mongoose.js';

const app = express();
app.use(express.json());

app.get('/users', async (req, res, next) => {
  try { res.json(await UserModel.find().limit(50).lean()); }
  catch (e) { next(e); }
});

export default app;
```

```js
// server.js
import app from './app.js';
import { connectMongo } from './db/mongoose.js';
import mongoose from 'mongoose';

const PORT = process.env.PORT ?? 3000;
await connectMongo();
const server = app.listen(PORT, () => console.log(`API auf :${PORT}`));

for (const sig of ['SIGINT','SIGTERM']) {
  process.on(sig, async () => {
    await mongoose.connection.close();
    server.close(() => process.exit(0));
  });
}
```

**Hinweise:** Indexe definieren (`schema.index()`), `.lean()` für schnellere Reads, Validierung/DTOs vorschalten.

---

### Zusammenfassung

* **PostgreSQL:** direkt mit `pg` (parametrisierte Queries, Pool) oder höher mit **Sequelize** (Modelle, Validierung, Migrations).
* **MongoDB:** **Mongoose** für Schema/Modelle, `.lean()` für Performance.
* Gemeinsames: `.env`, zentrale DB-Initialisierung, **graceful shutdown**, **Validierung**, Error-Handling, keine String-SQL.

**Quellen:**

* [Node.js – `pg` (PostgreSQL)](https://www.npmjs.com/package/pg) / [PostgreSQL Doku](https://www.postgresql.org/docs/)
* [Sequelize Offizielle Dokumentation](https://sequelize.org/)
* [Mongoose Dokumentation](https://mongoosejs.com/)
* [Express.js Offizielle Dokumentation](https://expressjs.com/de/)
* [Node.js Dokumentation](https://nodejs.org/docs)


  **[⬆ Наверх](#top)**

67. ### <a name="67"></a> Was ist Mongoose und wie wird es in Express verwendet?

## Was ist Mongoose und wie wird es in Express verwendet?

**Definition:**
Mongoose ist eine **Object Data Modeling (ODM) Bibliothek** für **MongoDB** in Node.js.

* Es definiert **Schemas und Modelle**, ähnlich wie ein ORM (z. B. Sequelize für SQL).
* Bietet **Validierung, Hooks, Query-APIs**, Middleware, Population (Joins-ähnlich) und erleichtert die Arbeit mit MongoDB in Express-Apps.

---

## Grundprinzip

1. **Schema** definieren → beschreibt die Struktur und Constraints einer Collection.
2. **Model** erstellen → repräsentiert die Collection in der App.
3. **CRUD**-Operationen ausführen → mit Mongoose-Methoden statt roher MongoDB-Queries.

---

## Beispiel: Integration in Express

### 1. Setup

```bash
npm install mongoose
```

```js
// db/mongoose.js
import mongoose from 'mongoose';

export async function connectMongo() {
  await mongoose.connect(process.env.MONGO_URI, {
    dbName: 'myapp', // optional, falls nicht in URI
  });
  console.log('MongoDB verbunden');
}
```

---

### 2. Schema & Modell

```js
// models/user.model.js
import mongoose from 'mongoose';

const userSchema = new mongoose.Schema({
  email: { type: String, required: true, unique: true, lowercase: true },
  name:  { type: String, required: true },
  age:   { type: Number, min: 0 },
}, { timestamps: true }); // createdAt, updatedAt automatisch

export const User = mongoose.model('User', userSchema);
```

---

### 3. Nutzung in Express-Routen

```js
// routes/users.routes.js
import { Router } from 'express';
import { User } from '../models/user.model.js';

const r = Router();

r.get('/', async (req, res, next) => {
  try {
    const users = await User.find().limit(20).lean(); // lean() → schneller, nur Plain-Objekte
    res.json({ data: users });
  } catch (e) { next(e); }
});

r.post('/', async (req, res, next) => {
  try {
    const user = await User.create(req.body); // Validierung durch Schema
    res.status(201).json(user);
  } catch (e) { e.status ??= 400; next(e); }
});

export default r;
```

---

### 4. Server-Start

```js
// server.js
import express from 'express';
import { connectMongo } from './db/mongoose.js';
import usersRouter from './routes/users.routes.js';
import mongoose from 'mongoose';

const app = express();
app.use(express.json());
app.use('/api/v1/users', usersRouter);

await connectMongo();

const PORT = process.env.PORT ?? 3000;
const server = app.listen(PORT, () => console.log(`API läuft auf :${PORT}`));

for (const sig of ['SIGINT','SIGTERM']) {
  process.on(sig, async () => {
    await mongoose.connection.close();
    server.close(() => process.exit(0));
  });
}
```

---

## Vorteile von Mongoose

* **Schemas + Validierung** → Typsicherheit für MongoDB.
* **Middleware/Hooks** (z. B. `pre('save')`, `post('remove')`).
* **Population** → Referenzen zwischen Collections ähnlich wie Joins.
* **Virtuals** → Felder, die nicht in DB gespeichert werden (z. B. `fullName`).
* **Indexes** deklarativ im Schema.

---

### Zusammenfassung

* **Mongoose = ODM für MongoDB** in Node.js/Express.
* Definiert **Schemas und Models**, die Validierung + Query-APIs bieten.
* Typische Verwendung in Express:

  * DB-Connection aufbauen,
  * Models importieren,
  * in Routen CRUD-Operationen mit Mongoose nutzen.

**Quellen:**

* [Mongoose Offizielle Dokumentation](https://mongoosejs.com/)
* [Express.js Dokumentation](https://expressjs.com/de/)
* [MDN – MongoDB Überblick](https://developer.mozilla.org/ru/docs/Glossary/MongoDB)

---

  **[⬆ Наверх](#top)**

68. ### <a name="68"></a> Wie implementiert man ein Repository Pattern mit Express?

## Repository Pattern mit Express implementieren

Ziel

* Controller/Route kennen **nur die Domänen-Methoden** (z. B. `createUser`, `getUserById`), nicht die DB-Details.
* Austauschbar: PostgreSQL via Sequelize/pg, MongoDB via Mongoose, … durch **Repository-Implementierungen**.

Ordnerstruktur (Beispiel)

```
src/
  app.js
  routes/
    users.routes.js
  controllers/
    users.controller.js
  services/
    users.service.js
  repositories/
    users.repository.js          // Interface/Abstraktion
    users.repository.sequelize.js// konkrete Implementierung
  db/
    sequelize.js
  validators/
    users.schema.js
```

Repository-Interface (Abstraktion)

```js
// src/repositories/users.repository.js
export class UsersRepository {
  async findById(id)            { throw new Error('not implemented'); }
  async findAll({ offset, limit }) { throw new Error('not implemented'); }
  async create(dto)             { throw new Error('not implemented'); }
  async update(id, dto)         { throw new Error('not implemented'); }
  async remove(id)              { throw new Error('not implemented'); }
}
```

Konkrete Implementierung (Sequelize, PostgreSQL)

```js
// src/repositories/users.repository.sequelize.js
import { UsersRepository } from './users.repository.js';
import { User } from '../db/sequelize.js';

export class SequelizeUsersRepository extends UsersRepository {
  async findById(id) {
    return User.findByPk(id);
  }
  async findAll({ offset = 0, limit = 10 } = {}) {
    const { rows, count } = await User.findAndCountAll({
      offset, limit, order: [['id', 'ASC']],
      attributes: ['id', 'email', 'name', 'role']
    });
    return { rows, count };
  }
  async create(dto) {
    return User.create(dto);
  }
  async update(id, dto) {
    const u = await User.findByPk(id);
    if (!u) return null;
    await u.update(dto);
    return u;
  }
  async remove(id) {
    const u = await User.findByPk(id);
    if (!u) return 0;
    await u.destroy();
    return 1;
  }
}
```

Service-Schicht (Geschäftslogik; nimmt ein Repository entgegen → testbar)

```js
// src/services/users.service.js
export class UsersService {
  constructor(usersRepo) { this.usersRepo = usersRepo; }

  async list({ page = 1, limit = 10 }) {
    const offset = (Number(page) - 1) * Number(limit);
    const { rows, count } = await this.usersRepo.findAll({ offset, limit: Number(limit) });
    return { data: rows, meta: { page: Number(page), limit: Number(limit), total: count } };
  }

  async get(id) {
    const user = await this.usersRepo.findById(id);
    if (!user) {
      const e = new Error('User nicht gefunden'); e.status = 404; throw e;
    }
    return user;
    }

  async create(dto) {
    // Beispiel: Business-Validierung
    // if (!dto.role) dto.role = 'user';
    return this.usersRepo.create(dto);
  }

  async update(id, dto) {
    const u = await this.usersRepo.update(id, dto);
    if (!u) { const e = new Error('User nicht gefunden'); e.status = 404; throw e; }
    return u;
  }

  async remove(id) {
    const n = await this.usersRepo.remove(id);
    if (!n) { const e = new Error('User nicht gefunden'); e.status = 404; throw e; }
    return;
  }
}
```

Controller/Handler (kennt nur Service)

```js
// src/controllers/users.controller.js
export class UsersController {
  constructor(usersService) { this.svc = usersService; }

  list = async (req, res, next) => {
    try { res.json(await this.svc.list(req.query)); } catch (e) { next(e); }
  };

  get = async (req, res, next) => {
    try { res.json(await this.svc.get(req.params.id)); } catch (e) { next(e); }
  };

  create = async (req, res, next) => {
    try { const u = await this.svc.create(req.body); res.status(201).json(u); }
    catch (e) { e.status ??= 400; next(e); }
  };

  update = async (req, res, next) => {
    try { res.json(await this.svc.update(req.params.id, req.body)); }
    catch (e) { e.status ??= 400; next(e); }
  };

  remove = async (req, res, next) => {
    try { await this.svc.remove(req.params.id); res.status(204).send(); }
    catch (e) { next(e); }
  };
}
```

Router (einfache “Composition/DI”)

```js
// src/routes/users.routes.js
import { Router } from 'express';
import { UsersController } from '../controllers/users.controller.js';
import { UsersService } from '../services/users.service.js';
import { SequelizeUsersRepository } from '../repositories/users.repository.sequelize.js';

const repo = new SequelizeUsersRepository();
const svc  = new UsersService(repo);
const ctrl = new UsersController(svc);

const r = Router();
r.get('/', ctrl.list);
r.get('/:id', ctrl.get);
r.post('/', ctrl.create);
r.put('/:id', ctrl.update);
r.delete('/:id', ctrl.remove);
export default r;
```

Sequelize-Setup (Beispiel)

```js
// src/db/sequelize.js
import { Sequelize, DataTypes, Model } from 'sequelize';

export const sequelize = new Sequelize(process.env.DATABASE_URL, {
  dialect: 'postgres', logging: false
});

export class User extends Model {}
User.init({
  email: { type: DataTypes.STRING, allowNull: false, unique: true, validate: { isEmail: true } },
  name:  { type: DataTypes.STRING, allowNull: false },
  role:  { type: DataTypes.ENUM('user','admin'), allowNull: false, defaultValue: 'user' }
}, { sequelize, modelName: 'User', tableName: 'users' });
```

App einbinden

```js
// src/app.js
import express from 'express';
import usersRouter from './routes/users.routes.js';

const app = express();
app.use(express.json());
app.use('/api/v1/users', usersRouter);

// Fehler-Handling (gekürzt)
app.use((req, res) => res.status(404).json({ error: 'Route nicht gefunden' }));
app.use((err, req, res, next) => res.status(err.status||500).json({ error: err.message }));

export default app;
```

Testbarkeit (Unit-Tests ohne DB)

```js
// Beispielhafte Mock-Repo-Instanz
class InMemoryUsersRepo {
  constructor() { this.data = [{ id: 1, email: 'a@b.de', name: 'A', role: 'user' }]; }
  async findAll() { return { rows: this.data, count: this.data.length }; }
  async findById(id) { return this.data.find(u => u.id == id) ?? null; }
  async create(dto) { const u = { id: Date.now(), ...dto }; this.data.push(u); return u; }
  async update(id, dto) { const i = this.data.findIndex(u => u.id == id); if (i<0) return null; this.data[i] = { ...this.data[i], ...dto }; return this.data[i]; }
  async remove(id) { const i = this.data.findIndex(u => u.id == id); if (i<0) return 0; this.data.splice(i,1); return 1; }
}
// → In Tests: `new UsersService(new InMemoryUsersRepo())`
```

Optionen/Varianten

* Mehrere Implementierungen (Sequelize/pg/Mongoose) parallel nutzbar; Auswahl per ENV.
* Transaktionen im Repository kapseln (z. B. `sequelize.transaction(...)`).
* Mapping/DTOs im Service/Controller, damit das Repository **nur DB-Details** kapselt.
* Caching (z. B. Redis) als Dekorator ums Repository implementieren.

Zusammenfassung

* Repository Pattern trennt **Datenzugriff** von **Business-Logik** und **HTTP-Schicht**.
* Express-Controller sprechen Services an; Services nutzen **Repositories** (austauschbar, testbar).
* Vorteile: bessere Testbarkeit, klare Verantwortlichkeiten, einfacher DB-Switch/Refactor.

Quellen

* Express.js – Routing/Strukturierung: [https://expressjs.com/de/guide/routing.html](https://expressjs.com/de/guide/routing.html)
* Node.js – Module/Best Practices: [https://nodejs.org/docs](https://nodejs.org/docs)
* Sequelize – Models/Queries/Transaktionen: [https://sequelize.org/](https://sequelize.org/)
* MDN Web Docs (RU) – Архитектурные паттерны/слои (allg. Konzepte): [https://developer.mozilla.org/ru/](https://developer.mozilla.org/ru/)


  **[⬆ Наверх](#top)**

69. ### <a name="69"></a> Unterschied zwischen SQL- und NoSQL-Integration in Express?

## Unterschied zwischen SQL- und NoSQL-Integration in Express

**1. Datenmodellierung**

* **SQL (z. B. PostgreSQL, MySQL):**

  * Tabellen, Zeilen, Spalten (relational, streng typisiert).
  * Beziehungen via **Joins**.
  * Schema muss meist im Voraus definiert werden.
* **NoSQL (z. B. MongoDB):**

  * Dokumente (JSON/BSON), Collections.
  * Beziehungen oft durch **Referenzen** oder **Embedded Documents**.
  * Flexibler, Schema optional (Schema on Read), aber Validierung wird auf App-Ebene benötigt.

---

**2. Bibliotheken in Express**

* **SQL:**

  * Low-Level: [`pg`](https://www.npmjs.com/package/pg) (PostgreSQL), [`mysql2`](https://www.npmjs.com/package/mysql2).
  * ORM/Query-Builder: Sequelize, TypeORM, Knex.
* **NoSQL:**

  * MongoDB: [Mongoose](https://mongoosejs.com/) (ODM), `mongodb` Node.js Driver.

---

**3. Verbindungsaufbau**
SQL (PostgreSQL via `pg`):

```js
import pg from 'pg';
const pool = new pg.Pool({ connectionString: process.env.DATABASE_URL });

app.get('/users', async (req, res, next) => {
  try {
    const { rows } = await pool.query('SELECT id, email FROM users');
    res.json(rows);
  } catch (e) { next(e); }
});
```

NoSQL (MongoDB via Mongoose):

```js
import mongoose from 'mongoose';
await mongoose.connect(process.env.MONGO_URI);

const User = mongoose.model('User', new mongoose.Schema({
  email: { type: String, required: true, unique: true }
}));

app.get('/users', async (req, res, next) => {
  try {
    const users = await User.find().lean();
    res.json(users);
  } catch (e) { next(e); }
});
```

---

**4. Transaktionen & Konsistenz**

* **SQL:** ACID-Transaktionen out of the box (`BEGIN`, `COMMIT`, `ROLLBACK`).
* **NoSQL (MongoDB):** Lange Zeit keine echten Multi-Dokument-Transaktionen, inzwischen ab MongoDB 4.0 verfügbar, aber teurer.

---

**5. Querying**

* **SQL:** deklarative Abfragen (JOIN, GROUP BY, Window Functions).
* **NoSQL:** flexible JSON-Queries, Aggregation-Pipelines, weniger stark typisiert.

---

**6. Skalierung**

* **SQL:** vertikale Skalierung (eine starke DB), horizontale Sharding-Ansätze sind komplex.
* **NoSQL:** horizontale Skalierung/Sharding eingebaut (z. B. MongoDB).

---

**7. Typische Einsatzszenarien**

* **SQL:** strukturierte Daten, viele Beziehungen, strenge Konsistenz (Banking, ERP).
* **NoSQL:** flexible/halb-strukturierte Daten, schnelle Iteration, hohe Skalierbarkeit (E-Commerce, IoT, Logging).

---

### Zusammenfassung

* **SQL in Express:** strukturierte Daten mit Joins, Anbindung via `pg`/ORM, ACID-Transaktionen.
* **NoSQL in Express:** flexible JSON-Dokumente, Anbindung via `mongoose`/Driver, horizontale Skalierung leichter.
* Wahl hängt ab von: **Datenstruktur**, **Konsistenzanforderungen**, **Skalierung** und **Entwicklungsgeschwindigkeit**.

**Quellen:**

* [PostgreSQL Dokumentation](https://www.postgresql.org/docs/)
* [Mongoose Dokumentation](https://mongoosejs.com/)
* [Express.js Offizielle Dokumentation](https://expressjs.com/de/)
* [MDN (RU) – NoSQL/SQL Überblick](https://developer.mozilla.org/ru/docs/Glossary/NoSQL)

---

  **[⬆ Наверх](#top)**

70. ### <a name="70"></a> Wie arbeitet man mit ORMs (z. B. Sequelize, Prisma) in Express?

## Arbeiten mit ORMs in Express (Sequelize & Prisma)

**Ziele:** Datenzugriff kapseln, Validierung/Relationen nutzen, Migrations/Transaktionen sicher anwenden, saubere Schichten (Routes → Controller → Service/Repository → ORM).

---

### Sequelize – Setup & Grundmuster

```js
// db/sequelize.js
import { Sequelize, DataTypes, Model } from 'sequelize';

export const sequelize = new Sequelize(process.env.DATABASE_URL, {
  dialect: 'postgres',
  logging: false
});

export class User extends Model {}
User.init({
  email: { type: DataTypes.STRING, allowNull: false, unique: true, validate: { isEmail: true } },
  name:  { type: DataTypes.STRING, allowNull: false }
}, { sequelize, modelName: 'User', tableName: 'users' });

export async function initDb() {
  await sequelize.authenticate();
  await sequelize.sync(); // In Produktion: Migrations statt sync()
}
```

```js
// routes/users.routes.js
import { Router } from 'express';
import { User } from '../db/sequelize.js';

const r = Router();

r.get('/', async (req, res, next) => {
  try {
    const users = await User.findAll({ attributes: ['id', 'email', 'name'], order: [['id', 'ASC']] });
    res.json({ data: users });
  } catch (e) { next(e); }
});

r.post('/', async (req, res, next) => {
  try {
    const u = await User.create(req.body); // Sequelize validiert nach Model-Definition
    res.status(201).json(u);
  } catch (e) { e.status ??= 400; next(e); }
});

export default r;
```

**Transaktionen (z. B. zwei Inserts atomar):**

```js
// services/user.service.js
import { sequelize } from '../db/sequelize.js';
import { User } from '../db/sequelize.js';

export async function createUserWithAudit(dto) {
  return sequelize.transaction(async (t) => {
    const user = await User.create(dto, { transaction: t });
    await sequelize.query(
      'INSERT INTO audit_log(action, entity, entity_id) VALUES ($1,$2,$3)',
      { bind: ['CREATE', 'User', user.id], transaction: t }
    );
    return user;
  });
}
```

**Migrations (Hinweis):** In Produktion die Sequelize-CLI nutzen (`sequelize-cli db:migrate`) statt `sync()`.

---

### Prisma – Setup & Grundmuster

* Prisma generiert einen **TypeScript/JS-Client** aus dem Datenmodell (in `schema.prisma`).
* Starke Typisierung der Queries (auch in JS nützlich durch klare API), sehr gute DX.

```js
// db/prisma.js
import { PrismaClient } from '@prisma/client';
export const prisma = new PrismaClient();
```

```js
// routes/users.prisma.routes.js
import { Router } from 'express';
import { prisma } from '../db/prisma.js';

const r = Router();

r.get('/', async (req, res, next) => {
  try {
    const users = await prisma.user.findMany({
      select: { id: true, email: true, name: true },
      orderBy: { id: 'asc' }
    });
    res.json({ data: users });
  } catch (e) { next(e); }
});

r.post('/', async (req, res, next) => {
  try {
    const u = await prisma.user.create({ data: req.body });
    res.status(201).json(u);
  } catch (e) { e.status ??= 400; next(e); }
});

export default r;
```

**Transaktionen (Prisma):**

```js
// services/user.prisma.service.js
import { prisma } from '../db/prisma.js';

export async function createUserWithAudit(dto) {
  return prisma.$transaction(async (tx) => {
    const user = await tx.user.create({ data: dto });
    await tx.audit_log.create({ data: { action: 'CREATE', entity: 'User', entityId: user.id } });
    return user;
  });
}
```

---

### Gemeinsame Best Practices (beide ORMs)

* **Schichten trennen:** Controller dünn halten, Business-Logik in Services, DB-Zugriff in Repository/Service.
* **Validierung/DTOs:** Vor ORM-Call Eingaben prüfen (z. B. Zod/Joi).
* **Projektion:** Nur benötigte Felder selektieren (`attributes` bei Sequelize / `select` bei Prisma).
* **Pagination:** Offset/Limit oder Cursor/Keyset; keine Full-Table-Reads.
* **Transaktionen:** Für zusammengehörige Änderungen zwingend nutzen.
* **Migrations:** Schema-Änderungen nur über Migrations-Tool des ORM.
* **Fehlerbehandlung:** Ein zentraler Error-Handler; ORM-Fehler (Unique, FK) in sinnvolle HTTP-Codes mappen (`409`, `422`).
* **Security:** Keine String-Konkatenation; bei Roh-SQL **Bindings** verwenden.
* **Tests:** DB-Zugriff mocken (Repository-Pattern) oder Test-DB/Transactions je Test zurückrollen.

---

### Wann welches ORM?

* **Sequelize:** Reif, flexibel, breite Community; gut, wenn man aktiv mit Models/Associations arbeitet oder Raw-SQL mischen will.
* **Prisma:** Sehr produktiv, klares API, starke Typen, schnelle Migrations; ideal für Greenfield-Projekte und klare Domänenmodelle.

---

### Zusammenfassung

* In Express binden ORMs wie **Sequelize** und **Prisma** DB-Zugriff sauber ein: Models/Client, Validierung, Transaktionen, Migrations.
* Controller bleiben schlank; **Services/Repositories** kapseln ORM-Logik.
* Nutzen: **Konsistenz, Sicherheit, Wartbarkeit** und klare API-Verträge (DTOs/Validierung).

**Quellen:**

* [Express.js Offizielle Dokumentation](https://expressjs.com/de/)
* [Node.js Dokumentation](https://nodejs.org/docs)
* [PostgreSQL Dokumentation](https://www.postgresql.org/docs/)
* [Sequelize Offizielle Dokumentation](https://sequelize.org/)
* [MDN Web Docs (RU) – HTTP/REST-Grundlagen](https://developer.mozilla.org/ru/)


  **[⬆ Наверх](#top)**

71. ### <a name="71"></a> Wie behandelt man Transaktionen in Express?

## Transaktionen in Express behandeln

Grundidee

* Transaktionen gehören in die **Service-/Repository-Schicht**, nicht in die Controller.
* Bei Fehlern: **Rollback**, bei Erfolg: **Commit**.
* Einheitliches Error-Handling: DB-Fehler (Unique, FK, Deadlocks) in passende HTTP-Codes mappen.

---

Sequelize (PostgreSQL): „managed transaction“

```js
// services/order.service.js
import { sequelize } from '../db/sequelize.js';
import { Order, OrderItem, Product } from '../db/models.js';

export async function createOrder(dto) {
  return sequelize.transaction(async (t) => {
    const order = await Order.create({ userId: dto.userId }, { transaction: t });

    for (const it of dto.items) {
      const product = await Product.findByPk(it.productId, { transaction: t });
      if (!product) {
        const e = new Error('Produkt nicht gefunden'); e.status = 404; throw e;
      }
      await OrderItem.create({
        orderId: order.id, productId: product.id, qty: it.qty
      }, { transaction: t });
    }

    return order; // Commit automatisch bei erfolgreichem Abschluss
  });
}
```

Sequelize: „unmanaged transaction“ (manuelles `commit`/`rollback`)

```js
import { sequelize } from '../db/sequelize.js';
import { Payment } from '../db/models.js';

export async function settlePayment(dto) {
  const t = await sequelize.transaction({ isolationLevel: 'READ COMMITTED' });
  try {
    const p = await Payment.create(dto, { transaction: t });
    // ... weitere DB-Calls
    await t.commit();
    return p;
  } catch (err) {
    await t.rollback();
    throw err;
  }
}
```

---

Node-Postgres (`pg`): klassische Transaktion

```js
// services/user.service.js
import pg from 'pg';
const pool = new pg.Pool({ connectionString: process.env.DATABASE_URL });

export async function registerUser({ email, name }) {
  const client = await pool.connect();
  try {
    await client.query('BEGIN');
    const { rows: [user] } = await client.query(
      'INSERT INTO users(email,name) VALUES($1,$2) RETURNING id,email,name',
      [email, name]
    );
    await client.query(
      'INSERT INTO audit_log(action, entity, entity_id) VALUES ($1,$2,$3)',
      ['CREATE', 'User', user.id]
    );
    await client.query('COMMIT');
    return user;
  } catch (e) {
    await client.query('ROLLBACK');
    throw e;
  } finally {
    client.release();
  }
}
```

Isolation Level in PostgreSQL steuern

```js
await client.query('BEGIN ISOLATION LEVEL REPEATABLE READ'); // oder SERIALIZABLE/READ COMMITTED
```

---

Prisma: Transaktion mit Callback

```js
// services/invoice.service.js
import { prisma } from '../db/prisma.js';

export async function createInvoice(dto) {
  return prisma.$transaction(async (tx) => {
    const inv = await tx.invoice.create({ data: { customerId: dto.customerId } });
    for (const line of dto.lines) {
      await tx.invoiceLine.create({ data: { invoiceId: inv.id, ...line } });
    }
    return inv; // Commit bei Erfolg
  });
}
```

---

Pattern: Transaktion in Service nutzen (Controller bleibt schlank)

```js
// controllers/order.controller.js
import * as svc from '../services/order.service.js';

export async function create(req, res, next) {
  try {
    const order = await svc.createOrder(req.body);
    res.status(201).json(order);
  } catch (e) { next(e); }
}
```

---

Tipps & Best Practices

* **Transaktionsgrenzen klein** halten (nur notwendige DB-Operationen).
* **Retry** bei `SERIALIZATION_FAILURE`/Deadlocks (exponentielles Backoff).
* **Konsistente Fehlercodes**: z. B. Unique-Verletzung → `409 Conflict`, Validierungsfehler → `422`.
* Bei Sequelize Raw-SQL stets mit **Bindings** arbeiten, in Transaktion: `{ transaction: t }`.
* Keine per-Request-Auto-Transaktion als globale Middleware erzwingen; explizit pro Use-Case im Service ist klarer/testbarer.
* In Produktion Migrations nutzen (keine Schema-Änderungen innerhalb Business-Transaktionen).

---

Zusammenfassung

* Transaktionen kapselt man in der **Service-Schicht**; Controller ruft nur an.
* Sequelize/Prisma bieten bequeme **Callback-Transaktionen**; `pg` nutzt klassisches `BEGIN/COMMIT/ROLLBACK`.
* Bei Fehlern Rollback, bei Erfolg Commit; Fehler sauber mappen und ggf. **Retries** vorsehen.

Quellen

* Express.js Offizielle Dokumentation: [https://expressjs.com/de/](https://expressjs.com/de/)
* Node.js Dokumentation (Process/Streams/DB-Basics): [https://nodejs.org/docs](https://nodejs.org/docs)
* PostgreSQL Dokumentation (Transaktionen/Isolation): [https://www.postgresql.org/docs/](https://www.postgresql.org/docs/)
* Sequelize Offizielle Dokumentation (Transaction API): [https://sequelize.org/](https://sequelize.org/)
* Prisma Dokumentation (`$transaction`): [https://www.prisma.io/docs/](https://www.prisma.io/docs/)


  **[⬆ Наверх](#top)**

72. ### <a name="72"></a> Wie implementiert man ein Logging-System in Express?

## Logging in Express: Strategien & Umsetzung

Ziele

* **Request-Logs** (Methode, URL, Dauer, Status).
* **Strukturierte Logs** (JSON) für Produktion; **lesbar** in Entwicklung.
* **Levels** (debug, info, warn, error), **Error-Stacktraces**, **Korrelation** (Request-ID).
* **Rotation/Transporte** (Datei, Konsole, ggf. APM/ELK).

---

### 1) Schnellstart: `morgan` (HTTP-Access-Logs)

```js
import express from 'express';
import morgan from 'morgan';

const app = express();

// Dev: farbig/kurz; Prod: kombiniertes Format
app.use(morgan(process.env.NODE_ENV === 'production' ? 'combined' : 'dev'));

app.get('/health', (req, res) => res.json({ status: 'ok' }));

app.listen(3000, () => console.log('Server auf 3000'));
```

* Gut für **Request-Logs**; weniger für App-Logs/Strukturierung.

---

### 2) Strukturierte Logs mit **pino** / **pino-http** (empfohlen Prod)

```js
import express from 'express';
import pino from 'pino';
import pinoHttp from 'pino-http';

const logger = pino({
  level: process.env.LOG_LEVEL ?? 'info',
  transport: process.env.NODE_ENV === 'production' ? undefined : { target: 'pino-pretty' }
});

const app = express();
app.use(pinoHttp({ logger, customProps: (req) => ({ requestId: req.id }) }));

app.get('/work', (req, res) => {
  req.log.info({ step: 'start' }, 'processing'); // pro-Request Logger
  res.json({ ok: true });
});

// Zentraler Error-Handler loggt Fehler
app.use((err, req, res, next) => {
  req.log?.error({ err }, 'unhandled error');
  res.status(500).json({ error: 'Internal error' });
});

app.listen(3000, () => logger.info('Server auf 3000'));
```

* **JSON-Logs** (maschinenlesbar), sehr schnell, Request-gebundener Logger.

---

### 3) Alternativ: **winston** (Transporte/Rotation)

```js
import express from 'express';
import winston from 'winston';
import 'winston-daily-rotate-file';

const transports = [
  new winston.transports.Console({ level: 'info' }),
  new winston.transports.DailyRotateFile({
    dirname: 'logs', filename: 'app-%DATE%.log', datePattern: 'YYYY-MM-DD', maxFiles: '14d',
    level: 'info'
  })
];

export const logger = winston.createLogger({
  level: process.env.LOG_LEVEL ?? 'info',
  format: winston.format.json(),
  transports
});

const app = express();

app.use((req, res, next) => {
  const start = process.hrtime.bigint();
  res.on('finish', () => {
    const durMs = Number((process.hrtime.bigint() - start) / 1000000n);
    logger.info({ method: req.method, url: req.originalUrl, status: res.statusCode, durMs });
  });
  next();
});

app.get('/users', (req, res) => res.json([]));

app.use((err, req, res, next) => {
  logger.error({ err, path: req.originalUrl });
  res.status(500).json({ error: 'Internal error' });
});

app.listen(3000, () => logger.info('Server auf 3000'));
```

* Flexible **Transporte** (Konsole, Datei, Rotate, HTTP).

---

### 4) Request-ID / Korrelation (Tracing-Light)

```js
import { randomUUID } from 'node:crypto';

function requestId() {
  return (req, res, next) => {
    req.id = req.headers['x-request-id'] || randomUUID();
    res.setHeader('X-Request-Id', req.id);
    next();
  };
}

// Mit pino-http kombinieren:
app.use(requestId());
```

* Jede Logzeile enthält `requestId` → einfaches Suchen in Logs.

---

### 5) Best Practices

* **Dev:** pretty-Logs (pino-pretty), **Prod:** JSON (maschinenlesbar).
* **Levels:** `debug` für Detail, `info` normal, `warn` erwartbare Probleme, `error` unerwartet.
* **Kein PII** loggen (Passwörter, Tokens, personenbezogene Daten).
* **Error-Logs** mit Stacktrace (aber keine sensiblen Daten an Client).
* **Rotation**/Retention konfigurieren (Dateisystem) oder **Stdout** an Log-Aggregation (Docker/K8s).
* **Health/Noise** dämpfen (z. B. `/health` nur auf `debug`).
* **Korrelation**: `X-Request-Id`, ggf. Trace-Header (W3C Trace Context).

---

### 6) Kombination mit Middleware/Fehler-Handling

* Früh `app.use(loggerMiddleware)` registrieren → alle Requests erfasst.
* **Zentraler Error-Handler** protokolliert `err` und liefert JSON-Fehler.
* Für **langsame** Requests Warnung (z. B. `durMs > 1000`).

---

### Zusammenfassung

* Für HTTP-Access: **morgan** (einfach).
* Für strukturierte, schnelle Prod-Logs: **pino/pino-http** (JSON, pretty in Dev).
* Für vielfältige Transporte/Rotation: **winston**.
* Essentials: **Levels**, **Request-ID**, **Error-Logs**, **keine sensiblen Daten**, **Rotation/Aggregation**.

**Quellen:**

* Express.js – Best Practices: [https://expressjs.com/de/advanced/best-practice-performance.html](https://expressjs.com/de/advanced/best-practice-performance.html)
* Node.js Dokumentation (Console/Streams/Process): [https://nodejs.org/docs](https://nodejs.org/docs)
* morgan (npm): [https://www.npmjs.com/package/morgan](https://www.npmjs.com/package/morgan)
* pino & pino-http: [https://www.npmjs.com/package/pino](https://www.npmjs.com/package/pino) , [https://www.npmjs.com/package/pino-http](https://www.npmjs.com/package/pino-http)
* winston: [https://www.npmjs.com/package/winston](https://www.npmjs.com/package/winston)


  **[⬆ Наверх](#top)**

73. ### <a name="73"></a> Wie integriert man Caching (z. B. Redis) in Express?

## Caching in Express mit Redis integrieren

Ziele

* Häufige, teure Responses zwischenspeichern (Reads beschleunigen).
* TTL/Invalidierung bei Mutationen.
* Ebenen: HTTP-Cache-Header + Server-seitiger Cache (Redis).

---

### 1) Redis-Client verbinden (ESM)

```js
// cache/redis.js
import Redis from 'ioredis';

export const redis = new Redis(process.env.REDIS_URL ?? 'redis://localhost:6379', {
  lazyConnect: true,
  maxRetriesPerRequest: 3
});

export async function connectRedis() {
  await redis.connect?.(); // ioredis verbindet sonst eager
  redis.on('error', (e) => console.error('Redis error:', e));
}
```

Server-Start:

```js
// server.js
import express from 'express';
import { connectRedis } from './cache/redis.js';
import routes from './routes.js';

const app = express();
app.use(express.json());
app.use(routes);

await connectRedis();

const PORT = process.env.PORT ?? 3000;
app.listen(PORT, () => console.log(`Server auf :${PORT}`));
```

---

### 2) Einfache Response-Caching-Middleware (GET)

```js
// cache/middleware.js
import { redis } from './redis.js';

export function cache({ ttlSec = 60, keyFn } = {}) {
  return async (req, res, next) => {
    try {
      const key = keyFn ? keyFn(req) : `cache:${req.method}:${req.originalUrl}`;
      if (req.method !== 'GET') return next();

      const hit = await redis.get(key);
      if (hit) {
        res.set('X-Cache', 'HIT');
        return res.type('application/json').send(hit);
      }

      // Response abfangen
      const originalJson = res.json.bind(res);
      res.json = (body) => {
        // nur serialisierbare Bodies cachen
        Promise.resolve(redis.setex(key, ttlSec, JSON.stringify(body))).catch(()=>{});
        res.set('X-Cache', 'MISS');
        return originalJson(body);
      };

      next();
    } catch (e) {
      next(); // bei Cache-Problemen normal weiter
    }
  };
}
```

Verwendung pro Route:

```js
// routes.js
import { Router } from 'express';
import { cache } from './cache/middleware.js';
import { getUsersFromDb, createUserInDb, updateUserInDb, deleteUserInDb } from './svc.js';

const r = Router();

r.get('/api/v1/users',
  cache({ ttlSec: 120, keyFn: (req) => `users:list:${req.query.page ?? 1}:${req.query.limit ?? 10}` }),
  async (req, res, next) => {
    try {
      const data = await getUsersFromDb(req.query);
      res.json({ data });
    } catch (e) { next(e); }
  }
);

export default r;
```

---

### 3) Cache-Invalidierung bei Mutationen (Write-Through / Delete-Keys)

```js
// routes.js (fortgesetzt)
import { redis } from './cache/redis.js';

r.post('/api/v1/users', async (req, res, next) => {
  try {
    const created = await createUserInDb(req.body);
    // betroffene Listen-Keys invalidieren (einfach: per Muster löschen)
    const keys = await redis.keys('users:list:*');
    if (keys.length) await redis.del(keys);
    res.status(201).json(created);
  } catch (e) { next(e); }
});

r.put('/api/v1/users/:id', async (req, res, next) => {
  try {
    const updated = await updateUserInDb(req.params.id, req.body);
    await redis.del(`users:detail:${req.params.id}`);
    const keys = await redis.keys('users:list:*');
    if (keys.length) await redis.del(keys);
    res.json(updated);
  } catch (e) { next(e); }
});

r.get('/api/v1/users/:id',
  cache({ ttlSec: 300, keyFn: (req) => `users:detail:${req.params.id}` }),
  async (req, res, next) => {
    try {
      const user = await getUserFromDb(req.params.id);
      if (!user) return res.status(404).json({ error: 'not found' });
      res.json(user);
    } catch (e) { next(e); }
  }
);

r.delete('/api/v1/users/:id', async (req, res, next) => {
  try {
    await deleteUserInDb(req.params.id);
    await redis.del(`users:detail:${req.params.id}`);
    const keys = await redis.keys('users:list:*');
    if (keys.length) await redis.del(keys);
    res.status(204).send();
  } catch (e) { next(e); }
});
```

Hinweise:

* `KEYS` ist O(N) – für große Keyspaces besser **Tagging/Set-basierte** Invalidierung nutzen (siehe unten).

---

### 4) Effizientere Invalidierung mit Tagging

```js
// cache/tags.js
import { redis } from './redis.js';

// Tag registrieren
export async function tagAdd(tag, key) {
  await redis.sadd(`tag:${tag}`, key);
}
// Alle Keys eines Tags löschen
export async function tagInvalidate(tag) {
  const keys = await redis.smembers(`tag:${tag}`);
  if (keys.length) await redis.del(...keys);
  await redis.del(`tag:${tag}`);
}
```

Beim Cachen zusätzlich Tag verknüpfen:

```js
// im cache() innerhalb von res.json:
await Promise.all([
  redis.setex(key, ttlSec, JSON.stringify(body)),
  tagAdd('users:list', key)
]);
```

Bei Mutationen:

```js
await tagInvalidate('users:list');
await redis.del(`users:detail:${id}`);
```

---

### 5) HTTP-Caching ergänzen (kostenloser Speed für GET)

```js
// einfache ETag/Cache-Control
import crypto from 'node:crypto';

function withEtag(req, res, body) {
  const etag = `W/"${crypto.createHash('sha1').update(JSON.stringify(body)).digest('hex')}"`;
  res.set('ETag', etag);
  res.set('Cache-Control', 'public, max-age=60');
  if (req.headers['if-none-match'] === etag) return res.status(304).end();
  res.json(body);
}
```

Verwendung:

```js
r.get('/api/v1/public', async (req, res, next) => {
  try {
    const body = await loadPublicData();
    return withEtag(req, res, body);
  } catch (e) { next(e); }
});
```

---

### 6) Best Practices

* Key-Design: klarer Namensraum (`app:env:resource:params`), kurze TTLs.
* Invalidierung: Ereignis-getrieben (nach Writes), Sets/Tags statt `KEYS`.
* Nur **idempotente GETs** cachen; POST/PUT/PATCH/DELETE niemals cachen.
* Response-Größe beachten; große Payloads evtl. komprimieren (`compression`).
* Fehlerfälle: Bei Redis-Ausfall App weiterlaufen lassen (Cache optional).
* Sensible Daten nicht im Cache persistieren oder verschlüsseln/kurze TTL.
* In verteilten Systemen: Redis als **Shared Cache** (nicht Memory-Cache).

---

### Zusammenfassung

* Redis per Client (z. B. ioredis) anbinden, GET-Responses mit TTL cachen.
* Cache-Middleware vor teuren Handlern verwenden; bei Mutationen gezielt **invalidieren**.
* Für große Projekte: Tagging/Set-basierte Invalidierung statt `KEYS`.
* HTTP-Caching (ETag/Cache-Control) ergänzen; Cache bleibt optional bei Ausfall.

**Quellen:**

* Express.js – Best Practices: [https://expressjs.com/de/advanced/best-practice-performance.html](https://expressjs.com/de/advanced/best-practice-performance.html)
* Node.js Dokumentation (HTTP/Streams/Krypto): [https://nodejs.org/docs](https://nodejs.org/docs)
* MDN (RU) – HTTP Caching (ETag/Cache-Control): [https://developer.mozilla.org/ru/docs/Web/HTTP/Caching](https://developer.mozilla.org/ru/docs/Web/HTTP/Caching)
* ioredis (npm): [https://www.npmjs.com/package/ioredis](https://www.npmjs.com/package/ioredis)
* Redis Dokumentation: [https://redis.io/docs/](https://redis.io/docs/)


  **[⬆ Наверх](#top)**

74. ### <a name="74"></a> Wie geht man mit Verbindungen zu externen APIs um?

## Umgang mit Verbindungen zu externen APIs in Express

Ziele

* Stabilität (Timeouts, Retries, Circuit Breaker)
* Sicherheit (Secrets in ENV, TLS, Input/Output-Validierung)
* Performance (Keep-Alive, Caching, Pagination, Streaming)
* Beobachtbarkeit (Logs, Metriken)

HTTP-Client wählen

* `fetch` (ab Node 18 eingebaut) oder `axios`.
* Eigener `Agent` (Keep-Alive) für Performance.

Beispiel: Fetch mit Timeout, Retry (exponentiell), AbortController

```js
// src/lib/http.js
import { setTimeout as delay } from 'node:timers/promises';
import https from 'node:https';

const agent = new https.Agent({ keepAlive: true, maxSockets: 50 });

export async function httpGetJson(url, {
  headers = {}, timeoutMs = 5000, retries = 2, backoffMs = 300
} = {}) {
  for (let attempt = 0; ; attempt++) {
    const controller = new AbortController();
    const t = setTimeout(() => controller.abort(), timeoutMs);

    try {
      const res = await fetch(url, { headers, agent, signal: controller.signal });
      clearTimeout(t);

      if (!res.ok) {
        // 5xx retrybar, 429 abhängig von Policy
        if (attempt < retries && (res.status >= 500 || res.status === 429)) {
          await delay(backoffMs * 2 ** attempt);
          continue;
        }
        const text = await res.text().catch(() => '');
        const err = new Error(`Upstream ${res.status}: ${text.slice(0,200)}`);
        err.status = 502; // Bad Gateway in eigener API
        throw err;
      }
      return await res.json();
    } catch (e) {
      clearTimeout(t);
      if (e.name === 'AbortError') {
        if (attempt < retries) { await delay(backoffMs * 2 ** attempt); continue; }
        const err = new Error('Upstream timeout');
        err.status = 504; // Gateway Timeout
        throw err;
      }
      // Netzwerkfehler retryen
      if (attempt < retries) { await delay(backoffMs * 2 ** attempt); continue; }
      e.status ??= 502;
      throw e;
    }
  }
}
```

Circuit Breaker (einfach)

```js
// src/lib/circuit.js
const state = { failCount: 0, openUntil: 0 };

export async function withCircuit(fn, { threshold = 5, coolOffMs = 10000 } = {}) {
  const now = Date.now();
  if (state.openUntil > now) {
    const e = new Error('Upstream unavailable (circuit open)');
    e.status = 503;
    throw e;
  }
  try {
    const res = await fn();
    state.failCount = 0;
    return res;
  } catch (e) {
    state.failCount++;
    if (state.failCount >= threshold) {
      state.openUntil = now + coolOffMs;
    }
    throw e;
  }
}
```

Express-Route mit Upstream-Call, Fehler-Mapping, Caching-Header

```js
// src/routes/weather.routes.js
import { Router } from 'express';
import { httpGetJson } from '../lib/http.js';
import { withCircuit } from '../lib/circuit.js';

const r = Router();

r.get('/weather', async (req, res, next) => {
  try {
    const city = encodeURIComponent(req.query.city ?? 'Leipzig');
    const url = `https://api.example.com/weather?city=${city}`;
    const data = await withCircuit(() => httpGetJson(url, {
      headers: { 'X-Api-Key': process.env.WEATHER_API_KEY },
      timeoutMs: 4000, retries: 2
    }));

    // nur benötigte Felder zurückgeben (Projektion)
    const dto = { temp: data.temp_c, cond: data.condition };
    res.set('Cache-Control', 'public, max-age=60'); // HTTP-Caching
    res.json(dto);
  } catch (e) {
    // Einheitliche Upstream-Fehler → 502/503/504
    next(e);
  }
});

export default r;
```

Rate-Limiting & Backoff Respektieren

* Auf `429` mit `Retry-After` reagieren (siehe Retry-Logik).
* Eigene Limits mit `express-rate-limit` auf den Proxy-Routen.

Auth & Secrets

* API-Keys/OAuth-Tokens **nur** aus `process.env`.
* Bei OAuth 2.0: Token-Refresh getrennt kapseln, Tokens sicher im Server-Speicher/DB.

Input/Output-Validierung (z. B. Zod)

```js
import { z } from 'zod';
const qSchema = z.object({ city: z.string().min(1) });

r.get('/weather', async (req, res, next) => {
  try {
    const { city } = qSchema.parse(req.query);
    // …
  } catch (e) { e.status = 400; next(e); }
});
```

Streaming externer APIs (große Antworten)

* `pipeline(reqUpstream, res)` oder `ReadableStream` → geringer RAM-Verbrauch.
* Bei JSON-Streams (NDJSON) chunkweise weiterreichen und `drain` beachten.

Caching (Server-seitig, z. B. Redis)

* Responses von teuren/oft gleichen Upstream-Calls mit TTL zwischenspeichern.
* Invalidation nach Geschäftsregeln.

Observability

* Strukturierte Logs (pino) inkl. Upstream-URL, Dauer, Status.
* Metriken (Counter/Histogram) für Latenz/Fehlerquote (z. B. prom-client).

Sicherheit

* TLS erzwingen (nur `https`-Endpoints).
* Keine sensiblen Upstream-Antworten direkt weiterleiten; nur whitelisten/projizieren.
* Zeit-/Größenlimits: `express.json({ limit: '1mb' })`.

Best Practices (Kurz)

* **Timeouts & Retries** (nur idempotente GET/HEAD/PUT).
* **Circuit Breaker** gegen Kaskadierung von Ausfällen.
* **Keep-Alive Agent** für Throughput.
* **Validierung & Projektion** der Daten.
* **HTTP-Cache-Header** + optional Redis.
* **Sauberes Fehler-Mapping**: 502/503/504 für Upstream-Probleme.
* **Logs/Metriken** pro Upstream-Call.

Zusammenfassung

* Externe API-Aufrufe in Helper/Service kapseln mit **Timeout, Retry, Circuit Breaker, Keep-Alive**.
* Ergebnisse **validieren, projizieren, cachen**; Fehler sauber in **5xx-Gateway-Codes** mappen.
* **Secrets aus ENV**, strukturiertes **Logging** und **Metriken** für Stabilität.

Quellen

* Node.js – HTTPS/HTTP/AbortController/Agent: [https://nodejs.org/docs](https://nodejs.org/docs)
* Express.js – Best Practices (Performance/Security): [https://expressjs.com/de/advanced/best-practice-performance.html](https://expressjs.com/de/advanced/best-practice-performance.html)
* MDN Web Docs (RU) – Fetch/Abort/HTTP-Caching/Statuscodes: [https://developer.mozilla.org/ru/](https://developer.mozilla.org/ru/)
* PostgreSQL/Sequelize/Redis (allg. ergänzend fürs Caching/Backpressure): [https://sequelize.org/](https://sequelize.org/) , [https://redis.io/docs/](https://redis.io/docs/)


  **[⬆ Наверх](#top)**

75. ### <a name="75"></a> Wie baut man eine WebSocket-Verbindung mit Express?

## WebSocket mit Express: Ansätze und Beispiel

Kernpunkte

* Express selbst spricht **HTTP**; für WebSockets nutzt man einen **HTTP-Server** + WS-Bibliothek (z. B. `ws`) oder **Socket.IO**.
* Setup: `createServer(app)` → Server an `ws` oder `socket.io` übergeben.
* Wichtige Themen: **Heartbeat (Ping/Pong)**, **Fehlerbehandlung**, **Auth**, **Skalierung**.

### Variante A: Reines WebSocket-Protokoll mit `ws`

```js
// server.js (ESM, type="module")
import express from 'express';
import { createServer } from 'node:http';
import { WebSocketServer } from 'ws';

const app = express();
app.get('/health', (_req, res) => res.json({ ok: true }));

// 1) Gemeinsamer HTTP-Server
const server = createServer(app);

// 2) WebSocket-Server auf demselben Port/Server
const wss = new WebSocketServer({ server, path: '/ws' });

// 3) Verbindungs- und Nachrichten-Handling
wss.on('connection', (ws, req) => {
  // Beispiel-Auth: Token aus Query (nur Demo – besser: Header prüfen)
  const url = new URL(req.url, `http://${req.headers.host}`);
  const token = url.searchParams.get('token');
  if (token !== process.env.WS_TOKEN) {
    ws.close(1008, 'Unauthorized');
    return;
  }

  // Heartbeat
  ws.isAlive = true;
  ws.on('pong', () => (ws.isAlive = true));

  ws.on('message', (data) => {
    // Erwartet JSON-Nachrichten
    try {
      const msg = JSON.parse(data.toString());
      // Echo + Broadcast-Beispiel
      ws.send(JSON.stringify({ type: 'ack', received: msg }));
      for (const client of wss.clients) {
        if (client !== ws && client.readyState === client.OPEN) {
          client.send(JSON.stringify({ type: 'broadcast', payload: msg }));
        }
      }
    } catch {
      ws.send(JSON.stringify({ type: 'error', message: 'Invalid JSON' }));
    }
  });

  ws.on('close', (code, reason) => {
    console.log('WS closed', code, reason.toString());
  });
});

// 4) Periodischer Ping zum Erkennen toter Verbindungen
const interval = setInterval(() => {
  for (const ws of wss.clients) {
    if (!ws.isAlive) return ws.terminate();
    ws.isAlive = false;
    ws.ping();
  }
}, 30000);

wss.on('close', () => clearInterval(interval));

const PORT = process.env.PORT ?? 3000;
server.listen(PORT, () => console.log(`HTTP+WS auf :${PORT} (ws://localhost:${PORT}/ws)`));
```

Ein minimaler Client (im Browser/Frontend):

```js
// client.js
const ws = new WebSocket('ws://localhost:3000/ws?token=MEIN_TOKEN');
ws.onopen = () => ws.send(JSON.stringify({ type: 'hello', name: 'Sergii' }));
ws.onmessage = (e) => console.log('Server:', e.data);
ws.onclose = (e) => console.log('Closed', e.code, e.reason);
```

Wann `ws`?

* Du brauchst **reines WebSocket** (keine Fallbacks, volle Kontrolle über Frames/Protokoll).
* Geringer Overhead, sehr schnell.

### Variante B: Socket.IO (WebSocket + Fallbacks, Räume, Reconnect)

```js
// server-socketio.js
import express from 'express';
import { createServer } from 'node:http';
import { Server as IOServer } from 'socket.io';

const app = express();
const server = createServer(app);
const io = new IOServer(server, {
  path: '/socket',
  cors: { origin: ['http://localhost:5173'], credentials: true }
});

io.use((socket, next) => {
  const token = socket.handshake.auth?.token;
  if (token !== process.env.WS_TOKEN) return next(new Error('Unauthorized'));
  next();
});

io.on('connection', (socket) => {
  socket.join('room:public');
  socket.emit('welcome', { id: socket.id });

  socket.on('message', (payload) => {
    io.to('room:public').emit('message', { from: socket.id, payload });
  });

  socket.on('disconnect', (reason) => {
    console.log('Socket disconnected:', reason);
  });
});

server.listen(3000, () => console.log('Socket.IO auf :3000'));
```

Wann Socket.IO?

* Du willst **Auto-Reconnect**, **Räume/Namespaces**, **Event-basierte API** und optionale **Long-Polling-Fallbacks**.

### Auth, Sicherheit, Betrieb

* **Auth**: Token/JWT prüfen (bei `ws` über Header `Sec-WebSocket-Protocol` oder Query; bei Socket.IO `handshake.auth`).
* **TLS/HTTPS**: In Produktion hinter TLS (Proxy/Ingress) betreiben.
* **Reverse Proxy**: `app.set('trust proxy', 1)` und ggf. WebSocket-Weiterleitung (NGINX: `proxy_set_header Upgrade $http_upgrade;`).
* **Skalierung**: Socket.IO per **Redis-Adapter** für mehrere Instanzen; bei `ws` lastverteilte Instanzen → Sticky Sessions oder statefreies Protokoll.
* **Backpressure**: Bei hohem Durchsatz `ws`-Sendestatus prüfen (`readyState`, `bufferedAmount`) und drosseln.
* **Protokoll**: Definiere ein schlankes JSON-Schema (`type`, `payload`) und validiere Eingaben.

### Zusammenfassung

* Express + WebSockets: HTTP-Server teilen, dann entweder **`ws`** (reines WS, schnell) oder **Socket.IO** (höherwertige Features).
* Wichtig: **Heartbeat (Ping/Pong)**, **Auth**, **Fehler-/Reconnect-Strategie**, **Skalierung** (Redis/Sticky Sessions).
* Produktion: TLS/Proxy korrekt konfigurieren, Backpressure beachten, Protokoll/Validierung definieren.

Quellen

* MDN – WebSockets API: [https://developer.mozilla.org/ru/docs/Web/API/WebSockets\_API](https://developer.mozilla.org/ru/docs/Web/API/WebSockets_API)
* Node.js – HTTP/HTTPS Server: [https://nodejs.org/docs](https://nodejs.org/docs)
* Express.js – Guide (Integration/Best Practices): [https://expressjs.com/de/](https://expressjs.com/de/)
* `ws` (npm, Doku): [https://www.npmjs.com/package/ws](https://www.npmjs.com/package/ws)
* Socket.IO Doku: [https://socket.io/docs/](https://socket.io/docs/)


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
