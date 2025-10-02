<a name="top"></a>

[На главную](../../README.md)

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
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


121. ### <a name="121"></a> Was ist Node.js und wofür wird es verwendet?

**Node.js** ist eine **JavaScript-Laufzeitumgebung**, die auf der **V8-Engine von Google Chrome** basiert. Sie ermöglicht es, JavaScript nicht nur im Browser, sondern auch **serverseitig** auszuführen.

### Hauptmerkmale:

* **Event-Driven & Non-Blocking I/O**: Node.js arbeitet asynchron und eignet sich für Anwendungen mit vielen gleichzeitigen Verbindungen.
* **Single-Threaded mit Event Loop**: Ein Thread verwaltet viele Anfragen effizient.
* **Cross-Plattform**: Funktioniert auf Windows, macOS, Linux.
* **Umfangreiches Ökosystem**: Über **npm** (Node Package Manager) stehen hunderttausende Pakete zur Verfügung.

### Typische Anwendungsfälle:

* **Backend-APIs** (REST, GraphQL)
* **Echtzeitanwendungen** (Chats, Multiplayer-Spiele, WebSockets)
* **Microservices**
* **Serverless Functions**
* **Build-Tools** (Webpack, Gulp, ESLint laufen selbst auf Node.js)

### Einfaches Beispiel:

```js
// server.js
const http = require('http');

// Einfache HTTP-Response
const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hallo aus Node.js!');
});

server.listen(3000, () => {
  console.log('Server läuft auf http://localhost:3000');
});
```

➡️ Starten: `node server.js`

---

### Zusammenfassung

Node.js ist eine serverseitige JavaScript-Laufzeitumgebung mit **asynchronem, eventbasiertem Modell**, ideal für **skalierbare Netzwerk- und Webanwendungen**.

📖 Quellen:

* [Node.js Dokumentation](https://nodejs.org/docs)
* [MDN: Einführung in Node.js (RU)](https://developer.mozilla.org/ru/docs/Learn/Server-side/Express_Nodejs/Introduction)

---

  **[⬆ Наверх](#top)**

122. ### <a name="122"></a> Wie funktioniert die V8 Engine?

**V8** ist die von Google entwickelte **JavaScript-Engine**, die in **Google Chrome** und **Node.js** verwendet wird. Sie übersetzt JavaScript-Code direkt in **Maschinencode**, was ihn sehr schnell und effizient macht.

---

### Funktionsweise von V8

1. **Parsing (Parser-Phase)**

   * Der Quellcode wird in einen **Abstract Syntax Tree (AST)** umgewandelt.
   * Beispiel: `let x = 5 + 2;` → Baumstruktur, die Operatoren und Operanden darstellt.

2. **Bytecode-Erzeugung (Ignition Interpreter)**

   * Der AST wird in **Bytecode** übersetzt, eine Zwischensprache, die schnell interpretiert werden kann.

3. **Optimierung (TurboFan JIT Compiler)**

   * Häufig ausgeführte Codebereiche (Hot Code) werden erkannt.
   * Dieser Code wird **Just-in-Time (JIT)** kompiliert und direkt in **Maschinencode** umgewandelt.

4. **Inline Caching & Hidden Classes**

   * **Hidden Classes**: Objekte erhalten interne Strukturen, ähnlich wie Klassen in Java oder C++, um den Zugriff auf Properties zu beschleunigen.
   * **Inline Caching**: Speichert, wie auf bestimmte Objekte zugegriffen wird, und optimiert wiederholte Zugriffe.

5. **Garbage Collection (Speicherverwaltung)**

   * V8 verwendet eine **Generational Garbage Collection** (Jung- und Altspeicherbereiche).
   * Unbenutzte Objekte werden regelmäßig entfernt, um Speicher freizugeben.

---

### Visualisierung (vereinfacht)

```text
JS-Code → Parser → AST → Ignition (Bytecode) 
       ↘ Hot Code → TurboFan (optimierter Maschinencode)
```

---

### Beispiel im Code

```js
function add(a, b) {
  return a + b;
}

for (let i = 0; i < 1_000_000; i++) {
  add(10, 20); // "Hot Code" → wird von V8 optimiert
}
```

* Anfangs läuft `add()` als **Bytecode**.
* Nach vielen Wiederholungen erkennt V8 ein Muster → kompiliert in **Maschinencode**.

---

### Zusammenfassung

Die **V8 Engine** übersetzt JavaScript in **Maschinencode** mit Hilfe von:

* **AST + Bytecode (Ignition Interpreter)**
* **JIT-Kompilierung (TurboFan Optimizer)**
* **Optimierungen wie Hidden Classes & Inline Caching**
* **Automatisches Speicher-Management (Garbage Collector)**

Dadurch läuft JavaScript in Node.js und Chrome **sehr performant**.

📖 Quellen:

* [V8 JavaScript Engine Docs](https://v8.dev/)
* [MDN: JavaScript engines](https://developer.mozilla.org/en-US/docs/Mozilla/Projects/SpiderMonkey/Introduction_to_the_JavaScript_shell)

---

  **[⬆ Наверх](#top)**

123. ### <a name="123"></a> Was ist Event Loop und wie funktioniert er?

Der **Event Loop** ist das zentrale Konzept in **Node.js**, das für die **asynchrone, nicht-blockierende Verarbeitung** von Operationen sorgt. Da Node.js **Single-Threaded** ist, übernimmt der Event Loop die Koordination von **Callbacks, Promises und I/O-Operationen**.

---

### Ablauf des Event Loops

Der Event Loop arbeitet in **Phasen**. Jede Phase verarbeitet eine bestimmte Art von Aufgaben:

1. **Timers**

   * Führt Callbacks von `setTimeout` und `setInterval` aus.

2. **Pending Callbacks**

   * Callbacks von abgeschlossenen I/O-Operationen, die auf ihre Ausführung warten.

3. **Idle/Prepare** *(intern, selten relevant)*

4. **Poll**

   * Kernstück: verarbeitet eingehende I/O-Events (z. B. Netzwerk, Filesystem).
   * Falls keine Events vorhanden: wartet oder wechselt in die nächste Phase.

5. **Check**

   * Führt `setImmediate`-Callbacks aus.

6. **Close Callbacks**

   * Callbacks für geschlossene Ressourcen, z. B. `socket.on('close')`.

**Microtasks (Promises, process.nextTick)**

* Werden **zwischen den Phasen** verarbeitet, bevor der Event Loop weitergeht.
* Haben höhere Priorität als Timer oder I/O.

---

### Beispiel

```js
setTimeout(() => console.log("Timeout"), 0);
setImmediate(() => console.log("Immediate"));
process.nextTick(() => console.log("NextTick"));
Promise.resolve().then(() => console.log("Promise"));

console.log("Sync");
```

**Mögliche Ausgabe:**

```
Sync
NextTick
Promise
Timeout
Immediate
```

**Erklärung:**

* `console.log("Sync")` → sofort ausgeführt.
* `process.nextTick` und **Promises (Microtasks)** → vor Timern.
* `setTimeout(..., 0)` → nächste Timer-Phase.
* `setImmediate` → Check-Phase.

---

### Visualisierung (vereinfacht)

```text
┌───────────────────────────┐
│   Event Loop              │
│ ┌─────┬─────┬─────┬─────┐ │
│ │Timers│Poll │Check│Close│ │
│ └─────┴─────┴─────┴─────┘ │
│   ↑ Microtasks (NextTick, Promises) 
└───────────────────────────┘
```

---

### Zusammenfassung

Der **Event Loop** sorgt dafür, dass Node.js trotz **Single-Threading** viele Anfragen gleichzeitig bearbeiten kann:

* **Asynchron** durch Callbacks, Promises, async/await.
* **Phasenbasiert**: Timer → I/O → Check → Close.
* **Microtasks** (Promises, `process.nextTick`) haben **höchste Priorität**.

📖 Quellen:

* [Node.js Docs – Event Loop](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick)
* [MDN – Concurrency model and Event Loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)

---

  **[⬆ Наверх](#top)**

124. ### <a name="124"></a> Unterschied zwischen Call Stack, Callback Queue und Event Loop?

### **1. Call Stack (Aufruf-Stack)**

* Eine **Stack-Struktur**, in der die aktuell ausgeführten Funktionen gespeichert werden.
* Arbeitet nach dem Prinzip **LIFO (Last In, First Out)**.
* Wenn eine Funktion beendet ist, wird sie vom Stack entfernt.

**Beispiel:**

```js
function a() { b(); }
function b() { c(); }
function c() { console.log("Hallo"); }

a(); 
// Stack: [a] → [a,b] → [a,b,c] → Ausgabe → Stack leer
```

---

### **2. Callback Queue (Task Queue / Message Queue)**

* Enthält **Callbacks von asynchronen Operationen** (z. B. `setTimeout`, I/O).
* Wenn der Call Stack leer ist, schiebt der **Event Loop** den nächsten Callback in den Call Stack.

**Beispiel:**

```js
setTimeout(() => console.log("Timeout"), 0);
console.log("Sync");
```

* `console.log("Sync")` läuft sofort im Call Stack.
* Der `setTimeout`-Callback landet in der **Callback Queue** und wird erst ausgeführt, wenn der Call Stack frei ist.

---

### **3. Event Loop**

* Vermittler zwischen **Call Stack** und **Callback Queue**.
* Aufgabe: **Überprüfen, ob der Call Stack leer ist**, und dann den nächsten Callback aus der Queue hineinlegen.
* Steuert auch die Ausführung von **Microtasks** (Promises, `process.nextTick`).

---

### **Zusammenspiel**

```js
console.log("Start");

setTimeout(() => console.log("Timeout"), 0);

Promise.resolve().then(() => console.log("Promise"));

console.log("End");
```

**Ablauf:**

1. Call Stack: `"Start"` → `"End"` wird direkt ausgeführt.
2. Promise-Callback landet in der **Microtask Queue** → wird **vor** `setTimeout` ausgeführt.
3. `setTimeout`-Callback kommt aus der **Callback Queue**, wenn der Stack leer ist.

**Ausgabe:**

```
Start
End
Promise
Timeout
```

---

### **Visualisierung**

```text
        ┌───────────────┐
        │   Call Stack  │
        └───────▲───────┘
                │
        ┌───────┴───────┐
        │  Event Loop    │
        └───────▲───────┘
                │
        ┌───────┴───────┐
        │ Callback Queue │
        └───────────────┘
```

👉 Microtasks laufen **zwischen** den Event Loop Zyklen, bevor normale Callbacks verarbeitet werden.

---

### **Zusammenfassung**

* **Call Stack**: Führt synchronen Code aus, speichert aktive Funktionen.
* **Callback Queue**: Warteschlange für asynchrone Callbacks (z. B. Timer, I/O).
* **Event Loop**: Kontrollmechanismus, der den Stack und die Queue verbindet; sorgt für asynchrone Verarbeitung.

📖 Quellen:

* [MDN – Event Loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)
* [Node.js Docs – Event Loop](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick)

---

  **[⬆ Наверх](#top)**

125. ### <a name="125"></a> Unterschied zwischen asynchronem und synchronem Code in Node.js?

### **Synchroner Code**

* Befehle werden **der Reihe nach** ausgeführt.
* Jeder Schritt blockiert die Ausführung, bis er abgeschlossen ist.
* Geeignet für **CPU-intensive Aufgaben**.

**Beispiel:**

```js
const fs = require('fs');

// Synchrones Lesen einer Datei
const data = fs.readFileSync('file.txt', 'utf8');
console.log(data);

console.log("Dieser Code wartet, bis die Datei gelesen wurde.");
```

➡️ Der zweite `console.log` wird **erst nach dem Lesen** der Datei ausgeführt.

---

### **Asynchroner Code**

* Befehle werden gestartet, aber **blockieren den Event Loop nicht**.
* Stattdessen wird ein **Callback, Promise oder async/await** genutzt, wenn die Operation fertig ist.
* Geeignet für **I/O-intensive Aufgaben** (Datenbank, API, Dateisystem).

**Beispiel mit Callback:**

```js
const fs = require('fs');

// Asynchrones Lesen einer Datei
fs.readFile('file.txt', 'utf8', (err, data) => {
  if (err) throw err;
  console.log(data);
});

console.log("Dieser Code läuft, während die Datei gelesen wird.");
```

➡️ `console.log("Dieser Code läuft...")` wird **vor** dem Dateiinhalten ausgeführt.

**Beispiel mit Promise / async/await:**

```js
const fs = require('fs').promises;

async function readFile() {
  const data = await fs.readFile('file.txt', 'utf8');
  console.log(data);
}

readFile();
console.log("Code läuft parallel weiter...");
```

---

### **Vergleich**

| Merkmal     | Synchroner Code        | Asynchroner Code            |
| ----------- | ---------------------- | --------------------------- |
| Ablauf      | Schritt für Schritt    | Parallel, non-blocking      |
| Performance | Blockiert Event Loop   | Hohe Skalierbarkeit         |
| Einsatz     | Kleine, schnelle Tasks | I/O, Netzwerke, DB-Abfragen |
| Beispiel    | `fs.readFileSync()`    | `fs.readFile()`, Promises   |

---

### **Zusammenfassung**

* **Synchron**: blockiert die Ausführung, einfacher Ablauf, aber nicht skalierbar.
* **Asynchron**: blockiert nicht, nutzt **Callbacks, Promises, async/await**, ideal für skalierbare Netzwerk-Apps.

📖 Quellen:

* [Node.js File System – fs](https://nodejs.org/api/fs.html)
* [MDN – async und await](https://developer.mozilla.org/de/docs/Learn/JavaScript/Asynchronous/Promises)

---

  **[⬆ Наверх](#top)**

126. ### <a name="126"></a> Unterschied zwischen process.nextTick(), setImmediate() und setTimeout()?

### **1. process.nextTick()**

* Führt eine Callback-Funktion **sofort nach der aktuellen Operation**, aber **vor dem nächsten Event Loop Durchlauf** aus.
* Hat höchste Priorität.
* Gefahr: Bei zu vielen `process.nextTick`-Aufrufen kann der Event Loop blockiert werden.

**Beispiel:**

```js
console.log("Start");

process.nextTick(() => {
  console.log("nextTick");
});

console.log("End");
```

➡️ Ausgabe:

```
Start
End
nextTick
```

---

### **2. setImmediate()**

* Führt eine Callback-Funktion in der **Check-Phase** des Event Loops aus.
* Läuft **nach I/O-Operationen** und nach `setTimeout(..., 0)` (in den meisten Fällen).

**Beispiel:**

```js
console.log("Start");

setImmediate(() => {
  console.log("Immediate");
});

console.log("End");
```

➡️ Ausgabe:

```
Start
End
Immediate
```

---

### **3. setTimeout(fn, 0)**

* Führt eine Callback-Funktion in der **Timer-Phase** des Event Loops aus.
* `0 ms` bedeutet nicht "sofort", sondern **mindestens eine Tick-Verzögerung**.
* Kann durch Systemlatenzen verzögert werden.

**Beispiel:**

```js
console.log("Start");

setTimeout(() => {
  console.log("Timeout 0");
}, 0);

console.log("End");
```

➡️ Ausgabe:

```
Start
End
Timeout 0
```

---

### **Vergleich**

| Funktion               | Phase im Event Loop        | Priorität                                         | Typische Nutzung           |
| ---------------------- | -------------------------- | ------------------------------------------------- | -------------------------- |
| **process.nextTick()** | Microtask-Queue (vor Loop) | Höchste Priorität                                 | Sofort nach aktuellem Code |
| **setImmediate()**     | Check-Phase                | Niedriger als nextTick, aber stabiler als Timeout | Callbacks nach I/O         |
| **setTimeout(fn, 0)**  | Timer-Phase                | Nach Microtasks, I/O abhängig                     | Verzögerte Ausführung      |

---

### **Kombiniertes Beispiel**

```js
setTimeout(() => console.log("Timeout 0"), 0);
setImmediate(() => console.log("Immediate"));
process.nextTick(() => console.log("NextTick"));
Promise.resolve().then(() => console.log("Promise"));

console.log("Sync");
```

**Typische Ausgabe:**

```
Sync
NextTick
Promise
Timeout 0
Immediate
```

---

### **Zusammenfassung**

* **process.nextTick()**: höchste Priorität, **vor** Event Loop Tick.
* **setImmediate()**: ausgeführt in der **Check-Phase**, meist nach Timern.
* **setTimeout(fn, 0)**: ausgeführt in der **Timer-Phase**, kann verzögert werden.

📖 Quellen:

* [Node.js Docs – process.nextTick()](https://nodejs.org/api/process.html#processnexttickcallback-args)
* [Node.js Docs – timers](https://nodejs.org/api/timers.html)
* [MDN – Concurrency model](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)

---

  **[⬆ Наверх](#top)**

127. ### <a name="127"></a> Was sind Streams in Node.js und welche Typen gibt es?

### **Streams in Node.js**

Ein **Stream** ist eine **abstrakte Schnittstelle** für die Arbeit mit Daten, die **stückweise (chunked)** anstatt komplett auf einmal verarbeitet werden.
Das ist besonders nützlich für **große Dateien, Netzwerkkommunikation oder Daten-Pipelines**, da nicht der gesamte Inhalt in den Speicher geladen werden muss.

---

### **Typen von Streams**

1. **Readable Streams (lesbar)**

   * Daten können **gelesen** werden.
   * Beispiele: `fs.createReadStream()`, HTTP-Anfragen (`req`).

   ```js
   const fs = require('fs');
   const readable = fs.createReadStream('input.txt', { encoding: 'utf8' });

   readable.on('data', chunk => {
     console.log("Chunk:", chunk);
   });
   ```

2. **Writable Streams (schreibbar)**

   * Daten können **geschrieben** werden.
   * Beispiele: `fs.createWriteStream()`, HTTP-Antwort (`res`).

   ```js
   const fs = require('fs');
   const writable = fs.createWriteStream('output.txt');

   writable.write("Hallo Welt\n");
   writable.end("Ende der Datei");
   ```

3. **Duplex Streams**

   * Können **gleichzeitig lesen und schreiben**.
   * Beispiele: TCP-Sockets (`net.Socket`).

   ```js
   const { Duplex } = require('stream');

   const duplex = new Duplex({
     read(size) { this.push("Daten vom Duplex\n"); this.push(null); },
     write(chunk, encoding, callback) { console.log("Geschrieben:", chunk.toString()); callback(); }
   });

   duplex.on('data', data => console.log("Gelesen:", data.toString()));
   duplex.write("Input");
   ```

4. **Transform Streams** (Spezialfall von Duplex)

   * Lesen, verarbeiten und schreiben Daten **transformiert**.
   * Beispiele: `zlib.createGzip()`, `crypto.createCipher()`.

   ```js
   const { Transform } = require('stream');

   const upperCase = new Transform({
     transform(chunk, encoding, callback) {
       callback(null, chunk.toString().toUpperCase());
     }
   });

   process.stdin.pipe(upperCase).pipe(process.stdout);
   // Eingabe in Konsole → Ausgabe in Großbuchstaben
   ```

---

### **Zusammenfassung**

* **Streams** = effiziente Verarbeitung großer Datenmengen **in kleinen Blöcken**.
* Typen:

  * **Readable** (lesen)
  * **Writable** (schreiben)
  * **Duplex** (lesen + schreiben)
  * **Transform** (lesen + schreiben + transformieren)

📖 Quellen:

* [Node.js Docs – Stream](https://nodejs.org/api/stream.html)
* [MDN – Streams](https://developer.mozilla.org/en-US/docs/Web/API/Streams_API)

---

  **[⬆ Наверх](#top)**

128. ### <a name="128"></a> Unterschied zwischen Buffer und Stream?

### **Buffer**

* Ein **temporärer Speicherbereich** im **RAM**, der Binärdaten speichert.
* Wird genutzt, wenn Daten **komplett oder teilweise** vorliegen müssen.
* Ideal für **kleine Datenmengen** oder wenn man **direkt mit Binärdaten** arbeitet.

**Beispiel:**

```js
const buffer = Buffer.from("Hallo");
console.log(buffer);           // <Buffer 48 61 6c 6c 6f>
console.log(buffer.toString()); // "Hallo"
```

➡️ Alles wird **sofort in den Speicher geladen**.

---

### **Stream**

* Abstraktion für **kontinuierliche Datenflüsse**.
* Daten werden **stückweise (chunks)** verarbeitet, ohne alles in den Speicher zu laden.
* Ideal für **große Dateien oder Netzwerkeingaben**.

**Beispiel:**

```js
const fs = require('fs');
const readable = fs.createReadStream('großeDatei.txt');

readable.on('data', chunk => {
  console.log("Chunk:", chunk.length);
});
```

➡️ Datei wird **Stück für Stück gelesen**, nicht komplett in den RAM geladen.

---

### **Vergleich**

| Merkmal          | Buffer                        | Stream                                   |
| ---------------- | ----------------------------- | ---------------------------------------- |
| Datenmenge       | Klein bis mittelgroß          | Groß (z. B. GB-Dateien, Video, Netzwerk) |
| Verarbeitung     | Alles im Speicher             | Stückweise (chunks)                      |
| Speicherbedarf   | Hoch bei großen Daten         | Konstant niedrig                         |
| Typische Nutzung | String → Binärdaten, Encoding | Dateisystem, HTTP, Pipes                 |

---

### **Zusammenfassung**

* **Buffer**: Speichert Daten vollständig im RAM → schneller Zugriff, aber nicht für große Daten geeignet.
* **Stream**: Verarbeitet Daten **nach und nach** → effizient und skalierbar bei großen Datenmengen.

📖 Quellen:

* [Node.js Docs – Buffer](https://nodejs.org/api/buffer.html)
* [Node.js Docs – Stream](https://nodejs.org/api/stream.html)

---

  **[⬆ Наверх](#top)**

129. ### <a name="129"></a> Wie arbeitet Node.js intern mit Non-Blocking I/O?

### **Non-Blocking I/O in Node.js**

Node.js ist **Single-Threaded**, aber dank **Non-Blocking I/O** kann es viele parallele Aufgaben gleichzeitig abwickeln, ohne den Event Loop zu blockieren. Das funktioniert durch die Kombination von:

1. **Libuv**

   * C-Bibliothek, die für **asynchrone I/O-Operationen** zuständig ist.
   * Verwaltet ein **Thread-Pool** (Standard: 4 Threads).
   * Nutzt **Betriebssystem-APIs** (epoll, kqueue, IOCP etc.) für effizientes Event-basiertes I/O.

2. **Event Loop**

   * Koordiniert Callbacks, Microtasks und I/O-Events.
   * Nimmt die Ergebnisse von Libuv entgegen und legt sie in die **Callback Queue**.

3. **Thread Pool**

   * Einige I/O-Operationen (z. B. **Dateisystem, DNS-Auflösung**) werden auf separate Threads ausgelagert.
   * Dadurch blockiert der Haupt-Thread (Event Loop) nicht.

---

### **Ablauf (vereinfacht)**

1. JavaScript-Code ruft eine I/O-Operation auf (z. B. `fs.readFile`).
2. Node.js übergibt die Anfrage an **Libuv**.
3. Libuv entscheidet:

   * Netzwerkoperation → nutzt **Betriebssystem-Events** (non-blocking Sockets).
   * Dateisystem/DNS → nutzt **Thread Pool**.
4. Wenn die Operation abgeschlossen ist, wird das Ergebnis zurück an den Event Loop geschickt.
5. Der Event Loop legt den zugehörigen Callback in die **Callback Queue**, sobald der Call Stack leer ist.

---

### **Beispiel: Datei asynchron lesen**

```js
const fs = require('fs');

console.log("Start");

fs.readFile("file.txt", "utf8", (err, data) => {
  if (err) throw err;
  console.log("Datei-Inhalt:", data);
});

console.log("End");
```

**Ablauf:**

1. `fs.readFile` → Libuv Thread Pool übernimmt.
2. `console.log("End")` läuft sofort, da `readFile` nicht blockiert.
3. Sobald die Datei fertig gelesen ist → Callback in die Queue.
4. Event Loop führt Callback aus.

**Ausgabe:**

```
Start
End
Datei-Inhalt: ...
```

---

### **Visualisierung**

```text
JS Code → Event Loop → Libuv → OS / Thread Pool → Callback Queue → Call Stack
```

---

### **Zusammenfassung**

* Node.js nutzt **Libuv + Event Loop + Thread Pool**, um I/O **nicht-blockierend** auszuführen.
* Netzwerk-I/O: Betriebssystem-Events (sehr effizient).
* File-System/DNS: Libuv-Thread-Pool.
* Vorteil: **Skalierbarkeit** → viele gleichzeitige Clients auf einem Single-Thread.

📖 Quellen:

* [Node.js Docs – Event Loop](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick)
* [Libuv Documentation](https://libuv.org/)
* [MDN – Asynchronous concepts](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Concepts)

---

  **[⬆ Наверх](#top)**

130. ### <a name="130"></a> Wie funktioniert das Modul-System in Node.js (CommonJS vs. ES Modules)?

### **Modul-System in Node.js**

Node.js unterstützt zwei Modulsysteme:

1. **CommonJS (CJS)** – traditionelles System, Standard bis Node.js v12.
2. **ES Modules (ESM)** – modernes System, basierend auf dem **ECMAScript-Standard**.

---

### **1. CommonJS (CJS)**

* Standard in Node.js (ältere Projekte).
* Module werden **synchron** geladen.
* Verwendung von `require()` und `module.exports`.

**Beispiel:**

```js
// math.js
function add(a, b) {
  return a + b;
}
module.exports = { add };

// index.js
const math = require('./math');
console.log(math.add(2, 3)); // 5
```

---

### **2. ES Modules (ESM)**

* ECMAScript-Standard, seit Node.js **v14 stabil**.
* Module werden **asynchron** geladen.
* Verwendung von `import` und `export`.
* Aktivierung:

  * `package.json` → `"type": "module"`
  * oder Dateiendung `.mjs`.

**Beispiel:**

```js
// math.mjs oder in "type": "module"
export function add(a, b) {
  return a + b;
}

// index.mjs
import { add } from './math.js';
console.log(add(2, 3)); // 5
```

---

### **Vergleich**

| Merkmal      | CommonJS (CJS)              | ES Modules (ESM)                  |
| ------------ | --------------------------- | --------------------------------- |
| Syntax       | `require`, `module.exports` | `import`, `export`                |
| Laden        | Synchron (zur Laufzeit)     | Asynchron (zur Parse-Zeit)        |
| Dateiendung  | `.js`                       | `.mjs` oder `"type": "module"`    |
| Standard in  | Node.js älteren Versionen   | Moderne JS-Umgebungen, Browser    |
| Tree-Shaking | ❌ Nicht unterstützt         | ✅ Unterstützt (z. B. in Bundlern) |

---

### **Besonderheiten**

* **Interop**:

  * In **ESM** kann man CJS-Module via `import pkg from 'cjs-modul'` nutzen.
  * In **CJS** kann man ESM nur dynamisch laden (`import()` statt `require`).
* **Top-Level Await**:

  * Nur in **ESM** erlaubt (`await` außerhalb von Funktionen).

**Beispiel:**

```js
// index.mjs
const response = await fetch("https://jsonplaceholder.typicode.com/todos/1");
const data = await response.json();
console.log(data);
```

---

### **Zusammenfassung**

* **CommonJS**: älteres Node.js-Modulsystem, synchron, `require/module.exports`.
* **ESM**: modernes System, asynchron, `import/export`, unterstützt Tree-Shaking und Top-Level Await.
* Heute: **neue Projekte → ESM**, alte Projekte oft noch **CJS**.

📖 Quellen:

* [Node.js Docs – Modules: CommonJS](https://nodejs.org/docs/latest/api/modules.html)
* [Node.js Docs – Modules: ECMAScript](https://nodejs.org/docs/latest/api/esm.html)
* [MDN – import/export](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Statements/import)

---


  **[⬆ Наверх](#top)**  

131. ### <a name="131"></a> Was ist require und was ist import?

### **require**

* Teil von **CommonJS (CJS)**.
* Lädt Module **synchron** zur Laufzeit.
* Gibt das zurück, was mit `module.exports` exportiert wurde.

**Beispiel:**

```js
// math.js
function add(a, b) {
  return a + b;
}
module.exports = { add };

// index.js
const math = require('./math');
console.log(math.add(2, 3)); // 5
```

---

### **import**

* Teil von **ES Modules (ESM)**.
* Lädt Module **asynchron** bereits beim Parsen.
* Kann **benannte Exporte** oder einen **Default-Export** importieren.

**Beispiel:**

```js
// math.js (ESM)
export function add(a, b) {
  return a + b;
}

// index.mjs oder in "type": "module"
import { add } from './math.js';
console.log(add(2, 3)); // 5
```

---

### **Vergleich require vs. import**

| Merkmal         | `require` (CJS)             | `import` (ESM)                                   |
| --------------- | --------------------------- | ------------------------------------------------ |
| System          | CommonJS                    | ECMAScript Module                                |
| Ladeart         | **Synchron** (zur Laufzeit) | **Asynchron** (zur Parse-Zeit)                   |
| Syntax          | `const x = require('x')`    | `import x from 'x'` oder `import { y } from 'x'` |
| Export          | `module.exports`            | `export` / `export default`                      |
| Tree-Shaking    | ❌ Nicht möglich             | ✅ Möglich (optimierte Bundles)                   |
| Top-Level Await | ❌ Nicht unterstützt         | ✅ Unterstützt                                    |

---

### **Besonderheiten**

* In **ESM** kann man **CJS-Module** importieren:

  ```js
  import pkg from 'lodash'; // lodash ist CJS
  ```
* In **CJS** kann man **ESM nur dynamisch** laden:

  ```js
  async function loadModule() {
    const esm = await import('./esmModule.mjs');
    esm.doSomething();
  }
  ```

---

### **Zusammenfassung**

* **require**: CommonJS, synchron, für ältere Node.js-Projekte.
* **import**: ES Modules, moderner Standard, asynchron, für neue Projekte.
* Heutzutage wird für **neue Node.js-Projekte ESM (import)** empfohlen.

📖 Quellen:

* [Node.js Docs – require (CJS)](https://nodejs.org/docs/latest/api/modules.html#requireid)
* [Node.js Docs – import (ESM)](https://nodejs.org/docs/latest/api/esm.html#import-statements)
* [MDN – import](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Statements/import)

---

  **[⬆ Наверх](#top)**

132. ### <a name="132"></a> Unterschied zwischen module.exports und exports?

### **Grundidee**

In **CommonJS (CJS)** sind `module.exports` und `exports` eng miteinander verbunden:

* `module.exports` ist das **eigentliche Objekt**, das aus einer Datei exportiert wird.
* `exports` ist nur eine **Referenz** auf `module.exports`.

Am Anfang gilt:

```js
module.exports === exports; // true
```

---

### **1. module.exports**

* Das **wirkliche Export-Objekt**.
* Alles, was hier zugewiesen wird, ist nach außen sichtbar.

**Beispiel:**

```js
// math.js
module.exports = function add(a, b) {
  return a + b;
};

// index.js
const add = require('./math');
console.log(add(2, 3)); // 5
```

➡️ Hier wird eine **Funktion direkt exportiert**.

---

### **2. exports**

* Ein **Alias auf module.exports**.
* Praktisch für **mehrere Exporte**.

**Beispiel:**

```js
// math.js
exports.add = (a, b) => a + b;
exports.sub = (a, b) => a - b;

// index.js
const math = require('./math');
console.log(math.add(5, 2)); // 3
console.log(math.sub(5, 2)); // 3
```

---

### ⚠️ Wichtig

Wenn du `exports` **neu zuweist**, verliert es die Verbindung zu `module.exports`.

**Beispiel – Fehler:**

```js
// math.js
exports = function add(a, b) { return a + b; };

// index.js
const add = require('./math');
console.log(add(2, 3)); // ❌ undefined
```

➡️ Weil hier nur `exports` überschrieben wird, aber nicht `module.exports`.

**Richtige Version:**

```js
module.exports = function add(a, b) { return a + b; };
```

---

### **Vergleich**

| Merkmal              | `module.exports`                      | `exports`                                 |
| -------------------- | ------------------------------------- | ----------------------------------------- |
| Was es ist           | Das echte Export-Objekt               | Alias/Referenz auf module.exports         |
| Nutzung              | Für Einzel-Export oder Überschreibung | Für mehrere Property-Exporte              |
| Alias zu Beginn      | ✅ Gleich                              | ✅ Gleich                                  |
| Neu zuweisen möglich | ✅ Ja                                  | ⚠️ Nein (dann verliert es die Verbindung) |

---

### **Zusammenfassung**

* `module.exports` = **das eigentliche Export-Objekt** (wird von `require` zurückgegeben).
* `exports` = **Referenz auf module.exports**, praktisch für mehrere Exporte.
* **Nie `exports = ...` nutzen**, sondern immer `module.exports = ...`, wenn man das Objekt komplett ersetzen will.

📖 Quellen:

* [Node.js Docs – module.exports](https://nodejs.org/docs/latest/api/modules.html#moduleexports)
* [MDN – CommonJS](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Modules/Modules_commonjs)

---

  **[⬆ Наверх](#top)**

133. ### <a name="133"></a> Wie setzt man Umgebungsvariablen in Node.js (process.env)?

### **Umgebungsvariablen in Node.js**

Umgebungsvariablen werden in Node.js über das Objekt **`process.env`** bereitgestellt.
Sie dienen dazu, **Konfigurationswerte** wie API-Keys, Datenbank-URLs oder Ports **außerhalb des Codes** zu speichern.

---

### **1. Zugriff**

```js
// Zugriff auf eine Variable
console.log(process.env.NODE_ENV); // z. B. "development"
console.log(process.env.PORT);     // z. B. 3000
```

---

### **2. Setzen von Umgebungsvariablen**

#### a) Direkt beim Starten

* **Linux / macOS**

```bash
PORT=4000 NODE_ENV=production node server.js
```

* **Windows (CMD)**

```cmd
set PORT=4000 && set NODE_ENV=production && node server.js
```

* **Windows (PowerShell)**

```powershell
$env:PORT=4000; $env:NODE_ENV="production"; node server.js
```

---

#### b) Nutzung einer `.env`-Datei mit `dotenv`

1. Installation:

```bash
npm install dotenv
```

2. `.env` Datei:

```
PORT=5000
NODE_ENV=development
DB_HOST=localhost
```

3. Nutzung in Node.js:

```js
require('dotenv').config();

console.log(process.env.PORT);     // 5000
console.log(process.env.DB_HOST);  // localhost
```

---

### **3. Typische Verwendung in Express**

```js
const express = require('express');
require('dotenv').config();

const app = express();
const PORT = process.env.PORT || 3000;

app.listen(PORT, () => {
  console.log(`Server läuft auf Port ${PORT}`);
});
```

---

### **Best Practices**

* **Keine geheimen Schlüssel im Code** → immer in `.env`.
* `.env` in **.gitignore** eintragen.
* Für Produktion: Variablen direkt im **Deployment-Environment** setzen (z. B. Docker, Kubernetes, Vercel, Heroku).

---

### **Zusammenfassung**

* Zugriff über **`process.env`**.
* Setzen per CLI (`PORT=3000 node app.js`) oder `.env` + `dotenv`.
* Wichtig für **Konfigurationsmanagement und Sicherheit**.

📖 Quellen:

* [Node.js Docs – process.env](https://nodejs.org/docs/latest/api/process.html#processenv)
* [dotenv Doku](https://www.npmjs.com/package/dotenv)

---

  **[⬆ Наверх](#top)**

134. ### <a name="134"></a> Was ist package-lock.json und warum wichtig?

### **package-lock.json**

Die Datei **`package-lock.json`** wird automatisch von **npm** erstellt, wenn du Pakete installierst.
Sie dokumentiert den **exakten Zustand der Abhängigkeiten** in einem Projekt.

---

### **Hauptzwecke**

1. **Exakte Versionssicherung**

   * Speichert die **konkreten Versionen** aller installierten Pakete (inkl. Unterabhängigkeiten).
   * Gewährleistet, dass alle Entwickler\:innen und Deployments **identische Pakete** nutzen.

2. **Schnellere Installationen**

   * npm kann Abhängigkeiten direkt aus `package-lock.json` installieren, ohne die Versionen neu aufzulösen.

3. **Sicherheit & Nachvollziehbarkeit**

   * Hilft beim **Auditing** (`npm audit`), da exakte Versionen bekannt sind.
   * Stellt sicher, dass keine unerwarteten Updates Bugs oder Sicherheitslücken einschleusen.

---

### **Beispiel**

`package.json` (nur Hauptpakete):

```json
{
  "dependencies": {
    "express": "^4.18.0"
  }
}
```

`package-lock.json` (genauer Zustand inkl. Unterabhängigkeiten):

```json
{
  "name": "mein-projekt",
  "lockfileVersion": 3,
  "dependencies": {
    "express": {
      "version": "4.18.2",
      "resolved": "https://registry.npmjs.org/express/-/express-4.18.2.tgz",
      "integrity": "sha512-...",
      "requires": {
        "accepts": "~1.3.8",
        "body-parser": "1.20.1"
      }
    }
  }
}
```

➡️ Während `package.json` nur sagt *„nimm eine 4.x Version von Express“*, fixiert `package-lock.json` exakt **4.18.2** + alle Unterabhängigkeiten.

---

### **Best Practices**

* **Immer im Repository versionieren** (zusammen mit `package.json`).
* **Nicht manuell bearbeiten** → nur durch `npm install` ändern lassen.
* Für Produktionsumgebungen:

  ```bash
  npm ci
  ```

  → Installiert **exakt** nach `package-lock.json` (schneller, stabiler).

---

### **Zusammenfassung**

* `package.json` = gewünschte Abhängigkeiten (mit Version-Range).
* `package-lock.json` = exakte Abhängigkeitsstruktur mit Versionen.
* Wichtig für **Reproduzierbarkeit, Konsistenz und Sicherheit** in Node.js-Projekten.

📖 Quellen:

* [npm Docs – package-lock.json](https://docs.npmjs.com/cli/v9/configuring-npm/package-lock-json)
* [npm Docs – npm ci](https://docs.npmjs.com/cli/v9/commands/npm-ci)

---

  **[⬆ Наверх](#top)**

135. ### <a name="135"></a> Unterschied zwischen global und lokaler Installation von npm-Paketen?

### **Lokale Installation**

* Standardmäßig installiert npm Pakete **projektbezogen** im Ordner `node_modules`.
* Abhängigkeiten werden in **`package.json` → dependencies/devDependencies** gespeichert.
* Jedes Projekt kann unterschiedliche Versionen desselben Pakets nutzen.

**Beispiel:**

```bash
npm install express
```

→ installiert `express` in `./node_modules/express`
→ Eintrag in `package.json`

```json
"dependencies": {
  "express": "^4.18.2"
}
```

---

### **Globale Installation**

* Pakete werden **systemweit** installiert.
* Geeignet für **CLI-Tools**, die von überall aufrufbar sein sollen.
* Abhängig vom Betriebssystem landen sie z. B. unter:

  * Linux/macOS: `/usr/local/lib/node_modules`
  * Windows: `%AppData%\npm\node_modules`

**Beispiel:**

```bash
npm install -g nodemon
```

→ `nodemon` kann jetzt überall im Terminal genutzt werden:

```bash
nodemon server.js
```

---

### **Vergleich**

| Merkmal                | Lokale Installation                     | Globale Installation                        |
| ---------------------- | --------------------------------------- | ------------------------------------------- |
| Speicherort            | `./node_modules` im Projekt             | Systemweit (`/usr/local/...`)               |
| Sichtbarkeit           | Nur im Projekt verfügbar                | Überall verfügbar (CLI)                     |
| Nutzung                | Bibliotheken, Frameworks, Projektabh.   | Tools wie `nodemon`, `eslint`, `npm`        |
| Versionsunabhängigkeit | Jedes Projekt kann eigene Version haben | Alle Projekte teilen eine Version           |
| package.json Eintrag   | Ja (`dependencies`)                     | Nein (außer man installiert explizit lokal) |

---

### **Best Practices**

* **Lokal installieren**: Bibliotheken/Frameworks (Express, React, Sequelize).
* **Global installieren**: Nur CLI-Tools, die projektübergreifend gebraucht werden (z. B. `nodemon`, `eslint`, `typescript`).
* Für Build/CI/CD → immer **lokale Installation** (reproduzierbar mit `package-lock.json`).

---

### **Zusammenfassung**

* **Lokal**: im Projekt, für Abhängigkeiten (Standard).
* **Global**: systemweit, für Tools im Terminal.
* Regel: *Bibliotheken lokal, Tools global.*

📖 Quellen:

* [npm Docs – global vs local installation](https://docs.npmjs.com/downloading-and-installing-packages-globally)
* [npm Docs – installing locally](https://docs.npmjs.com/downloading-and-installing-packages-locally)

---

  **[⬆ Наверх](#top)**

136. ### <a name="136"></a> Was sind Worker Threads in Node.js?

### **Worker Threads in Node.js**

**Problem:**
Node.js läuft standardmäßig **Single-Threaded**. Für **I/O-bound Tasks** (Datenbank, Netzwerk, Filesystem) reicht das, da Non-Blocking I/O effizient arbeitet.
Aber bei **CPU-bound Tasks** (z. B. Bildbearbeitung, Verschlüsselung, Machine Learning) blockiert der Event Loop → die App wird langsam.

**Lösung:**
Mit **Worker Threads** kann man **JavaScript in separaten Threads** ausführen, ohne den Haupt-Event-Loop zu blockieren.

---

### **Hauptmerkmale**

* Jeder Worker hat **eigenen Event Loop, V8-Instanz und Speicher**.
* Kommunikation erfolgt über **Message Passing** (`postMessage` / `on('message')`).
* Daten können auch über **SharedArrayBuffer** gemeinsam genutzt werden.
* Ideal für **CPU-intensive Berechnungen**.

---

### **Beispiel**

```js
// worker.js
const { parentPort } = require('worker_threads');

// Lange Berechnung
let result = 0;
for (let i = 0; i < 1e9; i++) {
  result += i;
}

parentPort.postMessage(result);
```

```js
// main.js
const { Worker } = require('worker_threads');

console.log("Main Thread gestartet");

const worker = new Worker('./worker.js');

worker.on('message', result => {
  console.log("Ergebnis aus Worker:", result);
});

console.log("Main Thread blockiert nicht");
```

**Mögliche Ausgabe:**

```
Main Thread gestartet
Main Thread blockiert nicht
Ergebnis aus Worker: 499999999500000000
```

➡️ Der Main Thread bleibt responsiv, während der Worker rechnet.

---

### **Vergleich zu Child Processes**

| Merkmal       | Worker Threads               | Child Processes (z. B. `spawn`)                    |
| ------------- | ---------------------------- | -------------------------------------------------- |
| Sprache       | JS im gleichen Prozess       | Separater Prozess (kann auch andere Sprachen sein) |
| Speicher      | Gemeinsamer Speicher möglich | Kein gemeinsamer Speicher                          |
| Kommunikation | Schneller (In-Memory)        | Langsamer (IPC)                                    |
| Einsatzgebiet | CPU-intensive Tasks in JS    | Externe Programme, Multisprache                    |

---

### **Zusammenfassung**

* **Worker Threads** = parallele Threads für **CPU-bound Tasks** in Node.js.
* Lösen Performanceprobleme bei rechenintensiven Aufgaben.
* Kommunikation über **Messages** oder **Shared Memory**.
* Unterschied zu Child Processes: leichter, schneller, aber auf JavaScript beschränkt.

📖 Quellen:

* [Node.js Docs – Worker Threads](https://nodejs.org/api/worker_threads.html)
* [MDN – Web Workers (ähnliches Konzept im Browser)](https://developer.mozilla.org/de/docs/Web/API/Web_Workers_API/Using_web_workers)

---

  **[⬆ Наверх](#top)**

137. ### <a name="137"></a> Unterschied zwischen cluster und child_process?

### **1. child\_process Modul**

* Dient zum **Starten neuer Prozesse** in Node.js.
* Jeder Prozess hat **eigene Speicherumgebung, eigenen Event Loop und eigene V8-Instanz**.
* Kommunikation über **Inter-Process Communication (IPC)**: `process.send()` und Events.
* Kann auch **externe Programme/Skripte** starten (z. B. `python`, `bash`).

**Beispiel:**

```js
const { spawn } = require('child_process');

const ls = spawn('ls', ['-lh']); // Linux/macOS

ls.stdout.on('data', data => {
  console.log(`Output: ${data}`);
});
```

➡️ Hier wird ein **Bash-Befehl** als separater Prozess gestartet.

---

### **2. cluster Modul**

* Baut **auf child\_process** auf.
* Speziell entwickelt, um Node.js-Server auf **mehreren CPU-Kernen** parallel laufen zu lassen.
* Jeder Cluster-Worker ist ein eigener Node.js-Prozess (wie bei `child_process`), aber die Verwaltung übernimmt das **cluster-Modul**.
* Hauptprozess („Master“) verteilt eingehende Verbindungen automatisch an Worker-Prozesse.

**Beispiel:**

```js
const cluster = require('cluster');
const http = require('http');
const os = require('os');

if (cluster.isPrimary) {
  const numCPUs = os.cpus().length;

  console.log(`Master ${process.pid} läuft`);
  for (let i = 0; i < numCPUs; i++) {
    cluster.fork(); // Startet Worker
  }
} else {
  http.createServer((req, res) => {
    res.writeHead(200);
    res.end(`Hallo von Worker ${process.pid}`);
  }).listen(3000);

  console.log(`Worker ${process.pid} gestartet`);
}
```

➡️ Master verteilt eingehende Anfragen auf mehrere Worker.

---

### **Vergleich**

| Merkmal          | **child\_process**                                  | **cluster**                                 |
| ---------------- | --------------------------------------------------- | ------------------------------------------- |
| Zweck            | Beliebige Prozesse starten (auch externe Programme) | Speziell für Skalierung von Node.js-Servern |
| Architektur      | Eigenes Management durch Entwickler                 | Automatisiertes Master/Worker-System        |
| Kommunikation    | IPC (`process.send`)                                | IPC (eingebaut für Master ↔ Worker)         |
| CPU-Auslastung   | Nicht optimiert                                     | Nutzt alle CPU-Kerne                        |
| Typische Nutzung | Skripte starten, Python, Shell-Befehle              | HTTP/Express-Server skalieren               |

---

### **Zusammenfassung**

* **child\_process**: Generisches Modul, startet neue Prozesse (Node.js oder externe Programme).
* **cluster**: Nutzt intern `child_process`, aber optimiert für **Lastverteilung auf mehrere CPU-Kerne** bei Node.js-Servern.

📖 Quellen:

* [Node.js Docs – child\_process](https://nodejs.org/api/child_process.html)
* [Node.js Docs – cluster](https://nodejs.org/api/cluster.html)

---

  **[⬆ Наверх](#top)**

138. ### <a name="138"></a> Wie behandelt man Exceptions (try/catch vs. process.on('uncaughtException'))?

### **1. Exceptions mit try/catch**

* Standardmethode für **synchronen Code**.
* Fängt Fehler ab, bevor sie den Event Loop verlassen.
* Sollte **immer bevorzugt** werden.

**Beispiel:**

```js
try {
  const result = JSON.parse("{ invalid json }");
  console.log(result);
} catch (err) {
  console.error("Fehler beim Parsen:", err.message);
}
```

---

### **2. Asynchrone Fehlerbehandlung**

* `try/catch` funktioniert **nicht direkt** bei asynchronem Code (Callbacks, Promises).

**Callback-Beispiel:**

```js
const fs = require('fs');

fs.readFile("file.txt", (err, data) => {
  if (err) {
    console.error("Fehler:", err.message);
    return;
  }
  console.log(data.toString());
});
```

**Promise/async-Beispiel:**

```js
async function loadFile() {
  try {
    const data = await fs.promises.readFile("file.txt", "utf8");
    console.log(data);
  } catch (err) {
    console.error("Fehler:", err.message);
  }
}
```

---

### **3. process.on('uncaughtException')**

* Fängt **ungefangene Fehler** ab, die sonst den Prozess beenden würden.
* **Nur als Notfalllösung** – nicht als normale Fehlerbehandlung!
* Nach einer `uncaughtException` ist der Prozess **instabil** → Empfehlung: **Fehler loggen und Prozess beenden**.

**Beispiel:**

```js
process.on('uncaughtException', (err) => {
  console.error("Uncaught Exception:", err.message);
  // Cleanup (Logs, offene Verbindungen schließen)
  process.exit(1); // kontrollierter Neustart empfohlen (z. B. mit PM2)
});

throw new Error("Fataler Fehler");
```

---

### **Best Practices**

* **Immer try/catch oder Promises mit `.catch()` nutzen** für erwartbare Fehler.
* `process.on('uncaughtException')` nur für Logging/Notfälle.
* Für **unbehandelte Promise-Fehler** gibt es `process.on('unhandledRejection')`.
* In Produktion: Prozessmanager (z. B. **PM2, Docker, Kubernetes**) nutzen, um Neustarts nach Abstürzen sicherzustellen.

---

### **Vergleich**

| Mechanismus                          | Zweck                                               | Empfehlung                          |
| ------------------------------------ | --------------------------------------------------- | ----------------------------------- |
| **try/catch**                        | Normale Fehlerbehandlung (sync/async via `await`)   | ✅ Ja                                |
| **Callback-Error-Pattern** (`err`)   | Asynchrone Fehlerbehandlung in Callbacks            | ✅ Ja                                |
| **process.on('uncaughtException')**  | Letzte Rettung, wenn Fehler nicht abgefangen wurden | ⚠️ Nur Logging, Prozess neu starten |
| **process.on('unhandledRejection')** | Fängt nicht behandelte Promise-Rejections           | ⚠️ Logging + Prozess neu starten    |

---

### **Zusammenfassung**

* **try/catch** und `.catch()` für kontrollierte Fehlerbehandlung.
* **process.on('uncaughtException')** = Notfall, Prozess danach beenden.
* Best Practice: Logging + Neustart durch Prozessmanager.

📖 Quellen:

* [Node.js Docs – Error Handling](https://nodejs.org/api/errors.html)
* [Node.js Docs – process events](https://nodejs.org/api/process.html#event-uncaughtexception)

---

  **[⬆ Наверх](#top)**

139. ### <a name="139"></a> Was ist Garbage Collection in Node.js?

### **Garbage Collection in Node.js**

**Definition:**
Garbage Collection (GC) ist der Prozess, bei dem die **V8 Engine** (auf der Node.js läuft) automatisch **nicht mehr genutzte Objekte aus dem Speicher entfernt**, um Speicherplatz freizugeben.

---

### **Wie funktioniert es?**

* Node.js verwendet die **V8 Garbage Collector Implementierung**.
* Nutzt ein **Generational Garbage Collection Modell**:

  1. **New Space (Junggeneration)** → kleine, kurzlebige Objekte.
  2. **Old Space (Alte Generation)** → langlebige Objekte.
  3. **Large Object Space** → sehr große Objekte (z. B. Buffers).
* Der GC verfolgt Referenzen → wenn ein Objekt **nicht mehr erreichbar** ist, wird es entfernt.

---

### **GC-Strategien**

1. **Mark-and-Sweep**

   * GC markiert erreichbare Objekte und löscht alle nicht markierten.

2. **Minor GC**

   * Räumt nur den **New Space** auf (schnell, häufig).

3. **Major GC**

   * Räumt den **Old Space** auf (langsamer, weniger oft).

---

### **Praktisches Beispiel**

```js
function test() {
  let data = new Array(1e6).fill("Hallo"); 
  // 'data' wird nach Funktionsende nicht mehr referenziert
}

test();

// Nach einiger Zeit sammelt der Garbage Collector 'data' ein.
```

---

### **Manuelles Triggern (nicht empfohlen in Produktion)**

```bash
node --expose-gc app.js
```

```js
if (global.gc) {
  global.gc(); // Erzwingt Garbage Collection
}
```

➡️ Nur zu Debugging-Zwecken (z. B. Memory-Leaks analysieren).

---

### **Monitoring Tools**

* `--inspect` mit Chrome DevTools → Heap-Snapshots.
* `clinic.js` oder `node --inspect-brk`.
* APM-Tools (z. B. New Relic, Datadog).

---

### **Best Practices**

* **Keine globalen Variablen ohne Grund** → verhindern Freigabe.
* **Event Listener entfernen**, wenn nicht mehr benötigt.
* **Große Arrays/Objekte dereferenzieren** (`obj = null`).
* Für **Streams** → `.destroy()` oder `.end()` nutzen.

---

### **Zusammenfassung**

* Garbage Collection in Node.js wird durch die **V8 Engine** erledigt.
* Entfernt automatisch **nicht mehr erreichbare Objekte**.
* Arbeitet mit **Minor/Major GC (Generational Model)**.
* Manuelles GC ist möglich, aber nur für Debugging sinnvoll.

📖 Quellen:

* [Node.js Docs – Memory Management](https://nodejs.org/en/docs/guides/garbage-collection/)
* [V8 Blog – Garbage Collection](https://v8.dev/blog/trash-talk)
* [MDN – Garbage collection](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Memory_Management)

---

  **[⬆ Наверх](#top)**

140. ### <a name="140"></a> Welche Nachteile hat Node.js bei CPU-intensiven Aufgaben?

### **Nachteile von Node.js bei CPU-intensiven Aufgaben**

1. **Single-Threaded Event Loop**

   * Node.js arbeitet standardmäßig mit **einem Thread**.
   * CPU-intensive Tasks (z. B. Bildbearbeitung, Hashing, Machine Learning) blockieren den **Event Loop** → keine weiteren Anfragen können bearbeitet werden.

2. **Blockierende Auswirkungen**

   * Während eine rechenintensive Funktion läuft, können **keine I/O-Operationen** (HTTP-Anfragen, DB-Abfragen) bearbeitet werden.
   * Führt zu **hoher Latenz** oder sogar **Time-outs** bei Clients.

3. **Fehlende native Parallelität**

   * Im Gegensatz zu Sprachen wie **Java, Go, C++** bietet Node.js keine echte Thread-basierte Parallelität für CPU-lastige Tasks.
   * Lösung nur über **Worker Threads**, **Cluster** oder **Child Processes**.

4. **Hoher Energieverbrauch bei Workarounds**

   * Parallelisierung über Worker Threads oder Cluster erfordert **mehr Speicher und Prozess-Kommunikation** (Overhead).

5. **Nicht optimal für bestimmte Anwendungen**

   * Schlechte Wahl für:

     * **Video-Transcoding**
     * **Bildverarbeitung**
     * **Wissenschaftliche Berechnungen**
     * **Kryptographie auf hohem Level**

---

### **Beispiel: CPU-bound Blockade**

```js
// CPU-intensive Berechnung
function heavyTask() {
  let sum = 0;
  for (let i = 0; i < 1e9; i++) {
    sum += i;
  }
  return sum;
}

const express = require('express');
const app = express();

app.get('/', (req, res) => {
  const result = heavyTask(); // Blockiert Event Loop
  res.send(`Ergebnis: ${result}`);
});

app.listen(3000, () => console.log("Server läuft auf Port 3000"));
```

➡️ Während `heavyTask()` läuft, können **andere Requests nicht beantwortet werden**.

---

### **Workarounds**

* **Worker Threads** für CPU-intensive Berechnungen.
* **Cluster** für Skalierung über mehrere CPU-Kerne.
* **Microservices-Architektur**: CPU-lastige Aufgaben in separaten Services (z. B. Python).
* **Offloading** in Message Queues (RabbitMQ, Kafka) und Verarbeitung durch spezialisierte Worker.

---

### **Zusammenfassung**

* CPU-intensive Aufgaben blockieren den **Event Loop** → schlechte Skalierung und hohe Latenz.
* Node.js ist für **I/O-bound** Workloads ideal, aber nicht für **CPU-bound**.
* Lösungen: **Worker Threads, Cluster, externe Services**.

📖 Quellen:

* [Node.js Docs – Worker Threads](https://nodejs.org/api/worker_threads.html)
* [Node.js Event Loop Guide](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick)
* [MDN – Concurrency model](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)

---

  **[⬆ Наверх](#top)**  

141. ### <a name="141"></a> Unterschied zwischen Callbacks, Promises und async/await?

**Callbacks**

* Eine Funktion wird als Argument an eine andere Funktion übergeben.
* Wird aufgerufen, wenn die asynchrone Operation fertig ist.
* Nachteil: „Callback Hell“ (verschachtelte Strukturen, schwer lesbarer Code).

```js
// Beispiel mit Callback
import fs from "fs";

fs.readFile("datei.txt", "utf-8", (err, data) => {
  if (err) {
    console.error("Fehler:", err);
    return;
  }
  console.log("Datei-Inhalt:", data);
});
```

---

**Promises**

* Objekt, das einen zukünftigen Wert repräsentiert.
* Hat Zustände: *pending → fulfilled / rejected*.
* Kann mit `.then()` und `.catch()` behandelt werden.
* Ermöglicht Kettenbildung und bessere Fehlerbehandlung.

```js
// Beispiel mit Promise
import fs from "fs/promises";

fs.readFile("datei.txt", "utf-8")
  .then((data) => console.log("Datei-Inhalt:", data))
  .catch((err) => console.error("Fehler:", err));
```

---

**async/await**

* Syntaktischer Zucker für Promises.
* Ermöglicht asynchronen Code in synchronem Stil.
* `await` pausiert die Ausführung, bis das Promise erfüllt oder abgelehnt ist.

```js
// Beispiel mit async/await
import fs from "fs/promises";

async function lesen() {
  try {
    const data = await fs.readFile("datei.txt", "utf-8");
    console.log("Datei-Inhalt:", data);
  } catch (err) {
    console.error("Fehler:", err);
  }
}

lesen();
```

---

### **Zusammenfassung**

* **Callbacks**: direktes Weitergeben von Funktionen → unübersichtlich bei vielen Verschachtelungen.
* **Promises**: strukturierter, mit Ketten (`then/catch`).
* **async/await**: moderner, einfacher zu lesen und zu warten.

📖 Quellen:

* [MDN: Callbacks](https://developer.mozilla.org/ru/docs/Glossary/Callback_function)
* [MDN: Promises](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Promise)
* [MDN: async/await](https://developer.mozilla.org/ru/docs/Learn/JavaScript/Asynchronous/Promises)


  **[⬆ Наверх](#top)**

142. ### <a name="142"></a> Typische Callback-Hell-Beispiele und wie man sie vermeidet?

**Callback-Hell-Beispiel**
Mehrere asynchrone Operationen nacheinander führen zu stark verschachtelten Strukturen:

```js
// Typische Callback-Hell-Struktur
import fs from "fs";

fs.readFile("datei1.txt", "utf-8", (err, data1) => {
  if (err) return console.error(err);

  fs.readFile("datei2.txt", "utf-8", (err, data2) => {
    if (err) return console.error(err);

    fs.readFile("datei3.txt", "utf-8", (err, data3) => {
      if (err) return console.error(err);

      console.log("Ergebnis:", data1, data2, data3);
    });
  });
});
```

Probleme:

* Schwer lesbarer und wartbarer Code
* Fehlerbehandlung muss in jedem Schritt wiederholt werden
* Logik ist schwer nachzuvollziehen

---

**Vermeidung mit Promises**

```js
// Promises statt verschachtelter Callbacks
import fs from "fs/promises";

fs.readFile("datei1.txt", "utf-8")
  .then((data1) =>
    fs.readFile("datei2.txt", "utf-8").then((data2) => [data1, data2])
  )
  .then(([data1, data2]) =>
    fs.readFile("datei3.txt", "utf-8").then((data3) => [data1, data2, data3])
  )
  .then(([data1, data2, data3]) => {
    console.log("Ergebnis:", data1, data2, data3);
  })
  .catch((err) => console.error("Fehler:", err));
```

---

**Vermeidung mit async/await**

```js
// Klarer und besser lesbar mit async/await
import fs from "fs/promises";

async function main() {
  try {
    const data1 = await fs.readFile("datei1.txt", "utf-8");
    const data2 = await fs.readFile("datei2.txt", "utf-8");
    const data3 = await fs.readFile("datei3.txt", "utf-8");

    console.log("Ergebnis:", data1, data2, data3);
  } catch (err) {
    console.error("Fehler:", err);
  }
}

main();
```

---

**Best Practices zur Vermeidung von Callback-Hell**

* **Promises** oder **async/await** verwenden
* **Promise.all()** nutzen, wenn Aufgaben parallel ausführbar sind

```js
// Parallel mit Promise.all()
const [data1, data2, data3] = await Promise.all([
  fs.readFile("datei1.txt", "utf-8"),
  fs.readFile("datei2.txt", "utf-8"),
  fs.readFile("datei3.txt", "utf-8"),
]);
console.log("Parallel Ergebnis:", data1, data2, data3);
```

---

### **Zusammenfassung**

* Callback-Hell entsteht durch **tiefe Verschachtelung** asynchroner Funktionen.
* Lösung: **Promises** oder **async/await** einsetzen.
* Mit `Promise.all()` können unabhängige Tasks parallel laufen.

📖 Quellen:

* [MDN – Callback-Funktion](https://developer.mozilla.org/ru/docs/Glossary/Callback_function)
* [MDN – Promise](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Promise)
* [Node.js – fs/promises](https://nodejs.org/docs/latest/api/fs.html#fspromisesapi)

---


  **[⬆ Наверх](#top)**

143. ### <a name="143"></a> Wie funktioniert Promise.all()?

**Funktionsweise von `Promise.all()`**

* Nimmt ein **Array von Promises** entgegen.
* Gibt ein **neues Promise** zurück.
* Dieses Promise wird:

  * **fulfilled**, wenn *alle* Promises erfüllt sind → liefert ein Array mit den Ergebnissen in derselben Reihenfolge wie die Eingabe.
  * **rejected**, wenn *ein einziges* Promise fehlschlägt → sofort abgelehnt mit dem ersten Fehler.

---

**Beispiel mit mehreren Promises**

```js
function task(ms, name) {
  return new Promise((resolve) =>
    setTimeout(() => resolve(`${name} fertig`), ms)
  );
}

async function runTasks() {
  try {
    const results = await Promise.all([
      task(1000, "A"),
      task(2000, "B"),
      task(1500, "C"),
    ]);

    console.log(results); 
    // Ausgabe nach ca. 2 Sek: ["A fertig", "B fertig", "C fertig"]
  } catch (err) {
    console.error("Fehler:", err);
  }
}

runTasks();
```

---

**Beispiel mit Fehler**

```js
function task(ms, name, fail = false) {
  return new Promise((resolve, reject) =>
    setTimeout(() => {
      fail ? reject(new Error(`${name} fehlgeschlagen`)) : resolve(`${name} fertig`);
    }, ms)
  );
}

async function runTasks() {
  try {
    const results = await Promise.all([
      task(1000, "A"),
      task(2000, "B", true), // schlägt fehl
      task(1500, "C"),
    ]);

    console.log(results);
  } catch (err) {
    console.error("Fehler gefangen:", err.message); 
    // Ausgabe: "Fehler gefangen: B fehlgeschlagen"
  }
}

runTasks();
```

---

**Typische Anwendungsfälle**

* Mehrere **unabhängige API-Requests** parallel ausführen.
* Dateien gleichzeitig laden.
* Datenbank-Queries parallel absetzen.

---

### **Zusammenfassung**

* `Promise.all()` → führt Promises **parallel** aus.
* Liefert Ergebnisse als Array in **gleicher Reihenfolge** zurück.
* Wird **sofort rejected**, wenn eines der Promises fehlschlägt.

📖 Quellen:

* [MDN: Promise.all()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Promise/all)
* [Node.js Promise APIs](https://nodejs.org/docs/latest/api/esm.html#promises)

---

  **[⬆ Наверх](#top)**

144. ### <a name="144"></a> Unterschied zwischen Promise.allSettled() und Promise.race()?

**`Promise.allSettled()`**

* Wartet, bis **alle Promises abgeschlossen** sind (egal ob fulfilled oder rejected).
* Gibt ein Array mit Objekten zurück, die den Status und das Ergebnis jedes Promises enthalten.
* Kein Abbruch bei Fehlern → nützlich, wenn man *alle Ergebnisse* braucht.

```js
const promises = [
  Promise.resolve("A fertig"),
  Promise.reject("B Fehler"),
  Promise.resolve("C fertig"),
];

const result = await Promise.allSettled(promises);

console.log(result);
/*
[
  { status: "fulfilled", value: "A fertig" },
  { status: "rejected", reason: "B Fehler" },
  { status: "fulfilled", value: "C fertig" }
]
*/
```

---

**`Promise.race()`**

* Liefert das Ergebnis des **ersten beendeten Promises** (egal ob fulfilled oder rejected).
* Nützlich, wenn nur das **schnellste Ergebnis** zählt (z. B. Timeout-Strategien).

```js
function task(ms, name, fail = false) {
  return new Promise((resolve, reject) =>
    setTimeout(() => fail ? reject(`${name} Fehler`) : resolve(`${name} fertig`), ms)
  );
}

try {
  const result = await Promise.race([
    task(2000, "A"),
    task(1000, "B"),
    task(1500, "C", true),
  ]);

  console.log(result); // Ausgabe nach 1 Sek: "B fertig"
} catch (err) {
  console.error("Fehler:", err);
}
```

---

### **Vergleich**

| Methode                  | Verhalten                                                       |
| ------------------------ | --------------------------------------------------------------- |
| **Promise.allSettled()** | Wartet auf alle → liefert Array mit Status & Wert/Fehler        |
| **Promise.race()**       | Liefert Ergebnis des ersten erfüllten/fehlgeschlagenen Promises |

---

### **Zusammenfassung**

* **`Promise.allSettled()`**: immer vollständiger Überblick, keine Abbrüche.
* **`Promise.race()`**: erstes Promise „gewinnt“, egal ob Erfolg oder Fehler.

📖 Quellen:

* [MDN: Promise.allSettled()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Promise/allSettled)
* [MDN: Promise.race()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Promise/race)

---

  **[⬆ Наверх](#top)**

145. ### <a name="145"></a> Wie funktioniert async/await intern?

**Funktionsweise von `async/await` intern**

1. **`async` Funktion**

   * Deklariert man eine Funktion mit `async`, wird sie **immer ein Promise zurückgeben**, egal ob man explizit ein Promise zurückgibt oder nicht.
   * Rückgabewert:

     * `return <Wert>` → wird zu `Promise.resolve(<Wert>)`
     * `throw <Fehler>` → wird zu `Promise.reject(<Fehler>)`

```js
async function test() {
  return 42; 
}
console.log(test()); // Promise { 42 }
```

---

2. **`await` Ausdruck**

   * `await` pausiert die Ausführung innerhalb der `async` Funktion, bis das Promise erfüllt oder abgelehnt ist.
   * Intern nutzt JavaScript den **Event Loop** und die **Microtask Queue** (Promises werden dort abgearbeitet).
   * Der restliche Code wird nach Erfüllung in eine neue Microtask gelegt.

```js
async function demo() {
  console.log("Start");
  const result = await Promise.resolve("fertig");
  console.log(result); // nach Microtask
  console.log("Ende");
}

demo();
console.log("außerhalb");

// Ausgabe:
// Start
// außerhalb
// fertig
// Ende
```

---

3. **Übersetzung in Promises**

   * `async/await` ist syntaktischer Zucker für Promises + `.then()`.
   * Beispiel mit `await`:

```js
// Mit async/await
async function lesen() {
  const data = await Promise.resolve("Daten");
  return data;
}

// Entspricht in etwa
function lesen() {
  return Promise.resolve("Daten").then((data) => {
    return data;
  });
}
```

---

4. **Fehlerbehandlung**

   * Mit `try/catch` abfangen → entspricht `.catch()` bei Promises.

```js
async function fehler() {
  try {
    const res = await Promise.reject("Problem");
    console.log(res);
  } catch (err) {
    console.error("Gefangen:", err);
  }
}

// Entspricht:
Promise.reject("Problem").catch((err) => console.error("Gefangen:", err));
```

---

### **Zusammenfassung**

* `async` → Funktion gibt immer ein **Promise** zurück.
* `await` → pausiert innerhalb der Funktion, setzt Rest in die **Microtask Queue**.
* Intern wird `async/await` zu einer Kombination aus **Promises + then/catch** kompiliert.
* Fehlerbehandlung über `try/catch`.

📖 Quellen:

* [MDN: async/await](https://developer.mozilla.org/ru/docs/Learn/JavaScript/Asynchronous/Promises#async_and_await)
* [Node.js Doku – Async Functions](https://nodejs.org/docs/latest/api/async_context.html)

---

  **[⬆ Наверх](#top)**

146. ### <a name="146"></a> Warum ist Error-Handling bei async/await kritisch?

**Warum Error-Handling bei `async/await` kritisch ist**

1. **Alle `async` Funktionen geben ein Promise zurück**

   * Wird ein Fehler geworfen (`throw`), entspricht das einem **`Promise.reject()`**.
   * Ohne Fehlerbehandlung endet das Promise abgelehnt → „UnhandledPromiseRejection“.
   * In Node.js führt das zu Warnungen, in neueren Versionen sogar zum Prozessabbruch.

---

2. **Fehler werden „unsichtbar“ ohne `try/catch`**

   * Anders als bei synchronem Code stoppt ein Fehler nicht sofort das Programm.
   * Der Fehler landet im Promise und muss explizit abgefangen werden.

```js
async function fehler() {
  JSON.parse("ungültig"); // SyntaxError
}

fehler(); 
// Ohne catch → UnhandledPromiseRejectionWarning in Node.js
```

---

3. **Best Practices für Error-Handling**

* **try/catch innerhalb async Funktionen**

```js
async function demo() {
  try {
    const res = await Promise.reject("Fehler!");
    console.log(res);
  } catch (err) {
    console.error("Gefangen:", err);
  }
}
demo();
```

* **`.catch()` beim Aufruf**

```js
async function api() {
  throw new Error("API down");
}

api().catch((err) => console.error("Fehler behandelt:", err.message));
```

* **Globale Fehlerbehandlung in Node.js**

```js
process.on("unhandledRejection", (reason) => {
  console.error("Unbehandeltes Promise:", reason);
});
```

---

4. **Warum kritisch?**

* Ohne sauberes Error-Handling → schwer reproduzierbare Bugs.
* Produktionssysteme können abstürzen oder in undefiniertem Zustand bleiben.
* In Backend-Apps (z. B. Express) muss man Fehler **immer** abfangen und an die Middleware weiterleiten.

---

### **Zusammenfassung**

* Fehler in `async/await` sind **Promises**, nicht normale Exceptions.
* Ohne **explizites Handling** drohen *UnhandledPromiseRejections* → instabile Anwendungen.
* Lösung: **try/catch**, `.catch()`, oder globale Fehler-Handler.

📖 Quellen:

* [MDN: Fehlerbehandlung bei async/await](https://developer.mozilla.org/ru/docs/Learn/JavaScript/Asynchronous/Promises#%D0%9E%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0_%D0%BE%D1%88%D0%B8%D0%B1%D0%BE%D0%BA)
* [Node.js Errors & Rejections](https://nodejs.org/docs/latest/api/process.html#event-unhandledrejection)

---

  **[⬆ Наверх](#top)**

147. ### <a name="147"></a> Unterschied zwischen for...of und forEach in async Code?

**Unterschied zwischen `for...of` und `forEach` in async Code**

---

### **`forEach`**

* Erwartet eine Callback-Funktion.
* Ignoriert `await` im Callback → der äußere Code wartet nicht.
* Läuft sofort durch, ohne die asynchronen Operationen abzuwarten.

```js
// Fehlerhaftes Verhalten
const arr = [1, 2, 3];

arr.forEach(async (num) => {
  await new Promise((res) => setTimeout(res, 1000));
  console.log(num);
});

console.log("Ende");
// Ausgabe:
// Ende (sofort)
// 1
// 2
// 3   (mit Verzögerung, aber parallel, nicht nacheinander)
```

---

### **`for...of`**

* Unterstützt `await` direkt.
* Jeder Durchlauf wartet auf den Abschluss des vorherigen → sequentielle Ausführung.

```js
const arr = [1, 2, 3];

for (const num of arr) {
  await new Promise((res) => setTimeout(res, 1000));
  console.log(num);
}

console.log("Ende");
// Ausgabe:
// 1 (nach 1 Sekunde)
// 2 (nach 2 Sekunden)
// 3 (nach 3 Sekunden)
// Ende
```

---

### **Parallel mit `Promise.all()`**

* Falls Operationen unabhängig sind, ist parallele Ausführung effizienter.

```js
const arr = [1, 2, 3];

await Promise.all(
  arr.map(async (num) => {
    await new Promise((res) => setTimeout(res, 1000));
    console.log(num);
  })
);

console.log("Ende");
// Ausgabe nach ~1 Sek: 1, 2, 3 (Reihenfolge nicht garantiert)
```

---

### **Vergleich**

| Kriterium       | `forEach`                            | `for...of`                      |
| --------------- | ------------------------------------ | ------------------------------- |
| `await` Support | Ignoriert `await` im Callback        | Unterstützt `await` nativ       |
| Ablauf          | Alles fast sofort → unkontrolliert   | Sequentiell, wartet pro Schritt |
| Parallelität    | Pseudo-parallel (nicht kontrolliert) | Seriell, aber zuverlässig       |
| Empfehlung      | Nicht für async geeignet             | Standard für async Iterationen  |

---

### **Zusammenfassung**

* `forEach` ist **nicht async-freundlich** → `await` wirkt dort nicht.
* `for...of` erlaubt **korrektes sequentielles Warten**.
* Für parallele Tasks → **`Promise.all()`** mit `.map()`.

📖 Quellen:

* [MDN: for...of](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for...of)
* [MDN: Array.prototype.forEach()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)

---

  **[⬆ Наверх](#top)**

148. ### <a name="148"></a> Was sind EventEmitter in Node.js?

**EventEmitter in Node.js**

1. **Definition**

* `EventEmitter` ist ein zentrales Modul in Node.js (`events`-Modul).
* Es implementiert das **Publisher/Subscriber-Muster**.
* Ein Objekt kann Ereignisse („events“) **emittieren** und andere Teile des Codes können darauf mit **Listenern** reagieren.

---

2. **Grundprinzip**

* `emitter.on(event, listener)` → registriert Listener.
* `emitter.emit(event, args)` → löst Ereignis aus.
* `emitter.removeListener` / `emitter.off` → entfernt Listener.
* `emitter.once` → Listener wird nur einmal ausgeführt.

---

3. **Beispiel**

```js
import { EventEmitter } from "events";

const emitter = new EventEmitter();

// Listener registrieren
emitter.on("greet", (name) => {
  console.log(`Hallo, ${name}!`);
});

// Event auslösen
emitter.emit("greet", "Sergii"); 
// Ausgabe: "Hallo, Sergii!"
```

---

4. **`once` Beispiel**

```js
emitter.once("init", () => {
  console.log("Initialisierung nur einmal!");
});

emitter.emit("init");  // wird ausgeführt
emitter.emit("init");  // wird ignoriert
```

---

5. **Praktische Anwendungsfälle**

* Kommunikation zwischen Modulen innerhalb einer Node.js-App.
* Eigene Events in Streams, Datenbanken oder Sockets.
* In Frameworks wie **Express** intern stark genutzt (z. B. `req`, `res` sind EventEmitter).

```js
// Beispiel mit HTTP-Server
import http from "http";

const server = http.createServer((req, res) => {
  res.end("Hallo Welt");
});

// EventEmitter im Einsatz
server.on("request", (req, res) => {
  console.log(`Neue Anfrage: ${req.url}`);
});

server.listen(3000);
```

---

### **Zusammenfassung**

* `EventEmitter` ist das Node.js-Pattern für Events (Pub/Sub).
* Methoden: `.on`, `.emit`, `.once`, `.off`.
* Basis für Streams, HTTP-Server, Socket.io, interne Node.js-Mechanismen.

📖 Quellen:

* [Node.js Dokumentation – EventEmitter](https://nodejs.org/docs/latest/api/events.html)
* [MDN: Observer Pattern (Grundidee)](https://developer.mozilla.org/ru/docs/Archive/Add-ons/Observer_Notifications)

---

  **[⬆ Наверх](#top)**

149. ### <a name="149"></a> Wie implementiert man Custom Events mit EventEmitter?

**Custom Events mit `EventEmitter` implementieren**

---

### 1) Eigene Event-Quelle erstellen (Klasse erweitern)

```js
// events/UserService.js
import { EventEmitter } from "events";

export class UserService extends EventEmitter {
  async createUser(payload) {
    // … Domain-Logik, z. B. DB-Insert
    const user = { id: 1, ...payload };
    this.emit("user:created", user);      // Custom Event
    return user;
  }

  async deleteUser(id) {
    // … DB-Löschung
    this.emit("user:deleted", { id });     // Custom Event
  }
}
```

**Verwendung & Listener registrieren**

```js
// app.js
import { UserService } from "./events/UserService.js";

const users = new UserService();

// Listener (Subscriber)
users.on("user:created", (user) => {
  console.log("Neu erstellt:", user);
});

users.on("user:deleted", ({ id }) => {
  console.log("Gelöscht:", id);
});

// einmaliger Listener
users.once("user:created", () => {
  console.log("Dieser Log kommt nur beim ersten Create.");
});

// Events auslösen
await users.createUser({ name: "Sergii" });
await users.deleteUser(1);
```

---

### 2) In Express-Routen emittieren (Entkopplung von Nebenwirkungen)

```js
// routes/users.js
import { Router } from "express";
import { UserService } from "../events/UserService.js";

const router = Router();
const users = new UserService();

router.post("/", async (req, res, next) => {
  try {
    const user = await users.createUser(req.body);
    res.status(201).json(user);
  } catch (e) {
    // Fehler-Event optional
    users.emit("user:error", e);
    next(e);
  }
});

export default router;
```

---

### 3) Best Practices

```js
import { EventEmitter } from "events";

class OrderService extends EventEmitter {
  constructor() {
    super();
    // Optional: Warnungen bei zu vielen Listenern vermeiden/prüfen
    this.setMaxListeners(20);
  }

  async place(order) {
    try {
      // … persistieren
      this.emit("order:placed", order);
    } catch (err) {
      // ACHTUNG: 'error' ist speziell — ohne Listener wirft Node eine Exception
      this.emit("error", err);
    }
  }
}

const orders = new OrderService();

// 'error' immer behandeln!
orders.on("error", (err) => {
  console.error("Order-Fehler:", err);
});

// Abmelden von Listenern
function onPlaced(o) { console.log("Placed:", o.id); }
orders.on("order:placed", onPlaced);

// später:
orders.off("order:placed", onPlaced); // oder removeListener(...)
```

**Wichtige Punkte**

* **Namenskonventionen**: Namensräume wie `"user:created"`, `"order:placed"`.
* **`error`-Event**: Ohne registrierten `error`-Listener wirft Node eine Ausnahme. Immer behandeln.
* **Lebenszyklus**: `on` (mehrfach), `once` (einmalig), `off/removeListener` (abbestellen), `removeAllListeners` (aufräumen).
* **Reihenfolge**: Listener werden in **Registrier-Reihenfolge** synchron aufgerufen.
* **Performance/Leaks**: `setMaxListeners(n)` sinnvoll setzen und ungenutzte Listener abmelden.

---

### 4) Typisierung (optional, TS-Idee in JS über JSDoc)

```js
// Durch JSDoc "Events" dokumentieren
/**
 * @typedef {"user:created"|"user:deleted"|"error"} UserEvents
 */

export class UserService extends EventEmitter {
  /** @param {import("events").Listener} listener */
  on(event, listener) { return super.on(event, listener); }
}
```

---

### **Zusammenfassung**

* Eigene Events = `emit("<namespace:event>", payload)`; Listener mit `on/once` registrieren.
* `error`-Event immer behandeln, sonst Ausnahme.
* Listener-Lebenszyklus aktiv managen (`off`, `removeAllListeners`, `setMaxListeners`).
* In Express sinnvoll für **Entkopplung** (Side-Effects wie Logging, E-Mail, Caching).

📖 Quellen:

* [Node.js Dokumentation – `events`](https://nodejs.org/docs/latest/api/events.html)
* [Node.js – Fehlerereignis `error`](https://nodejs.org/docs/latest/api/events.html#event-error)
* [MDN – Observer/Publish-Subscribe (allg. Konzept)](https://developer.mozilla.org/ru/docs/Archive/Add-ons/Observer_Notifications)


  **[⬆ Наверх](#top)**

150. ### <a name="150"></a> Unterschied zwischen once und on bei Events?

**Unterschied zwischen `.on()` und `.once()` bei Events in Node.js**

---

### `.on(event, listener)`

* Registriert einen Listener für ein bestimmtes Event.
* Der Listener wird **jedes Mal** ausgeführt, wenn das Event ausgelöst wird.
* Typisch für Events, die wiederholt auftreten können (z. B. `"data"`, `"connection"`).

```js
import { EventEmitter } from "events";

const emitter = new EventEmitter();

emitter.on("ping", () => {
  console.log("Ping empfangen");
});

emitter.emit("ping"); // → Ping empfangen
emitter.emit("ping"); // → Ping empfangen (erneut)
```

---

### `.once(event, listener)`

* Registriert einen Listener, der **nur einmal** aufgerufen wird.
* Danach wird der Listener automatisch entfernt.
* Praktisch für Initialisierungen, einmalige Aktionen (z. B. `"ready"`, `"connected"`).

```js
emitter.once("init", () => {
  console.log("Init nur einmal");
});

emitter.emit("init"); // → Init nur einmal
emitter.emit("init"); // → kein Aufruf mehr
```

---

### Vergleich in der Praxis

| Methode | Aufrufhäufigkeit | Einsatzgebiet                                      |
| ------- | ---------------- | -------------------------------------------------- |
| `.on`   | unbegrenzt       | wiederholte Events (z. B. Daten-Streams, Requests) |
| `.once` | nur einmal       | Initialisierung, Setup, einmalige Ereignisse       |

---

### **Zusammenfassung**

* `.on()` → Listener reagiert bei **jedem Event**.
* `.once()` → Listener reagiert **nur beim ersten Mal** und wird dann entfernt.
* Best Practice: `.once()` für Initial-Events, `.on()` für wiederkehrende Events.

📖 Quellen:

* [Node.js Doku – EventEmitter.on()](https://nodejs.org/docs/latest/api/events.html#emitteroneventname-listener)
* [Node.js Doku – EventEmitter.once()](https://nodejs.org/docs/latest/api/events.html#emitteronceeventname-listener)

---

  **[⬆ Наверх](#top)**  

151. ### <a name="151"></a> Unterschied zwischen SQL und NoSQL?

**Unterschied zwischen SQL und NoSQL**

---

### **SQL (Relationale Datenbanken)**

* Strukturierte Daten in **Tabellen** (Zeilen = Datensätze, Spalten = Attribute).
* Statische **Schemas** → feste Struktur, Änderungen oft aufwendig.
* **ACID**-Eigenschaften (Atomicity, Consistency, Isolation, Durability).
* Nutzt **SQL-Sprache** für Abfragen.
* Gut für: komplexe Relationen, strukturierte Daten, Transaktionen.

**Beispiele:** PostgreSQL, MySQL, Oracle, MS SQL Server.

```sql
-- SQL Beispiel: Tabelle "users"
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100) UNIQUE
);

-- Abfrage
SELECT id, name FROM users WHERE email = 'test@mail.com';
```

---

### **NoSQL (Nicht-relationale Datenbanken)**

* Flexible **Schema-Struktur** (schemalos oder dynamisch).
* Speichert Daten in unterschiedlichen Formaten:

  * **Dokumente** (JSON-ähnlich, z. B. MongoDB)
  * **Key-Value Stores** (z. B. Redis)
  * **Wide-Column Stores** (z. B. Cassandra)
  * **Graph-Datenbanken** (z. B. Neo4j)
* **BASE**-Eigenschaften (Basically Available, Soft state, Eventually consistent).
* Skalierung: horizontal einfacher durch Sharding.
* Gut für: große, unstrukturierte Datenmengen, flexible Modelle, schnelle Entwicklung.

**Beispiel MongoDB (Dokument-Speicher):**

```js
// Collection "users" (ähnlich JSON)
{
  "_id": 1,
  "name": "Sergii",
  "email": "test@mail.com",
  "hobbies": ["Coding", "Fitness"]
}
```

---

### **Vergleich**

| Kriterium          | SQL (Relational)                      | NoSQL (Nicht-relational)            |
| ------------------ | ------------------------------------- | ----------------------------------- |
| **Datenmodell**    | Tabellen, feste Spalten               | Dokumente, Key-Value, Graph, Column |
| **Schema**         | Strikt, vorab definiert               | Flexibel, schemalos                 |
| **Transaktionen**  | Stark (ACID)                          | Schwächer, oft eventual consistency |
| **Skalierung**     | Vertikal (größere Hardware)           | Horizontal (mehr Server)            |
| **Abfragesprache** | SQL                                   | Unterschiedlich (Mongo Query, API)  |
| **Einsatzgebiete** | Finanzwesen, ERP, strukturierte Daten | Big Data, Realtime Apps, IoT        |

---

### **Zusammenfassung**

* **SQL**: strukturiert, ACID, relational, streng im Schema → ideal für komplexe Relationen & Konsistenz.
* **NoSQL**: flexibel, verteilt, BASE, skalierbar → ideal für unstrukturierte, große Datenmengen.

📖 Quellen:

* [PostgreSQL Dokumentation](https://www.postgresql.org/docs/)
* [MongoDB Dokumentation](https://www.mongodb.com/docs/)
* [MDN – NoSQL Einführung](https://developer.mozilla.org/en-US/docs/Glossary/NoSQL)

---

  **[⬆ Наверх](#top)**

152. ### <a name="152"></a> Wann verwendet man relationale DB vs. dokumentbasierte DB?

**Wann relationale Datenbanken (SQL) vs. dokumentbasierte Datenbanken (NoSQL, z. B. MongoDB)?**

---

### **Relationale Datenbanken (SQL, z. B. PostgreSQL, MySQL)**

**Verwenden, wenn …**

* **Klare, stabile Strukturen** → Datenmodell ändert sich selten.
* **Starke Konsistenz** benötigt wird (z. B. Banktransaktionen, Buchhaltung).
* **Komplexe Relationen** bestehen (JOINs zwischen mehreren Tabellen).
* **ACID-Eigenschaften** wichtig sind → garantierte Transaktionen.
* **Analytische Abfragen** über viele Tabellen nötig sind.

**Beispiele:**

* Bankensysteme
* ERP-Systeme
* E-Commerce (Bestellungen, Rechnungen)
* Buchhaltungssysteme

---

### **Dokumentbasierte Datenbanken (NoSQL, z. B. MongoDB, CouchDB)**

**Verwenden, wenn …**

* **Flexible Strukturen** benötigt werden (Datenmodell kann sich oft ändern).
* **Schnelle Entwicklung** → kein aufwendiges Schema-Design.
* **Horizontale Skalierung** wichtig ist (Sharding, Cloud-native Apps).
* Daten eher **objektartig** (JSON/Document) sind, wie bei REST-/GraphQL-APIs.
* Große Mengen **unstrukturierter oder semi-strukturierter Daten** gespeichert werden müssen.

**Beispiele:**

* Social Media (Posts, Kommentare, Likes)
* IoT-Anwendungen (heterogene Sensordaten)
* Echtzeit-Apps (Chats, Live-Tracking)
* Content-Management-Systeme

---

### **Vergleich – Praxisentscheid**

| Kriterium       | Relationale DB (SQL)                 | Dokumentbasierte DB (NoSQL)      |
| --------------- | ------------------------------------ | -------------------------------- |
| **Schema**      | Streng, stabil                       | Flexibel, variabel               |
| **Konsistenz**  | Stark (ACID)                         | Eventual Consistency (BASE)      |
| **Datenmengen** | Eher mittelgroß, normalisierte Daten | Sehr groß, unstrukturierte Daten |
| **Relationen**  | Komplex (JOINs, Normalisierung)      | Einfach oder durch Referenzen    |
| **Skalierung**  | Vertikal (größere Hardware)          | Horizontal (mehr Server)         |
| **Beispiele**   | Banken, Rechnungen, ERP              | Social Media, IoT, Realtime-Apps |

---

### **Zusammenfassung**

* **Relationale DB**: geeignet für strukturierte Daten mit festen Relationen, wo **Konsistenz und Integrität** höchste Priorität haben.
* **Dokumentbasierte DB**: geeignet für dynamische, wachsende Datenmodelle mit **Flexibilität und Skalierbarkeit** als Priorität.

📖 Quellen:

* [PostgreSQL Docs](https://www.postgresql.org/docs/)
* [MongoDB Docs](https://www.mongodb.com/docs/)
* [MDN – NoSQL Überblick](https://developer.mozilla.org/en-US/docs/Glossary/NoSQL)

---

  **[⬆ Наверх](#top)**

153. ### <a name="153"></a> Unterschiede zwischen PostgreSQL, MySQL und SQLite?

**Unterschiede zwischen PostgreSQL, MySQL und SQLite**

---

### **PostgreSQL**

* **Art**: Objekt-relationales DBMS (ORDBMS).
* **Stärken**:

  * Sehr mächtig bei **komplexen Abfragen** (CTE, Window Functions).
  * **ACID**-konform, stark bei **Transaktionen**.
  * Unterstützung für **JSON, Arrays, benutzerdefinierte Typen, Stored Procedures**.
  * Geeignet für **große, skalierbare Systeme**.
* **Einsatzgebiete**: Unternehmens-Apps, Data Warehousing, APIs, Systeme mit komplexer Logik.

```sql
-- Beispiel PostgreSQL: JSON-Spalte abfragen
SELECT data->>'email'
FROM users
WHERE data->>'role' = 'admin';
```

---

### **MySQL**

* **Art**: Relationales DBMS.
* **Stärken**:

  * Sehr verbreitet, besonders im **Web-Umfeld** (LAMP-Stack).
  * **Schnell** bei Lese-Operationen.
  * Breite Community und viele Tools (phpMyAdmin, Workbench).
* **Schwächen**:

  * Früher schwächer bei **ACID**- und Transaktions-Support (inzwischen mit InnoDB verbessert).
  * Weniger mächtig bei komplexen Queries im Vergleich zu PostgreSQL.
* **Einsatzgebiete**: Web-Anwendungen, CMS (WordPress, Drupal, Joomla), E-Commerce.

```sql
-- Beispiel MySQL: einfache Abfrage
SELECT name, email 
FROM users 
WHERE active = 1 
ORDER BY created_at DESC;
```

---

### **SQLite**

* **Art**: Leichtgewichtiges, dateibasiertes relationales DBMS.
* **Stärken**:

  * Keine separate Server-Installation → läuft direkt in einer Datei.
  * Sehr **portabel**, minimaler Overhead.
  * Ideal für **Embedded Systems, Prototyping, Mobile Apps** (z. B. iOS, Android).
* **Schwächen**:

  * Nicht für **hohe Parallelität oder riesige Datenmengen** gedacht.
  * Begrenzte Features im Vergleich zu PostgreSQL/MySQL.
* **Einsatzgebiete**: Mobile Apps, kleine Tools, lokale Anwendungen, Tests.

```sql
-- Beispiel SQLite: einfache Tabelle
CREATE TABLE users (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  name TEXT,
  email TEXT
);
```

---

### **Vergleichstabelle**

| Merkmal         | PostgreSQL                         | MySQL                                   | SQLite                              |
| --------------- | ---------------------------------- | --------------------------------------- | ----------------------------------- |
| **Architektur** | Server-basiert                     | Server-basiert                          | Datei-basiert (kein Server)         |
| **Leistung**    | Stark bei komplexen Abfragen       | Stark bei Lesezugriffen                 | Klein, effizient für Einzelzugriffe |
| **Skalierung**  | Sehr gut (Clustering, Replikation) | Gut (Replikation, Sharding möglich)     | Schwach, kein Cluster               |
| **ACID**        | Vollständig, robust                | Abhängig vom Engine (InnoDB vs. MyISAM) | Ja, aber eingeschränkt              |
| **Einsatz**     | Enterprise, APIs, Big Data         | Web-Anwendungen, CMS, E-Commerce        | Mobile, Desktop, Prototypen         |

---

### **Zusammenfassung**

* **PostgreSQL** → für **Enterprise, komplexe Queries, hohe Konsistenz**.
* **MySQL** → für **Web-Apps, weit verbreitet, gute Performance bei Reads**.
* **SQLite** → für **lokale Apps, Mobile, Prototyping**.

📖 Quellen:

* [PostgreSQL Docs](https://www.postgresql.org/docs/)
* [MySQL Docs](https://dev.mysql.com/doc/)
* [SQLite Docs](https://sqlite.org/docs.html)

---

  **[⬆ Наверх](#top)**

154. ### <a name="154"></a> Unterschiede zwischen MongoDB und PostgreSQL?

**Unterschiede zwischen MongoDB und PostgreSQL**

---

### **PostgreSQL** (Relational / SQL)

* **Art**: Objekt-relationales DBMS (ORDBMS).
* **Datenmodell**: Tabellen (Zeilen + Spalten), striktes Schema.
* **Abfrage**: SQL (Structured Query Language).
* **Konsistenz**: **ACID**-konform (starke Transaktionssicherheit).
* **Skalierung**: primär vertikal (größere Hardware), aber auch Replikation/Cluster möglich.
* **Stärken**:

  * Komplexe Abfragen, Joins, Aggregationen.
  * Datenintegrität und strikte Konsistenz.
  * Unterstützung für JSON/Arrays zusätzlich zu relationalem Modell.

**Beispiel:**

```sql
-- Tabelle in PostgreSQL
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100) UNIQUE
);

-- SQL-Abfrage
SELECT id, name FROM users WHERE email = 'test@mail.com';
```

---

### **MongoDB** (Dokumentbasiert / NoSQL)

* **Art**: Dokument-orientierte NoSQL-Datenbank.
* **Datenmodell**: JSON-ähnliche Dokumente (BSON), flexibles Schema.
* **Abfrage**: Mongo Query API (JS-ähnlich).
* **Konsistenz**: **BASE**-Prinzip (eventual consistency möglich).
* **Skalierung**: horizontal sehr stark (Sharding, verteilte Systeme).
* **Stärken**:

  * Flexible Datenstrukturen → Schema kann sich ändern.
  * Sehr gut für Big Data, Realtime-Apps, IoT.
  * Entwicklerfreundlich für API-nahe JSON-Formate.

**Beispiel:**

```js
// Dokument in MongoDB
{
  "_id": 1,
  "name": "Sergii",
  "email": "test@mail.com",
  "hobbies": ["Coding", "Fitness"]
}

// Abfrage in MongoDB
db.users.find({ email: "test@mail.com" }, { name: 1 });
```

---

### **Vergleich**

| Kriterium          | PostgreSQL (SQL)                             | MongoDB (NoSQL)                          |
| ------------------ | -------------------------------------------- | ---------------------------------------- |
| **Datenmodell**    | Tabellen, festes Schema                      | Dokumente (BSON), flexibles Schema       |
| **Abfragesprache** | SQL                                          | JSON-ähnliche Queries                    |
| **Konsistenz**     | ACID (stark)                                 | BASE (eventual consistency)              |
| **Skalierung**     | Vertikal, Replikation, Cluster               | Horizontal (Sharding nativ)              |
| **Relationen**     | Stark (Joins, Constraints)                   | Schwach (Referenzen, keine echten Joins) |
| **Einsatz**        | Banking, ERP, Analytics, strukturierte Daten | Social Media, IoT, Big Data, Realtime    |

---

### **Zusammenfassung**

* **PostgreSQL** → relational, ACID, stark für **strukturierte Daten und komplexe Relationen**.
* **MongoDB** → dokumentorientiert, flexibel, stark für **dynamische Datenmodelle und horizontale Skalierung**.

📖 Quellen:

* [PostgreSQL Docs](https://www.postgresql.org/docs/)
* [MongoDB Docs](https://www.mongodb.com/docs/)
* [MDN – NoSQL Überblick](https://developer.mozilla.org/en-US/docs/Glossary/NoSQL)

---

  **[⬆ Наверх](#top)**

155. ### <a name="155"></a> Wie baut man eine DB-Verbindung in Express auf?

**DB-Verbindung in Express aufbauen (Beispiel: PostgreSQL mit Sequelize ORM)**

---

### 1) Installation

```bash
npm install sequelize pg pg-hstore
```

---

### 2) Sequelize konfigurieren (`db.js`)

```js
// db.js
import { Sequelize } from "sequelize";

export const sequelize = new Sequelize("meinedb", "meinuser", "passwort", {
  host: "localhost",
  dialect: "postgres",
  logging: false, // optional: SQL-Logs ausschalten
});

export async function connectDB() {
  try {
    await sequelize.authenticate();
    console.log("✅ Verbindung erfolgreich aufgebaut");
  } catch (err) {
    console.error("❌ Verbindung fehlgeschlagen:", err);
    process.exit(1);
  }
}
```

---

### 3) Model definieren (`models/User.js`)

```js
// models/User.js
import { DataTypes } from "sequelize";
import { sequelize } from "../db.js";

export const User = sequelize.define("User", {
  name: {
    type: DataTypes.STRING,
    allowNull: false,
  },
  email: {
    type: DataTypes.STRING,
    unique: true,
  },
});
```

---

### 4) Express-App mit DB verbinden (`app.js`)

```js
// app.js
import express from "express";
import { connectDB, sequelize } from "./db.js";
import { User } from "./models/User.js";

const app = express();
app.use(express.json());

// Route mit DB-Zugriff
app.post("/users", async (req, res, next) => {
  try {
    const user = await User.create(req.body);
    res.status(201).json(user);
  } catch (err) {
    next(err);
  }
});

// Start + DB Sync
const PORT = 3000;
app.listen(PORT, async () => {
  await connectDB();
  await sequelize.sync(); // erstellt Tabellen falls nicht vorhanden
  console.log(`🚀 Server läuft auf Port ${PORT}`);
});
```

---

### **Best Practices**

* **Environment-Variablen** für DB-Zugang (über `.env` + `dotenv` einlesen).
* **Pooling** aktivieren (wird von Sequelize automatisch unterstützt).
* Fehler mit Middleware (`next(err)`) behandeln.
* In großen Projekten: DB-Setup, Modelle und Routen modular trennen.

---

### **Zusammenfassung**

* DB-Verbindung in Express → über ORM wie **Sequelize** oder direkt mit **pg**.
* Schritte: DB-Config → Models → Verbindung herstellen → Routen mit DB-Zugriff.
* Best Practices: `.env` nutzen, Fehlerbehandlung, Sync/Migrations sauber managen.

📖 Quellen:

* [Sequelize Docs](https://sequelize.org/docs/v7/getting-started/)
* [PostgreSQL Docs](https://www.postgresql.org/docs/)
* [Express Docs](https://expressjs.com/de/)

---

  **[⬆ Наверх](#top)**

156. ### <a name="156"></a> Was sind Migrations in SQL-Datenbanken?

**Migrations in SQL-Datenbanken**

---

### **Definition**

* **Migrationen** sind versionierte **Änderungen am Datenbankschema** (z. B. Tabellen, Spalten, Indizes).
* Sie ermöglichen, eine Datenbank **schrittweise und reproduzierbar** von einer Version zur nächsten zu entwickeln.
* Werden oft in Dateien gespeichert (z. B. `202309061200-create-users.js`).

---

### **Warum wichtig?**

* **Teamarbeit**: Alle Entwickler nutzen dieselben DB-Strukturen.
* **Versionierung**: Historie der Änderungen ist nachvollziehbar.
* **Reproduzierbarkeit**: DB-Struktur kann auf jeder Umgebung (Dev, Test, Prod) identisch aufgebaut werden.
* **Rollback**: Fehlerhafte Migrationen können zurückgesetzt werden.

---

### **Beispiel (Sequelize Migration)**

```js
// migration: create-users.js
export async function up(queryInterface, Sequelize) {
  await queryInterface.createTable("Users", {
    id: {
      type: Sequelize.INTEGER,
      autoIncrement: true,
      primaryKey: true,
    },
    name: {
      type: Sequelize.STRING,
      allowNull: false,
    },
    email: {
      type: Sequelize.STRING,
      unique: true,
    },
    createdAt: Sequelize.DATE,
    updatedAt: Sequelize.DATE,
  });
}

export async function down(queryInterface) {
  await queryInterface.dropTable("Users");
}
```

* **`up`**: beschreibt die Änderung (z. B. Tabelle erstellen).
* **`down`**: beschreibt, wie man die Änderung rückgängig macht (Rollback).

---

### **Beispiel mit SQL direkt**

```sql
-- Migration: neue Spalte hinzufügen
ALTER TABLE users ADD COLUMN birthday DATE;

-- Rollback
ALTER TABLE users DROP COLUMN birthday;
```

---

### **Zusammenfassung**

* Migrationen = **Schema-Änderungen** in versionierter Form.
* Ermöglichen **konsistente und nachvollziehbare DB-Entwicklung**.
* Enthalten immer mindestens zwei Teile: **up (apply)** und **down (rollback)**.

📖 Quellen:

* [PostgreSQL Docs – ALTER TABLE](https://www.postgresql.org/docs/current/sql-altertable.html)
* [Sequelize Docs – Migrations](https://sequelize.org/docs/v7/other-topics/migrations/)

---

  **[⬆ Наверх](#top)**

157. ### <a name="157"></a> Unterschied zwischen INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN?

**Unterschied zwischen INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN**

---

### **1) INNER JOIN**

* Gibt **nur Datensätze zurück, die in beiden Tabellen übereinstimmen**.
* Alles, was keine Übereinstimmung hat, wird ausgeschlossen.

```sql
SELECT u.name, o.id
FROM users u
INNER JOIN orders o ON u.id = o.user_id;
```

➡️ Nur Benutzer mit Bestellungen werden angezeigt.

---

### **2) LEFT JOIN**

* Gibt **alle Datensätze der linken Tabelle** zurück, auch wenn keine Übereinstimmung in der rechten Tabelle existiert.
* Fehlende Werte in der rechten Tabelle werden als `NULL` dargestellt.

```sql
SELECT u.name, o.id
FROM users u
LEFT JOIN orders o ON u.id = o.user_id;
```

➡️ Alle Benutzer, auch ohne Bestellung (dann `order_id = NULL`).

---

### **3) RIGHT JOIN**

* Gegenteil von LEFT JOIN.
* Gibt **alle Datensätze der rechten Tabelle** zurück, auch wenn keine Übereinstimmung in der linken Tabelle existiert.

```sql
SELECT u.name, o.id
FROM users u
RIGHT JOIN orders o ON u.id = o.user_id;
```

➡️ Alle Bestellungen, auch wenn kein Benutzer dazu existiert (`user = NULL`).

---

### **4) FULL JOIN (FULL OUTER JOIN)**

* Gibt **alle Datensätze beider Tabellen** zurück.
* Wenn keine Übereinstimmung: auf der fehlenden Seite `NULL`.

```sql
SELECT u.name, o.id
FROM users u
FULL JOIN orders o ON u.id = o.user_id;
```

➡️ Alle Benutzer + alle Bestellungen, inkl. nicht zugeordneter Werte.

---

### **Grafische Übersicht**

| JOIN-Typ  | Ergebnis (Mengenlehre)          |
| --------- | ------------------------------- |
| **INNER** | Schnittmenge                    |
| **LEFT**  | Alles von links + Schnittmenge  |
| **RIGHT** | Alles von rechts + Schnittmenge |
| **FULL**  | Vereinigung beider Mengen       |

---

### **Zusammenfassung**

* **INNER JOIN**: nur Übereinstimmungen.
* **LEFT JOIN**: alle von links, rechts nur wenn Match.
* **RIGHT JOIN**: alle von rechts, links nur wenn Match.
* **FULL JOIN**: alles aus beiden Tabellen, egal ob Match.

📖 Quellen:

* [PostgreSQL Docs – Joins](https://www.postgresql.org/docs/current/tutorial-join.html)
* [W3Schools SQL JOIN](https://www.w3schools.com/sql/sql_join.asp)

---

  **[⬆ Наверх](#top)**

158. ### <a name="158"></a> Was sind Normalformen in relationalen Datenbanken?

**Normalformen in relationalen Datenbanken**

Normalisierung = Prozess, Daten **so zu strukturieren**, dass **Redundanzen minimiert** und **Datenanomalien** (Insert-, Update-, Delete-Anomalien) vermieden werden.

---

### **1. Normalform (1NF)**

* Jede Zelle enthält **nur atomare Werte** (keine Listen oder mehrfachen Werte).
* Jede Zeile ist eindeutig identifizierbar (Primärschlüssel).

❌ Schlecht:

| Kunde | Telefonnummern |
| ----- | -------------- |
| Max   | 123, 456       |

✅ 1NF:

| Kunde | Telefonnummer |
| ----- | ------------- |
| Max   | 123           |
| Max   | 456           |

---

### **2. Normalform (2NF)**

* Erfüllt **1NF**.
* **Keine partiellen Abhängigkeiten**: Nicht-Schlüsselattribute dürfen nicht nur von einem Teil eines zusammengesetzten Schlüssels abhängen.

❌ Schlecht (zusammengesetzter Schlüssel `KursID + StudentID`):

| KursID | StudentID | KursName | StudentName |
| ------ | --------- | -------- | ----------- |

➡️ `KursName` hängt nur von `KursID` ab → Verletzung 2NF.

✅ Lösung: Tabelle `Kurse` und `Studenten` separat führen.

---

### **3. Normalform (3NF)**

* Erfüllt **2NF**.
* **Keine transitive Abhängigkeit**: Nicht-Schlüsselattribute dürfen nicht indirekt vom Primärschlüssel abhängen.

❌ Schlecht:

| StudentID | Name | Stadt | PLZ |
| --------- | ---- | ----- | --- |

➡️ `Stadt` hängt nicht direkt von `StudentID` ab, sondern von `PLZ`.

✅ Lösung: `PLZ` in eigene Tabelle mit Zuordnung zu `Stadt` auslagern.

---

### **Boyce-Codd Normalform (BCNF)**

* Strengere Form der 3NF.
* Jede funktionale Abhängigkeit muss vom **Superkey** ausgehen.
* Verhindert Spezialfälle, wo 3NF nicht ausreicht.

---

### **Zusammenfassung**

* **1NF**: nur atomare Werte.
* **2NF**: keine partiellen Abhängigkeiten.
* **3NF**: keine transitiven Abhängigkeiten.
* **BCNF**: jede Abhängigkeit nur von einem Superkey.

📖 Quellen:

* [PostgreSQL Docs – Database Design](https://www.postgresql.org/docs/current/ddl.html)
* [MDN – Relationale Datenbanken](https://developer.mozilla.org/en-US/docs/Learn/Server-side/SQL/Database_design)

---

  **[⬆ Наверх](#top)**

159. ### <a name="159"></a> Unterschied zwischen 1NF, 2NF, 3NF?

**Unterschied zwischen 1NF, 2NF und 3NF**

---

### **1. Normalform (1NF)**

* Alle Werte sind **atomar** (keine Listen oder mehrfachen Werte in einer Zelle).
* Jede Zeile ist eindeutig durch einen Primärschlüssel identifizierbar.

❌ Schlecht:

| Kunde | Telefonnummern |
| ----- | -------------- |
| Max   | 123, 456       |

✅ 1NF:

| Kunde | Telefonnummer |
| ----- | ------------- |
| Max   | 123           |
| Max   | 456           |

---

### **2. Normalform (2NF)**

* Erfüllt **1NF**.
* **Keine partiellen Abhängigkeiten**: Attribute müssen vom gesamten Primärschlüssel abhängen, nicht nur von einem Teil (gilt nur bei zusammengesetzten Schlüsseln).

❌ Schlecht (PK = KursID + StudentID):

| KursID | StudentID | KursName | StudentName |
| ------ | --------- | -------- | ----------- |
| 1      | 11        | Mathe    | Max         |

➡️ `KursName` hängt nur von `KursID` ab → Verstoß gegen 2NF.

✅ Lösung: `Kurse` und `Studenten` in eigene Tabellen.

---

### **3. Normalform (3NF)**

* Erfüllt **2NF**.
* **Keine transitiven Abhängigkeiten**: Nicht-Schlüsselattribute dürfen nicht von anderen Nicht-Schlüsselattributen abhängen.

❌ Schlecht:

| StudentID | Name | PLZ | Stadt |
| --------- | ---- | --- | ----- |

➡️ `Stadt` hängt von `PLZ` ab, nicht direkt vom `StudentID`.

✅ Lösung: eigene Tabelle `PLZ → Stadt`.

---

### **Kurz-Vergleich**

| Normalform | Regel                                  | Beispiel-Problem                       |
| ---------- | -------------------------------------- | -------------------------------------- |
| **1NF**    | Nur atomare Werte, eindeutige Zeilen   | Mehrere Telefonnummern in einer Spalte |
| **2NF**    | Keine partiellen Abhängigkeiten vom PK | KursName hängt nur von KursID ab       |
| **3NF**    | Keine transitiven Abhängigkeiten       | Stadt hängt von PLZ statt PK ab        |

---

### **Zusammenfassung**

* **1NF**: atomare Werte.
* **2NF**: keine Abhängigkeit von Teil des Schlüssels.
* **3NF**: keine Abhängigkeit von Nicht-Schlüssel-Attributen.

📖 Quellen:

* [PostgreSQL Docs – Database Design](https://www.postgresql.org/docs/current/ddl.html)
* [MDN – Relationale Datenbanken](https://developer.mozilla.org/en-US/docs/Learn/Server-side/SQL/Database_design)

---

  **[⬆ Наверх](#top)**

160. ### <a name="160"></a> Wie funktioniert Indexierung in SQL-Datenbanken?

**Indexierung in SQL-Datenbanken**

---

### **Definition**

* Ein **Index** ist eine spezielle Datenstruktur, die den Zugriff auf Tabellenzeilen beschleunigt.
* Funktioniert ähnlich wie ein Inhaltsverzeichnis im Buch → statt jede Zeile zu durchsuchen, wird ein „Zeiger“ genutzt.
* Häufig implementiert als **B-Tree** (Balanced Tree), teilweise auch **Hash-Index**.

---

### **Funktionsweise**

1. Ohne Index → Datenbank muss oft einen **Full Table Scan** machen.
2. Mit Index → Datenbank kann gezielt an die richtigen Zeilen springen.
3. Index speichert Schlüsselwerte + Zeiger auf Zeilen im Speicher.

---

### **Beispiel (PostgreSQL / SQL Standard)**

```sql
-- Index anlegen auf Spalte email
CREATE INDEX idx_users_email ON users(email);

-- Abfrage wird jetzt schneller:
SELECT * FROM users WHERE email = 'test@mail.com';
```

* Ohne Index → gesamte Tabelle wird durchsucht.
* Mit Index → Suche über B-Tree in O(log n).

---

### **Arten von Indizes**

* **Primärschlüssel-Index**: automatisch bei PRIMARY KEY.
* **Unique Index**: garantiert Eindeutigkeit.
* **B-Tree Index**: Standard, effizient für Bereichsabfragen (`<`, `>`, `BETWEEN`).
* **Hash Index**: effizient für exakte Vergleiche (`=`).
* **GIN / GiST Index** (PostgreSQL): für Volltextsuche, JSON, Arrays.

---

### **Nachteile von Indizes**

* Mehr Speicherbedarf.
* Langsamere **INSERT/UPDATE/DELETE**, weil Indizes aktualisiert werden müssen.
* Zu viele Indizes → Performanceverlust statt -gewinn.

---

### **Best Practices**

* Indizes auf Spalten, die **häufig in WHERE, JOIN, ORDER BY** verwendet werden.
* Nicht jede Spalte indexieren → Balance zwischen **Lesegeschwindigkeit und Schreibaufwand**.
* **Composite Indexes** für mehrere Spalten (z. B. `(lastname, firstname)`).

---

### **Zusammenfassung**

* Indizes = **Strukturen zur Beschleunigung von Abfragen**.
* Bäume/Hashes statt Full Table Scan.
* Trade-off: schnellere **Reads**, langsamere **Writes** + mehr Speicher.

📖 Quellen:

* [PostgreSQL Docs – Indexes](https://www.postgresql.org/docs/current/indexes.html)
* [MySQL Docs – Indexes](https://dev.mysql.com/doc/refman/8.0/en/optimization-indexes.html)

---

  **[⬆ Наверх](#top)**

161. ### <a name="161"></a> Was ist ein Primärschlüssel und ein Fremdschlüssel?

**Primärschlüssel und Fremdschlüssel in relationalen Datenbanken**

---

### **Primärschlüssel (Primary Key)**

* Eindeutiger Identifikator für jede Zeile in einer Tabelle.
* Darf **nicht NULL** sein.
* Es kann pro Tabelle nur **einen Primärschlüssel** geben.
* Oft automatisch mit Index versehen → schnelle Suche.

**Beispiel:**

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100) NOT NULL,
  email VARCHAR(100) UNIQUE NOT NULL
);
```

➡️ `id` ist der Primärschlüssel, eindeutig für jeden Benutzer.

---

### **Fremdschlüssel (Foreign Key)**

* Spalte, die auf den **Primärschlüssel einer anderen Tabelle** verweist.
* Stellt eine **Beziehung** zwischen zwei Tabellen her.
* Gewährleistet **Referenzielle Integrität** (keine „verwaisten“ Datensätze).

**Beispiel:**

```sql
CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  user_id INT REFERENCES users(id), -- Fremdschlüssel
  product VARCHAR(100) NOT NULL
);
```

➡️ `user_id` verweist auf `users.id`.
➡️ Jede Bestellung gehört zu einem existierenden Benutzer.

---

### **Zusammenarbeit**

* **Primary Key** = eindeutige Identität in der „Master“-Tabelle.
* **Foreign Key** = stellt Beziehung zur „Master“-Tabelle her.

**JOIN Beispiel:**

```sql
SELECT u.name, o.product
FROM users u
INNER JOIN orders o ON u.id = o.user_id;
```

➡️ Zeigt Benutzer mit ihren Bestellungen.

---

### **Zusammenfassung**

* **Primärschlüssel**: eindeutige Identifikation einer Zeile.
* **Fremdschlüssel**: Verweis auf Primärschlüssel einer anderen Tabelle, sorgt für **Referenzielle Integrität**.

📖 Quellen:

* [PostgreSQL Docs – Constraints](https://www.postgresql.org/docs/current/ddl-constraints.html)
* [MySQL Docs – Foreign Keys](https://dev.mysql.com/doc/refman/8.0/en/create-table-foreign-keys.html)

---

  **[⬆ Наверх](#top)**

162. ### <a name="162"></a> Unterschied zwischen UNIQUE und PRIMARY KEY?

**Unterschied zwischen `UNIQUE` und `PRIMARY KEY` in SQL**

---

### **PRIMARY KEY**

* Eindeutiger Identifikator einer Zeile.
* Eigenschaften:

  * Jede Tabelle darf **nur einen PRIMARY KEY** haben.
  * Impliziert automatisch **UNIQUE** und **NOT NULL**.
  * Wird oft als **Clustered Index** (physische Sortierung) umgesetzt.
* Typisch: Spalte `id` mit AUTO INCREMENT / SERIAL.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(100) UNIQUE
);
```

---

### **UNIQUE**

* Gewährleistet, dass **alle Werte in einer Spalte (oder Kombination von Spalten) einzigartig** sind.
* Unterschiede:

  * **Mehrere UNIQUE Constraints** pro Tabelle erlaubt.
  * Erlaubt **NULL-Werte** (Ausnahme: manche DBs behandeln mehrere NULLs als erlaubt, z. B. PostgreSQL).
  * Nicht automatisch Primärschlüssel.

```sql
CREATE TABLE employees (
  emp_id SERIAL PRIMARY KEY,
  email VARCHAR(100) UNIQUE,
  phone VARCHAR(20) UNIQUE
);
```

➡️ `emp_id` identifiziert eindeutig den Datensatz.
➡️ `email` und `phone` dürfen nicht doppelt vorkommen, aber können NULL sein.

---

### **Vergleich**

| Merkmal            | PRIMARY KEY                       | UNIQUE                            |
| ------------------ | --------------------------------- | --------------------------------- |
| Eindeutigkeit      | Ja                                | Ja                                |
| NULL erlaubt?      | Nein                              | Ja (je nach DB, z. B. PostgreSQL) |
| Anzahl pro Tabelle | Nur **1**                         | Mehrere möglich                   |
| Zweck              | Identifiziert Datensatz eindeutig | Verhindert doppelte Werte         |

---

### **Zusammenfassung**

* **PRIMARY KEY** = eindeutiger Hauptschlüssel, genau 1 pro Tabelle, **keine NULLs**.
* **UNIQUE** = zusätzliche Eindeutigkeitsbedingung, mehrere pro Tabelle möglich, **NULL erlaubt**.

📖 Quellen:

* [PostgreSQL Docs – Constraints](https://www.postgresql.org/docs/current/ddl-constraints.html)
* [MySQL Docs – Unique Constraints](https://dev.mysql.com/doc/refman/8.0/en/create-table.html)

---

  **[⬆ Наверх](#top)**

163. ### <a name="163"></a> Unterschied zwischen HAVING und WHERE in SQL?

**Unterschied zwischen `WHERE` und `HAVING` in SQL**

---

### **WHERE**

* Filtert **Zeilen**, bevor eine Aggregation (`GROUP BY`) ausgeführt wird.
* Kann **keine Aggregatfunktionen** (`COUNT, SUM, AVG …`) enthalten.

```sql
-- Beispiel: Nur aktive Benutzer auswählen
SELECT name, city
FROM users
WHERE active = true;
```

---

### **HAVING**

* Filtert **Gruppen** nach einer Aggregation (`GROUP BY`).
* Kann **Aggregatfunktionen** enthalten.

```sql
-- Beispiel: Nur Städte mit mehr als 5 Benutzern
SELECT city, COUNT(*) AS user_count
FROM users
GROUP BY city
HAVING COUNT(*) > 5;
```

---

### **Vergleich mit GROUP BY**

```sql
-- Kombination von WHERE und HAVING
SELECT city, COUNT(*) AS user_count
FROM users
WHERE active = true               -- Zeilen-Filter
GROUP BY city
HAVING COUNT(*) > 5;              -- Gruppen-Filter
```

➡️ Ablauf:

1. `WHERE` filtert Zeilen.
2. `GROUP BY` fasst zusammen.
3. `HAVING` filtert die Gruppen.

---

### **Zusammenfassung**

* **WHERE**: Zeilenfilter → vor der Aggregation, keine Aggregatfunktionen.
* **HAVING**: Gruppenfilter → nach der Aggregation, mit Aggregatfunktionen.

📖 Quellen:

* [PostgreSQL Docs – SELECT](https://www.postgresql.org/docs/current/sql-select.html)
* [MySQL Docs – GROUP BY & HAVING](https://dev.mysql.com/doc/refman/8.0/en/group-by-handling.html)

---

  **[⬆ Наверх](#top)**

164. ### <a name="164"></a> Was sind Aggregate-Funktionen in SQL (z. B. COUNT, SUM, AVG)?

**Aggregate-Funktionen in SQL**

---

### **Definition**

* **Aggregatfunktionen** berechnen aus **mehreren Zeilen** einer Tabelle **einen einzelnen Wert**.
* Werden häufig mit **`GROUP BY`** kombiniert, können aber auch ohne Gruppierung auf die gesamte Tabelle angewendet werden.

---

### **Wichtige Aggregate-Funktionen**

1. **COUNT()** – Anzahl der Zeilen

```sql
SELECT COUNT(*) AS total_users
FROM users;
```

➡️ Zählt alle Zeilen.

2. **SUM()** – Summe von Werten

```sql
SELECT SUM(amount) AS total_sales
FROM orders;
```

➡️ Summiert die Werte der Spalte `amount`.

3. **AVG()** – Durchschnitt

```sql
SELECT AVG(salary) AS avg_salary
FROM employees;
```

➡️ Durchschnitt aller Gehälter.

4. **MIN() / MAX()** – Kleinster und größter Wert

```sql
SELECT MIN(price) AS lowest_price, MAX(price) AS highest_price
FROM products;
```

➡️ Zeigt Minimal- und Maximalwert.

---

### **Mit GROUP BY**

```sql
SELECT city, COUNT(*) AS user_count, AVG(age) AS avg_age
FROM users
GROUP BY city
HAVING COUNT(*) > 10;
```

➡️ Aggregiert Benutzer pro Stadt, filtert Städte mit mehr als 10 Benutzern.

---

### **Eigenschaften**

* Aggregatfunktionen ignorieren standardmäßig **NULL-Werte** (außer `COUNT(*)`).
* Können nicht direkt in **WHERE** verwendet werden → stattdessen `HAVING`.

---

### **Zusammenfassung**

* **Aggregate-Funktionen** fassen Daten zusammen (z. B. Anzahl, Summe, Durchschnitt).
* Typische Funktionen: **COUNT, SUM, AVG, MIN, MAX**.
* In Kombination mit **`GROUP BY`** → Analyse pro Gruppe möglich.

📖 Quellen:

* [PostgreSQL Docs – Aggregate Functions](https://www.postgresql.org/docs/current/functions-aggregate.html)
* [MySQL Docs – Aggregate Functions](https://dev.mysql.com/doc/refman/8.0/en/group-by-functions.html)

---

  **[⬆ Наверх](#top)**

165. ### <a name="165"></a> Wie baut man Many-to-Many Beziehungen in SQL?

**Many-to-Many (n\:m) Beziehungen in SQL**

---

### **Definition**

* Eine **n\:m-Beziehung** tritt auf, wenn mehrere Zeilen einer Tabelle mit mehreren Zeilen einer anderen Tabelle verknüpft werden können.
* Beispiel:

  * Ein **Student** besucht mehrere **Kurse**.
  * Ein **Kurs** wird von mehreren **Studenten** besucht.
* Lösung: eine **Zwischentabelle (Join Table / Mapping Table)** mit **Fremdschlüsseln** zu beiden Tabellen.

---

### **Beispiel**

#### 1) Tabellen erstellen

```sql
-- Studenten-Tabelle
CREATE TABLE students (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100) NOT NULL
);

-- Kurse-Tabelle
CREATE TABLE courses (
  id SERIAL PRIMARY KEY,
  title VARCHAR(100) NOT NULL
);
```

#### 2) Zwischentabelle für n\:m-Beziehung

```sql
CREATE TABLE student_courses (
  student_id INT REFERENCES students(id) ON DELETE CASCADE,
  course_id INT REFERENCES courses(id) ON DELETE CASCADE,
  PRIMARY KEY (student_id, course_id) -- zusammengesetzter PK
);
```

---

### **Einfügen von Daten**

```sql
-- Studenten
INSERT INTO students (name) VALUES ('Anna'), ('Tom');

-- Kurse
INSERT INTO courses (title) VALUES ('Mathe'), ('Informatik');

-- Beziehungen
INSERT INTO student_courses (student_id, course_id) VALUES 
(1, 1), -- Anna → Mathe
(1, 2), -- Anna → Informatik
(2, 2); -- Tom → Informatik
```

---

### **Abfragen**

* Alle Kurse eines Studenten:

```sql
SELECT s.name, c.title
FROM students s
JOIN student_courses sc ON s.id = sc.student_id
JOIN courses c ON c.id = sc.course_id
WHERE s.name = 'Anna';
```

➡️ Ergebnis: Anna → Mathe, Informatik

* Alle Studenten in einem Kurs:

```sql
SELECT c.title, s.name
FROM courses c
JOIN student_courses sc ON c.id = sc.course_id
JOIN students s ON s.id = sc.student_id
WHERE c.title = 'Informatik';
```

➡️ Ergebnis: Informatik → Anna, Tom

---

### **Zusammenfassung**

* **n\:m-Beziehungen** werden in SQL mit einer **Zwischentabelle** modelliert.
* Diese enthält die **Primärschlüssel beider Tabellen als Fremdschlüssel**.
* Abfragen erfolgen mit **JOINs** über die Zwischentabelle.

📖 Quellen:

* [PostgreSQL Docs – Constraints](https://www.postgresql.org/docs/current/ddl-constraints.html)
* [MDN – Relationale DB-Designs](https://developer.mozilla.org/en-US/docs/Learn/Server-side/SQL/Database_design)

---

  **[⬆ Наверх](#top)**

166. ### <a name="166"></a> Wie arbeitet man mit Transaktionen in PostgreSQL?

**Arbeiten mit Transaktionen in PostgreSQL**

---

### **Definition**

* Eine **Transaktion** ist eine Folge von SQL-Befehlen, die als **eine logische Einheit** ausgeführt wird.
* Sie garantiert **ACID-Eigenschaften**:

  * **Atomicity**: Alles oder nichts.
  * **Consistency**: DB bleibt konsistent.
  * **Isolation**: Parallele Transaktionen stören sich nicht.
  * **Durability**: Nach COMMIT dauerhaft gespeichert.

---

### **Grundbefehle in PostgreSQL**

```sql
BEGIN;                    -- Start einer Transaktion
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;                   -- Änderungen bestätigen
```

* Wenn ein Fehler auftritt:

```sql
ROLLBACK;                 -- Alle Änderungen rückgängig machen
```

---

### **Beispiel: Geldüberweisung**

```sql
BEGIN;

UPDATE accounts SET balance = balance - 500 WHERE id = 1;
-- Fehler prüfen, z. B. falls Konto nicht existiert
UPDATE accounts SET balance = balance + 500 WHERE id = 2;

COMMIT;
```

➡️ Wenn ein Schritt fehlschlägt → `ROLLBACK`.

---

### **Transaktionen mit Isolation Level**

```sql
BEGIN ISOLATION LEVEL SERIALIZABLE;

UPDATE products SET stock = stock - 1 WHERE id = 100;
INSERT INTO orders (product_id, quantity) VALUES (100, 1);

COMMIT;
```

➡️ Isolation Level bestimmt, wie stark parallele Transaktionen voneinander abgeschirmt werden.

---

### **Mit Node.js (pg Paket)**

```js
import pkg from "pg";
const { Pool } = pkg;

const pool = new Pool({ connectionString: "postgres://user:pass@localhost/db" });

async function transfer(fromId, toId, amount) {
  const client = await pool.connect();
  try {
    await client.query("BEGIN");
    await client.query("UPDATE accounts SET balance = balance - $1 WHERE id = $2", [amount, fromId]);
    await client.query("UPDATE accounts SET balance = balance + $1 WHERE id = $2", [amount, toId]);
    await client.query("COMMIT");
    console.log("✅ Transaktion erfolgreich");
  } catch (err) {
    await client.query("ROLLBACK");
    console.error("❌ Fehler:", err.message);
  } finally {
    client.release();
  }
}
```

---

### **Zusammenfassung**

* Transaktionen = logische Einheit von SQL-Operationen.
* Steuerung über `BEGIN`, `COMMIT`, `ROLLBACK`.
* Garantieren **ACID**.
* In Node.js über `pg` oder ORM (z. B. Sequelize `transaction`).

📖 Quellen:

* [PostgreSQL Docs – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)
* [Node-postgres Transactions](https://node-postgres.com/features/transactions)

---

  **[⬆ Наверх](#top)**

167. ### <a name="167"></a> Was ist ACID in Datenbanken?

**ACID in Datenbanken**

ACID ist ein Akronym für die vier zentralen Eigenschaften, die **Transaktionen in relationalen Datenbanken** sicherstellen:

---

### **1. Atomicity (Atomarität)**

* Eine Transaktion wird **entweder vollständig oder gar nicht** ausgeführt.
* Fehler → alle Änderungen werden mit **ROLLBACK** rückgängig gemacht.

```sql
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;  -- entweder beide Updates oder keines
```

---

### **2. Consistency (Konsistenz)**

* Nach einer Transaktion muss die Datenbank **in einem gültigen Zustand** bleiben.
* Integritätsregeln, Constraints (z. B. FOREIGN KEY, CHECK) dürfen nicht verletzt werden.

```sql
-- Konsistenzregel: balance >= 0
CHECK (balance >= 0);
```

---

### **3. Isolation (Isolation)**

* Parallele Transaktionen dürfen sich nicht gegenseitig beeinflussen.
* PostgreSQL unterstützt verschiedene **Isolation Levels**:

  * READ UNCOMMITTED
  * READ COMMITTED (Standard)
  * REPEATABLE READ
  * SERIALIZABLE

---

### **4. Durability (Dauerhaftigkeit)**

* Nach **COMMIT** bleiben Änderungen dauerhaft gespeichert – auch bei Systemabsturz.
* Wird durch Write-Ahead Logging (WAL) in PostgreSQL gewährleistet.

---

### **Zusammenfassung**

* **A (Atomicity)** → Alles oder nichts.
* **C (Consistency)** → Daten bleiben gültig.
* **I (Isolation)** → Parallele Transaktionen stören sich nicht.
* **D (Durability)** → Dauerhafte Speicherung nach COMMIT.

📖 Quellen:

* [PostgreSQL Docs – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)
* [MDN – Database Transactions](https://developer.mozilla.org/en-US/docs/Glossary/ACID)

---

  **[⬆ Наверх](#top)**

168. ### <a name="168"></a> Unterschied zwischen ACID und BASE Prinzipien?

**Unterschied zwischen ACID und BASE Prinzipien**

---

### **ACID (klassische relationale DBs, z. B. PostgreSQL, MySQL)**

* **Atomicity** → Transaktion: alles oder nichts.
* **Consistency** → DB bleibt immer in gültigem Zustand (Constraints, Regeln).
* **Isolation** → parallele Transaktionen stören sich nicht.
* **Durability** → Änderungen nach `COMMIT` dauerhaft gespeichert.

➡️ Ziel: **maximale Datenintegrität**, wichtig für Banken, ERP, Buchhaltung.

---

### **BASE (häufig in NoSQL-Systemen, z. B. MongoDB, Cassandra)**

* **Basically Available** → hohe Verfügbarkeit, System reagiert immer, auch wenn nicht alle Daten aktuell sind.
* **Soft state** → Zustand kann sich ändern, auch ohne Eingriff (z. B. durch Replikation).
* **Eventually consistent** → Daten werden irgendwann konsistent, aber nicht sofort.

➡️ Ziel: **Skalierbarkeit und Performance**, wichtig für Big Data, Social Media, Realtime-Apps.

---

### **Vergleich**

| Prinzip           | ACID (SQL, Relationale DBs) | BASE (NoSQL, Verteilte DBs)            |
| ----------------- | --------------------------- | -------------------------------------- |
| **Fokus**         | Konsistenz & Integrität     | Verfügbarkeit & Skalierbarkeit         |
| **Konsistenz**    | Strikt (sofort)             | Eventual Consistency (zeitverzögert)   |
| **Transaktionen** | Stark (atomar)              | Schwach oder nicht klassisch vorhanden |
| **Nutzung**       | Banken, Buchhaltung, ERP    | Social Media, IoT, E-Commerce (groß)   |
| **Beispiel DBs**  | PostgreSQL, MySQL, Oracle   | MongoDB, Cassandra, DynamoDB           |

---

### **Zusammenfassung**

* **ACID**: starke Transaktionen, sofortige Konsistenz → gut für Systeme mit strikter Datenintegrität.
* **BASE**: weiche Konsistenz, hohe Verfügbarkeit, horizontale Skalierung → gut für große, verteilte Systeme.

📖 Quellen:

* [PostgreSQL Docs – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)
* [MongoDB – Consistency and Availability](https://www.mongodb.com/docs/manual/core/replica-set-consistency/)
* [MDN – ACID vs. BASE](https://developer.mozilla.org/en-US/docs/Glossary/ACID)

---

  **[⬆ Наверх](#top)**

169. ### <a name="169"></a> Was ist ein Deadlock und wie vermeidet man ihn?

**Deadlock in Datenbanken**

---

### **Definition**

Ein **Deadlock** tritt auf, wenn **zwei oder mehr Transaktionen** sich gegenseitig blockieren:

* Transaktion A hält Sperre 1 und wartet auf Sperre 2.
* Transaktion B hält Sperre 2 und wartet auf Sperre 1.
  ➡️ Beide warten endlos → Stillstand.

---

### **Beispiel (PostgreSQL)**

```sql
-- Session 1
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
-- wartet später auf id = 2

-- Session 2
BEGIN;
UPDATE accounts SET balance = balance - 50 WHERE id = 2;
-- wartet später auf id = 1

-- Wenn beide Sessions jetzt auf die jeweils andere Zeile zugreifen:
-- Deadlock!
```

PostgreSQL erkennt Deadlocks automatisch → eine Transaktion wird abgebrochen mit
`ERROR: deadlock detected`.

---

### **Ursachen**

* Unterschiedliche Reihenfolge von Sperren (Lock Ordering).
* Lange Transaktionen mit vielen Locks.
* Kombination von Lese- und Schreibsperren.

---

### **Vermeidung von Deadlocks**

1. **Konsistente Sperr-Reihenfolge**

   * Immer in derselben Reihenfolge auf Tabellen/Zeilen zugreifen.

```sql
-- Immer erst Konto mit kleinerer ID updaten, dann größere
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
```

---

2. **Transaktionen kurz halten**

   * Möglichst wenige Operationen pro Transaktion.
   * Keine unnötigen Benutzerinteraktionen während einer offenen Transaktion.

---

3. **Geeignete Isolation Levels wählen**

   * Weniger restriktive Levels (`READ COMMITTED`) können Deadlocks reduzieren.

---

4. **Timeouts setzen**

   * In PostgreSQL:

   ```sql
   SET lock_timeout = '5s';
   ```

   ➝ Verhindert unendliches Warten.

---

5. **Retry-Logik im Code**

   * Falls DB eine Transaktion wegen Deadlock abbricht → erneut versuchen.

```js
// Beispiel mit node-postgres
async function safeTransaction(client, queries) {
  for (let attempt = 1; attempt <= 3; attempt++) {
    try {
      await client.query("BEGIN");
      await queries();
      await client.query("COMMIT");
      return;
    } catch (err) {
      await client.query("ROLLBACK");
      if (err.code === "40P01") { // Deadlock detected
        console.log(`Retry wegen Deadlock, Versuch ${attempt}`);
      } else {
        throw err;
      }
    }
  }
}
```

---

### **Zusammenfassung**

* **Deadlock** = zwei Transaktionen blockieren sich gegenseitig.
* PostgreSQL bricht automatisch eine Transaktion ab.
* **Vermeidung**: konsistente Sperr-Reihenfolge, kurze Transaktionen, Timeouts, Retry-Logik.

📖 Quellen:

* [PostgreSQL Docs – Explicit Locking](https://www.postgresql.org/docs/current/explicit-locking.html)
* [PostgreSQL Docs – Deadlocks](https://www.postgresql.org/docs/current/explicit-locking.html#LOCKING-DEADLOCKS)

---

  **[⬆ Наверх](#top)**

170. ### <a name="170"></a> Was ist Sharding und Partitionierung in Datenbanken?

**Sharding und Partitionierung in Datenbanken**

---

### **Partitionierung**

* **Definition**: Aufteilung **einer Tabelle** innerhalb **einer einzigen Datenbank** in mehrere Teile (Partitionen).
* Partitionen basieren auf **Spaltenwerten** (z. B. Datum, Bereich, Hash).
* Ziel: **Performance** und **Verwaltbarkeit** verbessern.

**Beispiel PostgreSQL (Range Partitionierung):**

```sql
CREATE TABLE orders (
  id SERIAL,
  order_date DATE NOT NULL,
  amount NUMERIC
) PARTITION BY RANGE (order_date);

CREATE TABLE orders_2023 PARTITION OF orders
  FOR VALUES FROM ('2023-01-01') TO ('2024-01-01');

CREATE TABLE orders_2024 PARTITION OF orders
  FOR VALUES FROM ('2024-01-01') TO ('2025-01-01');
```

➡️ Abfragen auf `orders` werden automatisch auf die passende Partition weitergeleitet.

---

### **Sharding**

* **Definition**: Aufteilung von Daten **über mehrere physische Server oder Datenbanken**.
* Jeder „Shard“ enthält einen Teil der Daten, z. B. nach **Benutzer-ID oder Region**.
* Ziel: **horizontale Skalierung** (mehr Server statt stärkerer Server).

**Beispiel MongoDB Sharding (vereinfachte Logik):**

* Benutzer mit IDs 1–1.000.000 → Shard A
* Benutzer mit IDs 1.000.001–2.000.000 → Shard B

---

### **Vergleich**

| Merkmal           | Partitionierung                    | Sharding                                        |
| ----------------- | ---------------------------------- | ----------------------------------------------- |
| **Ebene**         | Innerhalb einer Tabelle / einer DB | Zwischen mehreren DB-Instanzen/Servern          |
| **Ziel**          | Performance, Wartbarkeit           | Skalierbarkeit über mehrere Maschinen           |
| **Transaktionen** | Bleiben lokal in derselben DB      | Können komplexer sein (verteilte Transaktionen) |
| **Beispiel DBs**  | PostgreSQL Partitionierung         | MongoDB, Cassandra, CockroachDB                 |

---

### **Zusammenfassung**

* **Partitionierung** = Tabelle in Teile zerlegen → innerhalb einer DB.
* **Sharding** = Daten auf mehrere DB-Server verteilen → horizontale Skalierung.
* Beide Konzepte helfen bei **großen Datenmengen**, unterscheiden sich aber in **Scope und Ziel**.

📖 Quellen:

* [PostgreSQL Docs – Partitioning](https://www.postgresql.org/docs/current/ddl-partitioning.html)
* [MongoDB Docs – Sharding](https://www.mongodb.com/docs/manual/sharding/)

---

  **[⬆ Наверх](#top)**

171. ### <a name="171"></a> Unterschied zwischen vertikaler und horizontaler Skalierung?

**Unterschied zwischen vertikaler und horizontaler Skalierung**

---

### **Vertikale Skalierung (Scaling Up)**

* Mehr **Ressourcen** zu einem bestehenden Server hinzufügen:

  * mehr CPU-Kerne
  * mehr RAM
  * schnellere Festplatten
* Einfach umzusetzen, keine Änderungen in der Software nötig.
* **Grenzen**: Hardware hat Obergrenzen, oft teuer.
* **Beispiel**: PostgreSQL auf einem Server von 8 GB → 64 GB RAM aufrüsten.

---

### **Horizontale Skalierung (Scaling Out)**

* Mehrere **Server/Instanzen** hinzufügen und die Last verteilen.
* Erfordert Anpassungen in **Architektur** (Load Balancer, Replikation, Sharding).
* Potenziell unbegrenzt skalierbar.
* Komplexer (Datenkonsistenz, Netzwerk-Latenzen, Synchronisierung).
* **Beispiel**: PostgreSQL-Replikation → mehrere Read-Replicas oder MongoDB-Sharding.

---

### **Vergleich**

| Merkmal         | Vertikal (Up)               | Horizontal (Out)                            |
| --------------- | --------------------------- | ------------------------------------------- |
| **Ansatz**      | Mehr Leistung pro Server    | Mehr Server hinzufügen                      |
| **Grenzen**     | Hardware-Limit erreicht     | Nahezu unbegrenzt (Cloud, Cluster)          |
| **Kosten**      | Teure High-End-Maschinen    | Billigere Standard-Server                   |
| **Komplexität** | Einfach                     | Hoch (Replikation, Sharding, Load Balancer) |
| **Einsatz**     | Kleine bis mittlere Systeme | Große Systeme, Web-Apps, Big Data           |

---

### **Zusammenfassung**

* **Vertikal** = stärkerer Server, schnell & einfach, aber limitiert.
* **Horizontal** = mehr Server, skalierbar, aber komplexer.

📖 Quellen:

* [PostgreSQL Docs – Scalability](https://www.postgresql.org/docs/current/runtime-config-resource.html)
* [MongoDB Docs – Horizontal Scaling (Sharding)](https://www.mongodb.com/docs/manual/sharding/)

---

  **[⬆ Наверх](#top)**

172. ### <a name="172"></a> Wie funktioniert Replikation in SQL-DBs?

**Replikation in SQL-Datenbanken**

---

### **Definition**

Replikation = **Kopieren und Verteilen von Daten** von einer Datenbank (**Primary/Master**) auf eine oder mehrere andere (**Replica/Standby**).
➡️ Ziel: **Ausfallsicherheit**, **Lastverteilung**, **hohe Verfügbarkeit**.

---

### **Arten der Replikation**

1. **Master-Slave (Primary-Replica)**

* Alle **Schreiboperationen** laufen über den Master.
* Replicas sind **read-only** → entlasten Master bei Leseanfragen.
* Beispiel: PostgreSQL Streaming Replication.

```txt
Client (Writes) → Master → Replica1 (Reads)
                           → Replica2 (Reads)
```

---

2. **Master-Master (Multi-Primary)**

* Mehrere Knoten können **lesen und schreiben**.
* Erfordert Konfliktlösung bei gleichzeitigen Writes.
* Beispiel: MySQL Group Replication, Galera Cluster.

---

3. **Synchronous vs. Asynchronous**

* **Synchronous**: Master wartet, bis Replica bestätigt → höhere Konsistenz, aber langsamer.
* **Asynchronous**: Master schreibt sofort, Replica synchronisiert später → schneller, aber eventuell verzögerte Daten.

---

### **Beispiel PostgreSQL – Streaming Replication**

* Primary schreibt Änderungen in **Write-Ahead Log (WAL)**.
* Replica liest WAL-Einträge und spielt sie nach.

```conf
# postgresql.conf (Primary)
wal_level = replica
max_wal_senders = 10
```

```conf
# recovery.conf (Replica)
primary_conninfo = 'host=primary_user port=5432 user=replicator password=secret'
```

---

### **Vorteile**

* **Load Balancing**: Master für Writes, Replicas für Reads.
* **High Availability**: Fallback auf Replica bei Ausfall.
* **Disaster Recovery**: Daten auch an anderem Standort vorhanden.

### **Nachteile**

* Mehr **Komplexität** (Failover, Konflikte).
* Asynchrone Replikation → Risiko veralteter Daten.

---

### **Zusammenfassung**

* Replikation = Daten werden vom Master auf Replikas kopiert.
* Formen: **Master-Slave**, **Master-Master**, synchron/asynchron.
* Nutzen: **Performance, Ausfallsicherheit, Verfügbarkeit**.

📖 Quellen:

* [PostgreSQL Docs – High Availability & Replication](https://www.postgresql.org/docs/current/different-replication-solutions.html)
* [MySQL Docs – Replication](https://dev.mysql.com/doc/refman/8.0/en/replication.html)

---

  **[⬆ Наверх](#top)**

173. ### <a name="173"></a> Wie schützt man DB-Verbindungen in einer Express-App?

**DB-Verbindungen in einer Express-App schützen**

---

### 1) Geheimnisse sicher handhaben

* **.env / Umgebungsvariablen** statt Hardcoding.
* Keine Secrets loggen oder ins Repo pushen; Secret-Manager nutzen (Cloud/K8s).

```js
// app.js
import "dotenv/config"; // npm i dotenv
const { DB_URL } = process.env;
```

---

### 2) TLS/SSL aktivieren

* Transport verschlüsseln (Client ↔ DB).
* Zertifikate validieren (CA, rejectUnauthorized).

```js
// node-postgres (pg) mit TLS
import pkg from "pg";
const { Pool } = pkg;

export const pool = new Pool({
  connectionString: process.env.DB_URL, // z.B. postgres://user:pass@host:5432/db
  ssl: { require: true, rejectUnauthorized: true }, // CA bei Bedarf: ca: fs.readFileSync("ca.pem")
});
```

*PostgreSQL-Server: `ssl = on`, passende Zertifikate bereitstellen.*

---

### 3) Least Privilege & getrennte Nutzer

* **Nur benötigte Rechte** (SELECT/INSERT statt SUPERUSER).
* Getrennte Konten für App/Administration; Rotation der Passwörter.

---

### 4) Connection Pool richtig konfigurieren

* Limits, Timeouts, Leaks vermeiden; bei Shutdown sauber schließen.

```js
// Pool-Optionen + Shutdown
const pool = new Pool({ max: 10, idleTimeoutMillis: 10_000, connectionTimeoutMillis: 5_000 });

process.on("SIGTERM", async () => {
  await pool.end(); // Verbindungen sauber schließen
  process.exit(0);
});
```

---

### 5) Prepared Statements / ORM-Query-Parameter

* **SQL-Injection verhindern**: nie String-Konkatenation.

```js
// Sicherer parameterisierter Query
const { rows } = await pool.query(
  "SELECT * FROM users WHERE email = $1",
  [req.body.email]
);
```

*(Sequelize/Prisma setzen Parameter automatisch; rohen SQL nur mit Bind-Parametern verwenden.)*

---

### 6) Fehlerbehandlung & Logging

* DB-Fehler **nicht** 1:1 an Client; generische Messages, Details nur intern loggen.
* Zentraler Error-Handler, strukturierte Logs (z. B. pino/winston).

```js
// Express Error-Handler
app.use((err, _req, res, _next) => {
  console.error(err);               // intern detailliert
  res.status(500).json({ error: "Internal Server Error" }); // extern generisch
});
```

---

### 7) Netzwerk-Härtung

* DB **nicht öffentlich exponieren**; nur private Netzwerke/VPC/Sicherheitsgruppen.
* IP-Allowlist/Firewall, ggf. Proxy/Bastion.
* Rate-Limiting auf API-Ebene, damit Pool/DB nicht überlastet wird.

---

### 8) Timeouts, Retries, Circuit Breaker

* Kurzlebige Transaktionen; **statement\_timeout**/`lock_timeout` serverseitig.
* Im Client: Retries mit Backoff **nur** für idempotente Reads.

---

### 9) Monitoring & Auditing

* Metriken (Pool-Auslastung, Latenzen), Slow-Query-Log, Audit-Log aktivieren.
* Alarme bei Fehlercodes (z. B. `57P01`, `40P01`).

---

### 10) Migrations & Schema-Validierung

* Reproduzierbare Migrationspipelines; kein „hot editing“ in Produktion.
* Constraints (FK, CHECK, UNIQUE) als **Sicherheitsnetz** im Schema.

---

### **Zusammenfassung**

* Secrets in Umgebungsvariablen, **TLS**, **Least-Privilege-User**, **parametrisierte Queries**, gehärtetes Netzwerk, saubere **Pool- und Fehlerkonfiguration**, Timeouts/Monitoring.
* Ziel: Vertraulichkeit (TLS), Integrität (Constraints/Parametrisierung), Verfügbarkeit (Pool/Timeouts/Rate-Limit).

📖 Quellen:

* [Express.js – Fehlerbehandlung](https://expressjs.com/de/guide/error-handling.html)
* [node-postgres (pg) – Connection & SSL](https://node-postgres.com/features/connecting)
* [PostgreSQL – Secure TCP/SSL](https://www.postgresql.org/docs/current/ssl-tcp.html)
* [Sequelize – Sicherheit & SQL-Injection](https://sequelize.org/docs/v7/other-topics/security/)
* [OWASP – SQL Injection Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html)


  **[⬆ Наверх](#top)**

174. ### <a name="174"></a> Was sind ORM-Tools (z. B. Sequelize, Prisma, TypeORM)?

**ORM-Tools (Object-Relational Mapping)**

---

### **Definition**

* **ORM** = Object-Relational Mapping.
* Brücke zwischen **Objektorientiertem Code (z. B. JavaScript-Klassen)** und **relationalen Datenbanken (SQL)**.
* Ziel: Entwickler arbeiten mit **Objekten** statt mit rohem SQL.
* ORM übernimmt:

  * SQL-Generierung (INSERT, SELECT, JOIN …)
  * Migrationen
  * Beziehungen (1:1, 1\:n, n\:m)
  * Sicherheit (Prepared Statements gegen SQL-Injection)

---

### **Beispiele: Node.js ORM-Tools**

#### **1) Sequelize**

* Beliebt im Express-Umfeld.
* Unterstützt PostgreSQL, MySQL, SQLite, MSSQL.
* Definiert Models und Beziehungen.
* Migrationen integriert.

```js
// models/User.js
import { DataTypes } from "sequelize";
import { sequelize } from "../db.js";

export const User = sequelize.define("User", {
  name: DataTypes.STRING,
  email: { type: DataTypes.STRING, unique: true }
});

// Nutzung
const user = await User.create({ name: "Sergii", email: "test@mail.com" });
```

---

#### **2) Prisma**

* Modernes ORM mit eigenem **Schema-DSL**.
* Generiert **TypeScript-Typen** automatisch → stark typisiert.
* Query-Engine in Rust → sehr performant.

```prisma
// schema.prisma
model User {
  id    Int     @id @default(autoincrement())
  name  String
  email String  @unique
}
```

```ts
// Nutzung
import { PrismaClient } from "@prisma/client";
const prisma = new PrismaClient();

const user = await prisma.user.create({
  data: { name: "Sergii", email: "test@mail.com" }
});
```

---

#### **3) TypeORM**

* Starke Integration mit TypeScript (Dekoratoren, Entities).
* Nutzt **Klassendeklarationen** direkt als Tabellen.
* Unterstützt Active Record & Data Mapper Pattern.

```ts
// User.ts
import { Entity, PrimaryGeneratedColumn, Column } from "typeorm";

@Entity()
export class User {
  @PrimaryGeneratedColumn()
  id: number;

  @Column()
  name: string;

  @Column({ unique: true })
  email: string;
}
```

```ts
// Nutzung
import { AppDataSource } from "./data-source";
import { User } from "./entity/User";

const user = new User();
user.name = "Sergii";
user.email = "test@mail.com";
await AppDataSource.manager.save(user);
```

---

### **Vor- und Nachteile von ORMs**

**Vorteile**

* Schnelle Entwicklung, weniger SQL notwendig.
* Abstraktion über verschiedene DBs.
* Automatische Migrationen & Typensicherheit (z. B. Prisma).
* Sicherheit durch Prepared Statements.

**Nachteile**

* Performance: Generierter SQL oft weniger optimiert als handgeschriebener.
* Komplexe Queries schwerer abzubilden.
* ORM-Learning-Curve.

---

### **Zusammenfassung**

* **ORM**-Tools = Mapping zwischen Objekten und relationalen Tabellen.
* Beispiele: **Sequelize** (klassisch, weit verbreitet), **Prisma** (modern, typensicher), **TypeORM** (starke TypeScript-Integration).
* Vorteile: Schnelleres Arbeiten, weniger SQL.
* Nachteile: Performance, eingeschränkte Flexibilität bei komplexen Queries.

📖 Quellen:

* [Sequelize Docs](https://sequelize.org/)
* [Prisma Docs](https://www.prisma.io/docs)
* [TypeORM Docs](https://typeorm.io/)

---

  **[⬆ Наверх](#top)**

175. ### <a name="175"></a> Vorteile und Nachteile von ORM vs. Plain SQL?

**Vorteile und Nachteile von ORM vs. Plain SQL**

---

### **ORM (z. B. Sequelize, Prisma, TypeORM)**

✅ **Vorteile**

* **Produktivität**: weniger Boilerplate, schnelleres Arbeiten mit Models statt SQL.
* **Abstraktion**: einheitliche API für verschiedene Datenbanken.
* **Sicherheit**: Prepared Statements gegen SQL-Injection standardmäßig.
* **Wartbarkeit**: Migrations-Tools, klar strukturierte Models, Beziehungen.
* **Typisierung** (z. B. Prisma, TypeORM): weniger Fehler durch Autocomplete/Types.

❌ **Nachteile**

* **Performance**: generiertes SQL oft nicht optimal.
* **Komplexität**: bei komplexen Queries oder Performance-Tuning schwieriger.
* **Learning Curve**: jedes ORM hat eigene Syntax & Konzepte.
* **Abhängigkeit**: man ist vom ORM-Ökosystem abhängig (Updates, Bugs).

---

### **Plain SQL (direkt mit pg, mysql2 etc.)**

✅ **Vorteile**

* **Volle Kontrolle**: direkt SQL schreiben, genau was DB versteht.
* **Performance**: hochoptimierte Queries möglich (Joins, Index-Hints).
* **Transparenz**: keine „Blackbox“, man sieht sofort, was passiert.
* **Flexibilität**: geeignet für Spezialfeatures (z. B. PostgreSQL JSONB, Window Functions).

❌ **Nachteile**

* **Mehr Boilerplate**: wiederholte SQL-Strings, weniger DRY.
* **Fehleranfälliger**: Gefahr für SQL-Injection, wenn Parameter nicht sauber gebunden werden.
* **Weniger portabel**: SQL-Dialekte (Postgres vs. MySQL) unterscheiden sich.
* **Migrationsaufwand**: manuelle Pflege von Schemaänderungen.

---

### **Vergleich**

| Kriterium            | ORM                                 | Plain SQL                         |
| -------------------- | ----------------------------------- | --------------------------------- |
| **Entwicklung**      | Schnell, abstrahiert                | Mehr Aufwand, aber flexibel       |
| **Performance**      | Kann suboptimal sein                | Maximale Kontrolle, optimierbar   |
| **Sicherheit**       | Eingebaute SQL-Injection-Prävention | Entwickler muss aufpassen         |
| **Komplexe Queries** | Schwer abzubilden                   | Direkt und präzise möglich        |
| **Wartbarkeit**      | Automatische Migrationen, Models    | Manuelle Migrationen, SQL-Skripte |

---

### **Zusammenfassung**

* **ORM**: gut für schnelle Entwicklung, Standard-CRUD, Teams, wo Wartbarkeit zählt.
* **Plain SQL**: gut für Performance-kritische Systeme und komplexe Queries.
* Praxis: oft **Hybrid-Ansatz** → ORM für Standard, Raw SQL für Performance-Spezialfälle.

📖 Quellen:

* [Sequelize Docs – Raw Queries](https://sequelize.org/docs/v7/core-concepts/raw-queries/)
* [Prisma Docs – Raw Database Access](https://www.prisma.io/docs/concepts/components/prisma-client/raw-database-access)
* [PostgreSQL Docs – Advanced Queries](https://www.postgresql.org/docs/current/queries.html)

---

  **[⬆ Наверх](#top)**

176. ### <a name="176"></a> Wie implementiert man Soft Delete in einer Datenbank?

**Soft Delete in Datenbanken – Patterns & Umsetzung (PostgreSQL, Sequelize, Prisma)**

---

### 1) SQL-Pattern (PostgreSQL)

**Schema:** `deleted_at TIMESTAMPTZ NULL` (NULL = aktiv, sonst gelöscht)

```sql
-- Spalte für Soft Delete
ALTER TABLE users ADD COLUMN deleted_at TIMESTAMPTZ;

-- Soft Delete (statt DELETE)
UPDATE users SET deleted_at = NOW() WHERE id = 1;

-- Standard-Selektionsregel
SELECT * FROM users WHERE deleted_at IS NULL;

-- Partial Unique Index (nur für aktive Zeilen)
CREATE UNIQUE INDEX uniq_users_email_active
  ON users (email)
  WHERE deleted_at IS NULL;

-- Optional: View nur mit aktiven Datensätzen
CREATE VIEW users_active AS
SELECT * FROM users WHERE deleted_at IS NULL;
```

**Hinweise:**

* Partial Index hält Eindeutigkeit trotz Soft Delete aufrecht. ([PostgreSQL][1])
* Views kapseln die Filterlogik. ([PostgreSQL][2])

---

### 2) Sequelize (paranoid = eingebautes Soft Delete)

```js
// db.js
import { Sequelize, DataTypes } from "@sequelize/core";
export const sequelize = new Sequelize(process.env.DB_URL, { logging: false });

// models/User.js
export const User = sequelize.define(
  "User",
  {
    name: { type: DataTypes.STRING, allowNull: false },
    email: { type: DataTypes.STRING, unique: true },
    deletedAt: { type: DataTypes.DATE }, // Spalte für Soft Delete
  },
  { paranoid: true, deletedAt: "deletedAt" } // aktiviert Soft Delete
);

// Nutzung
const u = await User.create({ name: "Sergii", email: "a@b.com" });
await u.destroy();        // setzt deletedAt (Soft Delete)
await u.restore();        // wiederherstellen
const rows = await User.findAll();               // zeigt nur aktive
const all  = await User.findAll({ paranoid: false }); // inkl. gelöschte
```

Sequelize verwaltet `deletedAt`, filtert standardmäßig gelöschte Zeilen heraus und bietet `restore()`. ([sequelize.org][3])

---

### 3) Prisma (Middleware / Client-Erweiterung)

**Schema:**

```prisma
model User {
  id        Int       @id @default(autoincrement())
  name      String
  email     String    @unique
  deletedAt DateTime? // NULL = aktiv
}
```

**Soft Delete via Middleware (\$use / \$extends):**

```js
// prisma.ts
import { PrismaClient } from "@prisma/client";
export const prisma = new PrismaClient();

// Soft-Delete: wandelt delete in update { deletedAt: now() } um
prisma.$use(async (params, next) => {
  if (params.action === "delete") {
    params.action = "update";
    params.args["data"] = { deletedAt: new Date() };
  }
  if (params.action === "deleteMany") {
    params.action = "updateMany";
    params.args["data"] = { deletedAt: new Date() };
  }
  return next(params);
});
```

**Nur aktive standardmäßig lesen (ein Ansatz):**

```js
// Beispiel-Wrapper
const activeUsers = await prisma.user.findMany({
  where: { deletedAt: null },
});
```

Prisma empfiehlt Soft Delete per Middleware; offizielle Beispielseite zeigt das Grundmuster. Für modernere Projekte kann man dasselbe Prinzip mit **Client Extensions (\$extends)** abbilden. ([Prisma][4])

---

### 4) Kaskadierendes Soft Delete

* **FK mit ON DELETE CASCADE** wirkt nur bei *Hard Deletes*.
* Für Soft Delete: Applikationslogik (mehrere Updates) oder DB-Trigger, die Kindtabellen ebenfalls `deleted_at` setzen.
* In Sequelize existieren Optionen/Utilities für Kaskaden, bei Soft Deletes jedoch oft durch App-Logik/Hook zu realisieren. ([sequelize.org][5])

---

### 5) Typische Stolpersteine & Best Practices

* **Eindeutigkeit & Indizes:** Partial-Unique-Index mit `WHERE deleted_at IS NULL`. ([PostgreSQL][1])
* **Standardfilter zentralisieren:** View/ORM-Default Scope, damit gelöschte Datensätze nicht versehentlich auftauchen. ([PostgreSQL][2])
* **Wiederherstellen (Restore):** Pfade zum Rückgängigmachen bereitstellen (z. B. `restore()` in Sequelize). ([sequelize.org][6])
* **Auditing:** `deleted_by`, `deleted_reason` Felder erwägen.
* **Hard Delete Pfad:** admin-only, z. B. Sequelize `destroy({ force: true })` oder echtes `DELETE`.

---

### **Zusammenfassung**

* **Soft Delete** markiert Datensätze (z. B. `deleted_at`) statt sie zu löschen.
* PostgreSQL: `deleted_at` + **Partial-Unique-Index** + optional **View**.
* **Sequelize**: `paranoid` + `deletedAt` + `restore()` out-of-the-box.
* **Prisma**: über **Middleware/Extensions** Delete → Update umbiegen und standardmäßig `deletedAt: null` filtern.

📖 Quellen:

* **PostgreSQL**: Partial Indexes, CREATE VIEW. ([PostgreSQL][1])
* **Sequelize**: Paranoid/`deletedAt`, Restore. ([sequelize.org][3])
* **Prisma**: Soft-Delete-Middleware (offizielle Doku), Client-Erweiterungen. ([Prisma][4])

---

[1]: https://www.postgresql.org/docs/current/sql-createindex.html?utm_source=chatgpt.com "Documentation: 17: CREATE INDEX"
[2]: https://www.postgresql.org/docs/current/sql-createview.html?utm_source=chatgpt.com "Documentation: 17: CREATE VIEW"
[3]: https://sequelize.org/docs/v6/core-concepts/paranoid/?utm_source=chatgpt.com "Paranoid"
[4]: https://www.prisma.io/docs/concepts/components/prisma-client/middleware/soft-delete-middleware?utm_source=chatgpt.com "Middleware sample: soft delete - Prisma Documentation"
[5]: https://sequelize.org/api/v7/enums/_sequelize_core.index.manualondelete?utm_source=chatgpt.com "ManualOnDelete | Documentation"
[6]: https://sequelize.org/docs/v7/models/paranoid/?utm_source=chatgpt.com "Paranoid Models"


  **[⬆ Наверх](#top)**

177. ### <a name="177"></a> Unterschied zwischen NoSQL-Typen: Key-Value, Document, Graph, Column?

**Unterschied zwischen NoSQL-Datenbank-Typen: Key-Value, Document, Graph, Column**

---

### **1) Key-Value Stores**

* **Datenmodell:** Einfachste Form → Schlüssel (`key`) → Wert (`value`).
* **Vorteile:** extrem schnell, einfach, skalierbar.
* **Einsatz:** Caching, Sitzungsverwaltung, Konfiguration.
* **Beispiele:** Redis, Riak, DynamoDB (teilweise).

```txt
key: "session:123"
value: { "userId": 42, "expires": "2025-09-06T12:00:00" }
```

---

### **2) Document Stores**

* **Datenmodell:** JSON-/BSON-ähnliche Dokumente (verschachtelte Strukturen).
* **Schema-frei** oder flexibel.
* **Vorteile:** flexibel, API-nah (JSON für REST/GraphQL), gute Query-Möglichkeiten.
* **Einsatz:** Content-Management, User-Profile, IoT, dynamische Daten.
* **Beispiele:** MongoDB, CouchDB, Firebase Firestore.

```json
{
  "_id": 1,
  "name": "Sergii",
  "email": "sergii@mail.com",
  "hobbies": ["Coding", "Fitness"]
}
```

---

### **3) Graph-Datenbanken**

* **Datenmodell:** Knoten (Entities) + Kanten (Beziehungen).
* **Optimiert für:** Netzwerke, Relationen, Traversierungen.
* **Vorteile:** sehr effizient für Beziehungsabfragen („wer kennt wen?“).
* **Einsatz:** Social Media, Empfehlungen, Betrugserkennung.
* **Beispiele:** Neo4j, ArangoDB, Amazon Neptune.

```txt
(Node) User {id:1, name:"Sergii"} 
   ──[friend_of]──> (Node) User {id:2, name:"Anna"}
```

---

### **4) Column Stores (Wide-Column)**

* **Datenmodell:** Tabellenähnlich, aber Spaltenfamilien statt Zeilenorientierung.
* **Flexibler als SQL-Tabellen:** jede Zeile kann andere Spalten haben.
* **Vorteile:** sehr gut für Big Data, Analytics, Schreib-/Lese-Performance in großen Clustern.
* **Einsatz:** Data Warehousing, Echtzeit-Analytics, Logging.
* **Beispiele:** Apache Cassandra, HBase, ScyllaDB.

```txt
RowKey: user123
| name   | email            | last_login   |
|--------|------------------|--------------|
| Sergii | s@mail.com       | 2025-09-06   |
```

---

### **Vergleich**

| Typ           | Datenmodell     | Vorteile                | Typische Nutzung             | Beispiele        |
| ------------- | --------------- | ----------------------- | ---------------------------- | ---------------- |
| **Key-Value** | Key → Value     | extrem schnell, einfach | Cache, Sessions, Token-Store | Redis, DynamoDB  |
| **Document**  | JSON-Dokumente  | flexibel, schemafrei    | CMS, Profile, IoT            | MongoDB, CouchDB |
| **Graph**     | Knoten + Kanten | stark bei Beziehungen   | Social Media, Empfehlungen   | Neo4j, Neptune   |
| **Column**    | Spaltenfamilien | skalierbar für Big Data | Analytics, Logging, IoT      | Cassandra, HBase |

---

### **Zusammenfassung**

* **Key-Value**: schnell, einfach → Caching.
* **Document**: flexibel, JSON-nah → Web/IoT.
* **Graph**: optimiert für Relationen → Social Media, Empfehlung.
* **Column**: Big Data, Analytics → Data Warehousing, Logging.

📖 Quellen:

* [MDN – NoSQL Überblick](https://developer.mozilla.org/en-US/docs/Glossary/NoSQL)
* [MongoDB Docs – NoSQL Types](https://www.mongodb.com/nosql-explained)
* [Neo4j Docs – Graph DB Basics](https://neo4j.com/developer/graph-database/)
* [Cassandra Docs – Data Model](https://cassandra.apache.org/doc/latest/)

---

  **[⬆ Наверх](#top)**

178. ### <a name="178"></a> Wie funktioniert Indexierung in MongoDB?

**Indexierung in MongoDB**

---

### **Definition**

* Ein **Index** in MongoDB ist eine Datenstruktur (standardmäßig **B-Tree**), die den schnellen Zugriff auf Dokumente ermöglicht.
* Ohne Index muss MongoDB einen **Collection Scan** machen (jede Zeile prüfen).
* Mit Index → gezielte Suche, schneller, weniger RAM/CPU-Last.

---

### **Standardindex**

* Jede Collection erhält automatisch einen **Index auf `_id`**.

```js
db.users.getIndexes();
// Ausgabe: [{ key: { _id: 1 }, name: "_id_" }]
```

---

### **Indextypen in MongoDB**

1. **Single Field Index**

```js
db.users.createIndex({ email: 1 }); // 1 = ASC, -1 = DESC
db.users.find({ email: "test@mail.com" }); // nutzt Index
```

2. **Compound Index (mehrere Felder)**

```js
db.orders.createIndex({ userId: 1, createdAt: -1 });
db.orders.find({ userId: 42 }).sort({ createdAt: -1 });
```

3. **Unique Index**

```js
db.users.createIndex({ email: 1 }, { unique: true });
```

4. **Sparse Index**

* Enthält nur Dokumente, die das Feld besitzen.

```js
db.users.createIndex({ phone: 1 }, { sparse: true });
```

5. **Partial Index**

* Index nur für bestimmte Dokumente.

```js
db.users.createIndex(
  { email: 1 },
  { partialFilterExpression: { active: true } }
);
```

6. **Text Index (Volltextsuche)**

```js
db.articles.createIndex({ content: "text" });
db.articles.find({ $text: { $search: "mongodb index" } });
```

7. **Geospatial Index**

```js
db.places.createIndex({ location: "2dsphere" });
db.places.find({
  location: {
    $near: { $geometry: { type: "Point", coordinates: [13.4, 52.5] }, $maxDistance: 5000 }
  }
});
```

---

### **Index-Analyse**

* Mit `.explain()` prüfen, ob Query Index nutzt:

```js
db.users.find({ email: "test@mail.com" }).explain("executionStats");
```

---

### **Vor- und Nachteile**

✅ Vorteile:

* Schnellere Abfragen, weniger Collection Scans
* Unterstützt Sortierung, Unique Constraints, Volltext, Geo

❌ Nachteile:

* **Speicherbedarf**: Index braucht zusätzlichen Platz
* **Langsamere Writes**: INSERT/UPDATE/DELETE müssen Index aktualisieren
* **Zu viele Indizes** = Performanceverlust

---

### **Zusammenfassung**

* MongoDB-Indizes = **B-Tree-Strukturen** für schnellen Zugriff.
* Typen: Single, Compound, Unique, Sparse, Partial, Text, Geospatial.
* Analyse mit `.explain()`.
* Trade-off: schnelleres Lesen ↔ langsameres Schreiben + mehr Speicher.

📖 Quellen:

* [MongoDB Docs – Indexes](https://www.mongodb.com/docs/manual/indexes/)
* [MongoDB Docs – Index Types](https://www.mongodb.com/docs/manual/indexes/#index-types)

---

  **[⬆ Наверх](#top)**

179. ### <a name="179"></a> Was ist Aggregation Pipeline in MongoDB?

**Aggregation Pipeline in MongoDB**

---

### **Definition**

* Die **Aggregation Pipeline** ist ein Framework in MongoDB, mit dem man **mehrstufige Datenverarbeitung** auf Collections durchführen kann.
* Funktionsweise ähnlich wie eine **Pipeline in UNIX** oder **SQL-Abfragen mit GROUP BY, HAVING, JOINs**.
* Jeder Schritt (`Stage`) verarbeitet Dokumente und reicht das Ergebnis an die nächste Stage weiter.

---

### **Häufige Stages**

1. **\$match** → Filtert Dokumente (wie `WHERE` in SQL).

```js
db.orders.aggregate([
  { $match: { status: "completed" } }
]);
```

2. **\$group** → Gruppiert Dokumente, führt Aggregationen aus (SUM, AVG, COUNT).

```js
db.orders.aggregate([
  { $group: { _id: "$customerId", total: { $sum: "$amount" } } }
]);
```

3. **\$project** → Wählt Felder aus oder berechnet neue.

```js
db.orders.aggregate([
  { $project: { _id: 0, customerId: 1, amountWithTax: { $multiply: ["$amount", 1.19] } } }
]);
```

4. **\$sort** → Sortierung.

```js
db.orders.aggregate([
  { $sort: { total: -1 } }
]);
```

5. **\$lookup** → Join mit anderer Collection.

```js
db.orders.aggregate([
  { 
    $lookup: {
      from: "customers",
      localField: "customerId",
      foreignField: "_id",
      as: "customer"
    }
  }
]);
```

6. **\$unwind** → Array in mehrere Dokumente auflösen.

```js
db.users.aggregate([
  { $unwind: "$hobbies" }
]);
```

---

### **Komplexes Beispiel**

👉 Alle Kunden mit Gesamtsumme ihrer Bestellungen, nur > 1000€, sortiert nach Betrag:

```js
db.orders.aggregate([
  { $match: { status: "completed" } },
  { $group: { _id: "$customerId", totalSpent: { $sum: "$amount" } } },
  { $match: { totalSpent: { $gt: 1000 } } },
  { $sort: { totalSpent: -1 } },
  { $lookup: {
      from: "customers",
      localField: "_id",
      foreignField: "_id",
      as: "customer"
    }
  },
  { $project: { customer: 1, totalSpent: 1 } }
]);
```

---

### **Vergleich mit SQL**

* **SQL**:

```sql
SELECT c.name, SUM(o.amount) AS totalSpent
FROM orders o
JOIN customers c ON o.customerId = c.id
WHERE o.status = 'completed'
GROUP BY c.name
HAVING SUM(o.amount) > 1000
ORDER BY totalSpent DESC;
```

---

### **Zusammenfassung**

* Aggregation Pipeline = **mehrstufige Datenverarbeitung** in MongoDB.
* Stages: `$match`, `$group`, `$project`, `$sort`, `$lookup`, `$unwind`.
* Vergleichbar mit **SQL-Analysen (GROUP BY, JOIN, HAVING)**.
* Sehr leistungsfähig für Reporting, Analytics und komplexe Transformationen.

📖 Quellen:

* [MongoDB Docs – Aggregation](https://www.mongodb.com/docs/manual/aggregation/)
* [MongoDB Docs – Aggregation Pipeline Stages](https://www.mongodb.com/docs/manual/meta/aggregation-quick-reference/)

---

  **[⬆ Наверх](#top)**

180. ### <a name="180"></a> Unterschied zwischen Embedded Documents und Referenzen in MongoDB?

**Unterschied zwischen Embedded Documents und Referenzen in MongoDB**

---

### **1) Embedded Documents (eingebettete Dokumente)**

* Daten werden direkt im Hauptdokument gespeichert (**Denormalisierung**).
* Vorteil: **schneller Zugriff**, keine zusätzliche Query oder Join nötig.
* Nachteil: Duplizierte Daten → **Inkonsistenzen** möglich, wenn mehrfach gespeichert.

**Beispiel: User mit eingebetteten Adressen**

```json
{
  "_id": 1,
  "name": "Sergii",
  "addresses": [
    { "street": "Hauptstr. 1", "city": "Leipzig" },
    { "street": "Nebenweg 5", "city": "Berlin" }
  ]
}
```

➡️ Vorteil: schneller Zugriff auf User + Adressen in **einem Dokument**.

---

### **2) Referenzen (Normalized / Linking)**

* Dokumente sind getrennt, Beziehung über **IDs**.
* Vorteil: **weniger Duplikate**, konsistente Daten, gut bei **großen oder häufig veränderten Sub-Daten**.
* Nachteil: Man braucht oft **mehrere Queries** oder `$lookup` (Join in Aggregation).

**Beispiel: User und Adressen separat**

```json
// users
{ "_id": 1, "name": "Sergii" }

// addresses
{ "_id": 100, "userId": 1, "street": "Hauptstr. 1", "city": "Leipzig" }
{ "_id": 101, "userId": 1, "street": "Nebenweg 5", "city": "Berlin" }
```

Mit Aggregation `$lookup`:

```js
db.users.aggregate([
  {
    $lookup: {
      from: "addresses",
      localField: "_id",
      foreignField: "userId",
      as: "addresses"
    }
  }
]);
```

---

### **Vergleich**

| Merkmal             | Embedded Documents                  | Referenzen                                |
| ------------------- | ----------------------------------- | ----------------------------------------- |
| **Performance**     | Schnell (1 Query)                   | Langsamer (mehrere Queries/Lookup)        |
| **Datenkonsistenz** | Risiko durch Duplikate              | Bessere Konsistenz                        |
| **Datenmenge**      | Gut für kleine, überschaubare Daten | Gut für große oder veränderliche Daten    |
| **Abfragen**        | Einfach                             | Flexibler, aber komplexer                 |
| **Use Cases**       | Profile mit Settings, Bestell-Items | User ↔ Orders, viele-zu-viele-Beziehungen |

---

### **Zusammenfassung**

* **Embedded** = alles in einem Dokument → schnell, aber riskant bei großen oder duplizierten Daten.
* **Referenzen** = separate Dokumente mit IDs → konsistenter, aber Queries komplexer.
* Praxis: oft **Hybrid-Ansatz** → häufig gebrauchte Daten einbetten, seltene/veränderliche referenzieren.

📖 Quellen:

* [MongoDB Docs – Data Modeling](https://www.mongodb.com/docs/manual/core/data-model-design/)
* [MongoDB Docs – Data Model Examples](https://www.mongodb.com/docs/manual/data-modeling/)

---

  **[⬆ Наверх](#top)**  

181. ### <a name="181"></a> Wie deployt man eine Node/Express-App auf AWS/Heroku/Vercel?

**Deployment einer Node/Express-App: AWS, Heroku, Vercel (kurz & praxisnah)**

---

### **AWS (Elastic Beanstalk oder EC2)**

**Option A: Elastic Beanstalk (managed PaaS)**

1. App vorbereiten (`"start": "node server.js"` in `package.json`, Port aus `process.env.PORT` nutzen).
2. EB CLI installieren, Umgebung erstellen & deployen:

```bash
npm i -g ebcli
eb init               # Region/Plattform: Node.js wählen
eb create             # Umgebung anlegen
eb deploy             # deployen
```

3. Logs/Umgebung per `eb logs`, `eb setenv` verwalten.
   Doku: **Deploy Node/Express on Elastic Beanstalk**. ([docs.aws.amazon.com][1])

**Option B: EC2 (voller Root-Zugriff)**

1. EC2-Instance erstellen & per SSH verbinden.
2. Node.js installieren, App clonen, Prozessmanager (z. B. PM2) + Reverse Proxy (nginx) einrichten.
3. Systemdienste/Firewall/SSL (Let’s Encrypt) konfigurieren.
   Tut.: **Node.js auf EC2 einrichten**. ([docs.aws.amazon.com][2])

**Minimaler ESM-Server**

```js
// server.js
import express from "express";
const app = express();
app.get("/", (_req, res) => res.send("OK"));
const PORT = process.env.PORT || 3000;
app.listen(PORT, () => console.log("Listening on", PORT));
```

---

### **Heroku**

1. `Procfile` anlegen und Port binden:

```
web: npm start
```

2. Git-Repo verbinden & deployen:

```bash
heroku create
git push heroku main
heroku logs --tail
```

Wichtig: Heroku startet den `web`-Prozess, der **auf `process.env.PORT`** hören muss. Doku: *Deploying Node.js apps*, *Procfile*, *Getting Started*. ([devcenter.heroku.com][3])

---

### **Vercel**

**Zwei gängige Wege:**

1. **Express direkt deployen** (zero-config): Eine der Standard-Dateien exportiert die App **als Default** oder startet einen Listener.

```js
// index.js
import express from "express";
const app = express();
app.get("/", (_req, res) => res.send("Hi from Vercel + Express"));
export default app;                 // Vercel erkennt und betreibt als Function
// Alternative: app.listen(process.env.PORT || 3000)
```

Deploy via Git oder CLI:

```bash
npm i -g vercel
vercel dev     # lokal
vercel deploy  # oder: vc deploy
```

Docs: *Express on Vercel*, *Using Express with Vercel*, *Vercel Functions*. ([Vercel][4])

---

### **Environment-Variablen (alle Plattformen)**

* AWS EB: `eb setenv KEY=value`
* Heroku: `heroku config:set KEY=value`
* Vercel: Dashboard/`vercel env`
  (immer **keine Secrets** im Code; TLS/SSL aktivieren)

---

### **DB-Verbindung**

* Managed DB verwenden (AWS RDS / Heroku Postgres / Vercel + externe DB).
* Connection-String über Umgebungsvariablen (Pooling, SSL).
  (Details je nach Treiber/ORM)

---

### **Zusammenfassung**

* **AWS**: *Elastic Beanstalk* (managed, skalierend) oder *EC2* (volle Kontrolle).
* **Heroku**: `Procfile`, auf **`PORT`** hören, `git push heroku main`.
* **Vercel**: Express **exportieren** oder listen; deploy via Git/CLI.
* **Immer**: ENV-Variablen, Logs, Health-Checks, SSL, DB extern/managed.

Quellen: AWS Elastic Beanstalk (Node/Express), EC2-Setup; Heroku Node Deployment & Procfile; Vercel Express & Functions. ([docs.aws.amazon.com][1], [devcenter.heroku.com][3], [Vercel][4])

[1]: https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_nodejs_express.html?utm_source=chatgpt.com "Deploying a Node.js Express application to Elastic Beanstalk"
[2]: https://docs.aws.amazon.com/sdk-for-javascript/v3/developer-guide/setting-up-node-on-ec2-instance.html?utm_source=chatgpt.com "Setting up Node.js on an Amazon EC2 instance"
[3]: https://devcenter.heroku.com/articles/deploying-nodejs?utm_source=chatgpt.com "Deploying Node.js Apps on Heroku"
[4]: https://vercel.com/docs/frameworks/backend/express?utm_source=chatgpt.com "Express on Vercel"


  **[⬆ Наверх](#top)**

182. ### <a name="182"></a> Was ist der Unterschied zwischen Development- und Production-Umgebung?

**Unterschied zwischen Development- und Production-Umgebung**

---

### **Development (Entwicklungsumgebung)**

* Ziel: **Entwicklung & Testen**.
* Eigenschaften:

  * **Verbose Logging** (detaillierte Fehlermeldungen, Stacktraces).
  * Hot Reloading / Auto-Refresh (z. B. `nodemon`).
  * Debugging-Tools aktiv.
  * Weniger Sicherheitsmaßnahmen (z. B. schwächere CORS-Settings, Self-Signed SSL).
  * Datenbanken oft mit **Seed-Daten** oder lokalen Instanzen.
  * Performance nicht kritisch, Fokus auf Feedback.

**Node.js Beispiel:**

```bash
NODE_ENV=development
```

```js
if (process.env.NODE_ENV === "development") {
  app.use(morgan("dev")); // detailliertes Logging
}
```

---

### **Production (Produktivumgebung)**

* Ziel: **stabile, sichere, performante Ausführung für echte Benutzer**.
* Eigenschaften:

  * **Optimiertes Logging** (nur Errors/Warnings, keine sensiblen Daten).
  * Keine Debug-Tools oder Hot Reload.
  * **Sicherheits-Features aktiviert** (CORS, Rate Limiting, Helmet).
  * DB = echte Produktionsdaten, oft in Cloud (RDS, Atlas).
  * **Skalierung** (Load Balancer, Caching, Monitoring).
  * Fehlerseiten generisch („500 Internal Server Error“), keine Stacktraces für User.

**Node.js Beispiel:**

```bash
NODE_ENV=production
```

```js
if (process.env.NODE_ENV === "production") {
  app.use(helmet());         // Security-Header
  app.set("trust proxy", 1); // wenn hinter Proxy/Load Balancer
}
```

---

### **Vergleich**

| Merkmal           | Development                  | Production                           |
| ----------------- | ---------------------------- | ------------------------------------ |
| **Logging**       | ausführlich (Stacktraces)    | minimal, sicherheitsbewusst          |
| **Tools**         | Debugger, Hot Reload         | deaktiviert                          |
| **Sicherheit**    | weniger strikt               | sehr strikt (CORS, SSL, Rate-Limits) |
| **Performance**   | zweitrangig                  | hoch optimiert                       |
| **Datenbank**     | lokale Test-DB, Seed-Daten   | echte Produktiv-DB                   |
| **Fehlerausgabe** | detailliert (für Entwickler) | generisch (für User)                 |

---

### **Zusammenfassung**

* **Development** = flexibel, detailreich, für Entwicklerkomfort.
* **Production** = sicher, stabil, performant, für Endnutzer.
* Steuerung oft über **`NODE_ENV`** oder Config-Files.

📖 Quellen:

* [Node.js Docs – process.env.NODE\_ENV](https://nodejs.org/docs/latest/api/process.html#processenv)
* [Express Docs – Best Practices: Production](https://expressjs.com/en/advanced/best-practice-performance.html)

---

  **[⬆ Наверх](#top)**

183. ### <a name="183"></a> Wie nutzt man .env-Dateien für Konfigurationen?

**.env-Dateien für Konfigurationen in Node/Express**

---

### **1) Zweck**

* `.env` Dateien speichern **Konfigurationswerte** (DB-URL, API-Keys, Ports) außerhalb des Codes.
* Prinzip: **„Configuration over Code“** → keine Secrets ins Repo pushen.
* Typisch im **12-Factor App Design**.

---

### **2) Installation**

```bash
npm install dotenv
```

---

### **3) Beispiel .env Datei**

```env
# .env
NODE_ENV=development
PORT=3000
DB_URL=postgres://user:pass@localhost:5432/mydb
JWT_SECRET=supersecret
```

⚠️ `.env` gehört in **.gitignore**, damit keine Secrets ins Git-Repo gelangen.

---

### **4) Nutzung in Node/Express**

```js
// index.js
import "dotenv/config"; // lädt automatisch .env in process.env
import express from "express";

const app = express();

const PORT = process.env.PORT || 4000;
const DB_URL = process.env.DB_URL;

app.get("/", (_req, res) => {
  res.send(`Server läuft auf Port ${PORT}, DB: ${DB_URL}`);
});

app.listen(PORT, () => console.log(`🚀 Listening on ${PORT}`));
```

---

### **5) Best Practices**

* **Sensible Daten nie hardcoden** (API-Keys, DB-Passwörter).
* Unterschiedliche `.env` Dateien pro Umgebung:

  * `.env.development`
  * `.env.test`
  * `.env.production`
* Für Production: **Secrets via ENV Variablen** setzen (Heroku, Vercel, AWS EB → Dashboard/CLI).
* Typen beachten: alle Werte sind **Strings** → ggf. casten.

```js
const DEBUG = process.env.DEBUG === "true"; // String → Boolean
const PORT = Number(process.env.PORT) || 3000;
```

---

### **Zusammenfassung**

* `.env` speichert **Konfigurationswerte/Secrets** getrennt vom Code.
* Zugriff über `process.env.VARIABLE`.
* Mit **dotenv** laden, im Repo ignorieren, in Prod über echte ENV Variablen setzen.

📖 Quellen:

* [dotenv Doku](https://github.com/motdotla/dotenv)
* [12-Factor App – Config](https://12factor.net/config)

---

  **[⬆ Наверх](#top)**

184. ### <a name="184"></a> Wie optimiert man Node.js Apps für Production?

**Optimierung von Node.js/Express für Production (kurz & praxisnah)**

---

### 1) Produktionsmodus & Build

* `NODE_ENV=production` setzen (deaktiviert Dev-Features, optimiert Abhängigkeiten).

```js
// index.js
if (process.env.NODE_ENV === "production") {
  // prod-spezifische Einstellungen
}
```

Quelle: Node.js Prozess/ENV. ([nodejs.org][1])

---

### 2) HTTP-Ebene optimieren

* **Kompression** aktivieren, **keine Sync-Funktionen** verwenden, **korrekt loggen**.

```js
// app.js
import express from "express";
import compression from "compression";
const app = express();

app.use(compression());               // gzip/br
// keine fs.*Sync in hot paths
```

Leitfaden: Express Production – Performance. ([expressjs.com][2])

* **Keep-Alive** für ausgehende HTTP-Requests (Downstreams/APIs) nutzen.

```js
import http from "node:http";
const agent = new http.Agent({ keepAlive: true });
http.request({ host: "api", agent }, (res) => { /* ... */ });
```

Hinweis zu Agent/Keep-Alive. ([nodejs.org][3])

* Für **HTTPS** sind Keep-Alive und Timeout per Default gesetzt. ([nodejs.org][4])

---

### 3) Sicherheit aktivieren

* **TLS**, **Helmet**, sauberes **Input-Handling**, sichere Cookies, Rate-Limiting.

```js
import helmet from "helmet";
import rateLimit from "express-rate-limit";
app.use(helmet());
app.use(rateLimit({ windowMs: 60_000, max: 100 }));
```

Express Security Best Practices. ([expressjs.com][5])
Node.js Security Guidelines (Übersicht). ([nodejs.org][6])

---

### 4) Skalierung: Mehr Kerne & Arbeitsteilung

* **I/O-lastig**: **Cluster** nutzt mehrere Prozesse auf demselben Port.

```js
// cluster.js
import cluster from "node:cluster";
import os from "node:os";
import http from "node:http";

if (cluster.isPrimary) {
  os.cpus().forEach(() => cluster.fork());
} else {
  http.createServer((_q, r) => r.end("ok")).listen(process.env.PORT || 3000);
}
```

Cluster-Doku. ([nodejs.org][7])

* **CPU-lastig**: **worker\_threads** für parallele Berechnungen. ([nodejs.org][8])

* **Vor App**: Reverse Proxy/Load Balancer einsetzen (Nginx/ALB). Empfehlung in Express Best Practices. ([expressjs.com][2])

---

### 5) Caching & Antworten

* **HTTP-Caching**/ETags, **Response-Caching** für häufige, teure Endpunkte.
* **Ergebnisse zwischenspeichern** (z. B. In-Memory/Redis), wie in Express-Leitfaden angeraten. ([expressjs.com][2])

---

### 6) Fehlertoleranz & Prozesse

* **Auto-Restart** (Systemd/Container/Orchestrator), **Healthchecks**, **graceful shutdown**.
* In Express Fehler zentral abfangen (keine Stacktraces an Nutzer).

```js
app.use((err, _req, res, _next) => {
  // intern detailliert loggen
  res.status(500).json({ error: "Internal Server Error" });
});
```

Express Production – Fehlerbehandlung/Restart. ([expressjs.com][2])

---

### 7) Observability & Messen statt Raten

* **Performance messen** mit `perf_hooks` (Latenzen, Bottlenecks).

```js
import { performance, PerformanceObserver } from "node:perf_hooks";
const obs = new PerformanceObserver((list) => console.log(list.getEntries()));
obs.observe({ entryTypes: ["measure"] });

performance.mark("A");
await someAsyncWork();
performance.mark("B");
performance.measure("work", "A", "B");
```

`perf_hooks` Doku. ([nodejs.org][9])

* **Logging** schlank halten (keine sensiblen Daten), Produktions-Streams beachten. ([nodejs.org][1])

---

### 8) Plattform-Spezifisches

* **Setze Prod-ENV** (AWS EB/Heroku/Vercel), **Auto-Restart/Scaling** und **Load Balancer**. Express empfiehlt Cluster/Load Balancer im Prod-Betrieb. ([expressjs.com][2])
* Für externe APIs (AWS SDK) **Verbindungen wiederverwenden** (Keep-Alive/Env-Flag). ([docs.aws.amazon.com][10])

---

### **Zusammenfassung**

* Produktionsmodus aktivieren, Kompression/Keep-Alive nutzen, Sync-Calls vermeiden.
* Sicherheit: Helmet, TLS, Rate-Limit, saubere Fehlerausgaben.
* Skalieren mit **Cluster** (I/O) bzw. **worker\_threads** (CPU), davor LB/Proxy.
* Caching einsetzen, messen mit **perf\_hooks**, schlankes Logging.

**Weiterlesen:**

* Express: Production Performance & Security. ([expressjs.com][2])
* Node.js: Cluster, Worker Threads, perf\_hooks, HTTP/HTTPS Agent, Security. ([nodejs.org][7])

[1]: https://nodejs.org/api/process.html?utm_source=chatgpt.com "Process | Node.js v24.7.0 Documentation"
[2]: https://expressjs.com/en/advanced/best-practice-performance.html?utm_source=chatgpt.com "Performance Best Practices Using Express in Production"
[3]: https://nodejs.org/api/http.html?utm_source=chatgpt.com "HTTP | Node.js v24.7.0 Documentation"
[4]: https://nodejs.org/api/https.html?utm_source=chatgpt.com "HTTPS | Node.js v24.7.0 Documentation"
[5]: https://expressjs.com/en/advanced/best-practice-security.html?utm_source=chatgpt.com "Security Best Practices for Express in Production"
[6]: https://nodejs.org/en/learn/getting-started/security-best-practices?utm_source=chatgpt.com "Node.js Security Best Practices"
[7]: https://nodejs.org/api/cluster.html?utm_source=chatgpt.com "Cluster | Node.js v24.7.0 Documentation"
[8]: https://nodejs.org/api/worker_threads.html?utm_source=chatgpt.com "Worker threads | Node.js v24.7.0 Documentation"
[9]: https://nodejs.org/api/perf_hooks.html?utm_source=chatgpt.com "Performance measurement APIs | Node.js v24.7.0 ..."
[10]: https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/node-reusing-connections.html?utm_source=chatgpt.com "Reusing Connections with Keep-Alive in Node.js"


  **[⬆ Наверх](#top)**

185. ### <a name="185"></a> Unterschied zwischen PM2 und Nodemon?

**Unterschied zwischen PM2 und Nodemon**

---

### **Nodemon**

* **Zweck:** Entwicklungs-Tool.
* Beobachtet Dateien und startet die Node-App automatisch neu, wenn sich Code ändert.
* Keine Produktionsfeatures (kein Clustering, kein Load Balancer).
* Typisch: genutzt nur in **Development**.

```bash
# Installation
npm install --save-dev nodemon

# Start in Dev
npx nodemon server.js
```

➡️ Vorteil: Entwicklerkomfort (Hot Reload).
➡️ Nachteil: Nicht für Production geeignet.

---

### **PM2**

* **Zweck:** Produktions-Prozessmanager.
* Features:

  * Start/Stop/Restart/Reload von Prozessen.
  * **Clustering** (Multi-Core-Nutzung).
  * **Monitoring** (Logs, CPU/RAM, Fehler).
  * **Auto-Restart** bei Absturz.
  * Deployment-Scripts (`pm2 deploy`).
* Typisch: genutzt in **Production**, aber auch für Dev möglich.

```bash
# Installation
npm install -g pm2

# Start in Production
pm2 start server.js -i max   # Cluster-Modus (alle Kerne)

# Monitoring
pm2 monit
pm2 logs
```

➡️ Vorteil: Stabilität, Skalierung, Monitoring.
➡️ Nachteil: mehr Konfiguration, Overhead für kleine Projekte.

---

### **Vergleich**

| Merkmal        | Nodemon (Dev)            | PM2 (Prod)                       |
| -------------- | ------------------------ | -------------------------------- |
| **Zweck**      | Entwicklung (Hot Reload) | Produktion (Prozessmanager)      |
| **Neustarts**  | bei Codeänderung         | bei Absturz, manuell oder Deploy |
| **Clustering** | ❌ nein                   | ✅ ja (Multi-Core-Nutzung)        |
| **Monitoring** | ❌ nein                   | ✅ Logs, CPU/RAM, Dashboard       |
| **Einsatz**    | Dev                      | Prod (oder auch Dev)             |

---

### **Zusammenfassung**

* **Nodemon**: Entwicklungshelfer für automatisches Neustarten.
* **PM2**: Produktions-Prozessmanager mit Clustering, Monitoring und Auto-Restart.
* Praxis: **Nodemon in Dev**, **PM2 in Prod**.

📖 Quellen:

* [Nodemon Docs](https://nodemon.io/)
* [PM2 Docs](https://pm2.keymetrics.io/docs/usage/quick-start/)

---

  **[⬆ Наверх](#top)**

186. ### <a name="186"></a> Wie funktioniert Logging in Express/Node.js?

**Logging in Express/Node.js**

---

### **1) Grundprinzip**

* Logging = systematisches **Erfassen von Ereignissen** (z. B. Requests, Errors, Warnungen).
* Ziel: **Debugging, Monitoring, Auditing**.
* In Node.js: meist Kombination aus **Konsole**, **Middleware** (Express) und **externen Libraries**.

---

### **2) Einfaches Logging (console)**

```js
console.log("Info");
console.warn("Warnung");
console.error("Fehler", err);
```

➡️ Gut für **Development**, aber nicht strukturiert genug für **Production**.

---

### **3) HTTP-Request-Logging mit Middleware**

* Gängiges Tool: **morgan** (für Express).

```js
import express from "express";
import morgan from "morgan";

const app = express();
app.use(morgan("combined")); // Logformat (Apache-Style)

app.get("/", (_req, res) => res.send("OK"));
app.listen(3000);
```

➡️ Logs enthalten: Methode, Pfad, Statuscode, Response-Zeit.

---

### **4) Strukturierte Logs (JSON)**

* Für Production wichtig → maschinenlesbar, kompatibel mit Tools (ELK, Datadog, Loki).
* Libraries: **winston**, **pino**.

**Beispiel mit Winston**

```js
import winston from "winston";

const logger = winston.createLogger({
  level: "info",
  format: winston.format.json(),
  transports: [
    new winston.transports.Console(),
    new winston.transports.File({ filename: "errors.log", level: "error" })
  ],
});

logger.info("Server gestartet");
logger.error("DB-Verbindung fehlgeschlagen");
```

**Beispiel mit Pino (schneller)**

```js
import pino from "pino";
const logger = pino({ level: "info" });

logger.info({ port: 3000 }, "Server gestartet");
logger.error({ err }, "DB-Fehler");
```

---

### **5) Error-Logging in Express**

Custom Middleware fängt Fehler ab und loggt zentral:

```js
app.use((err, req, res, next) => {
  console.error("Error:", err.message); // besser: logger.error()
  res.status(500).json({ error: "Internal Server Error" });
});
```

---

### **6) Best Practices**

* **Dev vs. Prod unterscheiden** (verbose vs. JSON-Logs).
* **Keine sensiblen Daten** loggen (Passwörter, Tokens).
* **Log Levels** nutzen (`debug`, `info`, `warn`, `error`).
* **Rotation & Aufbewahrung** (z. B. mit `winston-daily-rotate-file`).
* **Zentrales Logging** für verteilte Systeme (ELK-Stack, CloudWatch, Loki, Datadog).

---

### **Zusammenfassung**

* Node/Express Logging = Konsole (Dev) + Middleware (HTTP-Logs) + strukturierte Logger (Prod).
* Tools: **morgan** (Requests), **winston/pino** (strukturierte Logs).
* Best Practices: unterschiedliche Level, zentrale Fehler-Handler, keine sensiblen Daten.

📖 Quellen:

* [Express Docs – Error Handling](https://expressjs.com/en/guide/error-handling.html)
* [Morgan Middleware](https://github.com/expressjs/morgan)
* [Winston Logger](https://github.com/winstonjs/winston)
* [Pino Logger](https://getpino.io/)

---

  **[⬆ Наверх](#top)**

187. ### <a name="187"></a> Welche Tools für Monitoring von Node.js Apps (z. B. NewRelic, PM2, Grafana)?

**Monitoring-Tools für Node.js Apps**

---

### **1) PM2 (eingebautes Monitoring + Prozessmanager)**

* **Primär:** Prozess- und Ressourcen-Überwachung.
* Features:

  * Auto-Restart bei Crash.
  * CPU- und RAM-Monitoring (`pm2 monit`).
  * Logs sammeln (`pm2 logs`).
  * Cluster-Support.
* Gut für **kleine bis mittlere Deployments**.

```bash
pm2 start server.js -i max
pm2 monit     # Ressourcen-Monitoring
pm2 logs      # Logs ansehen
```

📖 [PM2 Docs](https://pm2.keymetrics.io/docs/usage/monitoring/)

---

### **2) New Relic (APM – Application Performance Monitoring)**

* **Kommerzielles APM-Tool**, tiefe Integration.
* Features:

  * Transaktions- und Request-Tracing.
  * Fehler- und Performance-Analyse.
  * Metrics & Dashboards out-of-the-box.
* Gut für **Enterprise-Apps**, SaaS, Microservices.

📖 [New Relic for Node.js](https://docs.newrelic.com/docs/apm/agents/nodejs-agent/getting-started/introduction-new-relic-nodejs/)

---

### **3) Grafana + Prometheus**

* **Open Source Stack** für Metrics/Visualisierung.
* Prometheus sammelt Metriken → Grafana visualisiert sie.
* Mit `prom-client` für Node.js eigene Metriken exportieren.

```js
import express from "express";
import client from "prom-client";

const app = express();
const collectDefaultMetrics = client.collectDefaultMetrics;
collectDefaultMetrics();

app.get("/metrics", async (_req, res) => {
  res.set("Content-Type", client.register.contentType);
  res.end(await client.register.metrics());
});

app.listen(3000);
```

➡️ Grafana zeigt z. B. Requests/s, Latenzen, Error-Raten.

📖 [prom-client Docs](https://github.com/siimon/prom-client)

---

### **4) Elastic Stack (ELK: Elasticsearch, Logstash, Kibana)**

* Fokus: **Logs & Search**.
* Node.js schreibt strukturierte Logs (z. B. mit **pino/winston**) → Elasticsearch → Kibana Dashboard.
* Gut für **zentrales Logging & Analyse**.

📖 [Elastic Stack Docs](https://www.elastic.co/what-is/elk-stack)

---

### **5) OpenTelemetry (Standard für Observability)**

* Open Source Standard für **Tracing, Metrics, Logging**.
* Mit Export nach Prometheus, Jaeger, Grafana, Datadog usw.
* Vorteil: Vendor-neutral.

📖 [OpenTelemetry for Node.js](https://opentelemetry.io/docs/instrumentation/js/)

---

### **Vergleich (Kurz)**

| Tool/Stack              | Fokus                      | Einsatzgebiete                       |
| ----------------------- | -------------------------- | ------------------------------------ |
| **PM2**                 | Prozesse, Logs, CPU        | Kleine Apps, DevOps light            |
| **New Relic**           | APM (Performance, Tracing) | Enterprise, SaaS                     |
| **Grafana+Prometheus**  | Metrics & Dashboards       | Cloud, Microservices                 |
| **ELK (Elastic Stack)** | Logging & Suche            | Zentrales Log-Management             |
| **OpenTelemetry**       | Tracing, Vendor-neutral    | Multi-Cloud, Observability-Standards |

---

### **Zusammenfassung**

* **PM2**: schnell eingerichtet, Prozess- und Log-Monitoring.
* **New Relic**: tiefes Application Monitoring (Transaktionen, Errors).
* **Grafana/Prometheus**: Open Source Metrics + Dashboards.
* **ELK**: Log-Sammlung und Analyse.
* **OpenTelemetry**: Standard für Tracing & Metriken, flexibel in Export.

---

  **[⬆ Наверх](#top)**

188. ### <a name="188"></a> Was ist CI/CD und wie implementiert man es mit Node.js?

**CI/CD mit Node.js – kurz erklärt & umgesetzt**

---

### **Begriffe**

* **CI (Continuous Integration):** Bei jedem Push/PR automatisch **builden, testen, linten**.
* **CD (Continuous Delivery/Deployment):** Nach erfolgreichem CI **paketieren & ausrollen** (manuell oder automatisch). ([Jenkins][1])

---

### **Projekt vorbereiten (Scripts)**

```js
// package.json (Auszug)
{
  "scripts": {
    "lint": "eslint .",
    "test": "node --test",
    "build": "tsc -p tsconfig.json || echo 'skip'",
    "start": "node dist/server.js"
  }
}
```

---

### **GitHub Actions – CI (Node 20, Cache, Tests)**

```yaml
# .github/workflows/ci.yml
name: ci
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v5
      - uses: actions/setup-node@v4
        with:
          node-version: 20
          cache: npm
      - run: npm ci
      - run: npm run lint
      - run: npm test
      - run: npm run build
```

* `setup-node@v4` mit **Dependency-Cache**; **`npm ci`** für reproduzierbare, schnelle Builds. ([GitHub Docs][2], [GitHub][3], [docs.npmjs.com][4])

---

### **GitHub Actions – CD (Beispiel Docker Push)**

```yaml
# .github/workflows/cd.yml
name: cd
on:
  push:
    branches: [main]
jobs:
  docker:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v5
      - uses: actions/setup-node@v4
        with: { node-version: 20, cache: npm }
      - run: npm ci && npm run build
      # hier: Login & Push zu eurer Registry (Beispiel, je nach Registry-Action)
      # - uses: docker/login-action@v3
      # - uses: docker/build-push-action@v6
```

* Anschließend Deployment (z. B. zu AWS, Render, Fly.io) per Job/Action oder externem CD-System. ([GitHub Docs][2])

---

### **GitLab CI – Minimalpipeline**

```yaml
# .gitlab-ci.yml
image: node:20
cache: { paths: [node_modules/] }
stages: [test, build]
install:
  stage: test
  script:
    - npm ci
    - npm test
build:
  stage: build
  script:
    - npm run build
```

* GitLab Quickstart/Beispiele siehe Doku. ([GitLab Документация][5])

---

### **Jenkins – Idee (Declarative Pipeline)**

```groovy
// Jenkinsfile (Kurzskizze)
pipeline {
  agent any
  stages {
    stage('Install & Test') { steps { sh 'npm ci && npm test' } }
    stage('Build')         { steps { sh 'npm run build' } }
    stage('Deploy')        { when { branch 'main' } steps { sh './deploy.sh' } }
  }
}
```

* Siehe Jenkins Pipeline-Doku/Tutorial. ([Jenkins][1])

---

### **Best Practices**

* **`npm ci` statt `npm install`** in CI, mit `package-lock.json` (schneller & deterministisch). ([docs.npmjs.com][4])
* **Caching** von Dependencies (Actions `cache: npm`) und **Artefakten**. ([GitHub Docs][2])
* **Branch-/Tag-Regeln**: PR → nur CI; `main`/Release-Tag → CD.
* **Secrets** als **ENV/Secrets-Store**, nicht im Repo.
* **Quality Gates**: Lint, Tests, Coverage, SCA vor Deploy.
* **Blue/Green/Canary** für risikoreduzierte Releases (plattformabhängig).

---

### **Zusammenfassung**

* **CI**: Automatisches **Build/Test/Lint** bei jedem Commit.
* **CD**: Automatisches oder manuelles **Deploy** nach erfolgreichem CI.
* Umsetzung in Node.js: **`npm ci` + Caching**, Workflows in **GitHub Actions / GitLab CI / Jenkins**, Secrets sicher verwalten, Deploy nach Branch/Tag.

**Quellen**

* GitHub Actions: **Node-Workflows & setup-node** (Cache) ([GitHub Docs][2], [GitHub][3])
* npm: **`npm ci`** Doku ([docs.npmjs.com][4])
* GitLab CI: Quick Start & Examples ([GitLab Документация][5])
* Jenkins: Pipeline Basics & Tutorial ([Jenkins][6])

Wenn du willst, passe ich dir eine konkrete **GitHub-Actions-Pipeline** für dein Projekt (ESM, Tests, Docker, Deploy) an.

[1]: https://www.jenkins.io/doc/pipeline/tour/hello-world/?utm_source=chatgpt.com "Creating your first Pipeline"
[2]: https://docs.github.com/en/actions/use-cases-and-examples/building-and-testing/building-and-testing-nodejs?utm_source=chatgpt.com "Building and testing Node.js - GitHub Actions"
[3]: https://github.com/actions/setup-node?utm_source=chatgpt.com "actions/setup-node"
[4]: https://docs.npmjs.com/cli/v8/commands/npm-ci/?utm_source=chatgpt.com "npm-ci"
[5]: https://docs.gitlab.com/ci/quick_start/?utm_source=chatgpt.com "Tutorial: Create and run your first GitLab CI/CD pipeline"
[6]: https://www.jenkins.io/doc/book/pipeline/?utm_source=chatgpt.com "Pipeline"


  **[⬆ Наверх](#top)**

189. ### <a name="189"></a> Wie baut man ein Docker-Image für eine Node/Express-App?

**Docker-Image für eine Node/Express-App bauen (Best Practices, kompakt)**

---

### 1) Projekt vorbereiten

* App muss auf `process.env.PORT` hören.
* `NODE_ENV=production` im Image setzen.
* **`.dockerignore`**: `node_modules`, `npm-debug.log`, `.git`, `dist` (falls neu gebaut wird), etc.  ([Docker Documentation][1])

```js
# .dockerignore
node_modules
npm-debug.log
.git
Dockerfile*
.dockerignore
```

---

### 2) Multi-Stage Dockerfile (klein, schnell, sicher)

* Offizielles **Node-Image** (Alpine) nutzen.
* Abhängigkeits-Cache via getrenntem COPY von `package*.json`.
* Produktion: `npm ci --omit=dev`.
* Non-root‐User `node` verwenden.  ([Docker Hub][2], [Docker Documentation][3])

```js
# Dockerfile
# ---- Base (Abhängigkeiten) ----
FROM node:20-alpine AS deps
WORKDIR /app
COPY package*.json ./
RUN npm ci

# ---- Build (falls TypeScript/Build) ----
FROM node:20-alpine AS build
WORKDIR /app
COPY --from=deps /app/node_modules ./node_modules
COPY . .
# Beispiel: TS-Build, sonst Zeile weglassen
# RUN npm run build

# ---- Runtime (schlank) ----
FROM node:20-alpine AS runtime
ENV NODE_ENV=production
WORKDIR /app

# optional: system user (Node-Image hat bereits 'node')
USER node

# nur nötige Files kopieren
COPY --chown=node:node package*.json ./
RUN npm ci --omit=dev

# App-Code (bei TS: nur dist/)
COPY --chown=node:node . .

# Port & Healthcheck
EXPOSE 3000
HEALTHCHECK --interval=30s --timeout=3s --start-period=10s \
  CMD node -e "fetch('http://127.0.0.1:'+(process.env.PORT||3000)).then(r=>process.exit(r.ok?0:1)).catch(()=>process.exit(1))" || exit 1

# Start
CMD ["node", "server.js"]
```

---

### 3) Express (ESM) minimal

```js
// server.js
import express from "express";
const app = express();

app.get("/", (_req, res) => res.send("OK"));
const PORT = process.env.PORT || 3000;
app.listen(PORT, () => console.log("Listening on", PORT));
```

---

### 4) Build & Run

```js
# Build
docker build -t my-express:prod .

# Run (Port weiterreichen)
docker run -e PORT=3000 -p 3000:3000 my-express:prod
```

---

### 5) Hinweise

* **Multi-Stage** reduziert Image-Größe deutlich; `.dockerignore` beschleunigt Builds.
* **`npm ci`** für reproduzierbare, schnelle Installationen; in Runtime-Stage `--omit=dev`.
* **Offizielle Images** werden gepflegt und sind empfohlen (Sicherheit/Updates).  ([Docker Documentation][1], [Docker Hub][2])

---

### **Zusammenfassung**

* Nutze **Multi-Stage**, **.dockerignore**, **npm ci**, **NODE\_ENV=production**, **non-root** und **Healthcheck**.
* Baue klein & deterministisch, starte über `node server.js`, exponiere `PORT`.

**Weiterlesen:**

* Docker: **Building best practices**; **Containerize Node.js**; **Dockerfile Konzepte**; **Node Official Image**. ([Docker Documentation][1], [Docker Hub][2])

[1]: https://docs.docker.com/build/building/best-practices/?utm_source=chatgpt.com "Building best practices"
[2]: https://hub.docker.com/_/node?utm_source=chatgpt.com "node - Official Image"
[3]: https://docs.docker.com/docker-hub/image-library/trusted-content/?utm_source=chatgpt.com "Trusted content | Docker Docs"


  **[⬆ Наверх](#top)**

190. ### <a name="190"></a> Unterschied zwischen Skalierung mit Clustering und Load Balancing?

**Unterschied zwischen Clustering und Load Balancing (Node.js & allgemeine Systeme)**

---

### **Clustering (innerhalb eines Servers)**

* Nutzt **mehrere Prozesse** auf **einer Maschine**.
* In Node.js: **Cluster-Modul** startet Worker-Prozesse (jeder eigener Event Loop).
* Master verteilt eingehende Requests auf Worker (meist Round-Robin).
* Vorteil: bessere **CPU-Auslastung** auf Multi-Core-Servern.
* Grenze: Skalierung bleibt auf **einem Server** beschränkt.

**Beispiel Node.js Cluster:**

```js
import cluster from "node:cluster";
import os from "node:os";
import express from "express";

if (cluster.isPrimary) {
  os.cpus().forEach(() => cluster.fork()); // 1 Worker pro CPU
} else {
  const app = express();
  app.get("/", (_req, res) => res.send(`PID: ${process.pid}`));
  app.listen(3000);
}
```

---

### **Load Balancing (über mehrere Server/Instanzen)**

* Verteilt Requests auf **mehrere Maschinen oder Container**.
* Umsetzung:

  * **Hardware/Cloud Load Balancer** (AWS ELB, Nginx, HAProxy, Traefik).
  * Worker-Prozesse können auf unterschiedlichen Hosts laufen.
* Vorteile:

  * **Horizontale Skalierung** (theoretisch unbegrenzt).
  * **Hochverfügbarkeit** (Ausfall einer Instanz → andere übernehmen).

**Beispiel Nginx als Load Balancer:**

```nginx
upstream myapp {
  server 192.168.1.10:3000;
  server 192.168.1.11:3000;
}
server {
  listen 80;
  location / {
    proxy_pass http://myapp;
  }
}
```

---

### **Vergleich**

| Merkmal             | Clustering                   | Load Balancing                       |
| ------------------- | ---------------------------- | ------------------------------------ |
| **Ebene**           | Innerhalb eines Servers      | Zwischen mehreren Servern/Containern |
| **Skalierung**      | Vertikal (Multi-Core nutzen) | Horizontal (mehr Maschinen)          |
| **Implementierung** | Node.js Cluster, PM2         | Nginx, HAProxy, AWS ELB, K8s         |
| **Grenzen**         | begrenzt auf 1 Host          | skalierbar über viele Hosts          |
| **Zweck**           | CPU-Kerne besser ausnutzen   | Verfügbarkeit + Traffic-Verteilung   |

---

### **Zusammenfassung**

* **Clustering** = mehrere Node-Prozesse **auf einer Maschine**, nutzt Multi-Core.
* **Load Balancing** = verteilt Traffic **über mehrere Maschinen/Instanzen**.
* Praxis: oft **Kombination** → Cluster pro Server + Load Balancer davor.

📖 Quellen:

* [Node.js Docs – Cluster](https://nodejs.org/docs/latest/api/cluster.html)
* [NGINX Docs – Load Balancing](https://nginx.org/en/docs/http/load_balancing.html)

---

  **[⬆ Наверх](#top)**  

191. ### <a name="191"></a> Welche Testing-Frameworks nutzt man mit Node.js/Express (Mocha, Jest, Supertest)?

**Testing-Frameworks für Node.js/Express (Mocha, Jest, Supertest und mehr)**

---

### **1) Mocha**

* **Test Runner** (führt Tests aus, async-Support, Hooks).
* Flexibel, braucht Assertion-Library (z. B. **Chai**) & Mocking-Tools extra.
* Stärken: hohe Anpassbarkeit, breite Community.

```js
// test/user.test.js
import { strict as assert } from "assert";

describe("User Service", () => {
  it("should return user", () => {
    const user = { name: "Sergii" };
    assert.equal(user.name, "Sergii");
  });
});
```

📖 [Mocha Docs](https://mochajs.org/)

---

### **2) Jest**

* All-in-One: Test Runner + Assertion + Mocking.
* Sehr beliebt (Facebook/Meta, React-Ökosystem).
* Features: Snapshot-Tests, Mocks, Code Coverage out-of-the-box.
* Einfach für **Unit- und Integrationstests**.

```js
// user.test.js
test("returns user", () => {
  const user = { name: "Sergii" };
  expect(user.name).toBe("Sergii");
});
```

📖 [Jest Docs](https://jestjs.io/)

---

### **3) Supertest (Integration/E2E für Express)**

* Nutzt man **zusätzlich zu Mocha/Jest**, um HTTP-Endpunkte zu testen.
* Simuliert Requests gegen Express ohne echten Server.

```js
// app.test.js
import request from "supertest";
import app from "../app.js"; // Express App

describe("GET /", () => {
  it("responds with OK", async () => {
    const res = await request(app).get("/");
    expect(res.status).toBe(200);
    expect(res.text).toBe("OK");
  });
});
```

📖 [Supertest Docs](https://github.com/ladjs/supertest)

---

### **Weitere Tools**

* **Chai**: Assertions für Mocha.
* **Sinon**: Mocks, Spies, Stubs.
* **AVA**: Minimalistischer Test Runner, parallelisierte Tests.
* **node\:test**: Eingebaut ab Node.js 18, leichtgewichtig.

---

### **Typische Kombinationen**

* **Jest + Supertest** → Express API testen (Standard bei vielen Projekten).
* **Mocha + Chai + Supertest** → flexible klassische Variante.
* **Node\:test + Supertest** → modern, ohne externe Runner.

---

### **Zusammenfassung**

* **Mocha** = flexibler Runner, braucht Chai/Sinon.
* **Jest** = All-in-One (empfohlen für viele Node/React-Apps).
* **Supertest** = für Integrationstests mit Express (ergänzt Jest/Mocha).
* Praxis: **Jest + Supertest** ist meist die erste Wahl für Express-Apps.

📖 Quellen:

* [Mocha](https://mochajs.org/)
* [Jest](https://jestjs.io/)
* [Supertest](https://github.com/ladjs/supertest)

---

  **[⬆ Наверх](#top)**

192. ### <a name="192"></a> Unterschied zwischen Unit-Test, Integrationstest und End-to-End-Test?

**Unterschied zwischen Unit-Test, Integrationstest und End-to-End-Test (E2E)**

---

### **1) Unit-Test**

* Testet **eine einzelne Funktion/Komponente** isoliert.
* Keine Abhängigkeiten zu DB, Netzwerk oder externen Modulen (Mocks/Stubs statt echter Services).
* Ziel: sicherstellen, dass **kleinste Bausteine** korrekt funktionieren.

**Beispiel:**

```js
// sum.js
export const sum = (a, b) => a + b;

// sum.test.js (Jest)
import { sum } from "./sum.js";
test("adds numbers", () => {
  expect(sum(2, 3)).toBe(5);
});
```

---

### **2) Integrationstest**

* Testet **Zusammenspiel mehrerer Module/Komponenten**.
* Nutzt häufig echte DB (Test-DB), API-Endpoints oder Services.
* Ziel: prüfen, ob Komponenten **korrekt interagieren**.

**Beispiel (Express + Supertest):**

```js
import request from "supertest";
import app from "../app.js";

describe("Integration: GET /users", () => {
  it("returns users from DB", async () => {
    const res = await request(app).get("/users");
    expect(res.status).toBe(200);
    expect(res.body).toEqual(expect.arrayContaining([]));
  });
});
```

---

### **3) End-to-End-Test (E2E)**

* Simuliert **realen Nutzerfluss** über das gesamte System.
* Läuft gegen echte API + echte DB + ggf. Frontend (Browser).
* Tools: **Cypress, Playwright, Selenium**.
* Ziel: sicherstellen, dass die App **als Ganzes** funktioniert.

**Beispiel (Cypress – User Login Flow):**

```js
// cypress/e2e/login.cy.js
describe("Login Flow", () => {
  it("logs in user", () => {
    cy.visit("/login");
    cy.get("input[name=email]").type("test@mail.com");
    cy.get("input[name=password]").type("123456");
    cy.get("button[type=submit]").click();
    cy.contains("Willkommen, Test");
  });
});
```

---

### **Vergleich**

| Testtyp         | Ebene           | Abhängigkeiten    | Ziel                             |
| --------------- | --------------- | ----------------- | -------------------------------- |
| **Unit-Test**   | Funktion/Modul  | keine (Mock)      | einzelne Bausteine korrekt       |
| **Integration** | Module + DB/API | echte Komponenten | Zusammenspiel funktioniert       |
| **E2E**         | Gesamtsystem    | alle (real)       | Endnutzer-Erlebnis sicherstellen |

---

### **Zusammenfassung**

* **Unit** → isoliert, schnell, viele kleine Tests.
* **Integration** → echte Komponenten interagieren.
* **E2E** → kompletter Nutzer-Flow.
* Praxis: **Test-Pyramide** → viele Unit-Tests, weniger Integrationstests, wenige E2E-Tests.

📖 Quellen:

* [MDN – Testing](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Testing)
* [Cypress Docs](https://docs.cypress.io/guides/overview/why-cypress)
* [Jest Docs](https://jestjs.io/docs/getting-started)

---

  **[⬆ Наверх](#top)**

193. ### <a name="193"></a> Wie testet man REST APIs mit Supertest?

**REST-APIs mit Supertest testen (Express + ESM)**

---

### 1) App exportieren (ohne `.listen()`)

```js
// app.js
import express from "express";
const app = express();

app.use(express.json());

app.get("/health", (_req, res) => res.type("text").send("OK"));

app.get("/users", (_req, res) => {
  res.json([{ id: 1, name: "Sergii" }]);
});

app.post("/users", (req, res) => {
  const { name } = req.body;
  if (!name) return res.status(400).json({ error: "name required" });
  res.status(201).json({ id: 2, name });
});

export default app; // wichtig: App exportieren, NICHT hier listen
```

---

### 2) Basis-Test (Jest + Supertest)

```js
// __tests__/users.test.js
import request from "supertest";
import app from "../app.js";

describe("Users API", () => {
  test("GET /health -> 200 text/plain", async () => {
    await request(app)
      .get("/health")
      .expect("Content-Type", /text/)
      .expect(200, "OK");
  });

  test("GET /users -> 200 JSON array", async () => {
    const res = await request(app).get("/users").expect(200);
    expect(res.headers["content-type"]).toMatch(/json/);
    expect(res.body).toEqual(expect.arrayContaining([expect.objectContaining({ id: 1 })]));
  });

  test("POST /users valid -> 201 JSON", async () => {
    const res = await request(app)
      .post("/users")
      .send({ name: "Anna" })              // Body
      .set("Accept", "application/json")   // Header
      .expect("Content-Type", /json/)
      .expect(201);

    expect(res.body).toMatchObject({ id: expect.any(Number), name: "Anna" });
  });

  test("POST /users invalid -> 400", async () => {
    await request(app).post("/users").send({}).expect(400);
  });
});
```

---

### 3) Query, Header, Auth, Cookies

```js
// Query-Parameter & Header
await request(app)
  .get("/users")
  .query({ limit: 10 })          // ?limit=10
  .set("X-Trace-Id", "abc-123")
  .expect(200);

// Bearer-Token
await request(app)
  .get("/protected")
  .set("Authorization", "Bearer TESTTOKEN")
  .expect(401); // z. B. wenn invalid
```

**Session/Cookies über Agent:**

```js
import request from "supertest";
const agent = request.agent(app);

await agent.post("/login").send({ email: "a@b.com", password: "x" }).expect(200);
await agent.get("/me").expect(200); // Cookie wird automatisch mitgesendet
```

---

### 4) Fehlerfälle & Edge Cases

* **Validierung**: fehlende Felder → `400`
* **Nicht gefunden**: `404`
* **Konflikt** (z. B. Unique): `409`
* **Serverfehler**: `500` (zentraler Error-Handler testbar)

```js
await request(app).get("/unknown").expect(404);
```

---

### 5) Test-DB oder Mocks

* Für Integrationstests: **Test-Datenbank** (z. B. PostgreSQL in Docker) + Migrations/Seeds.
* Für Unit-Tests der Services: **DB-Aufrufe mocken** (z. B. mit Jest Mocks).

---

### 6) Setup (Jest)

```json
// package.json (Auszug)
{
  "type": "module",
  "scripts": {
    "test": "jest --runInBand"
  }
}
```

> Tipp: Server nur in `server.js` starten und **nicht** in `app.js`. Supertest greift direkt auf die App zu – schneller & stabiler.

---

### **Zusammenfassung**

* **App exportieren**, nicht im Test hören lassen.
* Mit **Supertest** Requests simulieren: `.get/.post`, `.send()`, `.set()`, `.query()`, `.expect()`.
* **Agent** für Cookies/Sessions.
* **Edge Cases** (400/404/500) und **Header/Content-Type** mittesten.
* Für echte Integrationen: **Test-DB** nutzen, sonst **mocken**.

📖 Quellen:

* [Supertest – Doku/README](https://github.com/ladjs/supertest)
* [Express – Error Handling](https://expressjs.com/de/guide/error-handling.html)
* [Jest – Getting Started](https://jestjs.io/docs/getting-started)


  **[⬆ Наверх](#top)**

194. ### <a name="194"></a> Was sind Mocks und Stubs im Testing?

**Mocks und Stubs** sind Test-Doubles, also Platzhalterobjekte, die man im Software-Testing einsetzt, um Abhängigkeiten zu simulieren. Sie helfen, isolierte Tests zu schreiben.

---

### **Stubs**

* Stellen eine **vordefinierte Antwort** auf bestimmte Aufrufe bereit.
* Sie haben kein komplexes Verhalten, sondern liefern statische Werte zurück.
* Einsatz: Wenn eine Funktion einen Rückgabewert benötigt, aber die echte Implementierung nicht aufgerufen werden soll (z. B. Datenbankzugriff).

```js
// Beispiel mit Stub
function getUserFromDB(id) {
  return { id, name: "Max Mustermann" }; // Stub: feste Antwort
}

export function getUserName(id) {
  const user = getUserFromDB(id);
  return user.name;
}
```

---

### **Mocks**

* Gehen einen Schritt weiter: Sie **überprüfen auch, ob bestimmte Methoden aufgerufen wurden** (z. B. wie oft, mit welchen Parametern).
* Werden oft mit Testframeworks wie **Jest** oder **Sinon** erstellt.

```js
import { jest } from "@jest/globals";

// Beispiel mit Mock
test("sendEmail wird mit richtiger Adresse aufgerufen", () => {
  const sendEmail = jest.fn(); // Mock-Funktion
  const emailService = { sendEmail };

  emailService.sendEmail("test@example.com");

  expect(sendEmail).toHaveBeenCalledWith("test@example.com");
  expect(sendEmail).toHaveBeenCalledTimes(1);
});
```

---

### **Unterschied**

* **Stub** = ersetzt Logik durch feste Werte.
* **Mock** = wie Stub, aber zusätzlich mit Erwartungskontrolle (welche Methoden wurden aufgerufen, mit welchen Argumenten).

---

### **Zusammenfassung**

* **Stub**: liefert vorbereitete Werte zurück, ohne Logik.
* **Mock**: kontrolliert zusätzlich Aufrufe und Parameter.
* Beide dienen dazu, Tests zu isolieren und externe Abhängigkeiten zu vermeiden.

🔗 Quellen:

* [MDN – Testing-Guide](https://developer.mozilla.org/ru/docs/Learn/Tools_and_testing/Testing)
* [Jest Dokumentation](https://jestjs.io/docs/mock-functions)

---

  **[⬆ Наверх](#top)**

195. ### <a name="195"></a> Wie testet man asynchronen Code in Jest?

### Grundprinzipien (Jest)

Asynchronen Code testest du in Jest auf vier gängige Arten:

1. **Promise zurückgeben**
2. **`async/await` verwenden**
3. **`.resolves` / `.rejects` Matchers**
4. **Callback-APIs mit `done`** (nur wenn du eine echte Callback-API testen musst)
   Zusätzlich: **Fake Timers** für zeitabhängigen Code.

---

### 1) Promise zurückgeben

```js
// __tests__/user.test.js
import { test, expect } from '@jest/globals';
import { fetchUser } from '../user.js'; // gibt ein Promise zurück

test('liefert Nutzer', () => {
  // WICHTIG: return, damit Jest auf das Promise wartet
  return fetchUser(1).then(user => {
    expect(user.name).toBe('Max');
  });
});
```

*Referenz:* Jest „Testing Asynchronous Code“. ([jestjs.io][1])

---

### 2) Mit `async/await`

```js
import { test, expect } from '@jest/globals';
import { fetchUser } from '../user.js';

test('liefert Nutzer (async/await)', async () => {
  const user = await fetchUser(1);
  expect(user.name).toBe('Max');
});
```

*Hintergrund zu Promises & `async/await`:* MDN. ([MDN Web Docs][2])

---

### 3) Fehlerfälle mit `.rejects`

```js
import { test, expect } from '@jest/globals';
import { fetchUser } from '../user.js';

test('wirft bei 404', async () => {
  await expect(fetchUser(-1)).rejects.toThrow(/not found/);
});
```

*Referenz:* Jest `.resolves`/`.rejects`. ([jestjs.io][1])

---

### 4) Legacy-Callbacks mit `done`

```js
import { test, expect } from '@jest/globals';
import { readFileCb } from '../fs-legacy.js'; // (path, cb)

test('liest Datei (Callback)', done => {
  readFileCb('/tmp/a.txt', (err, data) => {
    try {
      expect(err).toBeNull();
      expect(data).toContain('hello');
      done(); // signalisiert Testende
    } catch (e) {
      done(e); // Fehler an Jest weiterreichen
    }
  });
});
```

**Hinweis:** `done` **nicht** mit `async` mischen. Entweder Promise/`async` **oder** `done`. ([Stack Overflow][3])

---

### 5) Zeitabhängigen Code testen (Fake Timers)

```js
// __tests__/timer.test.js
import { test, expect, jest, beforeEach, afterEach } from '@jest/globals';

function delay(ms) {
  return new Promise(res => setTimeout(res, ms));
}

beforeEach(() => {
  jest.useFakeTimers(); // Timer faken
});

afterEach(() => {
  jest.useRealTimers(); // zurücksetzen
});

test('wartet 1s und ruft Callback', async () => {
  const cb = jest.fn();

  // Effekt, der nach 1s feuert
  const work = (async () => {
    await delay(1000);
    cb();
  })();

  // Zeit „vorspulen“ – async-Variante spült auch Microtasks/Promises
  await jest.advanceTimersByTimeAsync(1000);

  await work; // optional: sicherstellen, dass Task abgeschlossen ist
  expect(cb).toHaveBeenCalledTimes(1);
});
```

*Referenz:* Jest Timer Mocks & `jest`-API (Fake Timers, `advanceTimersByTime*`, `runAllTimers*`). ([jestjs.io][4])

**Warum Fake Timers?** Du bekommst deterministische Tests ohne echtes Warten; hilfreich bei `setTimeout`/`setInterval`. Sie interagieren mit dem **Node.js Timers**-Modul bzw. Event Loop. ([nodejs.org][5])

---

### Praktische Tipps

* **Kein Mix aus `done` und `async`** in einem Test. ([Stack Overflow][3])
* Bei erwarteten Fehlern ggf. `expect.assertions(n)` nutzen, um sicherzustellen, dass Assertions wirklich ausgeführt wurden. ([jestjs.io][1])
* Für komplexe Promise-Ketten mit Timern die **async**-Timer-APIs verwenden (`advanceTimersByTimeAsync`, `runAllTimersAsync`). ([Stack Overflow][6], [GitHub][7])

---

### Zusammenfassung

* **Promises zurückgeben** oder **`async/await`** verwenden; für Fehler **`.rejects`**.
* **`done`** nur für echte Callback-APIs.
* **Fake Timers** geben Kontrolle über zeitabhängigen Code; nutze die **async**-Varianten für Promises.

**Quellen**

* Jest: *Testing Asynchronous Code*, *Timer Mocks*, *The Jest Object*. ([jestjs.io][1])
* MDN: *Promises*, *`async`/`await`*. ([MDN Web Docs][8])
* Node.js: *Timers API*. ([nodejs.org][5])

Möchtest du ein kurzes Beispiel mit **Express + Supertest** (z. B. async Route Handler + Fake Timers)?

[1]: https://jestjs.io/docs/asynchronous?utm_source=chatgpt.com "Testing Asynchronous Code"
[2]: https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Async_JS/Promises?utm_source=chatgpt.com "How to use promises - Learn web development | MDN"
[3]: https://stackoverflow.com/questions/58713379/is-done-required-in-async-jest-tests?utm_source=chatgpt.com "Is done required in async Jest tests?"
[4]: https://jestjs.io/docs/timer-mocks?utm_source=chatgpt.com "Timer Mocks"
[5]: https://nodejs.org/api/timers.html?utm_source=chatgpt.com "Timers | Node.js v24.7.0 Documentation"
[6]: https://stackoverflow.com/questions/44741102/how-to-make-jest-wait-for-all-asynchronous-code-to-finish-execution-before-expec?utm_source=chatgpt.com "How to make Jest wait for all asynchronous code to finish ..."
[7]: https://github.com/jestjs/jest/issues/15260?utm_source=chatgpt.com "advanceTimersByTime() and task queue flushing - notes · ..."
[8]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises?utm_source=chatgpt.com "Using promises - JavaScript | MDN - Mozilla"


  **[⬆ Наверх](#top)**

196. ### <a name="196"></a> Unterschied zwischen beforeAll, beforeEach, afterAll, afterEach?

### Unterschied zwischen `beforeAll`, `beforeEach`, `afterAll`, `afterEach` in Jest

Diese Hooks steuern, **wann Setup- und Teardown-Code** im Testlauf ausgeführt wird.

---

### **beforeAll**

* Wird **einmal vor allen Tests** in einer Test-Suite (`describe`-Block oder global) ausgeführt.
* Typisch für: Initialisierung, die für alle Tests gleich ist (z. B. Datenbankverbindung aufbauen).

```js
import { beforeAll, test, expect } from '@jest/globals';

let db;

beforeAll(async () => {
  db = await connectDB(); // einmal vor allen Tests
});

test('Nutzer 1', async () => {
  const user = await db.getUser(1);
  expect(user).toBeDefined();
});
```

---

### **beforeEach**

* Wird **vor jedem Test** ausgeführt.
* Typisch für: Zurücksetzen von Zuständen, Anlegen von Testdaten, Mock-Reset.

```js
import { beforeEach, test, expect } from '@jest/globals';

let arr;

beforeEach(() => {
  arr = []; // jedes Mal neu
});

test('Array ist leer', () => {
  expect(arr).toHaveLength(0);
});

test('Element hinzufügen', () => {
  arr.push(1);
  expect(arr).toContain(1);
});
```

---

### **afterEach**

* Wird **nach jedem Test** ausgeführt.
* Typisch für: Aufräumen nach jedem Test (z. B. Dateien löschen, DB-Einträge entfernen, Mocks zurücksetzen).

```js
import { afterEach, test } from '@jest/globals';

afterEach(() => {
  jest.clearAllMocks(); // alle Mocks resetten
});

test('Mock 1', () => {
  const fn = jest.fn();
  fn();
  expect(fn).toHaveBeenCalledTimes(1);
});
```

---

### **afterAll**

* Wird **einmal nach allen Tests** in der Suite ausgeführt.
* Typisch für: Ressourcen freigeben (z. B. DB-Verbindung schließen, Server stoppen).

```js
import { afterAll } from '@jest/globals';

let server;

beforeAll(() => {
  server = startServer();
});

afterAll(() => {
  server.close(); // nach allen Tests
});
```

---

### **Zusammenfassung**

* **beforeAll / afterAll** → genau einmal pro Test-Suite.
* **beforeEach / afterEach** → vor bzw. nach jedem einzelnen Test.
* Nutzen: Setup, Teardown, saubere Testumgebung.

🔗 Quellen:

* [Jest – Setup and Teardown](https://jestjs.io/docs/setup-teardown)
* [MDN – Unit testing overview](https://developer.mozilla.org/ru/docs/Learn/Tools_and_testing/Testing/Unit_testing)

---

  **[⬆ Наверх](#top)**

197. ### <a name="197"></a> Was bedeutet Test Coverage?

### **Test Coverage**

**Definition**
Test Coverage beschreibt den Anteil des Programmcodes, der durch automatisierte Tests ausgeführt wird. Sie ist eine **Metrik zur Messung der Testqualität** und zeigt, wie viel Prozent des Codes während der Testläufe abgedeckt werden.

---

### **Arten der Coverage**

1. **Statement Coverage**

   * Misst, wie viele Anweisungen (Statements) im Code mindestens einmal ausgeführt wurden.
   * Beispiel: `if (x > 0) console.log("Positiv");` → Nur ausgeführt, wenn `x > 0` getestet wird.

2. **Branch Coverage**

   * Misst, ob alle möglichen Pfade/Verzweigungen (`if`, `else`, `switch`) getestet wurden.

3. **Function Coverage**

   * Misst, ob jede definierte Funktion mindestens einmal aufgerufen wurde.

4. **Line Coverage**

   * Misst, wie viele Zeilen Code tatsächlich ausgeführt wurden.

---

### **Beispiel**

```js
// user.js
export function checkAge(age) {
  if (age >= 18) {
    return "adult";
  } else {
    return "minor";
  }
}
```

* Test 1: `checkAge(20)` → deckt `if`-Pfad ab.
* Test 2: `checkAge(15)` → deckt `else`-Pfad ab.

**Nur wenn beide Tests existieren, ist Branch Coverage = 100%.**

---

### **In Jest Coverage messen**

```bash
npx jest --coverage
```

Ergebnis: HTML-Report mit Angaben zu Statements, Branches, Functions, Lines.

---

### **Wichtige Hinweise**

* **Hohe Coverage ≠ gute Tests.**
  100% Coverage bedeutet nur, dass jeder Code ausgeführt wurde – nicht, dass die Logik korrekt geprüft wurde.
* Coverage ist ein **Indikator**, kein Selbstzweck.

---

### **Zusammenfassung**

* Test Coverage misst, wie viel Code durch Tests abgedeckt wird.
* Typen: **Statements, Branches, Functions, Lines**.
* Tools wie Jest generieren Coverage-Reports.
* **100% Coverage garantiert nicht korrekte Logik**, nur Ausführung.

🔗 Quellen:

* [Jest – Code Coverage](https://jestjs.io/docs/cli#--coverage)
* [MDN – Code Testing Overview](https://developer.mozilla.org/ru/docs/Learn/Tools_and_testing/Testing/Your_first_tests)

---

  **[⬆ Наверх](#top)**

198. ### <a name="198"></a> Was sind Best Practices für Test-Driven Development (TDD)?

### **Best Practices für Test-Driven Development (TDD)**

TDD basiert auf dem **Red-Green-Refactor-Zyklus**:

1. **Red** → Schreibe einen fehlschlagenden Test.
2. **Green** → Implementiere minimalen Code, damit der Test besteht.
3. **Refactor** → Verbessere den Code, ohne Tests zu brechen.

---

### **Best Practices**

1. **Kleine Schritte**

   * Schreibe **kleine, fokussierte Tests** für eine Funktion oder Methode.
   * Vermeide große Test-Suites ohne Zwischenfeedback.

2. **Eine Erwartung pro Test**

   * Jeder Test sollte **genau ein Verhalten** prüfen, nicht mehrere gleichzeitig.

3. **Tests vor Code**

   * Immer zuerst den Test schreiben, dann den Code.
   * So wird sichergestellt, dass der Code **testbar** ist.

4. **Klarer Fokus auf Anforderungen**

   * Tests orientieren sich an **fachlichen Anforderungen**.
   * Beispiel: „Ein Nutzer unter 18 darf sich nicht registrieren“.

5. **Schnelle Tests**

   * Tests sollten **schnell** laufen, damit sie häufig ausgeführt werden können.
   * Externe Systeme (DB, API) am besten mocken.

6. **Gute Lesbarkeit**

   * Testcode sollte wie **Dokumentation** wirken.
   * Namen wie `shouldReturnErrorIfUserIsTooYoung()` statt `test1()`.

7. **Refactor nicht vergessen**

   * Nach Green-Phase den Code aufräumen: Duplikate entfernen, saubere Architektur einhalten.

8. **Testabdeckung sinnvoll nutzen**

   * Coverage nutzen, um Lücken zu finden, aber nicht als Selbstzweck.

9. **Integration und Unit-Tests kombinieren**

   * Unit-Tests für Logik, Integrationstests für Zusammenspiel der Module.

10. **CI/CD-Pipeline**

    * Tests in die Pipeline integrieren, um automatisch Qualität zu sichern.

---

### **Beispiel (Node.js mit Jest)**

```js
// Schritt 1: Test schreiben (Red)
import { test, expect } from '@jest/globals';
import { isAdult } from '../user.js';

test('gibt true zurück, wenn Alter >= 18', () => {
  expect(isAdult(20)).toBe(true);
});

// Schritt 2: Minimaler Code (Green)
export function isAdult(age) {
  return age >= 18;
}

// Schritt 3: Refactor
// (z. B. Alter validieren, sprechendere Namen, etc.)
```

---

### **Zusammenfassung**

* TDD folgt dem **Red-Green-Refactor-Zyklus**.
* Schreibe **kleine, klare, schnelle Tests**.
* Fokus auf Anforderungen, nicht auf Implementierung.
* Tests als **lebende Dokumentation**.
* Unit- und Integrationstests kombinieren, CI/CD nutzen.

🔗 Quellen:

* [MDN – Testen in JavaScript](https://developer.mozilla.org/ru/docs/Learn/Tools_and_testing/Testing)
* [Jest Dokumentation](https://jestjs.io/docs/getting-started)

---

  **[⬆ Наверх](#top)**

199. ### <a name="199"></a> Unterschied zwischen TDD und BDD (Behavior Driven Development)?

### **Unterschied zwischen TDD und BDD**

---

### **TDD (Test-Driven Development)**

* Fokus: **Codequalität und technische Implementierung**.
* Zyklus: **Red → Green → Refactor**.
* Tests werden auf **Funktionsebene** geschrieben (Unit-Tests).
* Beispiel: Testet, ob eine Funktion `isAdult(20)` `true` zurückgibt.

```js
// TDD-Beispiel mit Jest
import { test, expect } from '@jest/globals';
import { isAdult } from '../user.js';

test('returns true if age >= 18', () => {
  expect(isAdult(20)).toBe(true);
});
```

---

### **BDD (Behavior-Driven Development)**

* Fokus: **Verhalten der Software aus Anwendersicht**.
* Nutzt eine **domänenspezifische Sprache** (z. B. Gherkin mit „Given-When-Then“).
* Tests beschreiben **Use-Cases und Business-Logik**.
* Ziel: bessere Zusammenarbeit zwischen Entwicklern, Testern und Fachseite.

```gherkin
# BDD-Beispiel mit Gherkin
Feature: Altersprüfung
  Scenario: Nutzer ist volljährig
    Given ein Nutzer mit Alter 20
    When ich die Altersprüfung durchführe
    Then sollte das Ergebnis "adult" sein
```

Umsetzung mit **Cucumber.js**:

```js
// step_definitions/steps.js
import { Given, When, Then } from '@cucumber/cucumber';
import { expect } from 'chai';
import { isAdult } from '../../user.js';

let result;

Given('ein Nutzer mit Alter {int}', function (age) {
  this.age = age;
});

When('ich die Altersprüfung durchführe', function () {
  result = isAdult(this.age);
});

Then('sollte das Ergebnis {string} sein', function (expected) {
  expect(result ? "adult" : "minor").to.equal(expected);
});
```

---

### **Direkter Vergleich**

| Aspekt     | **TDD**                              | **BDD**                                    |
| ---------- | ------------------------------------ | ------------------------------------------ |
| Fokus      | Code, technische Implementierung     | Verhalten, fachliche Anforderungen         |
| Sprache    | Technisch (z. B. Jest, Mocha, JUnit) | Natürlich/geschäftsnah (z. B. Gherkin)     |
| Beteiligte | Entwickler                           | Entwickler, Tester, Business-Analysten     |
| Testtyp    | Unit-Tests                           | Akzeptanztests, Integrationstests          |
| Ziel       | Fehlerfreier, sauberer Code          | Gemeinsames Verständnis, richtige Features |

---

### **Zusammenfassung**

* **TDD**: Entwickler-zentriert, testet **wie** etwas implementiert wird.
* **BDD**: Anwender-zentriert, testet **was** das System aus Sicht des Users tun soll.
* Beide können kombiniert werden: TDD für **Technik**, BDD für **Verhalten/Use-Cases**.

🔗 Quellen:

* [MDN – Testing Overview](https://developer.mozilla.org/ru/docs/Learn/Tools_and_testing/Testing)
* [Cucumber.js Dokumentation](https://cucumber.io/docs/installation/javascript/)
* [Jest Dokumentation](https://jestjs.io/docs/getting-started)

---

  **[⬆ Наверх](#top)**

200. ### <a name="200"></a> Welche Rolle spielt Continuous Testing in CI/CD?

### **Continuous Testing in CI/CD**

**Definition**
Continuous Testing bedeutet, dass automatisierte Tests **kontinuierlich in der gesamten CI/CD-Pipeline** ausgeführt werden – von Commit bis Deployment. Ziel: **frühes Erkennen von Fehlern** und **schnelles Feedback**.

---

### **Rolle in CI/CD**

1. **Frühes Feedback**

   * Jeder Code-Commit löst Tests aus (Unit, Integration, End-to-End).
   * Fehler werden sofort sichtbar → weniger Kosten für späte Bugfixes.

2. **Qualitätssicherung**

   * Tests sind ein „Quality Gate“: Nur wenn Tests bestehen, wird Code weiter in die nächste Pipeline-Stufe (Build, Deploy) übernommen.

3. **Automatisierung**

   * Tests laufen automatisch in CI/CD-Tools wie GitHub Actions, GitLab CI, Jenkins.
   * Entwickler müssen nicht manuell prüfen.

4. **Risikominimierung**

   * Regressionen und Sicherheitslücken werden früh erkannt.
   * Stabile Releases durch konsequentes Testen.

---

### **Beispiel GitHub Actions (Node.js mit Jest)**

```yaml
name: CI

on: [push, pull_request]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 20
      - run: npm install
      - run: npm test -- --coverage
```

👉 Bei jedem Commit/Pull Request werden Tests automatisch ausgeführt.

---

### **Zusammenfassung**

* Continuous Testing ist ein zentraler Teil von **CI/CD**, sorgt für **automatisiertes, schnelles Feedback** und verhindert, dass fehlerhafter Code deployed wird.
* Tests dienen als **Quality Gate** in der Pipeline.
* Praktisch umgesetzt mit CI/CD-Tools (GitHub Actions, GitLab CI, Jenkins).

🔗 Quellen:

* [MDN – Testing Overview](https://developer.mozilla.org/ru/docs/Learn/Tools_and_testing/Testing)
* [Jest Dokumentation](https://jestjs.io/docs/cli)
* [GitHub Actions – Testing Workflows](https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-nodejs)

---

  **[⬆ Наверх](#top)**      

201. ### <a name="201"></a> Was ist SQL Injection und wie verhindert man sie?

### **SQL Injection**

**Definition**
SQL Injection ist eine Sicherheitslücke, bei der **unsichere Benutzereingaben direkt in SQL-Statements eingefügt werden**. Ein Angreifer kann dadurch eigene SQL-Befehle einschleusen, um Daten auszulesen, zu manipulieren oder zu löschen.

---

### **Beispiel (unsicherer Code)**

```js
// ❌ Gefahr: direkte String-Konkatenation
import express from "express";
import pg from "pg";

const app = express();
const pool = new pg.Pool();

app.get("/user", async (req, res) => {
  const name = req.query.name; 
  const result = await pool.query(
    `SELECT * FROM users WHERE name = '${name}'`
  );
  res.json(result.rows);
});
```

👉 Eingabe: `?name=' OR '1'='1` führt dazu, dass alle Nutzer zurückgegeben werden.

---

### **Verhinderung von SQL Injection**

1. **Prepared Statements / Parameterized Queries**

   * Eingaben werden als Parameter übergeben, nicht in den SQL-String eingebettet.

   ```js
   // ✅ Sicher: Parametrisierte Query
   const result = await pool.query(
     "SELECT * FROM users WHERE name = $1",
     [req.query.name]
   );
   ```

2. **ORMs wie Sequelize oder Prisma**

   * Abstraktionsebene über SQL, automatische Nutzung von Prepared Statements.

   ```js
   // Sequelize-Beispiel
   const user = await User.findOne({
     where: { name: req.query.name }
   });
   ```

3. **Input Validierung & Escaping**

   * Validierung von Eingaben (z. B. nur erlaubte Zeichen).
   * Aber: kein Ersatz für Prepared Statements.

4. **Least Privilege Prinzip**

   * Datenbanknutzer nur mit minimalen Rechten (kein DROP/DELETE ALL).

5. **Security Tools**

   * Code-Scanner (z. B. ESLint-Security-Plugins, Snyk).
   * WAF (Web Application Firewall).

---

### **Zusammenfassung**

* **SQL Injection** = Manipulation von SQL über unsichere Eingaben.
* Verhindern durch: **Prepared Statements**, **ORMs**, **Validierung**, **Least Privilege**.
* Nie Benutzereingaben direkt in SQL-Strings einsetzen.

🔗 Quellen:

* [PostgreSQL – SQL Injection Prevention](https://www.postgresql.org/docs/current/sql-security.html)
* [MDN – SQL Injection](https://developer.mozilla.org/ru/docs/Glossary/SQL_Injection)
* [Sequelize Sicherheit](https://sequelize.org/docs/v6/other-topics/security/)

---

  **[⬆ Наверх](#top)**      

202. ### <a name="202"></a> Was ist NoSQL Injection?

### **NoSQL Injection**

**Definition**
NoSQL Injection ist eine Angriffstechnik, bei der Angreifer **unsichere Benutzereingaben in NoSQL-Abfragen einschleusen**, um die Logik zu manipulieren oder unbefugten Zugriff zu erlangen.
Sie ähnelt der klassischen **SQL Injection**, betrifft aber **NoSQL-Datenbanken** wie MongoDB, CouchDB oder Firebase.

---

### **Beispiel (unsicherer Code mit MongoDB)**

```js
// ❌ Unsicher: direkte Übergabe von User-Eingaben
import express from "express";
import { MongoClient } from "mongodb";

const app = express();
const client = new MongoClient("mongodb://localhost:27017");
await client.connect();
const db = client.db("testdb");
const users = db.collection("users");

app.get("/login", async (req, res) => {
  const { user, pass } = req.query;
  const result = await users.findOne({ username: user, password: pass });
  res.json(result);
});
```

👉 Angreifer könnte `?user[$ne]=null&pass[$ne]=null` eingeben → Query wird immer **true**, Login wird umgangen.

---

### **Typische Angriffsmethoden**

* **Operator Injection**: Einschleusen von MongoDB-Operatoren (`$ne`, `$gt`, `$or`).
* **JavaScript Injection** (bei älteren Versionen mit `$where`-Operator).
* **JSON Manipulation**: Übermittlung von Objekten statt Strings.

---

### **Schutzmaßnahmen**

1. **Input Validierung & Typprüfung**

   * Nur erwartete Typen erlauben (z. B. String statt Objekt).
   * Beispiel mit Joi/Validator:

   ```js
   import Joi from "joi";
   const schema = Joi.object({
     user: Joi.string().alphanum().required(),
     pass: Joi.string().min(6).required(),
   });
   ```

2. **Parameterisierung durch ORM/ODM**

   * Nutzung von **Mongoose** oder ähnlichen Tools, die Eingaben escapen.

   ```js
   // ✅ Sicherer Login mit Mongoose
   const user = await User.findOne({
     username: req.query.user,
     password: req.query.pass
   }).lean();
   ```

3. **Keine direkte Übergabe komplexer Objekte**

   * Nur primitive Werte akzeptieren, niemals ganze Objekte aus User-Input übernehmen.

4. **Least Privilege Prinzip**

   * Datenbank-User nur mit minimal nötigen Rechten.

---

### **Zusammenfassung**

* **NoSQL Injection** = Manipulation von NoSQL-Abfragen durch unsichere Eingaben.
* Besonders kritisch in **MongoDB** (Operatoren `$ne`, `$or`).
* Schutz: **Input-Validierung, Typprüfung, sichere ODMs, Least Privilege**.

🔗 Quellen:

* [OWASP – NoSQL Injection](https://owasp.org/www-community/attacks/NoSQL_Injection)
* [MongoDB Security Docs](https://www.mongodb.com/docs/manual/security/)

---

  **[⬆ Наверх](#top)**      

203. ### <a name="203"></a> Unterschied zwischen XSS und CSRF?

### **Unterschied zwischen XSS und CSRF**

---

### **XSS (Cross-Site Scripting)**

* **Ziel:** Einschleusen von **schädlichem JavaScript** in eine Webseite.
* **Angriff:** Angreifer bringt Opfer dazu, **fremden Code im Browser** auszuführen.
* **Folgen:**

  * Session Hijacking (Cookies klauen)
  * Keylogging
  * DOM-Manipulation
  * Phishing

**Beispiel (unsicherer Code):**

```js
// ❌ Unsicher: direkte Ausgabe von User-Input
app.get("/profile", (req, res) => {
  res.send(`<h1>${req.query.name}</h1>`); 
});

// Eingabe: ?name=<script>alert('XSS')</script>
```

---

### **CSRF (Cross-Site Request Forgery)**

* **Ziel:** Opfer dazu bringen, **ungewollte Aktionen** auf einer vertrauenswürdigen Seite auszuführen.
* **Angriff:** Angreifer nutzt **Session/Authentifizierung des Opfers**.
* **Folgen:**

  * Überweisungen im Banking-System
  * Passwortänderungen
  * Account-Manipulation

**Beispiel (unsicherer Code):**

```html
<!-- Opfer ist eingeloggt bei bank.com -->
<!-- Angreifer-Seite enthält: -->
<img src="https://bank.com/transfer?amount=1000&to=attacker" />
```

👉 Browser sendet automatisch Cookies → Überweisung wird ausgeführt.

---

### **Direkter Vergleich**

| Aspekt       | **XSS**                                     | **CSRF**                                            |
| ------------ | ------------------------------------------- | --------------------------------------------------- |
| Fokus        | Einschleusen von **Code** ins Opfer-Browser | Missbrauch von **Authentifizierung** des Opfers     |
| Angriffsziel | Client (Browser, User)                      | Server (durch legitime Session des Users)           |
| Folgen       | Script-Ausführung, Datendiebstahl, Phishing | Aktionen im Namen des Users                         |
| Abwehr       | Input-Sanitizing, Output-Encoding, CSP      | CSRF-Tokens, SameSite-Cookies, Double Submit Cookie |

---

### **Zusammenfassung**

* **XSS**: Angriff auf den **Browser**, Ziel ist die **Ausführung von Schadcode**.
* **CSRF**: Angriff auf den **Server**, Ziel ist die **Ausführung unerwünschter Aktionen** mit gültiger Session.
* Schutz: **XSS → Input-Sanitizing & CSP**, **CSRF → Tokens & sichere Cookies**.

🔗 Quellen:

* [MDN – Cross-site scripting (XSS)](https://developer.mozilla.org/ru/docs/Glossary/Cross-site_scripting)
* [OWASP – CSRF](https://owasp.org/www-community/attacks/csrf)

---

  **[⬆ Наверх](#top)**      

204. ### <a name="204"></a> Wie schützt man REST-APIs mit JWT?

### **REST-API-Schutz mit JWT (JSON Web Token)**

**JWT** ist ein kompakter Token-Standard, der Authentifizierungs- und Autorisierungsinformationen enthält. Er wird zwischen **Client** und **Server** im **HTTP-Header** übertragen.

---

### **Ablauf**

1. **Login**

   * User sendet Credentials (z. B. E-Mail/Passwort) an `/login`.
   * Server prüft Daten und erstellt ein JWT (signiert mit Secret oder Private Key).
   * Token wird an den Client zurückgegeben.

2. **Gesicherte Requests**

   * Client schickt JWT im `Authorization`-Header:

     ```
     Authorization: Bearer <token>
     ```
   * Server validiert Token (Signatur + Ablaufzeit).
   * Zugriff auf geschützte Ressourcen wird gewährt.

3. **Token Ablauf**

   * Tokens haben `exp` (Expiry Claim).
   * Nach Ablauf → Client muss neuen Token anfordern (oft über Refresh Token).

---

### **Beispiel (Express.js + jsonwebtoken)**

```js
// auth.js
import jwt from "jsonwebtoken";

const SECRET = "mein_geheimes_token"; // in .env speichern!

// Token generieren (Login)
export function generateToken(user) {
  return jwt.sign({ id: user.id, role: user.role }, SECRET, {
    expiresIn: "1h",
  });
}

// Middleware zum Schutz von Routen
export function authMiddleware(req, res, next) {
  const authHeader = req.headers["authorization"];
  if (!authHeader) return res.status(401).json({ error: "No token" });

  const token = authHeader.split(" ")[1];
  try {
    const payload = jwt.verify(token, SECRET);
    req.user = payload; // User-Infos aus Token
    next();
  } catch (err) {
    return res.status(403).json({ error: "Invalid token" });
  }
}
```

```js
// server.js
import express from "express";
import { generateToken, authMiddleware } from "./auth.js";

const app = express();
app.use(express.json());

// Login-Route
app.post("/login", (req, res) => {
  const { username, password } = req.body;
  if (username === "admin" && password === "1234") {
    const token = generateToken({ id: 1, role: "admin" });
    return res.json({ token });
  }
  res.status(401).json({ error: "Unauthorized" });
});

// Geschützte Route
app.get("/profile", authMiddleware, (req, res) => {
  res.json({ message: `Hallo User ${req.user.id}`, role: req.user.role });
});

app.listen(3000, () => console.log("Server läuft auf Port 3000"));
```

---

### **Best Practices**

* **Secrets in `.env`** speichern, nicht im Code.
* **Short-lived Tokens** verwenden (`expiresIn`), Refresh Tokens nutzen.
* **HTTPS** erzwingen, um Token-Leaks zu verhindern.
* **Rollen/Claims** ins JWT einfügen (RBAC).
* **Blacklist/Invalidate Tokens** bei Logout oder Sicherheitsvorfällen.

---

### **Zusammenfassung**

* JWT schützt REST-APIs durch **stateless Authentifizierung**.
* Ablauf: **Login → Token → geschützte Routen mit Middleware**.
* Best Practices: **kurze Lebensdauer, Refresh Tokens, HTTPS, Secret sicher speichern**.

🔗 Quellen:

* [JWT.io – Einführung](https://jwt.io/introduction)
* [Express.js Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* [Node.js jsonwebtoken Package](https://github.com/auth0/node-jsonwebtoken)

---

  **[⬆ Наверх](#top)**      

205. ### <a name="205"></a> Unterschied zwischen JWT und OAuth2?

### **Unterschied zwischen JWT und OAuth2**

---

### **JWT (JSON Web Token)**

* **Was es ist:**
  Ein **Token-Format** (RFC 7519) für den sicheren Transport von Claims (z. B. User-ID, Rollen).
* **Eigenschaften:**

  * Kompakt, Base64-encoded
  * Signiert (HMAC oder RSA/ECDSA) → Manipulation erkennbar
  * Enthält Claims: `iss`, `sub`, `exp`, eigene Daten
* **Nutzung:**

  * Häufig für **Authentifizierung** in REST-APIs (stateless login).
  * Token wird direkt im `Authorization: Bearer <token>` Header übertragen.

**Beispiel JWT Payload:**

```json
{
  "sub": "12345",
  "role": "admin",
  "exp": 1694018400
}
```

---

### **OAuth2**

* **Was es ist:**
  Ein **Autorisierungs-Framework** (RFC 6749), das beschreibt, **wie ein Client Zugriff auf Ressourcen eines Users** bei einem Ressource-Server erhält.
* **Eigenschaften:**

  * Rollen: **Resource Owner**, **Client**, **Authorization Server**, **Resource Server**
  * Flows: Authorization Code, Implicit, Client Credentials, Device Code
  * Liefert **Access Tokens** (oft in JWT-Format, aber nicht zwingend)
* **Nutzung:**

  * Delegierte Autorisierung (z. B. „Login mit Google“)
  * Ermöglicht Drittanbietern Zugriff auf User-Daten ohne Passwortweitergabe

**Beispiel Flow (Authorization Code):**

1. User loggt sich bei Google ein.
2. App erhält **Authorization Code**.
3. App tauscht Code beim Auth-Server gegen **Access Token**.
4. App nutzt Token, um Ressourcen beim Resource Server abzufragen.

---

### **Direkter Vergleich**

| Aspekt         | **JWT**                                   | **OAuth2**                                       |
| -------------- | ----------------------------------------- | ------------------------------------------------ |
| Typ            | Token-Format                              | Autorisierungs-Framework                         |
| Zweck          | Authentifizierung / Informationstransport | Zugriffskontrolle & Delegation von Rechten       |
| Standardisiert | RFC 7519                                  | RFC 6749                                         |
| Enthält        | Claims (User-ID, Rollen, Metadaten)       | Access Tokens (oft JWT), Refresh Tokens          |
| Verwendung     | API-Login, stateless Sessions             | „Login mit…“, API-Zugriff im Namen eines Nutzers |
| Abhängigkeit   | Kann allein genutzt werden                | Kann JWT nutzen, muss aber nicht                 |

---

### **Zusammenfassung**

* **JWT** = Token-Format zur Übertragung von Claims (oft für Authentifizierung).
* **OAuth2** = Framework für **Autorisierung** und Delegation (liefert Tokens, meist JWT).
* Verhältnis: **OAuth2 kann JWT verwenden, muss aber nicht**.

🔗 Quellen:

* [JWT.io – Einführung](https://jwt.io/introduction)
* [OAuth2 Spezifikation (RFC 6749)](https://datatracker.ietf.org/doc/html/rfc6749)
* [MDN – OAuth](https://developer.mozilla.org/en-US/docs/Glossary/OAuth)

---

  **[⬆ Наверх](#top)**      

206. ### <a name="206"></a> Unterschied zwischen Session-basiertem und Token-basiertem Auth?

### **Unterschied zwischen Session-basierter und Token-basierter Authentifizierung**

---

### **Session-basierte Authentifizierung**

* **Funktionsweise**

  * Nach Login speichert der Server eine **Session** (z. B. in Memory oder DB).
  * Client erhält eine **Session-ID** (Cookie).
  * Bei jedem Request sendet der Client Cookie → Server prüft Session.
* **Eigenschaften**

  * Server ist „stateful“ (muss Sessions speichern).
  * Gut geeignet für klassische Web-Apps (mit Cookies, Server-Render).
  * Skalierung schwieriger (Sessions müssen zwischen Servern geteilt werden).

**Beispiel-Flow**

1. User loggt sich ein.
2. Server erstellt Session: `{id: 123, user: "Max"}`.
3. Client speichert Cookie: `sessionId=123`.
4. Jeder Request → Server prüft Session in DB.

---

### **Token-basierte Authentifizierung (z. B. mit JWT)**

* **Funktionsweise**

  * Nach Login erstellt Server ein **Token** (z. B. JWT, signiert).
  * Client speichert Token (im LocalStorage oder als Cookie).
  * Bei jedem Request sendet der Client das Token im Header (`Authorization: Bearer ...`).
  * Server validiert Token (Signatur + Ablaufzeit), ohne in DB nachzuschauen.
* **Eigenschaften**

  * Server ist „stateless“ (kein Session-Storage nötig).
  * Ideal für **APIs, Microservices, Mobile Apps**.
  * Leicht horizontal skalierbar.
  * Risiko: Bei Token-Leak ist Zugriff möglich, bis Token abläuft.

**Beispiel-Flow**

1. User loggt sich ein.
2. Server gibt JWT zurück: `{sub: "123", role: "admin", exp: ...}`.
3. Client speichert JWT.
4. Jeder Request → JWT im Header, Server prüft Signatur.

---

### **Direkter Vergleich**

| Aspekt        | **Session-basiert**                 | **Token-basiert (JWT)**                  |
| ------------- | ----------------------------------- | ---------------------------------------- |
| Zustand       | Stateful (Session-Store)            | Stateless (keine Speicherung nötig)      |
| Speicherung   | Session-ID im Cookie                | Token im Header oder Cookie              |
| Skalierung    | Schwieriger (Session-Sharing nötig) | Einfach (jeder Server kann Token prüfen) |
| Sicherheit    | Sicherer bei kurzen Sessions        | Token-Leak kritisch bis Expiry           |
| Einsatzgebiet | Klassische Web-Apps                 | REST-APIs, SPAs, Mobile Apps             |

---

### **Zusammenfassung**

* **Session-basiert**: Server speichert Status, Client sendet Session-ID → gut für Web-Apps, weniger skalierbar.
* **Token-basiert**: Server bleibt stateless, Client sendet Token (z. B. JWT) → gut für APIs/Microservices, skalierbarer.

🔗 Quellen:

* [MDN – HTTP Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)
* [JWT.io Einführung](https://jwt.io/introduction)
* [Express.js Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

207. ### <a name="207"></a> Wie konfiguriert man sichere CORS-Regeln?

### **Sichere CORS-Konfiguration (Cross-Origin Resource Sharing)**

---

#### Grundprinzipien

* **Whitelist statt Wildcard:** Nur explizite Origins erlauben (keine `*`, außer bei **ohne** Credentials).
* **Nur nötige Methoden/Headers freigeben:** Minimalprinzip.
* **Credentials nur wenn nötig:** `Access-Control-Allow-Credentials: true` **nie** mit `Access-Control-Allow-Origin: *` kombinieren.
* **Preflight kontrollieren:** Nur benötigte Werte erlauben, sinnvolles `Access-Control-Max-Age` setzen.
* **TLS/HTTPS erzwingen:** Besonders bei Cookies/Authorization-Headern.
* **CSRF bedenken:** CORS ≠ CSRF-Schutz; ggf. CSRF-Tokens/SameSite-Cookies nutzen.

---

### **Express mit `cors` (empfohlen)**

```js
// server.mjs
import express from "express";
import cors from "cors";

const app = express();

// 1) Whitelist definieren
const WHITELIST = [
  "https://app.example.com",
  "https://admin.example.com"
];

// 2) Dynamische Origin-Validierung
const corsOptions = {
  origin(origin, cb) {
    // z. B. für Tools/Healthchecks ohne Origin:
    if (!origin) return cb(null, false);           // keine CORS-Header setzen
    if (WHITELIST.includes(origin)) return cb(null, true);
    return cb(new Error("Not allowed by CORS"));
  },
  methods: ["GET", "POST", "PUT", "DELETE"],       // minimal halten
  allowedHeaders: ["Content-Type", "Authorization"],
  exposedHeaders: ["X-Request-Id"],                // nur wenn wirklich nötig
  credentials: true,                                // nur wenn Cookies/HTTP Auth nötig
  maxAge: 600,                                      // Preflight-Ergebnis 10 Min. cachen
  optionsSuccessStatus: 204                         // saubere Preflight-Antwort
};

app.use(cors(corsOptions));
// Optional: Preflight explizit bedienen
app.options("*", cors(corsOptions));

app.get("/api/data", (req, res) => {
  res.json({ ok: true });
});

app.listen(3000);
```

**Hinweise:**

* **Credentials + Whitelist:** Bei `credentials: true` **muss** `Access-Control-Allow-Origin` eine **konkrete** Origin sein (kein `*`).
* **Nur nötige Methoden/Headers freigeben.**
* **Staging/Prod trennen:** Whitelist aus ENV laden; in Dev evtl. `http://localhost:5173` o. ä. ergänzen.

---

### **Alternative: Öffentliche, rein lesende API (ohne Credentials)**

```js
import cors from "cors";
app.use(cors({
  origin: "*",                  // nur sicher, wenn keinerlei Cookies/Secrets
  methods: ["GET"],             // read-only
  allowedHeaders: ["Content-Type"],
  credentials: false
}));
```

> Für **öffentliche** Daten ohne Auth geeignet; andernfalls **nicht** verwenden.

---

### **Manuell (nur bei Spezialfällen)**

```js
// Minimaler, strikter Header-Set
app.use((req, res, next) => {
  const origin = req.headers.origin;
  const WHITELIST = new Set(["https://app.example.com"]);
  if (WHITELIST.has(origin)) {
    res.setHeader("Access-Control-Allow-Origin", origin);
    res.setHeader("Vary", "Origin");                // wichtig für Caches
    res.setHeader("Access-Control-Allow-Methods", "GET,POST");
    res.setHeader("Access-Control-Allow-Headers", "Content-Type,Authorization");
    res.setHeader("Access-Control-Allow-Credentials", "true");
    res.setHeader("Access-Control-Max-Age", "600");
  }
  if (req.method === "OPTIONS") return res.sendStatus(204);
  next();
});
```

---

### **Cookies & CSRF**

* Bei Cookie-Auth: `SameSite=None; Secure` setzen, nur über HTTPS senden.
* CSRF separat absichern (z. B. CSRF-Tokens, Double-Submit-Cookie).
  CORS allein verhindert **keine** CSRF-Angriffe.

---

### **Zusammenfassung**

* **Whitelist** konkrete Origins, **keine** Wildcards mit Credentials.
* **Minimalprinzip** für Methoden/Headers/Exposed Headers.
* **Preflight** sauber beantworten und mit `maxAge` cachen.
* **HTTPS** erzwingen; **CSRF** separat adressieren.
* In Express `cors`-Middleware mit **dynamischer Origin-Funktion** verwenden.

**Quellen / Weiterführend**

* [MDN – CORS Überblick](https://developer.mozilla.org/ru/docs/Web/HTTP/CORS)
* [MDN – `Access-Control-*` Header](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers/Access-Control-Allow-Origin)
* [Express.js – CORS Middleware](https://expressjs.com/de/resources/middleware/cors.html)
* [MDN – SameSite-Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers/Set-Cookie/SameSite)


  **[⬆ Наверх](#top)**      

208. ### <a name="208"></a> Was ist HTTPS und wie implementiert man es in Node.js?

### **Was ist HTTPS?**

* **HTTPS** = HTTP über **TLS/SSL**. Es verschlüsselt Transportdaten, stellt **Integrität** sicher und ermöglicht **Authentizität** über Zertifikate (CA-signiert).
* Schützt u. a. Login-Daten, Cookies, Tokens und API-Payloads vor Mitlesen/Manipulation.

---

### **Voraussetzungen**

* **Zertifikat + privater Schlüssel** (typisch von einer CA wie Let’s Encrypt).
* Optional **Intermediate/Chain** (CA-Bundle).
* **TLS-fähiger Server** (direkt in Node.js oder via Reverse Proxy wie Nginx/Traefik).

---

### **Implementierung in Node.js (nativ, mit Express)**

```js
// server.mjs
import fs from "node:fs";
import https from "node:https";
import http from "node:http";
import express from "express";

const app = express();
app.get("/health", (_req, res) => res.json({ ok: true }));

// 1) HTTPS-Server mit Zertifikat starten
const options = {
  key: fs.readFileSync("/etc/letsencrypt/live/example.com/privkey.pem"),
  cert: fs.readFileSync("/etc/letsencrypt/live/example.com/fullchain.pem"),
  // optional: ca: fs.readFileSync("chain.pem"),
  // starke Ciphers/TLS-Versionen werden systemweit konfiguriert
};

https.createServer(options, app).listen(443, () => {
  console.log("HTTPS läuft auf :443");
});

// 2) HTTP -> HTTPS Redirect (sauberer Migrationspfad)
http.createServer((req, res) => {
  const host = req.headers.host?.replace(/:\d+$/, "");
  res.writeHead(301, { Location: `https://${host}${req.url}` });
  res.end();
}).listen(80);
```

**Hinweise**

* Zertifikats-Pfad für Let’s Encrypt je nach Setup (z. B. `/etc/letsencrypt/...`).
* In Containern/Clouds oft **TLS-Termination** am Ingress/Proxy; Node lauscht dann nur auf **HTTP** (z. B. Port 3000).

---

### **Sicherheits-Ergänzungen (empfohlen)**

```js
// security.mjs
import express from "express";
import helmet from "helmet";

const app = express();

// HSTS: nach erfolgreichem HTTPS-Betrieb aktivieren (z. B. 6 Monate)
app.use(helmet.hsts({ maxAge: 15552000, includeSubDomains: true, preload: false }));

// Weitere sinnvolle Header
app.use(helmet.frameguard({ action: "deny" }));
app.use(helmet.xssFilter());          // legacy: heute Teil von helmet() baseline
app.use(helmet.noSniff());

export default app;
```

* **HSTS** zwingt künftige Zugriffe auf HTTPS; erst aktivieren, wenn HTTPS stabil läuft (sonst Lock-in).
* Bei Betrieb **hinter Proxy**: `app.set('trust proxy', 1)` setzen, damit `req.secure` korrekt ist und Cookie-Flags (Secure) funktionieren.

---

### **HTTP/2 (optional)**

```js
// http2.mjs
import fs from "node:fs";
import http2 from "node:http2";
import express from "express";

const app = express();
app.get("/", (_req, res) => res.send("Hello HTTP/2"));

const server = http2.createSecureServer({
  key: fs.readFileSync("/path/privkey.pem"),
  cert: fs.readFileSync("/path/fullchain.pem"),
  allowHTTP1: true, // Fallback auf HTTP/1.1
}, app);

server.listen(443);
```

* **Vorteile**: Multiplexing, Header-Kompression.
* In vielen Deployments übernimmt HTTP/2 bereits der **Reverse Proxy**.

---

### **Zertifikate beziehen (Praxis)**

* **Let’s Encrypt** via **Certbot** auf dem Host/Proxy (empfohlen): Proxy terminiert TLS und leitet an Node weiter.
* **Lokale Entwicklung**: self-signed Zertifikat (nur zu Testzwecken).

---

### **Best Practices**

* **TLS nur über HTTPS**; in Prod **immer** HTTPS erzwingen (Redirect + HSTS).
* **Secrets** (Keys, Pfade) aus **ENV**/Secret-Store, nicht hardcoden.
* **Kein Mixed Content** (alle Ressourcen über HTTPS laden).
* **Reverse Proxy bevorzugen** (einfachere Zertifikatsrotation, HTTP/2/3, OCSP Stapling).
* **Security-Header** mit `helmet` setzen; Cookies `Secure` und ggf. `SameSite=None`.

---

### **Zusammenfassung**

* **HTTPS = HTTP über TLS**: Vertraulichkeit, Integrität, Authentizität.
* In Node.js: `https.createServer({ key, cert }, app)`; HTTP→HTTPS Redirect; Security-Header + HSTS.
* Produktion: oft **TLS-Termination am Proxy**, Node bleibt schlank.

**Quellen / Weiterführend**

* MDN: [Einführung zu HTTPS](https://developer.mozilla.org/ru/docs/Web/HTTP/Overview#https) • [HSTS](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers/Strict-Transport-Security)
* Node.js Docs: [`https` Modul](https://nodejs.org/docs/latest/api/https.html) • [`http2` Modul](https://nodejs.org/docs/latest/api/http2.html)
* Express: [Sicherheits-Best-Practices](https://expressjs.com/de/advanced/best-practice-security.html) • [Behind Proxies](https://expressjs.com/en/guide/behind-proxies.html)
* Let’s Encrypt: [Certbot – Getting Started](https://certbot.eff.org/)


  **[⬆ Наверх](#top)**      

209. ### <a name="209"></a> Welche Sicherheits-Header kann man mit Helmet setzen?

### **Sicherheits-Header mit Helmet in Express**

**Helmet** ist ein Express-Middleware-Paket, das gängige HTTP-Sicherheits-Header setzt. Standardmäßig aktiviert `helmet()` mehrere Header, weitere können gezielt konfiguriert werden.

---

### **Wichtige Header**

1. **Content-Security-Policy (CSP)**

   * Kontrolliert, von wo Skripte, Styles, Bilder etc. geladen werden dürfen.
   * Schutz vor **XSS** und Daten-Injection.

   ```js
   import helmet from "helmet";
   app.use(helmet.contentSecurityPolicy({
     directives: {
       defaultSrc: ["'self'"],
       scriptSrc: ["'self'", "cdn.example.com"],
       objectSrc: ["'none'"],
     },
   }));
   ```

2. **Strict-Transport-Security (HSTS)**

   * Erzwingt HTTPS für künftige Requests.
   * Schutz vor **SSL Stripping**.

   ```js
   app.use(helmet.hsts({
     maxAge: 60 * 60 * 24 * 180, // 180 Tage
     includeSubDomains: true,
     preload: true,
   }));
   ```

3. **X-Frame-Options** (heute über `frameguard`)

   * Verhindert, dass Seiten in `<iframe>` eingebettet werden.
   * Schutz vor **Clickjacking**.

   ```js
   app.use(helmet.frameguard({ action: "deny" }));
   ```

4. **X-Content-Type-Options**

   * Verhindert, dass Browser MIME-Typen „erraten“.
   * Schutz vor **MIME Sniffing**.

   ```js
   app.use(helmet.noSniff());
   ```

5. **X-XSS-Protection** *(älter, heute oft deprecated)*

   * Aktiviert XSS-Filter in alten Browsern.
   * Heutzutage ersetzt durch CSP.

   ```js
   app.use(helmet.xssFilter());
   ```

6. **Referrer-Policy**

   * Kontrolliert, wie viel Referrer-Info gesendet wird.
   * Schutz der **Privatsphäre**.

   ```js
   app.use(helmet.referrerPolicy({ policy: "no-referrer" }));
   ```

7. **Permissions-Policy (früher Feature-Policy)**

   * Legt fest, welche Browser-Features (z. B. Geolocation, Kamera) erlaubt sind.

   ```js
   app.use(helmet.permittedCrossDomainPolicies());
   ```

8. **Cross-Origin-Resource-Policy (CORP)**

   * Schutz vor ungewolltem Datenzugriff über andere Origins.

   ```js
   app.use(helmet.crossOriginResourcePolicy({ policy: "same-origin" }));
   ```

9. **Cross-Origin-Opener-Policy (COOP)**

   * Isolation des Browsing-Kontexts.
   * Schutz vor **Side-Channel-Angriffen** (Spectre).

   ```js
   app.use(helmet.crossOriginOpenerPolicy({ policy: "same-origin" }));
   ```

10. **Cross-Origin-Embedder-Policy (COEP)**

    * Stellt sicher, dass eingebettete Ressourcen CORS-kompatibel sind.
    * Wichtig für SharedArrayBuffer.

    ```js
    app.use(helmet.crossOriginEmbedderPolicy({ policy: "require-corp" }));
    ```

---

### **Minimalbeispiel**

```js
import express from "express";
import helmet from "helmet";

const app = express();

// Basis-Sicherheitsheader aktivieren
app.use(helmet());

// Zusätzliche CSP
app.use(helmet.contentSecurityPolicy({
  directives: {
    defaultSrc: ["'self'"],
    imgSrc: ["'self'", "data:"],
    scriptSrc: ["'self'", "cdn.example.com"],
  },
}));

app.listen(3000, () => console.log("Server läuft auf Port 3000"));
```

---

### **Zusammenfassung**

* **Helmet** setzt Header für **CSP, HSTS, X-Frame-Options, X-Content-Type-Options, Referrer-Policy, COOP, COEP, CORP**.
* Ziel: Schutz vor **XSS, Clickjacking, Datenlecks, Side-Channel-Angriffen**.
* **CSP + HSTS** gehören zu den wichtigsten und sollten gezielt konfiguriert werden.

🔗 Quellen

* [Helmet.js Offizielle Dokumentation](https://helmetjs.github.io/)
* [MDN – Sicherheits-Header Übersicht](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers)
* [Express.js Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

210. ### <a name="210"></a> Wie schützt man API-Keys in einer Node.js App?

### **API-Keys in Node.js sicher handhaben**

---

#### 1) **Nicht ins Repo commiten**

* `.env` in `.gitignore`
* Pre-commit-Checks (z. B. `git-secrets`, `pre-commit`) nutzen.
* **Lecks** sofort rotieren.

```bash
# .gitignore
.env
.env.*
```

---

#### 2) **Environment Variables statt Hardcoding**

* Keys **nur** aus `process.env` lesen; in Prod per CI/Container-Secret setzen.
* `.env` nur lokal; in CI/CD über Secret Store.

```js
// config.mjs
import 'dotenv/config'; // nur lokal/Dev
const { THIRD_PARTY_API_KEY } = process.env;
if (!THIRD_PARTY_API_KEY) throw new Error('THIRD_PARTY_API_KEY fehlt');
export default { THIRD_PARTY_API_KEY };
```

---

#### 3) **Server-seitiges Proxy-Muster (nie im Frontend exponieren)**

* Frontends bekommen **niemals** den Key; Backend ruft Drittanbieter-API auf.

```js
// routes/proxy.mjs
import express from "express";
import axios from "axios";
import cfg from "../config.mjs";

const router = express.Router();

router.get("/weather", async (req, res) => {
  const { city } = req.query;
  const r = await axios.get("https://api.example.com/weather", {
    params: { q: city },
    headers: { "X-API-Key": cfg.THIRD_PARTY_API_KEY }, // Key nur serverseitig
    timeout: 5000,
  });
  res.json(r.data);
});

export default router;
```

---

#### 4) **Secret-Manager verwenden (Prod)**

* Cloud-Optionen: **AWS Secrets Manager**, **GCP Secret Manager**, **Azure Key Vault**, **HashiCorp Vault**.
* Vorteile: Rotation, Audit, Zugriffskontrolle (IAM), verschlüsselte Speicherung.

---

#### 5) **Least Privilege & Rotation**

* Scope/Quotas so klein wie möglich (IP- oder Referrer-Bindung).
* **Kurzlebige Keys/Tokens** bevorzugen; regelmäßige Rotation automatisieren.

---

#### 6) **Transport & Speicherung**

* **Immer HTTPS** zu Dritt-APIs.
* Keine Logs mit Secrets; **Log-Redaction** aktivieren.
* In Containern: Secrets **nicht** ins Image backen; über **Docker/K8s Secrets** injizieren.

---

#### 7) **Validierung & Fail-Closed**

* Beim Start **Env-Validierung** (z. B. Zod/Joi); bei Fehlen **Crashen** statt unsicher weiterlaufen.

```js
// env-validate.mjs
import { z } from "zod";
const Env = z.object({ THIRD_PARTY_API_KEY: z.string().min(20) });
Env.parse(process.env);
```

---

#### 8) **Client-Schutz (wenn unvermeidlich)**

* Wenn ein Anbieter nur clientseitig ist (ungünstig): **eigenes Rate-Limit**, Anomaly Detection, Domain/Referer-Locks, aber: **Risiko bleibt hoch** → besser Proxy.

---

### **Zusammenfassung**

* **Nie hardcoden, nie ins Frontend**: Keys aus `process.env`, per **Secret-Manager** bereitstellen.
* **Proxy-Pattern**, **Least Privilege**, **Rotation**, **HTTPS**, **keine Logs mit Secrets**.
* **Container/CI**: Secrets zur Laufzeit injizieren, nicht ins Image/Repo.

**Quellen / Weiterführend**

* Node.js: [`process.env`](https://nodejs.org/docs/latest/api/process.html#processenv)
* Express: [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* MDN: [HTTPS & Security Overview](https://developer.mozilla.org/ru/docs/Web/HTTP/Overview)
* OWASP: [Secrets Management Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_Cheat_Sheet.html)


  **[⬆ Наверх](#top)**      

211. ### <a name="211"></a> Was ist der Unterschied zwischen Authentifizierung und Autorisierung?

### **Unterschied zwischen Authentifizierung und Autorisierung**

---

### **Authentifizierung (Authentication)**

* **Frage:** *Wer bist du?*
* **Ziel:** Identität des Benutzers feststellen.
* **Mittel:**

  * Benutzername + Passwort
  * Token (JWT, OAuth2 Access Token)
  * Zertifikate
  * Biometrie (Fingerabdruck, FaceID)

**Beispiel (Login-Flow)**

```js
// Prüfen, ob User existiert und Passwort korrekt ist
if (username === "max" && password === "secret123") {
  // Authentifizierung erfolgreich
}
```

---

### **Autorisierung (Authorization)**

* **Frage:** *Was darfst du tun?*
* **Ziel:** Zugriff auf Ressourcen und Aktionen kontrollieren.
* **Mittel:**

  * Rollen (RBAC – Role Based Access Control)
  * Rechte auf Ressourcen (z. B. nur Admin darf löschen)
  * Claims im JWT (`role: "admin"`)

**Beispiel (Routen-Absicherung in Express)**

```js
// Middleware für Autorisierung
function requireAdmin(req, res, next) {
  if (req.user?.role !== "admin") {
    return res.status(403).json({ error: "Access denied" });
  }
  next();
}

app.delete("/user/:id", requireAdmin, (req, res) => {
  res.json({ message: "User gelöscht" });
});
```

---

### **Direkter Vergleich**

| Aspekt    | **Authentifizierung**               | **Autorisierung**               |
| --------- | ----------------------------------- | ------------------------------- |
| Frage     | Wer bist du?                        | Was darfst du tun?              |
| Zeitpunkt | Immer zuerst (Login, Token-Prüfung) | Danach (Ressourcenzugriff)      |
| Mittel    | Passwörter, Tokens, Zertifikate     | Rollen, Rechte, Policies        |
| Ergebnis  | Identität bestätigt                 | Zugriff gewährt oder verweigert |

---

### **Zusammenfassung**

* **Authentifizierung** = Identität prüfen (*Login*).
* **Autorisierung** = Berechtigungen prüfen (*Rechte*).
* Reihenfolge: Erst **Authentifizierung**, dann **Autorisierung**.

🔗 Quellen:

* [MDN – Authentication](https://developer.mozilla.org/en-US/docs/Glossary/Authentication)
* [MDN – Authorization](https://developer.mozilla.org/en-US/docs/Glossary/Authorization)
* [OWASP – Authentication Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

---

  **[⬆ Наверх](#top)**      

212. ### <a name="212"></a> Welche Möglichkeiten gibt es, Authentifizierung in Express zu implementieren?

### **Optionen für Authentifizierung in Express**

---

#### 1) **Session-/Cookie-basiert (stateful)**

* Geeignet für klassische Web-Apps.
* Speicherung der Session serverseitig (Store/DB); Browser sendet Cookie.
* Schutz: `Secure`, `HttpOnly`, `SameSite`, CSRF-Token.

```js
// app.mjs
import express from "express";
import session from "express-session";
import passport from "passport";
import Local from "passport-local";
import bcrypt from "bcrypt";

const users = [{ id: 1, email: "a@b.c", passHash: await bcrypt.hash("secret", 12) }];

passport.use(new Local.Strategy(
  { usernameField: "email", passwordField: "password" },
  async (email, password, done) => {
    const u = users.find(x => x.email === email);
    if (!u || !(await bcrypt.compare(password, u.passHash))) return done(null, false);
    return done(null, { id: u.id, email: u.email });
  }
));
passport.serializeUser((u, done) => done(null, u.id));
passport.deserializeUser((id, done) => done(null, users.find(x => x.id === id)));

const app = express();
app.use(express.json());
app.use(session({
  secret: process.env.SESSION_SECRET,
  resave: false, saveUninitialized: false,
  cookie: { httpOnly: true, secure: true, sameSite: "lax" }
}));
app.use(passport.initialize());
app.use(passport.session());

app.post("/login", passport.authenticate("local"), (req, res) => res.json({ ok: true }));
app.get("/me", (req, res) => req.isAuthenticated() ? res.json(req.user) : res.sendStatus(401));

app.listen(3000);
```

---

#### 2) **Token-basiert/JWT (stateless)**

* Ideal für SPAs/Mobile/REST-APIs.
* Client sendet `Authorization: Bearer <jwt>`; Server prüft Signatur & `exp`.

```js
// auth.mjs
import jwt from "jsonwebtoken";
const SECRET = process.env.JWT_SECRET;

export const signToken = (user) => jwt.sign({ sub: user.id, role: user.role }, SECRET, { expiresIn: "1h" });

export const requireAuth = (req, res, next) => {
  const token = req.headers.authorization?.split(" ")[1];
  try { req.user = jwt.verify(token, SECRET); next(); }
  catch { return res.sendStatus(401); }
};

// usage:
// app.post("/login", (req,res)=> res.json({ token: signToken({ id:1, role:"user" }) }));
// app.get("/profile", requireAuth, (req,res)=> res.json({ id: req.user.sub }));
```

---

#### 3) **OAuth2/OpenID Connect (Delegation, „Login mit …“)**

* Nutzung externer Identity Provider (Google, GitHub, Auth0, Keycloak).
* Meist via Passport-Strategien; Ergebnis oft **Session** oder **JWT**.

```js
// oauth.mjs (Skizze)
import passport from "passport";
import { Strategy as GitHubStrategy } from "passport-github2";

passport.use(new GitHubStrategy({
  clientID: process.env.GH_ID, clientSecret: process.env.GH_SECRET,
  callbackURL: "https://app.example.com/auth/github/callback"
}, (_at, _rt, profile, done) => done(null, { id: profile.id, name: profile.username })));
```

---

#### 4) **API-Key / HMAC (Service-zu-Service)**

* Einfach für interne Services; Schlüssel gehört **nur** ins Backend/Secret-Store.

```js
// apiKey.mjs
export const requireApiKey = (req, res, next) =>
  req.get("X-API-Key") === process.env.INTERNAL_API_KEY ? next() : res.sendStatus(401);
```

---

#### 5) **Mutual TLS (mTLS)**

* Beidseitige Zertifikatsprüfung; stark für interne, sensitive Services (Ingress/Proxy).

---

#### 6) **Passkeys/WebAuthn (phishing-resistent)**

* Passwortlos (FIDO2); Integration z. B. via WebAuthn-Libraries; häufig mit Sessions kombiniert.

---

### **Best Practices (kurz)**

* **Passwörter hashen** (Argon2/Bcrypt), niemals im Klartext speichern.
* **HTTPS erzwingen**, Cookies `Secure`/`HttpOnly`/`SameSite`.
* **Rate Limiting**, Brute-Force-Schutz, MFA/2FA wo möglich.
* Bei **Cookies**: CSRF-Schutz (Tokens), bei **JWT**: kurze TTL + Refresh-Flow, Token-Invalidierung bei Logout/Leak.
* Secrets aus **ENV/Secret-Manager**, nicht hardcoden.

---

### **Zusammenfassung**

* Hauptpfade: **Session/Cookie** (stateful) vs. **JWT** (stateless); **OAuth2/OIDC** für Delegation; **API-Key/mTLS** für Services.
* Auswahl nach Use-Case (Browser-App vs. API/Mobile, Skalierung, Sicherheitsniveau).
* Immer: sichere Speicherung, HTTPS, Least Privilege, zusätzliche Schutzmechanismen (CSRF/Rate Limit/MFA).

**Quellen**

* [Express – Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* [Express – Middleware/Session](https://expressjs.com/en/resources/middleware/session.html)
* [Node.js Dokumentation – `crypto`](https://nodejs.org/docs/latest/api/crypto.html)
* [MDN – Authentication](https://developer.mozilla.org/en-US/docs/Glossary/Authentication)
* [Passport.js Dokumentation](http://www.passportjs.org/)
* [jsonwebtoken (GitHub)](https://github.com/auth0/node-jsonwebtoken)


  **[⬆ Наверх](#top)**      

213. ### <a name="213"></a> Unterschied zwischen Session-basiertem und Token-basiertem Login?

### **Unterschied zwischen Session-basiertem und Token-basiertem Login**

---

### **Session-basiert (stateful)**

* **Ablauf:**

  1. User loggt sich ein → Server erstellt **Session** (im Speicher oder DB).
  2. Client erhält **Session-ID** als Cookie.
  3. Bei jedem Request sendet Client Cookie → Server prüft Session.
* **Eigenschaften:**

  * Server muss **Session-Store** verwalten → **stateful**.
  * Gut für klassische Web-Apps.
  * Skalierung schwieriger (Sessions zwischen Servern teilen).

```js
// Express Beispiel
import session from "express-session";

app.use(session({
  secret: process.env.SESSION_SECRET,
  resave: false,
  saveUninitialized: false,
  cookie: { httpOnly: true, secure: true }
}));
```

---

### **Token-basiert (stateless, z. B. JWT)**

* **Ablauf:**

  1. User loggt sich ein → Server erstellt **JWT** (signiert).
  2. Client speichert Token (LocalStorage oder Cookie).
  3. Bei jedem Request sendet Client `Authorization: Bearer <jwt>`.
  4. Server prüft Signatur + Ablaufzeit → kein Session-Store nötig.
* **Eigenschaften:**

  * Server ist **stateless** → leicht skalierbar.
  * Ideal für **APIs, SPAs, Mobile Apps**.
  * Risiko: Token-Leak gewährt Zugriff bis Ablauf.

```js
// Express JWT Middleware
import jwt from "jsonwebtoken";

const requireAuth = (req, res, next) => {
  const token = req.headers.authorization?.split(" ")[1];
  try {
    req.user = jwt.verify(token, process.env.JWT_SECRET);
    next();
  } catch {
    res.sendStatus(401);
  }
};
```

---

### **Direkter Vergleich**

| Aspekt         | **Session-basiert**                        | **Token-basiert (JWT)**                  |
| -------------- | ------------------------------------------ | ---------------------------------------- |
| Speicherung    | Session-ID im Cookie                       | JWT im Header (oder Cookie)              |
| Server-Zustand | Stateful (Session-Store nötig)             | Stateless (nur Token-Validierung)        |
| Skalierbarkeit | Schwieriger (z. B. Redis-Store nötig)      | Einfach (jeder Server kann Token prüfen) |
| Sicherheit     | Session Hijacking möglich; Schutz mit CSRF | Token-Leak kritisch bis `exp`            |
| Einsatzgebiet  | Klassische Web-Apps                        | REST-APIs, SPAs, Mobile Apps             |

---

### **Zusammenfassung**

* **Session-Login**: Server speichert Sitzungen, gut für klassische Web-Apps, schwerer skalierbar.
* **Token-Login**: Server bleibt stateless, gut für APIs/Microservices, einfacher zu skalieren, erfordert gutes Token-Management.

🔗 Quellen

* [MDN – HTTP Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)
* [JWT.io Einführung](https://jwt.io/introduction)
* [Express – Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

214. ### <a name="214"></a> Wie funktioniert express-session und wann sollte man es nutzen?

### **Funktionsweise von `express-session`**

* `express-session` ist eine Middleware, die **Session-Management** in Express ermöglicht.
* Ablauf:

  1. Beim ersten Request legt der Server eine **Session-ID** an und speichert Session-Daten (standardmäßig im Speicher, besser Redis/Mongo/SQL).
  2. Diese Session-ID wird als **Cookie (`connect.sid`)** an den Client gesendet.
  3. Bei jedem weiteren Request sendet der Client das Cookie mit.
  4. Der Server findet anhand der ID die Session-Daten und weiß, welcher User dazugehört.

**Beispiel:**

```js
import express from "express";
import session from "express-session";

const app = express();

app.use(session({
  secret: process.env.SESSION_SECRET, // geheim halten
  resave: false, // keine unnötigen DB-Saves
  saveUninitialized: false, // nur bei echten Sessions speichern
  cookie: {
    httpOnly: true,   // schützt vor XSS
    secure: true,     // nur über HTTPS senden
    sameSite: "lax"   // CSRF-Schutz
  }
}));

app.get("/set", (req, res) => {
  req.session.user = { id: 1, name: "Max" }; // Daten in Session speichern
  res.send("Session gesetzt");
});

app.get("/get", (req, res) => {
  res.json(req.session.user || "Keine Session");
});

app.listen(3000);
```

---

### **Wann sollte man `express-session` nutzen?**

✅ **Geeignet für:**

* Klassische **Server-gerenderte Web-Apps** mit Formular-Login.
* Szenarien, in denen **Cookies** ohnehin genutzt werden.
* Kleinere bis mittlere Anwendungen ohne hohen Skalierungsbedarf.
* Wenn Sessions mit **Redis/Mongo** zentral gespeichert werden (skalierbar).

❌ **Weniger geeignet für:**

* **REST-APIs / SPAs / Mobile Apps** → dort sind stateless Tokens (z. B. JWT) üblicher.
* Anwendungen, die **horizontale Skalierung** ohne Shared Session Store brauchen.

---

### **Zusammenfassung**

* `express-session` speichert Sitzungsdaten serverseitig und identifiziert Clients über ein Cookie mit Session-ID.
* Nutzen: Einfach, sicher (mit HTTPS + sicheren Cookies), besonders für klassische Web-Apps.
* Für APIs und Microservices ist meist **JWT (stateless)** die bessere Wahl.

🔗 Quellen

* [Express – Session Middleware](https://expressjs.com/en/resources/middleware/session.html)
* [MDN – HTTP Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)

---

  **[⬆ Наверх](#top)**      

215. ### <a name="215"></a> Was ist der Unterschied zwischen Cookies und Tokens?

### **Unterschied zwischen Cookies und Tokens**

---

### **Cookies**

* **Definition:** Kleine Datenpakete, die der Server im Browser speichert und bei jedem Request automatisch mitsendet.
* **Eigenschaften:**

  * Werden per `Set-Cookie`-Header gesetzt.
  * Automatisch vom Browser an die gleiche Domain gesendet.
  * Können `HttpOnly`, `Secure`, `SameSite` Flags enthalten → Schutz vor XSS/CSRF.
  * Typisch für **Session-basierte Authentifizierung** (Cookie enthält Session-ID).

**Beispiel:**

```http
Set-Cookie: sessionId=abc123; HttpOnly; Secure; SameSite=Lax
```

👉 Browser hängt das Cookie automatisch an jeden Request zu `example.com` an.

---

### **Tokens (z. B. JWT)**

* **Definition:** Digitale Datenblöcke (meist JSON-basiert, signiert), die Informationen (Claims) enthalten.
* **Eigenschaften:**

  * Werden vom Client explizit gespeichert (z. B. LocalStorage, SessionStorage oder auch in Cookies).
  * Müssen manuell im Request mitgeschickt werden (z. B. Header `Authorization: Bearer <token>`).
  * Typisch für **stateless Authentifizierung** in REST-APIs und Microservices.

**Beispiel:**

```http
Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
```

---

### **Direkter Vergleich**

| Aspekt             | **Cookies**                              | **Tokens**                                |
| ------------------ | ---------------------------------------- | ----------------------------------------- |
| Speicherung        | Browser verwaltet automatisch            | Client entscheidet (LocalStorage, Header) |
| Übertragung        | Automatisch bei Requests zur Domain      | Manuell im Header/Body/Query              |
| Nutzung            | Session-ID, kleine Daten                 | JWTs mit Claims (User-ID, Rolle, Ablauf)  |
| Stateful/Stateless | Meist **stateful** (Session auf Server)  | **stateless** (Server prüft Signatur)     |
| Schutzmechanismen  | Flags (`HttpOnly`, `Secure`, `SameSite`) | Kurze TTL, Refresh Tokens, Signatur       |
| Einsatz            | Klassische Web-Apps                      | REST-APIs, SPAs, Mobile Apps              |

---

### **Zusammenfassung**

* **Cookies**: Browser-gesteuert, gut für Session-Management in klassischen Web-Apps.
* **Tokens**: Flexibel, stateless, besser für APIs und Microservices.
* Kombination möglich: Token kann **in einem Cookie** gespeichert werden (mit `HttpOnly` + `Secure`).

🔗 Quellen

* [MDN – Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)
* [JWT.io Einführung](https://jwt.io/introduction)
* [Express Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

216. ### <a name="216"></a> Was ist JWT (JSON Web Token) und wie funktioniert es?

### **JWT (JSON Web Token)**

---

### **Definition**

* **JWT** ist ein kompakter, URL-sicherer Token-Standard (RFC 7519).
* Dient zur **sicheren Übertragung von Claims** (z. B. User-ID, Rollen, Ablaufzeit).
* Typisch für **Authentifizierung und Autorisierung** in Web-Apps und APIs.

---

### **Aufbau**

Ein JWT besteht aus **drei Base64URL-kodierten Teilen**, durch `.` getrennt:

```
header.payload.signature
```

1. **Header** – enthält Metadaten (z. B. Algorithmus, Typ).

   ```json
   { "alg": "HS256", "typ": "JWT" }
   ```

2. **Payload** – enthält Claims (Infos über User/Rollen).

   ```json
   { "sub": "123456", "name": "Max", "role": "admin", "exp": 1694018400 }
   ```

3. **Signature** – Signatur über Header+Payload mit Secret/Private Key.

   ```js
   HMACSHA256(base64Url(header) + "." + base64Url(payload), secret)
   ```

---

### **Funktionsweise (Flow)**

1. **Login:** User meldet sich mit Credentials an.
2. **Token-Erstellung:** Server erstellt JWT, signiert ihn und gibt ihn zurück.
3. **Client-Speicherung:** Client speichert Token (z. B. LocalStorage, Cookie).
4. **Request:** Client sendet Token bei jedem Request im Header:

   ```
   Authorization: Bearer <jwt>
   ```
5. **Verifizierung:** Server prüft Signatur + Ablaufzeit (`exp`).
6. **Zugriff:** Falls gültig → Zugriff gewährt, sonst **401 Unauthorized**.

---

### **Beispiel in Node.js (Express + jsonwebtoken)**

```js
// auth.mjs
import jwt from "jsonwebtoken";

const SECRET = process.env.JWT_SECRET;

// Token erzeugen
export function createToken(user) {
  return jwt.sign({ sub: user.id, role: user.role }, SECRET, { expiresIn: "1h" });
}

// Middleware zur Verifikation
export function authMiddleware(req, res, next) {
  const token = req.headers.authorization?.split(" ")[1];
  if (!token) return res.sendStatus(401);

  try {
    req.user = jwt.verify(token, SECRET);
    next();
  } catch {
    res.sendStatus(403);
  }
}
```

---

### **Best Practices**

* **Kurze Lebensdauer** (`exp`) + Refresh Tokens.
* **HTTPS erzwingen** → Schutz vor Token-Leaks.
* **Secret/Private Key** sicher speichern (ENV, Secret Manager).
* **Rollen/Claims** nutzen (RBAC, ABAC).
* **Blacklist/Token-Invalidierung** bei Logout oder Sicherheitsvorfällen.

---

### **Zusammenfassung**

* **JWT = JSON-basiertes Token** mit Header, Payload, Signatur.
* Wird für **stateless Authentifizierung und Autorisierung** in APIs genutzt.
* Server prüft nur **Signatur & Ablauf**, kein Session-Store nötig.

🔗 Quellen

* [JWT.io – Einführung](https://jwt.io/introduction)
* [RFC 7519 – JSON Web Token](https://datatracker.ietf.org/doc/html/rfc7519)
* [Express Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

217. ### <a name="217"></a> Welche Vorteile und Nachteile hat JWT gegenüber Sessions?

### **JWT vs. Sessions – Vorteile & Nachteile**

---

### ✅ **Vorteile von JWT gegenüber Sessions**

1. **Stateless**

   * Server muss keine Sessions speichern → weniger Memory/DB-Last.
   * Ideal für **Microservices** und horizontale Skalierung (Load Balancing).

2. **Einfacher Cross-Domain-Einsatz**

   * Token kann in Header (`Authorization: Bearer ...`) gesendet werden → unabhängig von Cookies.
   * Praktisch für **Mobile Apps, SPAs, APIs**.

3. **Selbstenthaltend**

   * Token enthält Claims (z. B. `userId`, `role`) → Server braucht oft keine DB-Query für Basisinfos.

4. **Standardisiert & kompatibel**

   * JWT ist weit verbreitet (OAuth2, OpenID Connect).
   * Viele Bibliotheken verfügbar.

---

### ❌ **Nachteile von JWT gegenüber Sessions**

1. **Token-Invalidierung schwierig**

   * Ein ausgestelltes JWT bleibt gültig bis `exp`.
   * Kein zentraler „Kill-Switch“ (außer Blacklist/Revocation-Store).

2. **Größe & Overhead**

   * JWT ist größer als eine Session-ID, da Payload + Signatur enthalten sind.
   * Muss bei jedem Request mitgeschickt werden.

3. **Sicherheitsrisiko bei Leaks**

   * Wird ein Token gestohlen → nutzbar bis Ablaufzeit.
   * Erfordert **HTTPS, kurze TTL, Refresh-Tokens**.

4. **Komplexität**

   * Mehr Moving Parts: Signierung, Ablaufzeiten, Refresh-Mechanismen.
   * Bei falscher Konfiguration (z. B. kein `exp`) sehr riskant.

---

### **Direkter Vergleich**

| Aspekt         | **Sessions (Cookie-basiert)**       | **JWT (Token-basiert)**              |
| -------------- | ----------------------------------- | ------------------------------------ |
| Speicherung    | Session-ID serverseitig (DB/Memory) | Token im Client (Header, Storage)    |
| Server-Zustand | **Stateful**                        | **Stateless**                        |
| Skalierung     | Shared Store nötig (Redis, DB)      | Einfach, jeder Server prüft Signatur |
| Invalidierung  | Sofort möglich (Session löschen)    | Schwer (Blacklist/kurze TTL nötig)   |
| Größe          | Klein (nur ID)                      | Größer (Payload + Signatur)          |
| Sicherheit     | Schutz durch Cookies + CSRF-Token   | Schutz durch Signatur + HTTPS nötig  |
| Einsatz        | Klassische Web-Apps                 | APIs, SPAs, Mobile, Microservices    |

---

### **Zusammenfassung**

* **JWT**: Ideal für **stateless, verteilte Systeme** (APIs, Mobile, Microservices). Problematisch bei **Logout/Token-Invalidierung**.
* **Sessions**: Einfach und sicher invalidierbar, aber **stateful** → schwieriger bei Skalierung.

🔗 Quellen

* [JWT.io – Introduction](https://jwt.io/introduction)
* [Express – Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* [MDN – Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)

---

  **[⬆ Наверх](#top)**      

218. ### <a name="218"></a> Wie speichert man ein JWT sicher im Browser (LocalStorage vs. HttpOnly-Cookie)?

### **JWT sicher im Browser speichern: LocalStorage vs. HttpOnly-Cookie**

---

### **Kurzüberblick**

* **LocalStorage**

  * ✅ Wird **nicht automatisch** gesendet → **weniger CSRF-Risiko**
  * ❌ **Bei XSS leicht auslesbar** → Token-Diebstahl möglich
* **HttpOnly-Cookie**

  * ✅ **Nicht per JS auslesbar** → besser gegen **XSS-Exfiltration**
  * ❌ Wird **automatisch** gesendet → **CSRF-Schutz** zwingend (SameSite/CSRF-Token)

---

### **Empfohlene Praxis (modernes Setup)**

* **Access-Token**: **kurzlebig** (z. B. 5–10 min), **in-memory** im SPA halten und per `Authorization: Bearer` senden.
* **Refresh-Token**: **HttpOnly + Secure + SameSite**-Cookie (Server-Rotation).
* Zusätzlich: **CSP**, Eingabevalidierung, Framework-Sanitizing → XSS-Risiko minimieren.

---

### **Vergleich im Detail**

| Kriterium         | **LocalStorage**                               | **HttpOnly-Cookie**                                                        |
| ----------------- | ---------------------------------------------- | -------------------------------------------------------------------------- |
| Zugriff durch JS  | Ja → **XSS-Gefahr**                            | Nein → **Schutz vor Token-Exfiltration**                                   |
| CSRF-Risiko       | Gering (Header manuell gesetzt)                | Hoch ohne Maßnahmen (Cookie auto-send) → **SameSite**/**CSRF-Token** nötig |
| Handhabung in SPA | Einfach (Lesen/Schreiben)                      | Etwas komplexer (Server setzt/verifiziert; Pfad/Domain/SameSite beachten)  |
| Übertragung       | Per Header (`Authorization`)                   | Automatisch per Cookie (bei passender Domain/SameSite)                     |
| Persistenz        | Überlebt Reload (gut, aber auch bei Diebstahl) | Steuerbar über Cookie-Flags/TTL                                            |

---

### **Beispiel: Access in Memory + Refresh im HttpOnly-Cookie (Express)**

```js
// auth.routes.mjs
import express from "express";
import jwt from "jsonwebtoken";

const router = express.Router();
const { JWT_SECRET, REFRESH_SECRET } = process.env;

// Login: gibt Access-Token (Body) + Refresh-Token (HttpOnly-Cookie) zurück
router.post("/login", (req, res) => {
  const user = { id: 1, role: "user" }; // Beispiel
  const access = jwt.sign({ sub: user.id, role: user.role }, JWT_SECRET, { expiresIn: "10m" });
  const refresh = jwt.sign({ sub: user.id }, REFRESH_SECRET, { expiresIn: "7d" });

  res.cookie("rt", refresh, {
    httpOnly: true,
    secure: true,            // nur über HTTPS
    sameSite: "Lax",         // "None" falls Cross-Site nötig (dann zwingend Secure)
    path: "/auth/refresh",
    maxAge: 7 * 24 * 3600 * 1000
  });
  return res.json({ access }); // Access-Token im Body an SPA; SPA speichert in-memory
});

// Refresh-Endpoint: liest HttpOnly-Cookie, gibt neuen Access-Token aus
router.post("/refresh", (req, res) => {
  const token = req.cookies?.rt;
  if (!token) return res.sendStatus(401);
  try {
    const { sub } = jwt.verify(token, REFRESH_SECRET);
    const access = jwt.sign({ sub, role: "user" }, JWT_SECRET, { expiresIn: "10m" });
    return res.json({ access });
  } catch {
    return res.sendStatus(403);
  }
});

export default router;
```

Frontend sendet geschützte Requests mit **in-memory** Access-Token:

```js
// frontend (z. B. React): Request mit Bearer-Header
const res = await fetch("/api/profile", {
  headers: { Authorization: `Bearer ${accessToken}` }
});
```

---

### **CSRF-Schutz bei Cookies**

Wenn du **HttpOnly-Cookies** mit Sessions/Refresh nutzt:

* **SameSite=Lax/Strict** wo möglich, **SameSite=None; Secure** nur wenn Cross-Site nötig.
* **CSRF-Token** (Synchronizer/Double-Submit) für state-verändernde Requests:

```js
// Beispielprüfung eines CSRF-Headers
app.use((req, res, next) => {
  if (req.method !== "GET" && req.path.startsWith("/api")) {
    const token = req.get("X-CSRF-Token");
    if (token !== req.session?.csrfToken) return res.sendStatus(403);
  }
  next();
});
```

---

### **Wenn trotzdem LocalStorage genutzt wird**

* **Strikte CSP** (`script-src 'self'` + keine gefährlichen Inline-Skripte)
* **Framework-Sanitizing** (keine untrusted HTML-Injection)
* **Kurze TTL**, **Rotation**, **Logout** → Token sofort verwerfen
* **Kein** Eintrag in Logs/Analytics

---

### **Zusammenfassung**

* **Sicherster gängiger Kompromiss**: **Access-Token in-memory**, **Refresh-Token im HttpOnly-Cookie** (+ SameSite/HTTPS/CSRF-Token).
* **LocalStorage** ist bequem, aber **XSS-anfällig**; **HttpOnly-Cookies** schützen vor Exfiltration, benötigen jedoch **CSRF-Schutz**.
* Immer: **HTTPS**, **kurze TTL**, **Rotation**, **CSP** und robuste **Input-Validierung**.

**Quellen / Weiterführend**

* MDN: [Cookies & `Set-Cookie`](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies) • [SameSite](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers/Set-Cookie/SameSite) • [Web Storage API](https://developer.mozilla.org/ru/docs/Web/API/Web_Storage_API/Using_the_Web_Storage_API) • [CSRF](https://developer.mozilla.org/ru/docs/Glossary/CSRF)
* Express: [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* Node.js: [`http`/Cookies allgemein](https://nodejs.org/docs/latest/api/http.html)
* JWT: [JWT.io Introduction](https://jwt.io/introduction)


  **[⬆ Наверх](#top)**      

219. ### <a name="219"></a> Wie verhindert man JWT-Manipulation?

### **JWT-Manipulation verhindern – Best Practices**

---

### **Hauptangriffsflächen**

* **Signaturalgorithmus/„alg“-Verwirrung** (z. B. `none` oder HS256↔RS256-Tricks).
* **Gefälschte Header/Claims** (z. B. manipuliertes `kid`, falsches `iss`/`aud`).
* **Gestohlene/erratene Secrets**, schwache Schlüssel, fehlende Rotation.
* **Fehlende Prüfung von Ablauf/Zeiten** (`exp`, `nbf`, `iat`).

---

### **Schutzmaßnahmen (Checkliste)**

1. **Signatur prüfen & Algorithmus whitelisten**

   * Nur erlaubte Algos (z. B. `RS256` oder `HS256`) erlauben; **`none` strikt verbieten**.
2. **Starke Keys & Secret-Management**

   * Lange, zufällige Secrets (bei HS256) oder **asymmetrische Keys (RS256)**.
   * Secrets/Keys aus **ENV/Secret-Manager**, nie im Code/Repo.
3. **Claims validieren**

   * **`exp`** (Ablauf), **`nbf`**, **`iat`** (mit kleiner Clock-Skew), **`iss`** (Issuer), **`aud`** (Audience), ggf. **`jti`** (Nonce/Replay-Schutz).
4. **Key-Rotation & Revocation**

   * **Kid** nur gegen **bekannte Key-IDs** (Pinning) akzeptieren; bei RS256 **JWKS** nutzen.
   * Token-Invalidierung (Denylist) für kompromittierte/abgemeldete Tokens.
5. **Kein Vertrauen in Header**

   * Header-Infos (z. B. `alg`, `kid`, `typ`) **niemals blind** übernehmen; Server-Policy gilt.
6. **Kurze TTL + Refresh-Flow**

   * Kurze `exp`-Zeiten für Access-Tokens; Refresh-Tokens separat absichern (HttpOnly-Cookie).
7. **Transport-Sicherheit**

   * **Nur HTTPS**; keine Tokens in URLs/Logs.
8. **Audience-Trennung**

   * Unterschiedliche `aud` pro Service/Client, verhindert Token-Reuse zwischen Systemen.

---

### **Beispiel: Sichere Verifikation (HS256)**

```js
// verify.mjs
import jwt from "jsonwebtoken";

const SECRET = process.env.JWT_SECRET;

// Erlaubte Algos explizit whitelisten; Claims prüfen
export function verifyAccessToken(token) {
  return jwt.verify(token, SECRET, {
    algorithms: ["HS256"],      // keine "none" oder falsche Algos
    issuer: "https://auth.example.com",
    audience: "example.api",
    clockTolerance: 5           // Sekunden Toleranz für Uhrabweichung
  });
}
```

---

### **Beispiel: RS256 mit JWKS (Key-Rotation + kid-Pinning)**

```js
// jwks-verify.mjs
import jwt from "jsonwebtoken";
import jwksClient from "jwks-rsa";

const client = jwksClient({
  jwksUri: "https://auth.example.com/.well-known/jwks.json",
  cache: true,
  cacheMaxEntries: 5,
  cacheMaxAge: 10 * 60 * 1000
});

// Key anhand des 'kid' sicher auflösen (nur aus bekannter JWKS-Quelle!)
function getKey(header, cb) {
  if (!header.kid) return cb(new Error("Missing kid"));
  client.getSigningKey(header.kid, (err, key) => {
    if (err) return cb(err);
    cb(null, key.getPublicKey());
  });
}

export function verifyAccessTokenRS256(token) {
  return new Promise((resolve, reject) => {
    jwt.verify(token, getKey, {
      algorithms: ["RS256"],
      issuer: "https://auth.example.com",
      audience: "example.api",
      clockTolerance: 5
    }, (err, payload) => err ? reject(err) : resolve(payload));
  });
}
```

---

### **Express-Middleware (robuste Fehlerbehandlung)**

```js
// auth.middleware.mjs
import { verifyAccessTokenRS256 } from "./jwks-verify.mjs";

export async function requireAuth(req, res, next) {
  try {
    const token = req.headers.authorization?.split(" ")[1];
    if (!token) return res.status(401).json({ error: "No token" });

    // Verifikation inkl. Algo/iss/aud/exp/nbf
    req.user = await verifyAccessTokenRS256(token);
    return next();
  } catch (e) {
    return res.status(403).json({ error: "Invalid token" });
  }
}
```

---

### **Zusammenfassung**

* **Algorithmen whitelisten**, **Signatur/Claims strikt prüfen**, **Secrets/Keys sicher managen**.
* **RS256 + JWKS** vereinfacht Rotation und verhindert Algorithmen-Verwirrung.
* **Kurze TTL, HTTPS, keine Tokens in URL/Logs**, optional **Denylist** für Revocation.

**Quellen / Weiterführend**

* JWT: [RFC 7519](https://datatracker.ietf.org/doc/html/rfc7519) • [JWT.io Introduction](https://jwt.io/introduction)
* OWASP: [JWT Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/JSON_Web_Token_for_Java_Cheat_Sheet.html)
* Express: [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* Node.js: [`crypto` Grundlagen](https://nodejs.org/docs/latest/api/crypto.html)


  **[⬆ Наверх](#top)**      

220. ### <a name="220"></a> Was sind die Bestandteile eines JWT (Header, Payload, Signature)?

### **Bestandteile eines JWT (JSON Web Token)**

Ein JWT besteht aus **drei Base64URL-kodierten Teilen**, die durch Punkte (`.`) getrennt sind:

```
header.payload.signature
```

---

### **1) Header**

* Enthält **Metadaten** über das Token.
* Typischerweise:

  * `alg`: verwendeter Algorithmus (z. B. HS256, RS256)
  * `typ`: Typ des Tokens (meist `"JWT"`)

**Beispiel:**

```json
{
  "alg": "HS256",
  "typ": "JWT"
}
```

Nach Base64URL-Kodierung:

```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9
```

---

### **2) Payload**

* Enthält die **Claims** (Informationen).
* Drei Arten von Claims:

  * **Registered Claims** (standardisierte): `sub` (Subject/User-ID), `iss` (Issuer), `aud` (Audience), `exp` (Expiry), `iat` (Issued At)
  * **Public Claims**: frei definierbar, sollten kollisionsfrei sein
  * **Private Claims**: nur zwischen Kommunikationspartnern vereinbart

**Beispiel:**

```json
{
  "sub": "1234567890",
  "name": "Max Mustermann",
  "role": "admin",
  "iat": 1516239022,
  "exp": 1516242622
}
```

Nach Base64URL-Kodierung:

```
eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6Ik1heCBNdXN0ZXJtYW5uIiwicm9sZSI6ImFkbWluIiwiaWF0IjoxNTE2MjM5MDIyfQ
```

---

### **3) Signature**

* Sichert die **Integrität und Authentizität** des Tokens.
* Berechnung:

  ```
  HMACSHA256(
    base64UrlEncode(header) + "." + base64UrlEncode(payload),
    secret
  )
  ```
* Bei asymmetrischen Verfahren (`RS256`/`ES256`) wird die Signatur mit dem **Private Key** erstellt und mit dem **Public Key** geprüft.

**Beispiel (HS256, geheim = „mysecret“):**

```
SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c
```

---

### **Komplettes JWT (Header.Payload.Signature)**

```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.
eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6Ik1heCBNdXN0ZXJtYW5uIiwicm9sZSI6ImFkbWluIiwiaWF0IjoxNTE2MjM5MDIyfQ.
SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c
```

---

### **Zusammenfassung**

* **Header**: Metadaten (Algorithmus, Typ).
* **Payload**: Claims (User-Daten, Rollen, Zeitangaben).
* **Signature**: Prüft Integrität und Authentizität.
* Nur Header + Payload sind kodiert, aber **nicht verschlüsselt** → sensible Daten nie im Klartext speichern.

🔗 Quellen

* [RFC 7519 – JSON Web Token](https://datatracker.ietf.org/doc/html/rfc7519)
* [JWT.io – Debugger](https://jwt.io/)

---

  **[⬆ Наверх](#top)**      

221. ### <a name="221"></a> Wie setzt man Token-Expiration (Refresh Token vs. Access Token)?

### **Token-Expiration: Access Token vs. Refresh Token**

---

### **Access Token**

* **Zweck:** Direkt für API-Zugriffe verwenden.
* **Lebensdauer:** **sehr kurz** (z. B. 5–15 Minuten).
* **Warum kurz:**

  * Minimiert Risiko bei Token-Leak.
  * Kein Blacklist-Handling nötig, da ablaufende Tokens automatisch unbrauchbar werden.

**Beispiel (JWT-Erstellung mit Ablauf):**

```js
import jwt from "jsonwebtoken";

const accessToken = jwt.sign(
  { sub: user.id, role: user.role },
  process.env.JWT_SECRET,
  { expiresIn: "15m" }
);
```

---

### **Refresh Token**

* **Zweck:** Dient dazu, **neue Access Tokens** zu bekommen.
* **Lebensdauer:** **länger** (z. B. Tage bis Wochen, oft 7–30 Tage).
* **Aufbewahrung:** Sicher speichern → **HttpOnly, Secure, SameSite-Cookie** oder Server-seitiger Token-Store.
* **Sicherheitsmaßnahmen:**

  * Refresh Token Rotation: bei jedem Refresh ein neues ausstellen, altes invalidieren.
  * Blacklist/Denylist für kompromittierte Tokens.

**Beispiel (Refresh-Endpoint in Express):**

```js
import jwt from "jsonwebtoken";
import express from "express";
const router = express.Router();

router.post("/refresh", (req, res) => {
  const refreshToken = req.cookies?.refreshToken;
  if (!refreshToken) return res.sendStatus(401);

  try {
    const payload = jwt.verify(refreshToken, process.env.REFRESH_SECRET);
    const newAccess = jwt.sign(
      { sub: payload.sub, role: payload.role },
      process.env.JWT_SECRET,
      { expiresIn: "15m" }
    );
    return res.json({ accessToken: newAccess });
  } catch {
    return res.sendStatus(403);
  }
});
```

---

### **Best Practices**

* **Access Token kurzlebig** → reduziert Schaden bei Diebstahl.
* **Refresh Token langlebig, aber sicher speichern** (HttpOnly-Cookie).
* **Rotation & Blacklist** nutzen, um kompromittierte Tokens zu sperren.
* **Immer HTTPS** nutzen, Tokens nie in URLs oder Logs speichern.

---

### **Zusammenfassung**

* **Access Token:** Kurzlebig (Minuten), für direkte API-Zugriffe.
* **Refresh Token:** Länger lebig (Tage/Wochen), für Erneuerung von Access Tokens.
* Kombination = **sicheres, skalierbares Auth-System** für REST-APIs.

🔗 Quellen

* [JWT.io – Introduction](https://jwt.io/introduction)
* [OWASP – Token Best Practices](https://cheatsheetseries.owasp.org/cheatsheets/JSON_Web_Token_Cheat_Sheet_for_Java.html)
* [Express Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

222. ### <a name="222"></a> Wie implementiert man Refresh Tokens in einer Express-App?

### **Refresh Tokens in einer Express-App – Umsetzung (mit Rotation & Revoke)**

---

#### **Ziele**

* **Kurzlebiges Access-Token** (z. B. 10 min) für API-Zugriffe.
* **Langlebiges Refresh-Token** (z. B. 7–30 Tage) nur zum Erneuern.
* **HttpOnly-Cookie** für Refresh-Token, **Rotation** bei jedem Refresh, **Revoke** (Blacklist/Store).

---

## 1) **Token-Utilities (ESM)**

```js
// src/tokens.mjs
import crypto from "node:crypto";
import jwt from "jsonwebtoken";

const {
  JWT_SECRET,            // z. B. 256-bit random
  REFRESH_SECRET         // separater Secret/Key
} = process.env;

export const createAccessToken = (sub, role) =>
  jwt.sign({ sub, role }, JWT_SECRET, { expiresIn: "10m", issuer: "https://auth.example.com", audience: "example.api" });

export const createRefreshToken = (sub, jti) =>
  jwt.sign({ sub, jti }, REFRESH_SECRET, { expiresIn: "7d", issuer: "https://auth.example.com", audience: "example.api" });

export const verifyAccess = (token) =>
  jwt.verify(token, JWT_SECRET, { algorithms: ["HS256"], issuer: "https://auth.example.com", audience: "example.api" });

export const verifyRefresh = (token) =>
  jwt.verify(token, REFRESH_SECRET, { algorithms: ["HS256"], issuer: "https://auth.example.com", audience: "example.api" });

// stabile, irreversible Speicherung des Refresh-Tokens (Hash)
export const sha256 = (s) => crypto.createHash("sha256").update(s).digest("hex");

// zufällige jti (Token-ID) generieren
export const newJti = () => crypto.randomUUID();
```

---

## 2) **Refresh-Store (z. B. Redis)**

> In Produktion **Redis** o. ä. verwenden; hier ein In-Memory-Fallback.

```js
// src/refreshStore.mjs
// Struktur: key = sha256(refreshToken), value = { sub, jti, expMs }
const store = new Map();

export async function saveRefresh(hash, { sub, jti, expMs }) {
  store.set(hash, { sub, jti, expMs });
}
export async function findRefresh(hash) {
  const v = store.get(hash);
  if (!v) return null;
  if (Date.now() > v.expMs) { store.delete(hash); return null; }
  return v;
}
export async function revokeRefresh(hash) { store.delete(hash); }
export async function rotateRefresh(oldHash, newHash, payload) {
  store.delete(oldHash);
  store.set(newHash, payload);
}
```

---

## 3) **Auth-Middleware (Access-Token prüfen)**

```js
// src/requireAuth.mjs
import { verifyAccess } from "./tokens.mjs";

export function requireAuth(req, res, next) {
  const raw = req.headers.authorization;
  const token = raw?.startsWith("Bearer ") ? raw.slice(7) : null;
  if (!token) return res.status(401).json({ error: "No access token" });
  try {
    req.user = verifyAccess(token); // { sub, role, iat, exp, ... }
    next();
  } catch {
    res.status(403).json({ error: "Invalid/expired access token" });
  }
}
```

---

## 4) **Routes: Login, Refresh (Rotation), Logout**

```js
// src/auth.routes.mjs
import express from "express";
import jwt from "jsonwebtoken";
import { createAccessToken, createRefreshToken, verifyRefresh, newJti, sha256 } from "./tokens.mjs";
import { saveRefresh, findRefresh, revokeRefresh, rotateRefresh } from "./refreshStore.mjs";

export const authRouter = express.Router();

// Demo: "User prüfen" (ersetze durch echte DB/Passwortprüfung)
async function authenticate(email, password) {
  if (email === "user@example.com" && password === "secret123") return { id: "u1", role: "user" };
  return null;
}

function setRefreshCookie(res, token, maxAgeMs) {
  res.cookie("rt", token, {
    httpOnly: true,
    secure: true,          // Produktion: nur HTTPS
    sameSite: "Lax",       // "None" wenn Cross-Site SPA → dann secure: true zwingend
    path: "/auth/refresh", // Cookie nur an Refresh-Route senden
    maxAge: maxAgeMs
  });
}

// 1) Login: Access + Refresh ausstellen
authRouter.post("/login", async (req, res) => {
  const { email, password } = req.body ?? {};
  const user = await authenticate(email, password);
  if (!user) return res.status(401).json({ error: "Invalid credentials" });

  const jti = newJti();
  const access = createAccessToken(user.id, user.role);
  const refresh = createRefreshToken(user.id, jti);

  // Refresh-Token sicher (gehasht) speichern
  const decoded = jwt.decode(refresh);                // nur um exp zu lesen
  const expMs = decoded.exp * 1000;
  await saveRefresh(sha256(refresh), { sub: user.id, jti, expMs });

  setRefreshCookie(res, refresh, expMs - Date.now());
  res.json({ access }); // Access-Token geht an Client (idealerweise in-memory halten)
});

// 2) Refresh: prüfen, rotieren, neues Access + neues Refresh
authRouter.post("/refresh", async (req, res) => {
  const cookie = req.cookies?.rt;
  if (!cookie) return res.status(401).json({ error: "No refresh cookie" });

  try {
    const payload = verifyRefresh(cookie); // { sub, jti, iat, exp }
    const stored = await findRefresh(sha256(cookie));
    if (!stored || stored.sub !== payload.sub || stored.jti !== payload.jti) {
      return res.status(403).json({ error: "Refresh invalid" });
    }

    // Rotation: altes invalidieren, neues ausstellen
    const newJ = newJti();
    const newAccess = createAccessToken(payload.sub, /* role optional */ "user");
    const newRefresh = createRefreshToken(payload.sub, newJ);
    const newDecoded = jwt.decode(newRefresh);
    const newExpMs = newDecoded.exp * 1000;

    await rotateRefresh(sha256(cookie), sha256(newRefresh), { sub: payload.sub, jti: newJ, expMs: newExpMs });

    setRefreshCookie(res, newRefresh, newExpMs - Date.now());
    return res.json({ access: newAccess });
  } catch {
    return res.status(403).json({ error: "Refresh invalid/expired" });
  }
});

// 3) Logout: Refresh widerrufen + Cookie löschen
authRouter.post("/logout", async (req, res) => {
  const cookie = req.cookies?.rt;
  if (cookie) await revokeRefresh(sha256(cookie));
  res.clearCookie("rt", { path: "/auth/refresh" });
  res.sendStatus(204);
});
```

---

## 5) **Server-Setup (CORS, Cookies, Security)**

```js
// src/server.mjs
import "dotenv/config";
import express from "express";
import cookieParser from "cookie-parser";
import cors from "cors";
import helmet from "helmet";
import { authRouter } from "./auth.routes.mjs";
import { requireAuth } from "./requireAuth.mjs";

const app = express();
app.use(helmet());               // Security-Header
app.use(express.json());
app.use(cookieParser());

// CORS: nur erlaubte Origins, Credentials falls Cookie genutzt
app.use(cors({
  origin: ["https://app.example.com", "http://localhost:5173"],
  credentials: true
}));

app.use("/auth", authRouter);

// geschützte Beispielroute
app.get("/api/me", requireAuth, (req, res) => {
  res.json({ sub: req.user.sub });
});

app.listen(3000, () => console.log("API on :3000"));
```

---

## **Wichtige Hinweise**

* **Rotation**: Bei jedem `/refresh` neues Refresh-Token + altes sofort widerrufen (Schutz gegen Replay).
* **Speicherung**: Refresh-Token **gehasht** im Store ablegen; bei Leak einer DB sind Tokens nicht direkt nutzbar.
* **TTL**: Access kurz (5–15 min), Refresh länger (7–30 Tage).
* **HTTPS Pflicht**, Cookies: `HttpOnly`, `Secure`, `SameSite`.
* **CORS + Cookies**: Bei Cross-Site **`SameSite=None; Secure`** und `credentials: true` + Whitelist-Origin.
* **Revocation**: Bei Logout/Leak Refresh widerrufen (Store-Eintrag löschen).
* **Algorithmen whitelisten** und Claims prüfen (`iss`, `aud`, `exp`, `nbf`).

---

### **Zusammenfassung**

* **Login**: Access (kurz) + Refresh (lang) ausstellen; Refresh im **HttpOnly-Cookie**.
* **Refresh-Flow**: Refresh verifizieren → **rotieren** → neues Access & Refresh → altes widerrufen.
* **Sicherheit**: **HTTPS**, Cookie-Flags, **gehashter Refresh-Store**, Claim-Validierung, CORS-Whitelist.

**Quellen / Weiterführend**

* Node.js: [`http`/Sicherheit](https://nodejs.org/docs/latest/api/http.html) • [`crypto`](https://nodejs.org/docs/latest/api/crypto.html)
* Express: [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html) • [CORS Middleware](https://expressjs.com/de/resources/middleware/cors.html)
* MDN: [HTTP Cookies & SameSite](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)
* JWT: [RFC 7519](https://datatracker.ietf.org/doc/html/rfc7519) • [JWT.io Introduction](https://jwt.io/introduction)
* OWASP: [JWT Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/JSON_Web_Token_for_Java.html)


  **[⬆ Наверх](#top)**      

223. ### <a name="223"></a> Was ist OAuth2 und wie unterscheidet es sich von JWT?

### **OAuth2 vs. JWT**

---

### **OAuth2 (Open Authorization 2.0)**

* **Definition:** Framework (RFC 6749) für **delegierte Autorisierung**.
* **Zweck:** Ein Client (z. B. eine App) darf im Namen eines Users auf Ressourcen bei einem Resource-Server zugreifen.
* **Komponenten:**

  * **Resource Owner** (der User)
  * **Client** (z. B. App)
  * **Authorization Server** (stellt Tokens aus)
  * **Resource Server** (stellt geschützte Daten bereit)
* **Flows:** Authorization Code, Client Credentials, Device Code, Implicit (deprecated).
* **Ergebnis:** Ausgabe eines **Access Tokens** (manchmal auch Refresh Tokens).
* **Token-Format:** Kann **JWT sein, muss aber nicht** (kann auch ein undurchsichtiger String sein).

**Beispiel: "Login mit Google"** → App bekommt ein Access Token von Google, um im Namen des Users auf Gmail oder Google Drive zuzugreifen.

---

### **JWT (JSON Web Token)**

* **Definition:** Standard (RFC 7519) für ein **Token-Format**.
* **Zweck:** Claims (z. B. User-ID, Rollen, Ablaufzeit) kompakt und sicher übertragen.
* **Aufbau:** `header.payload.signature`
* **Nutzung:**

  * Authentifizierung/Autorisierung in APIs
  * Als Access Token in OAuth2 oder alleinstehend
* **Eigenschaften:**

  * Selbstenthaltend (enthält Claims direkt)
  * Signiert (Integritätssicherung)
  * Gültig bis Ablaufzeit (`exp`)

---

### **Direkter Vergleich**

| Aspekt       | **OAuth2**                                               | **JWT**                                     |
| ------------ | -------------------------------------------------------- | ------------------------------------------- |
| Typ          | Framework für **Autorisierung**                          | Token-Format (Standard)                     |
| Zweck        | Zugriffskontrolle für Drittanbieter im Namen eines Users | Transport von Claims (User-Daten, Rollen)   |
| Enthält      | Regeln, Rollen, Flows, Scopes                            | Header, Payload, Signatur                   |
| Ergebnis     | Access Token (kann JWT sein oder nicht)                  | Ein spezielles Format für Tokens            |
| Nutzung      | „Login mit …“, API-Zugriff, Delegation                   | API-Login, stateless Auth, OAuth2-Tokens    |
| Abhängigkeit | Nutzt ggf. JWT als Access/ID-Token                       | Kann unabhängig von OAuth2 verwendet werden |

---

### **Zusammenfassung**

* **OAuth2** = **Autorisierungs-Framework**: beschreibt, *wie* ein Client Zugriff erhält.
* **JWT** = **Token-Format**: beschreibt, *wie* ein Token aufgebaut ist.
* Verhältnis: OAuth2 **kann JWT als Token-Format verwenden**, aber nicht zwingend.

🔗 Quellen

* [RFC 6749 – OAuth 2.0](https://datatracker.ietf.org/doc/html/rfc6749)
* [RFC 7519 – JSON Web Token (JWT)](https://datatracker.ietf.org/doc/html/rfc7519)
* [MDN – OAuth](https://developer.mozilla.org/en-US/docs/Glossary/OAuth)
* [JWT.io – Introduction](https://jwt.io/introduction)

---

  **[⬆ Наверх](#top)**      

224. ### <a name="224"></a> Unterschied zwischen OAuth2 und OpenID Connect?

### **Unterschied zwischen OAuth2 und OpenID Connect (OIDC)**

---

### **OAuth2 (RFC 6749)**

* **Definition:** Autorisierungs-Framework.
* **Zweck:** Ein Client (z. B. App) erhält **Zugriff auf Ressourcen** im Namen des Users.
* **Fokus:** **Autorisierung** (Was darf der Client tun?).
* **Ergebnis:** Access Token (Format kann JWT sein, muss aber nicht).
* **Beispiel:** Eine App erhält Zugriff auf die Google Drive Dateien eines Users.

---

### **OpenID Connect (OIDC, auf OAuth2 aufgebaut)**

* **Definition:** Identity Layer **on top of OAuth2** (Spezifikation von OpenID Foundation).
* **Zweck:** Liefert **Authentifizierung** – also: *Wer ist der User?*
* **Fokus:** **Identität + Login**.
* **Erweiterungen gegenüber OAuth2:**

  * **ID Token** (immer JWT-Format), enthält User-Identität (`sub`, `email`, `name` etc.).
  * **UserInfo Endpoint**: API, um zusätzliche Profildaten abzufragen.
  * **Standardisierte Scopes:** `openid`, `profile`, `email`.
* **Beispiel:** „Login mit Google“ (OIDC): App bekommt ID Token → bestätigt die Identität des Users.

---

### **Direkter Vergleich**

| Aspekt          | **OAuth2**                   | **OpenID Connect (OIDC)**                     |
| --------------- | ---------------------------- | --------------------------------------------- |
| Typ             | Autorisierungs-Framework     | Identitätsschicht über OAuth2                 |
| Fokus           | Zugriff auf Ressourcen       | Authentifizierung (User-Identität)            |
| Token           | Access Token (kann JWT sein) | ID Token (immer JWT) + Access Token           |
| Standard-Scopes | Keine festgelegt             | `openid`, `profile`, `email`, …               |
| User-Info       | Nicht spezifiziert           | Standardisierter **UserInfo Endpoint**        |
| Ergebnis        | „Was darf die App tun?“      | „Wer ist der User?“ + Zugriff (falls gewollt) |

---

### **Zusammenfassung**

* **OAuth2**: Autorisierung – Zugriff auf Ressourcen im Namen des Users.
* **OIDC**: Erweiterung von OAuth2 für **Authentifizierung und Identität**.
* Verhältnis: OIDC **nutzt OAuth2**, liefert aber zusätzlich **ID Tokens und UserInfo**.

🔗 Quellen

* [OAuth 2.0 (RFC 6749)](https://datatracker.ietf.org/doc/html/rfc6749)
* [OpenID Connect Core Spec](https://openid.net/specs/openid-connect-core-1_0.html)
* [MDN – OAuth](https://developer.mozilla.org/en-US/docs/Glossary/OAuth)

---

  **[⬆ Наверх](#top)**      

225. ### <a name="225"></a> Wie integriert man Social Logins (Google, Facebook, GitHub) in Express?

### **Social Logins (Google, GitHub, Facebook) in Express**

---

## **Ansatz**

* Verwende **OAuth 2.0 / OpenID Connect** mit **Passport**-Strategien.
* Ablauf: **/auth/provider → Consent → /auth/provider/callback → Session oder JWT ausstellen**.

---

## **Setup (gemeinsam)**

```bash
npm i express passport express-session jsonwebtoken
npm i passport-google-oauth20 passport-github2 passport-facebook
```

```js
// src/app.mjs
import express from "express";
import session from "express-session";
import passport from "passport";

const app = express();
app.use(session({
  secret: process.env.SESSION_SECRET,
  resave: false, saveUninitialized: false,
  cookie: { httpOnly: true, secure: true, sameSite: "lax" }
}));
app.use(passport.initialize());
app.use(passport.session());

// Minimal: User ins/aus der Session
passport.serializeUser((user, done) => done(null, user));
passport.deserializeUser((obj, done) => done(null, obj));

app.get("/me", (req, res) => req.user ? res.json(req.user) : res.sendStatus(401));
export default app;
```

---

## **Google Login (OIDC, „passport-google-oauth20“)**

```js
// src/auth.google.mjs
import passport from "passport";
import { Strategy as GoogleStrategy } from "passport-google-oauth20";
import jwt from "jsonwebtoken";

passport.use(new GoogleStrategy({
  clientID: process.env.GOOGLE_CLIENT_ID,
  clientSecret: process.env.GOOGLE_CLIENT_SECRET,
  callbackURL: "https://your.app/auth/google/callback" // in Google Console whitelisten
}, async (_at, _rt, profile, done) => {
  // Hier: User in DB finden/erstellen
  const user = { id: profile.id, name: profile.displayName, provider: "google" };
  return done(null, user);
}));

export function googleRoutes(app) {
  app.get("/auth/google",
    passport.authenticate("google", { scope: ["openid", "profile", "email"], prompt: "select_account" })
  );

  app.get("/auth/google/callback",
    passport.authenticate("google", { failureRedirect: "/login" }),
    (req, res) => {
      // Optional: Statt Session ein JWT ausstellen
      const token = jwt.sign({ sub: req.user.id }, process.env.JWT_SECRET, { expiresIn: "1h" });
      res.cookie("access", token, { httpOnly: true, secure: true, sameSite: "Lax" });
      res.redirect("/"); // oder SPA-Callback
    }
  );
}
```

---

## **GitHub Login („passport-github2“)**

```js
// src/auth.github.mjs
import passport from "passport";
import { Strategy as GitHubStrategy } from "passport-github2";

passport.use(new GitHubStrategy({
  clientID: process.env.GH_CLIENT_ID,
  clientSecret: process.env.GH_CLIENT_SECRET,
  callbackURL: "https://your.app/auth/github/callback"
}, async (_at, _rt, profile, done) => {
  const user = { id: profile.id, name: profile.username, provider: "github" };
  return done(null, user);
}));

export function githubRoutes(app) {
  app.get("/auth/github",
    passport.authenticate("github", { scope: ["user:email"] })
  );
  app.get("/auth/github/callback",
    passport.authenticate("github", { failureRedirect: "/login" }),
    (_req, res) => res.redirect("/")
  );
}
```

---

## **Facebook Login („passport-facebook“)**

```js
// src/auth.facebook.mjs
import passport from "passport";
import { Strategy as FacebookStrategy } from "passport-facebook";

passport.use(new FacebookStrategy({
  clientID: process.env.FB_APP_ID,
  clientSecret: process.env.FB_APP_SECRET,
  callbackURL: "https://your.app/auth/facebook/callback",
  profileFields: ["id", "displayName", "emails"]
}, async (_at, _rt, profile, done) => {
  const user = { id: profile.id, name: profile.displayName, provider: "facebook" };
  return done(null, user);
}));

export function facebookRoutes(app) {
  app.get("/auth/facebook", passport.authenticate("facebook", { scope: ["email"] }));
  app.get("/auth/facebook/callback",
    passport.authenticate("facebook", { failureRedirect: "/login" }),
    (_req, res) => res.redirect("/")
  );
}
```

---

## **Server start + Routen zusammenführen**

```js
// src/server.mjs
import app from "./app.mjs";
import { googleRoutes } from "./auth.google.mjs";
import { githubRoutes } from "./auth.github.mjs";
import { facebookRoutes } from "./auth.facebook.mjs";

googleRoutes(app);
githubRoutes(app);
facebookRoutes(app);

app.listen(3000, () => console.log("Auth-Server auf :3000"));
```

---

## **Best Practices**

* **HTTPS erzwingen**, Callback-URLs exakt in Provider-Konsolen konfigurieren.
* **State/CSRF-Schutz**: Passport setzt per Default `state` in manchen Strategien — bei SPAs zusätzlich CSRF bedenken.
* **Scopes minimal** halten (Least Privilege).
* **Sessions vs. JWT**: Für SPAs oft **JWT** (kurze TTL) + **Refresh-Flow**; für SSR klassisch **Session**.
* **CORS**: Bei Cross-Site-Szenarien korrekte `origin`-Whitelist + `credentials`.
* **Datenschutz**: Nur benötigte Profildaten speichern; Benutzer zustimmen lassen.

---

### **Zusammenfassung**

* Social Logins in Express via **Passport**-Strategien (Google OIDC, GitHub, Facebook).
* **/auth/{provider} → Callback → Session oder JWT**.
* Achte auf **HTTPS, korrekte Callback-URLs, Scopes, CSRF/state** und entscheide **Session vs. JWT** je nach Architektur.

**Quellen / Weiterführend**

* Express: [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* Passport: [passportjs.org](http://www.passportjs.org/) • [Google OAuth 2.0](http://www.passportjs.org/packages/passport-google-oauth20/) • [GitHub](http://www.passportjs.org/packages/passport-github2/) • [Facebook](http://www.passportjs.org/packages/passport-facebook/)
* MDN: [OAuth – Überblick](https://developer.mozilla.org/en-US/docs/Glossary/OAuth)
* Node.js: [`crypto` / Sicherheit](https://nodejs.org/docs/latest/api/crypto.html)


  **[⬆ Наверх](#top)**      

226. ### <a name="226"></a> Wie implementiert man eine Middleware zum Schutz von privaten Routen?

### **Middleware zum Schutz privater Routen (Express)**

---

#### **JWT-basierter Schutz (stateless APIs)**

```js
// middleware/authJwt.mjs
import jwt from "jsonwebtoken";

const { JWT_SECRET } = process.env;

// Authentifizierung: prüft Bearer-Token, setzt req.user
export function requireAuth(req, res, next) {
  const token = req.headers.authorization?.startsWith("Bearer ")
    ? req.headers.authorization.slice(7)
    : null;

  if (!token) return res.status(401).json({ error: "No token" });

  try {
    // Algorithmus/Issuer/Audience in Prod whitelisten
    req.user = jwt.verify(token, JWT_SECRET /*, { algorithms: ["HS256"], issuer: "...", audience: "..." } */);
    next();
  } catch {
    return res.status(403).json({ error: "Invalid or expired token" });
  }
}

// Autorisierung: nur bestimmte Rollen zulassen
export const requireRole = (...roles) => (req, res, next) => {
  if (!req.user) return res.status(401).json({ error: "Not authenticated" });
  return roles.includes(req.user.role)
    ? next()
    : res.status(403).json({ error: "Forbidden" });
};
```

```js
// routes.mjs
import express from "express";
import { requireAuth, requireRole } from "./middleware/authJwt.mjs";

const router = express.Router();

// privat (alle eingeloggten Nutzer)
router.get("/me", requireAuth, (req, res) => res.json({ sub: req.user.sub, role: req.user.role }));

// nur Admins
router.delete("/users/:id", requireAuth, requireRole("admin"), (req, res) => {
  // ... löschen
  res.sendStatus(204);
});

export default router;
```

**Hinweise**

* **401**: nicht authentifiziert; **403**: authentifiziert, aber **keine** Berechtigung.
* Für Refresh-Flow: Access-Token kurzlebig halten; Refresh separat (z. B. Cookie).

---

#### **Session-/Cookie-basierter Schutz (stateful Web-Apps)**

```js
// middleware/authSession.mjs
export function requireSession(req, res, next) {
  // gesetzt durch express-session + ggf. passport
  if (req.isAuthenticated?.() || req.session?.user) return next();
  return res.status(401).json({ error: "Login required" });
}

export const requireSessionRole = (...roles) => (req, res, next) => {
  const role = req.user?.role || req.session?.user?.role;
  return role && roles.includes(role) ? next() : res.status(403).json({ error: "Forbidden" });
};
```

---

#### **Robuste Fehlerbehandlung und Reihenfolge**

```js
// app.mjs
import express from "express";
import routes from "./routes.mjs";

const app = express();
app.use(express.json());

// öffentliche Routen zuerst …
app.get("/public/health", (_req, res) => res.json({ ok: true }));

// … dann geschützte Routen
app.use("/api", routes);

// zentrales Error-Handling (letzter Middleware-Layer)
app.use((err, _req, res, _next) => {
  console.error(err);
  res.status(500).json({ error: "Internal Server Error" });
});

export default app;
```

---

#### **Optionale Härtung**

* **Rate Limiting** auf private Routen.
* **CORS** restriktiv konfigurieren.
* **Helmet** für Sicherheits-Header.
* **Input-Validierung** vor der Business-Logik.

---

### **Zusammenfassung**

* Middleware trennt **Authentifizierung** (Identität prüfen) von **Autorisierung** (Rechte prüfen).
* Für **APIs**: JWT-Middleware (`Authorization: Bearer`) + rollenbasierte Checks.
* Für **SSR/Web-Apps**: Session-Middleware (`express-session`/`passport`).
* Richtige **Statuscodes** (401/403), Reihenfolge der Middlewares und zentrales Error-Handling beachten.

**Quellen / Weiterführend**

* **Express**: [Guide: Using middleware](https://expressjs.com/de/guide/using-middleware.html) • [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* **Node.js**: [`http`/Fehlerbehandlung](https://nodejs.org/docs)
* **MDN**: [HTTP Status 401/403](https://developer.mozilla.org/ru/docs/Web/HTTP/Status)


  **[⬆ Наверх](#top)**      

227. ### <a name="227"></a> Wie prüft man Benutzerrollen (Role-Based Access Control, RBAC) in Express?

### **RBAC in Express: Rollen prüfen**

---

#### **1) Rollen aus JWT prüfen (stateless APIs)**

```js
// middleware/rbac.mjs
export const requireRole = (...roles) => (req, res, next) => {
  // req.user wird vorher in requireAuth (JWT-Verify) gesetzt
  const role = req.user?.role;
  if (!role) return res.status(401).json({ error: "Not authenticated" });
  return roles.includes(role)
    ? next()
    : res.status(403).json({ error: "Forbidden" });
};

// usage (Route):
// router.delete("/users/:id", requireAuth, requireRole("admin"), ctrl.deleteUser);
```

---

#### **2) Rollen aus Session/Cookie prüfen (stateful Web-Apps)**

```js
// middleware/rbacSession.mjs
export const requireSessionRole = (...roles) => (req, res, next) => {
  const role = req.user?.role || req.session?.user?.role;
  if (!role) return res.status(401).json({ error: "Login required" });
  return roles.includes(role) ? next() : res.status(403).json({ error: "Forbidden" });
};
```

---

#### **3) Feinere Kontrolle: Permissions/Scopes**

```js
// rbac/policy.mjs
const policy = {
  admin:   ["user:read", "user:write", "order:refund"],
  manager: ["user:read", "order:refund"],
  user:    ["user:read:self"]
};

export const requirePermission = (perm) => (req, res, next) => {
  const role = req.user?.role;
  if (!role) return res.status(401).json({ error: "Not authenticated" });
  return policy[role]?.includes(perm)
    ? next()
    : res.status(403).json({ error: "Forbidden" });
};

// usage:
// router.post("/orders/:id/refund", requireAuth, requirePermission("order:refund"), refundCtrl);
```

---

#### **4) DB-basierte RBAC (z. B. Sequelize)**

```js
// Beispiel: User gehört zu vielen Roles (User <-> Role via UserRole)
import { User, Role } from "../models/index.mjs";

export async function loadUserWithRoles(req, _res, next) {
  if (!req.user?.sub) return next();
  const u = await User.findByPk(req.user.sub, {
    include: [{ model: Role, attributes: ["name"] }],
    attributes: ["id"]
  });
  req.user.roles = u?.Roles?.map(r => r.name) ?? [];
  next();
}

export const requireAnyRole = (...roles) => (req, res, next) =>
  roles.some(r => req.user?.roles?.includes(r))
    ? next()
    : res.status(403).json({ error: "Forbidden" });

// usage:
// app.use(loadUserWithRoles);
// router.get("/admin", requireAuth, requireAnyRole("admin", "superuser"), handler);
```

---

#### **5) Gute Praxis**

* **Trenne AuthN und AuthZ**: Erst `requireAuth`, dann RBAC-Middleware.
* **Konsistente Statuscodes**: **401** (nicht eingeloggt), **403** (keine Rechte).
* **Least Privilege**: nur notwendige Rechte vergeben.
* **Claims + DB kombinieren**: schnelle Checks aus JWT (Rolle), sensible Checks gegen DB.
* **Cachings & Invalidierung**: Rollenänderungen berücksichtigen (z. B. `roleVersion`-Claim).
* **Auditing**: Zugriffsentscheidungen loggen (ohne sensible Daten).

---

### **Zusammenfassung**

* RBAC in Express per **Middleware**: Rollen/Permissions prüfen nach erfolgreicher Authentifizierung.
* Varianten: **JWT-Claims** (schnell, stateless), **Session** (stateful), **DB-gestützt** (flexibel).
* Beachte **Least Privilege** und korrekte **401/403**-Antworten.

**Quellen / Weiterführend**

* Express: [Using middleware](https://expressjs.com/de/guide/using-middleware.html) • [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* MDN: [HTTP 401/403](https://developer.mozilla.org/ru/docs/Web/HTTP/Status)
* Sequelize: [Associations](https://sequelize.org/docs/v6/advanced-association-concepts/advanced-many-to-many/)


  **[⬆ Наверх](#top)**      

228. ### <a name="228"></a> Was ist Policy-Based Access Control (PBAC)?

### **Policy-Based Access Control (PBAC)**

---

### **Definition**

* **PBAC** (auch **ABAC – Attribute-Based Access Control**) ist ein **feingranulares Zugriffsmodell**, bei dem **Policies (Regeln)** definieren, ob ein User Zugriff auf eine Ressource erhält.
* Entscheidungen basieren nicht nur auf Rollen (wie bei RBAC), sondern auf **Attributen**:

  * User-Attribute (z. B. Rolle, Abteilung, Alter)
  * Ressourcen-Attribute (z. B. Besitzer, Sensitivität, Status)
  * Kontext-Attribute (z. B. Uhrzeit, Ort, IP-Adresse)

---

### **Vergleich mit RBAC**

| Aspekt       | **RBAC (Role-Based)**                      | **PBAC / ABAC (Policy-Based)**                                   |
| ------------ | ------------------------------------------ | ---------------------------------------------------------------- |
| Modell       | User ↔ Rolle ↔ Rechte                      | User + Ressource + Kontext → Policy                              |
| Flexibilität | Mittel – Rollen definieren statisch Rechte | Hoch – Regeln können beliebige Attribute einbeziehen             |
| Beispiel     | „Admins dürfen löschen“                    | „User darf löschen, wenn er Besitzer ist UND es < 18:00 Uhr ist“ |

---

### **Beispiel-Policy (Ausdruck)**

```json
{
  "effect": "allow",
  "actions": ["delete:document"],
  "conditions": {
    "resource.ownerId": "${user.id}",
    "time.hour": "<=18"
  }
}
```

---

### **Express-Implementierung (PBAC Middleware, pseudo)**

```js
// policyEngine.mjs
export function checkPolicy(user, resource, action) {
  // Beispielregel: Owner darf löschen, aber nur tagsüber
  const hour = new Date().getHours();
  if (action === "delete:document") {
    return resource.ownerId === user.id && hour < 18;
  }
  return false;
}

// Middleware
export const requirePolicy = (action, resourceLoader) => async (req, res, next) => {
  const resource = await resourceLoader(req); // z. B. DB-Dokument laden
  if (!checkPolicy(req.user, resource, action)) {
    return res.status(403).json({ error: "Forbidden" });
  }
  req.resource = resource;
  next();
};

// usage:
router.delete("/docs/:id", requireAuth, requirePolicy("delete:document", async (req) => {
  return await Document.findByPk(req.params.id);
}), (req, res) => {
  req.resource.destroy();
  res.sendStatus(204);
});
```

---

### **Vorteile von PBAC**

✅ Sehr flexibel, auch dynamische Bedingungen möglich
✅ Gut für komplexe Organisationen mit vielen Kontextbedingungen
✅ Policies sind deklarativ und können zentral verwaltet werden

### **Nachteile von PBAC**

❌ Komplexer als RBAC (Policy-Engine, Verwaltung)
❌ Höherer Rechenaufwand (Attribute prüfen, DB-Abfragen)
❌ Schwerer zu debuggen und auditieren als feste Rollen

---

### **Zusammenfassung**

* **PBAC/ABAC** = Zugriffskontrolle über **dynamische Policies**, nicht nur feste Rollen.
* Basiert auf **User-, Ressourcen- und Kontext-Attributen**.
* Vorteil: **hohe Flexibilität**; Nachteil: **höhere Komplexität**.
* In Express implementierbar über **Policy-Middleware + Resource-Loader**.

**Quellen / Weiterführend**

* [NIST Guide zu ABAC](https://csrc.nist.gov/publications/detail/sp/800-162/final)
* [OWASP – Access Control](https://owasp.org/www-community/Access_Control)
* [Express.js Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

229. ### <a name="229"></a> Wie schützt man REST-Endpunkte vor unautorisierten Zugriffen?

### **REST-Endpunkte vor unautorisiertem Zugriff schützen**

---

#### **1) Authentifizierung (z. B. JWT)**

```js
// middleware/auth.mjs
import jwt from "jsonwebtoken";
const { JWT_SECRET } = process.env;

export function requireAuth(req, res, next) {
  const token = req.headers.authorization?.startsWith("Bearer ")
    ? req.headers.authorization.slice(7)
    : null;
  if (!token) return res.status(401).json({ error: "No token" });
  try {
    req.user = jwt.verify(token, JWT_SECRET, {
      algorithms: ["HS256"], issuer: "https://auth.example.com", audience: "example.api"
    });
    next();
  } catch { return res.status(403).json({ error: "Invalid/expired token" }); }
}
```

---

#### **2) Autorisierung (RBAC/Scopes)**

```js
// middleware/rbac.mjs
export const requireRole = (...roles) => (req, res, next) =>
  req.user && roles.includes(req.user.role)
    ? next()
    : res.status(403).json({ error: "Forbidden" });

// Nutzung
// router.delete("/users/:id", requireAuth, requireRole("admin"), ctrl.deleteUser);
```

---

#### **3) Prinzip „deny by default“ (Routing-Reihenfolge)**

```js
// app.mjs
app.use("/public", publicRoutes);
app.use("/api", requireAuth, apiRoutes); // alles private per Default
```

---

#### **4) Transport- & Header-Sicherheit**

* **HTTPS erzwingen** (+ HSTS via `helmet.hsts`), **keine Tokens in URLs**.
* **Security-Header** mit `helmet()` setzen (CSP, X-Frame-Options, NoSniff, …).
* **CORS** restriktiv: Whitelist-Origns, keine `*` mit Credentials.
  Quellen: [MDN HTTPS](https://developer.mozilla.org/ru/docs/Web/HTTP/Overview#https), [Helmet/Express](https://expressjs.com/de/advanced/best-practice-security.html), [MDN CORS](https://developer.mozilla.org/ru/docs/Web/HTTP/CORS)

---

#### **5) Schutz gegen CSRF (bei Cookie-Auth)**

* **SameSite**-Cookies (`Lax/Strict`) oder `SameSite=None; Secure` bei Cross-Site.
* **CSRF-Token** für state-ändernde Requests (Synchronizer/Double-Submit).
  Quelle: [MDN – CSRF](https://developer.mozilla.org/ru/docs/Glossary/CSRF)

---

#### **6) Rate Limiting & Brute-Force-Schutz**

* Request- und Login-Endpunkte begrenzen; Backoff/Lockout bei vielen Fehlversuchen.
  Quelle: [Express Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

#### **7) Eingabevalidierung & Deserialisierung**

* Schemas (z. B. Zod/Joi) vor der Business-Logik; **NoSQL/SQL-Injection** verhindern (parametrisierte Queries/ORM).
  Quellen: [MDN – Form validation/Validation](https://developer.mozilla.org/ru/docs/Learn/Forms/Form_validation), [Sequelize Security](https://sequelize.org/)

---

#### **8) Minimale Rechte & Ressourcen-Isolation**

* **RBAC/Scopes** pro Route/Service, **Least Privilege** in DB und externen APIs.
* Sensible Endpunkte zusätzlich mit **IP-Allowlist**/**mTLS** (intern).

---

#### **9) Logging & Auditing**

* Zugriffsentscheidungen (401/403), Auth-Fehler, ungewöhnliche Muster loggen (ohne Secrets).

---

#### **10) API-Keys für Service-zu-Service**

```js
// middleware/apiKey.mjs
export const requireApiKey = (req, res, next) =>
  req.get("X-API-Key") === process.env.INTERNAL_API_KEY ? next() : res.sendStatus(401);
```

---

### **Zusammenfassung**

* **AuthN**: z. B. JWT-Middleware; **AuthZ**: RBAC/Scopes → „deny by default“.
* **Transport/Headers**: HTTPS, Helmet, restriktives CORS; bei Cookies **CSRF-Schutz**.
* **Hardening**: Rate-Limiting, Validierung, Least-Privilege, Logging; intern ggf. **API-Key/mTLS**.

**Quellen**

* [MDN – HTTPS](https://developer.mozilla.org/ru/docs/Web/HTTP/Overview#https) • [CORS](https://developer.mozilla.org/ru/docs/Web/HTTP/CORS) • [CSRF](https://developer.mozilla.org/ru/docs/Glossary/CSRF)
* [Express – Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* [Sequelize – Security Hinweise](https://sequelize.org/)


  **[⬆ Наверх](#top)**      

230. ### <a name="230"></a> Wie kann man Public Routes von Private Routes in Express trennen?

### **Trennung von Public und Private Routes in Express**

---

#### **1) Ordner- & Router-Struktur**

* **Public Routes**: ohne Authentifizierung (z. B. `/login`, `/register`, `/health`).
* **Private Routes**: nur mit Authentifizierung (JWT, Session, API-Key).

```js
// routes/public.mjs
import { Router } from "express";
const publicRouter = Router();

publicRouter.get("/health", (_req, res) => res.json({ status: "ok" }));
publicRouter.post("/login", authController.login);

export default publicRouter;

// routes/private.mjs
import { Router } from "express";
import { requireAuth } from "../middleware/auth.mjs";

const privateRouter = Router();
privateRouter.use(requireAuth); // Middleware für alle nachfolgenden Routen

privateRouter.get("/profile", (req, res) => res.json({ user: req.user }));
privateRouter.delete("/users/:id", requireAuth, requireRole("admin"), userCtrl.delete);

export default privateRouter;
```

---

#### **2) Mounting in `app.mjs`**

```js
import express from "express";
import publicRouter from "./routes/public.mjs";
import privateRouter from "./routes/private.mjs";

const app = express();
app.use(express.json());

// Public: ohne Auth
app.use("/public", publicRouter);

// Private: nur mit Auth
app.use("/api", privateRouter);

export default app;
```

---

#### **3) Middleware-Ansatz „Deny by default“**

* Alles unter `/api` ist per Default privat → `requireAuth` als globaler Guard.
* Nur explizit definierte Public-Routen sind frei erreichbar.

```js
app.use("/api", requireAuth, apiRouter);
```

---

#### **4) Route-Metadaten (für große Apps)**

* Im Router-Array definieren, ob eine Route **public** oder **private** ist.
* Middleware prüft automatisch.

```js
const routes = [
  { path: "/login", handler: loginCtrl, public: true },
  { path: "/profile", handler: profileCtrl, public: false }
];

routes.forEach(r => {
  if (r.public) app.get(r.path, r.handler);
  else app.get(r.path, requireAuth, r.handler);
});
```

---

#### **5) Best Practices**

* **Trennung in Module** (public vs. private Router).
* **Globales requireAuth** für `/api`.
* **Least Privilege**: Private Routes zusätzlich mit RBAC/Policies schützen.
* **Public Routes restriktiv halten** (Login, Docs, Health, evtl. Registration).
* **Immer HTTPS**, Security-Header (Helmet), Rate-Limiting auf sensiblen Routen.

---

### **Zusammenfassung**

* Public und Private Routes in Express trennt man durch **eigene Router** + **Middleware (requireAuth)**.
* Bestes Muster: `/public/*` frei, `/api/*` standardmäßig geschützt.
* Für große Apps: Route-Metadaten oder Role/Policy-basierte Middleware einsetzen.

🔗 Quellen

* [Express – Router](https://expressjs.com/de/guide/routing.html)
* [Express – Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

231. ### <a name="231"></a> Was ist CSRF und wie hängt es mit Session-Authentifizierung zusammen?

### **CSRF (Cross-Site Request Forgery) & Sessions**

---

### **Was ist CSRF?**

* **CSRF** = Angriff, bei dem ein Opfer ungewollte Requests an eine vertrauenswürdige Seite sendet, während es dort **authentifiziert** ist.
* Der Browser hängt automatisch Cookies (inkl. **Session-Cookie**) an die Anfrage → der Server glaubt, die Aktion kommt vom User.
* Beispiel:

  ```html
  <!-- Opfer ist eingeloggt bei bank.com -->
  <img src="https://bank.com/transfer?to=attacker&amount=1000" />
  ```

  → Browser sendet Session-Cookie mit → Überweisung läuft.

---

### **Zusammenhang mit Session-Authentifizierung**

* Bei **Session-basiertem Login** wird die Authentifizierung über ein **Session-Cookie** gespeichert.
* Cookies werden **automatisch bei jeder Anfrage** mitgeschickt (same-origin Policy).
* Dadurch kann ein Angreifer das Cookie „missbrauchen“, wenn er das Opfer dazu bringt, eine manipulierte Anfrage an die Seite auszuführen.
* **JWT im Header (`Authorization: Bearer …`)** ist weniger anfällig für CSRF, da Tokens nicht automatisch gesendet werden → aber anfällig für XSS, wenn sie im LocalStorage stehen.

---

### **Schutzmaßnahmen bei Session-Auth**

1. **CSRF-Tokens** (Synchronizer Token Pattern):

   * Server gibt ein zufälliges Token pro Session aus → Client muss es in jedem POST/PUT/DELETE mitschicken.
   * Angreifer kann Token nicht erraten.

   ```html
   <form method="POST" action="/transfer">
     <input type="hidden" name="csrfToken" value="random12345" />
   </form>
   ```

2. **SameSite-Cookies**

   * `Set-Cookie: sessionId=abc; HttpOnly; Secure; SameSite=Lax`
   * Verhindert, dass Cookies bei Cross-Site-Requests mitgeschickt werden.
   * `Lax` blockiert POST-Formulare von fremden Domains.

3. **Zusätzlich:**

   * **HTTPS erzwingen** (Secure-Flag).
   * **Double-Submit Cookie Pattern** (CSRF-Token in Cookie + Header).
   * **Referer/Origin-Header prüfen** (ergänzend).

---

### **Zusammenfassung**

* **CSRF** nutzt aus, dass Browser Cookies (z. B. **Session-Cookies**) automatisch mitsenden.
* Besonders relevant bei **Session-basiertem Login**.
* Schutz: **CSRF-Tokens, SameSite-Cookies, HTTPS**.
* Bei **JWT im Header** weniger anfällig, dafür stärker auf **XSS-Schutz** achten.

🔗 Quellen

* [MDN – CSRF](https://developer.mozilla.org/ru/docs/Glossary/CSRF)
* [OWASP – CSRF Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html)
* [Express Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

232. ### <a name="232"></a> Wie verhindert man Session Fixation?

### **Session Fixation – Erklärung & Schutz**

---

### **Was ist Session Fixation?**

* Angriff, bei dem ein Angreifer dem Opfer **eine bekannte Session-ID unterschiebt** (z. B. per Link oder Cookie).
* Loggt sich das Opfer danach ein, wird die Session-ID **weiterverwendet** → Angreifer kennt gültige Session-ID und kann die Sitzung übernehmen.

---

### **Beispiel**

1. Angreifer ruft `https://shop.com/login?sessionId=abc123` auf.
2. Opfer klickt auf den Link → Browser übernimmt Session-ID.
3. Opfer loggt sich ein → Session wird **nicht erneuert**, bleibt `abc123`.
4. Angreifer kennt `abc123` → hat Zugriff auf Opfer-Session.

---

### **Schutzmaßnahmen**

#### 1) **Session-ID nach Login erneuern (Session Regeneration)**

* Wichtigster Schutz: **neue Session-ID nach erfolgreichem Login**.

```js
// Express + express-session
app.post("/login", (req, res, next) => {
  const { username, password } = req.body;
  if (isValidUser(username, password)) {
    // Session-ID erneuern, alte Daten löschen
    req.session.regenerate((err) => {
      if (err) return next(err);
      req.session.user = { name: username };
      res.json({ message: "Login erfolgreich" });
    });
  } else {
    res.status(401).json({ error: "Invalid credentials" });
  }
});
```

---

#### 2) **Sichere Cookies setzen**

* **HttpOnly** → kein Zugriff per JavaScript (XSS-Schutz).
* **Secure** → nur über HTTPS.
* **SameSite=Lax/Strict** → erschwert CSRF.

```js
app.use(session({
  secret: process.env.SESSION_SECRET,
  resave: false,
  saveUninitialized: false,
  cookie: {
    httpOnly: true,
    secure: true,
    sameSite: "lax"
  }
}));
```

---

#### 3) **Session Timeout & Inaktivitäts-Timeout**

* Automatisches Abmelden nach einer Zeit → verkleinert Angriffsfenster.

---

#### 4) **Keine Session-IDs in URL/Query-Params**

* Immer Cookies für Session-ID nutzen, niemals `?sessionId=...`.

---

#### 5) **Zusätzliche Checks**

* **IP- oder User-Agent-Bindung** (optional, aber Vorsicht bei NAT/Shared Devices).
* **Logout → Session sofort invalidieren** (`req.session.destroy()`).

---

### **Zusammenfassung**

* **Session Fixation** = Angriff, bei dem der Angreifer dem Opfer eine bekannte Session-ID unterschiebt.
* **Hauptschutz:** Session-ID nach Login **regenerieren**.
* Weitere Maßnahmen: sichere Cookies, HTTPS, Timeout, keine Session-IDs in URLs.

🔗 Quellen

* [OWASP – Session Fixation](https://owasp.org/www-community/attacks/Session_fixation)
* [Express – Best Practices Security](https://expressjs.com/de/advanced/best-practice-security.html)
* [MDN – HttpOnly/Secure Cookies](https://developer.mozilla.org/ru/docs/Web/HTTP/Cookies)

---

  **[⬆ Наверх](#top)**      

233. ### <a name="233"></a> Welche Best Practices gibt es für Passwort-Hashing (bcrypt, argon2)?

### **Passwort-Hashing Best Practices (bcrypt, argon2)**

---

#### **Grundsätze**

* **Nie Klartext** oder einfache Hashes (MD5/SHA-1/SHA-256) für Passwörter nutzen.
* **Passwort-Hashfunktionen** mit Arbeitsschwierigkeit verwenden: **Argon2id** (empfohlen), **bcrypt** (bewährt), alternativ **scrypt**.
* **Einzigartiger Salt** pro Passwort (bei argon2/bcrypt integriert).
* **Konstante Zeit vergleichen** (Timing-Angriffe vermeiden).
* **Pepper** optional zusätzlich zum Hash (in ENV/Secret-Manager halten).
* **Kosten regelmäßig erhöhen** (Hardware wird schneller → Rehash bei Login, wenn zu schwach).

---

#### **Empfohlene Parameter**

* **Argon2id** (bevorzugt):

  * `timeCost`: 2–5
  * `memoryCost`: 64–256 MB (z. B. 2^16 = 65 536 KiB)
  * `parallelism`: 1–4
* **bcrypt**:

  * `cost`/`saltRounds`: **12–14** (Produktion), mindestens 10 für Dev/Tests
* **scrypt** (Node `crypto.scrypt`):

  * sinnvolle N/r/p wählen; in Node-Defaults belassen oder OWASP-Empfehlungen folgen

> Parameter hängen von **Latenz-Budget** und **Server-Ressourcen** ab; mit Benchmarks validieren.

---

#### **Node.js – Beispiele (ESM)**

**Argon2id (empfohlen)**

```js
// hash-argon2.mjs
import argon2 from "argon2"; // npm i argon2

const opts = { type: argon2.argon2id, timeCost: 3, memoryCost: 1 << 16, parallelism: 1 };

export async function hashPassword(plain) {
  return argon2.hash(plain, opts);         // beinhaltet Salt & Parameter
}

export async function verifyPassword(hash, plain) {
  return argon2.verify(hash, plain, opts); // constant-time Verify
}
```

**bcrypt**

```js
// hash-bcrypt.mjs
import bcrypt from "bcrypt"; // npm i bcrypt
const ROUNDS = 12;

export async function hashPassword(plain) {
  return bcrypt.hash(plain, ROUNDS);       // Salt automatisch integriert
}

export async function verifyPassword(hash, plain) {
  return bcrypt.compare(plain, hash);      // constant-time Compare
}
```

**scrypt (Core-Alternative)**

```js
// hash-scrypt.mjs
import { randomBytes, scryptSync, timingSafeEqual } from "node:crypto";

export function hashPassword(plain) {
  const salt = randomBytes(16);
  const dk = scryptSync(plain, salt, 64);         // Key derivation
  return `${salt.toString("hex")}:${dk.toString("hex")}`;
}

export function verifyPassword(stored, plain) {
  const [saltHex, dkHex] = stored.split(":");
  const hash = scryptSync(plain, Buffer.from(saltHex, "hex"), 64);
  return timingSafeEqual(hash, Buffer.from(dkHex, "hex"));
}
```

---

#### **Integration (DB/Sequelize)**

* Spalte z. B. `password_hash TEXT NOT NULL`.
* **Nur Hash speichern** (nie Pepper/Salt separat nötig bei argon2/bcrypt).
* Beim Login: verifizieren → falls zu niedriger Work-Factor → **Rehash** und speichern.

```js
// user.model.mjs (Sequelize Hook)
import { Model, DataTypes } from "sequelize";
import { hashPassword } from "../security/hash-argon2.mjs";

export class User extends Model {}
User.init({
  email: { type: DataTypes.STRING, unique: true },
  passwordHash: { type: DataTypes.TEXT, allowNull: false }
}, { sequelize, modelName: "User" });

User.beforeCreate(async (user) => {
  user.passwordHash = await hashPassword(user.passwordHash); // pass plain in temp field o. Ä.
});
```

---

#### **Weitere Sicherheitsmaßnahmen**

* **Pepper** (z. B. `HMAC(pepper, password)` vor dem Hash) im **Secret-Manager** halten.
* **Rate Limiting** & **Account Lockout** bei Login-Versuchen.
* **MFA/2FA** anbieten.
* **Sichere Passwortrichtlinien** + z. B. HaveIBeenPwned-Check (client-seitig anonymisiert).
* **Sichere Passwort-Reset-Tokens**: kryptografisch zufällig, kurzlebig, einmalig.
* **Transport**: Immer **HTTPS**; keine Passwörter/Hashes in Logs.

---

### **Zusammenfassung**

* Nutze **Argon2id** (oder **bcrypt**) mit **angemessenem Work-Factor**, Salt ist integriert.
* **Rehash bei Login**, wenn Parameter zu schwach; **Pepper**, **Rate-Limit**, **HTTPS**, **MFA** ergänzen.
* In Node: **argon2/bcrypt** Libraries oder **`crypto.scrypt`**; vergleiche **constant-time**.

**Quellen / Weiterführend**

* Node.js: [`crypto.scrypt`](https://nodejs.org/docs/latest/api/crypto.html#cryptoscryptpassword-salt-keylen-options-callback) • [`crypto.timingSafeEqual`](https://nodejs.org/docs/latest/api/crypto.html#cryptotimingsafeequala-b)
* MDN: [Passwörter sicher speichern (Übersicht Hashing/KDF)](https://developer.mozilla.org/ru/docs/Glossary/Salt)
* OWASP: [Password Storage Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html)
* Sequelize: [Hooks](https://sequelize.org/docs/v6/other-topics/hooks/)


  **[⬆ Наверх](#top)**      

234. ### <a name="234"></a> Warum sollte man niemals Passwörter im Klartext speichern?

### **Warum niemals Passwörter im Klartext speichern?**

---

#### **1) Risiko bei Datenlecks**

* Datenbanken können durch **Hacks, Fehlkonfiguration oder Insider** kompromittiert werden.
* Wenn Passwörter im Klartext gespeichert sind → **Angreifer hat sofort Zugriff** auf alle Konten.
* Nutzer recyceln oft Passwörter → auch **andere Dienste** (E-Mail, Banking) sind gefährdet.

---

#### **2) Verletzung von Datenschutz & Gesetzen**

* DSGVO (EU) und OWASP-Best Practices verbieten **unsichere Speicherung**.
* Ein Klartext-Leak führt zu **hohen Bußgeldern und Image-Schäden**.
* Vertrauen der Nutzer geht verloren → Reputationsrisiko.

---

#### **3) Technische Standards**

* **Best Practice**: Passwörter mit **KDF (Key Derivation Function)** wie **bcrypt, Argon2, scrypt** **gehasht und gesalzen** speichern.
* Hashing ist **einseitig** → aus dem Hash kann das Passwort nicht einfach zurückgerechnet werden.
* Salt verhindert Rainbow-Table-Angriffe; Work-Factor macht Brute-Force extrem teuer.

---

#### **4) Beispiel**

**Falsch (Klartext in DB):**

```sql
id | email              | password
1  | user@example.com   | geheim123
```

**Richtig (gehashte Werte):**

```sql
id | email              | password_hash
1  | user@example.com   | $argon2id$v=19$m=65536,t=3,p=1$...
```

Beim Login:

* User gibt Passwort ein.
* Server hasht Eingabe mit denselben Parametern.
* Vergleich: Hashes stimmen überein → Zugang.

---

### **Zusammenfassung**

* **Klartext-Passwörter = sofortiger Komplettverlust** bei Datenlecks.
* **Gesetzlich und sicherheitstechnisch unzulässig.**
* Immer **gehashte & gesalzene Speicherung** mit sicheren Algorithmen (Argon2id/bcrypt).

🔗 Quellen

* [OWASP – Password Storage Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html)
* [MDN – Salt & Hash](https://developer.mozilla.org/ru/docs/Glossary/Salt)
* [NIST SP 800-63B – Digital Identity Guidelines](https://pages.nist.gov/800-63-3/sp800-63b.html)

---

  **[⬆ Наверх](#top)**      

235. ### <a name="235"></a> Wie implementiert man Zwei-Faktor-Authentifizierung (2FA) in einer Node.js-App?

### **2FA in einer Node.js/Express-App – Praxisleitfaden**

---

## **Varianten**

* **TOTP (App-basiert, RFC 6238)**: Nutzer scannt QR-Code (Google Authenticator, Authy), gibt 6-stelligen Code ein.
* **WebAuthn/Passkeys**: Phishing-resistent (Hardware-Key/Plattform-Authenticator).
* **SMS/E-Mail-Codes**: Einfach, aber schwächer (Abfangen/Weiterleitung möglich).
  Empfehlung: **TOTP oder WebAuthn**; SMS/E-Mail nur als Fallback.

---

## **TOTP-Implementierung (Express + `speakeasy` + `qrcode`)**

### 1) Installation

```bash
npm i speakeasy qrcode express cookie-parser helmet
```

### 2) Enrollment (Secret erzeugen + QR)

```js
// routes/2fa.mjs
import { Router } from "express";
import speakeasy from "speakeasy";
import qrcode from "qrcode";

export const twoFaRouter = Router();

// Nutzer muss bereits per Passwort authentifiziert sein
twoFaRouter.post("/enable", async (req, res) => {
  // Secret generieren (base32 speichern)
  const secret = speakeasy.generateSecret({
    name: `MyApp (${req.user.email})`,  // erscheint im Authenticator
    length: 20
  });

  // QR-DataURL erzeugen
  const otpauth = secret.otpauth_url;
  const qrDataUrl = await qrcode.toDataURL(otpauth);

  // Secret **verschlüsselt** in DB speichern (oder HSM/Secrets-Store)
  await db.user.update({ where: { id: req.user.id }, data: {
    totpSecretB32: secret.base32, // besser: verschlüsselt
    is2faEnabled: false           // erst nach erfolgreicher Verifikation auf true
  }});

  res.json({ qrDataUrl, manualKey: secret.base32 });
});
```

### 3) Verifikation beim Setup (Schritt zur Aktivierung)

```js
twoFaRouter.post("/verify-setup", async (req, res) => {
  const { token } = req.body; // 6-stelliger Code
  const user = await db.user.findByPk(req.user.id);

  const ok = speakeasy.totp.verify({
    secret: user.totpSecretB32,
    encoding: "base32",
    token,
    window: 1 // geringe Toleranz gegen Zeitdrift
  });

  if (!ok) return res.status(400).json({ error: "Invalid TOTP" });

  await db.user.update({ where: { id: user.id }, data: { is2faEnabled: true }});
  res.sendStatus(204);
});
```

### 4) Login-Flow (Passwort → TOTP)

```js
// 1) Passwort prüfen → temporär markieren, dass 2FA nötig ist
app.post("/login", async (req, res) => {
  const user = await verifyPasswordLogin(req.body);
  if (!user) return res.status(401).json({ error: "Invalid credentials" });

  if (user.is2faEnabled) {
    // kurzlebiges „pre-auth“-Ticket (z. B. signierter JWT/Cookie mit 2–5 Min TTL)
    res.cookie("preauth", issuePreAuth(user.id), { httpOnly: true, secure: true, sameSite: "Lax", maxAge: 5*60*1000 });
    return res.status(206).json({ require2fa: true }); // Client zeigt 2FA-Form
  }

  return res.json({ access: issueAccessToken(user), refresh: issueRefreshToken(user) });
});

// 2) TOTP prüfen → finale Tokens ausstellen
app.post("/login/2fa", async (req, res) => {
  const userId = verifyPreAuth(req.cookies.preauth); // validiert & extrahiert userId
  if (!userId) return res.status(401).json({ error: "Preauth expired" });

  const user = await db.user.findByPk(userId);
  const ok = speakeasy.totp.verify({
    secret: user.totpSecretB32,
    encoding: "base32",
    token: req.body.token,
    window: 1
  });
  if (!ok) return res.status(400).json({ error: "Invalid TOTP" });

  // Preauth entfernen, finale Tokens ausstellen
  res.clearCookie("preauth");
  return res.json({ access: issueAccessToken(user), refresh: issueRefreshToken(user) });
});
```

### 5) Middleware: Schutz nach Login

```js
// middleware/require2fa.mjs
export function require2FA(req, res, next) {
  if (req.user?.is2faEnabled && !req.user?.amr?.includes("otp")) {
    return res.status(403).json({ error: "2FA required" });
  }
  next();
}

// Idee: Beim erfolgreichen 2FA-Login `amr: ["pwd","otp"]` im JWT setzen.
```

### 6) Backup-Codes (Recovery)

```js
// Einmalige Backup-Codes generieren & gehasht speichern
import { randomBytes, createHash, timingSafeEqual } from "node:crypto";

function genBackupCodes(n = 10) {
  return Array.from({ length: n }, () =>
    randomBytes(5).toString("hex")  // z. B. 10 Zeichen
  );
}

function hash(code) { return createHash("sha256").update(code).digest("hex"); }
```

* Codes **nur einmal** anzeigen, **gehasht** speichern, bei Nutzung sofort invalidieren.

---

## **WebAuthn / Passkeys (stärker als TOTP)**

* Implementierbar mit `@simplewebauthn/server` (Server) + `@simplewebauthn/browser` (Client).
* Vorteile: **Phishing-resistent**, keine Codes, kein Secret auf dem Server (nur Public Keys).
* Eignet sich als **zweiter Faktor** oder **passwortlos**.
  👉 Siehe MDN-WebAuthn-Überblick in den Quellen.

---

## **Sicherheit & Betrieb**

* **Secrets schützen**: TOTP-Secret verschlüsselt speichern; nie loggen.
* **Zeit-Synchronisation**: Server-Uhr via NTP; kleine `window`-Toleranz.
* **Rate Limiting**: 2FA-Endpunkte drosseln, Lockout/Backoff.
* **Gerät merken** (optional): Signierter „trusted device“-Cookie mit begrenzter TTL.
* **Backup & Recovery**: Backup-Codes anbieten, Support-Prozess definieren.
* **HTTPS verpflichtend**, Cookies `HttpOnly`/`Secure`/`SameSite`.

---

### **Zusammenfassung**

* **TOTP**: Schnell umgesetzt mit `speakeasy` + QR; Secret sicher speichern, `window` klein halten.
* **Login-Flow**: Passwort → Preauth → TOTP → finale Tokens; **Rate-Limits & Backup-Codes**.
* **WebAuthn/Passkeys**: noch sicherer; für MFA oder passwordless geeignet.

**Quellen / Weiterführend**

* MDN: [WebAuthn – Überblick](https://developer.mozilla.org/en-US/docs/Web/API/Web_Authentication_API) • [Cookies/SameSite](https://developer.mozilla.org/ru/docs/Web/HTTP/Headers/Set-Cookie/SameSite)
* Node.js: [`crypto`-Modul](https://nodejs.org/docs/latest/api/crypto.html)
* Express: [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* (Normativ) RFCs: **TOTP RFC 6238**, **HOTP RFC 4226** (Hintergrund zu Einmalpasswörtern)


  **[⬆ Наверх](#top)**      

236. ### <a name="236"></a> Was ist der Unterschied zwischen Single Sign-On (SSO) und klassischem Login?

### **Unterschied: Single Sign-On (SSO) vs. klassisches Login**

---

### **Klassisches Login**

* Jeder Dienst (App, Website) hat **eigene Benutzerverwaltung**.
* User gibt **Benutzername + Passwort** direkt bei der App ein.
* Authentifizierung läuft lokal, Tokens/Sessions werden nur für diese App erzeugt.
* Nachteile:

  * Viele verschiedene Logins nötig (Passwort-Wiederverwendung = Risiko).
  * Keine zentrale Kontrolle für Admins.
  * User Experience schlechter.

---

### **Single Sign-On (SSO)**

* User authentifiziert sich **einmal zentral** bei einem **Identity Provider (IdP)** (z. B. Keycloak, Auth0, Azure AD, Google).
* Danach können mehrere Anwendungen (Service Provider, SP) auf diese Authentifizierung vertrauen.
* Technische Grundlage: **Protokolle** wie OAuth2, OpenID Connect, SAML.
* Vorteile:

  * **Ein Login für viele Systeme** (einheitliches Token, z. B. ID-Token oder SAML-Assertion).
  * Bessere **User Experience** (keine Mehrfach-Logins).
  * Bessere **Sicherheit** (zentrale MFA/2FA, Policies, schnelle Account-Sperre).
  * Weniger Passwortspeicherung in einzelnen Apps.

---

### **Direkter Vergleich**

| Aspekt            | **Klassisches Login**                   | **SSO**                                     |
| ----------------- | --------------------------------------- | ------------------------------------------- |
| Benutzerkonto     | Pro App/Dienst separat                  | Zentrales Konto beim IdP                    |
| Authentifizierung | Lokal in der App                        | Zentral über IdP (OAuth2/OIDC/SAML)         |
| Login-Anzahl      | Für jede App separat                    | Einmaliger Login → Zugang zu allen Apps     |
| Sicherheit        | Jede App muss Passwort sicher speichern | Passwort nur beim IdP; zentrale MFA möglich |
| User Experience   | Weniger komfortabel                     | Komfortabler (ein Login für viele Apps)     |

---

### **Zusammenfassung**

* **Klassisches Login**: Jede App prüft Credentials selbst; mehrfache Logins, höherer Verwaltungsaufwand.
* **SSO**: Zentrale Authentifizierung über einen Identity Provider → **ein Login für viele Anwendungen**, sicherer und bequemer.

🔗 Quellen

* [MDN – Authentication](https://developer.mozilla.org/en-US/docs/Glossary/Authentication)
* [OAuth 2.0 (RFC 6749)](https://datatracker.ietf.org/doc/html/rfc6749)
* [OpenID Connect Core](https://openid.net/specs/openid-connect-core-1_0.html)

---

  **[⬆ Наверх](#top)**      

237. ### <a name="237"></a> Wie funktioniert Authentifizierung mit Passport.js?

### **Authentifizierung mit Passport.js**

---

### **Grundidee**

* **Passport.js** ist ein **Middleware-Framework** für **Express**, das viele Auth-Strategien bereitstellt (über 500, z. B. Local, JWT, OAuth2, Google, GitHub).
* Trennt **Authentifizierung** (Identität prüfen) von **Autorisierung** (Rechte prüfen).
* Arbeitet über **Strategien**: Jede Strategie implementiert, *wie* User überprüft werden (Passwort, Token, Provider).

---

### **Ablauf**

1. **Strategie konfigurieren** (z. B. Local, JWT, Google).
2. **Login-Route** → `passport.authenticate("strategie")`.
3. Bei Erfolg: Passport setzt `req.user`.
4. **Sessions optional**: User-ID wird in Session gespeichert (serialize/deserialize).
5. Zugriff auf geschützte Routen → Middleware prüft `req.isAuthenticated()` oder Token.

---

### **Beispiel: Local Strategy (User/Passwort + Session)**

```js
// auth.mjs
import passport from "passport";
import { Strategy as LocalStrategy } from "passport-local";
import bcrypt from "bcrypt";
import { User } from "./models/user.mjs";

// 1. Strategie definieren
passport.use(new LocalStrategy(
  { usernameField: "email", passwordField: "password" },
  async (email, password, done) => {
    try {
      const user = await User.findOne({ where: { email } });
      if (!user) return done(null, false, { message: "Unknown user" });

      const match = await bcrypt.compare(password, user.passwordHash);
      if (!match) return done(null, false, { message: "Wrong password" });

      return done(null, user); // Erfolg → req.user = user
    } catch (err) {
      return done(err);
    }
  }
));

// 2. Session-Support
passport.serializeUser((user, done) => done(null, user.id));
passport.deserializeUser(async (id, done) => {
  const user = await User.findByPk(id);
  done(null, user);
});
```

```js
// app.mjs
import express from "express";
import session from "express-session";
import passport from "passport";
import "./auth.mjs";

const app = express();
app.use(express.json());
app.use(session({ secret: process.env.SESSION_SECRET, resave: false, saveUninitialized: false }));
app.use(passport.initialize());
app.use(passport.session());

// Login-Route
app.post("/login", passport.authenticate("local", {
  successRedirect: "/profile",
  failureRedirect: "/login"
}));

// Geschützte Route
app.get("/profile", (req, res) => {
  if (!req.isAuthenticated()) return res.status(401).json({ error: "Not logged in" });
  res.json(req.user);
});
```

---

### **Beispiel: JWT Strategy (statt Session)**

```js
// jwt-auth.mjs
import passport from "passport";
import { Strategy as JwtStrategy, ExtractJwt } from "passport-jwt";

passport.use(new JwtStrategy({
  jwtFromRequest: ExtractJwt.fromAuthHeaderAsBearerToken(),
  secretOrKey: process.env.JWT_SECRET
}, async (payload, done) => {
  try {
    // z. B. User in DB prüfen
    return done(null, { id: payload.sub, role: payload.role });
  } catch (err) {
    return done(err, false);
  }
}));

// usage in Route:
app.get("/api/private",
  passport.authenticate("jwt", { session: false }),
  (req, res) => res.json({ user: req.user })
);
```

---

### **Best Practices**

* **Sessions**: für klassische Web-Apps (Cookies).
* **JWT**: für SPAs/Mobile/REST-APIs (stateless).
* **OAuth2/OpenID Connect**: für Social Logins („Login mit Google/GitHub“).
* Immer: **HTTPS, sichere Cookies, bcrypt/argon2 für Passwörter, Rate-Limiting**.

---

### **Zusammenfassung**

* Passport.js = **flexibles Auth-Framework für Express** mit Strategien.
* Ablauf: Strategie → `passport.authenticate` → `req.user`.
* Nutzbar mit **Sessions (stateful)** oder **JWT/OAuth2 (stateless)**.

🔗 Quellen

* [Passport.js Dokumentation](http://www.passportjs.org/)
* [Express – Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* [MDN – Authentication vs. Authorization](https://developer.mozilla.org/en-US/docs/Glossary/Authentication)

---

  **[⬆ Наверх](#top)**      

238. ### <a name="238"></a> Welche Vorteile bietet Passport.js in Express?

### **Vorteile von Passport.js in Express**

---

#### **1) Viele fertige Authentifizierungsstrategien**

* Über **500 Strategien** verfügbar: Local (User/Passwort), JWT, OAuth2, OpenID Connect, Social Logins (Google, GitHub, Facebook, Twitter …).
* Spart Zeit, da man keine eigenen Flows komplett neu implementieren muss.

---

#### **2) Einheitliche Middleware-Schnittstelle**

* Immer gleiches Muster:

  ```js
  passport.authenticate("strategie", options)
  ```
* Unabhängig davon, ob es sich um Session, JWT oder OAuth handelt.

---

#### **3) Flexibel (Session vs. JWT)**

* Kann mit **Sessions** (stateful, Cookies) oder **JWT/OAuth** (stateless) genutzt werden.
* Anpassbar für REST-APIs, SPAs, Mobile-Apps und klassische Web-Apps.

---

#### **4) Saubere Trennung von Auth-Logik**

* Authentifizierung wird aus den Routes herausgehalten.
* Strategie = Login-Logik, Middleware = Schutz von Endpunkten.
* Erhöht **Wartbarkeit** und **Klarheit im Code**.

---

#### **5) Integration mit Express**

* Nahtlos in Express-Middleware-Kette einsetzbar.
* Unterstützt `req.isAuthenticated()`, `req.user`, Sessions → sehr einfaches Role/Permission-Handling.

---

#### **6) Community & Ökosystem**

* Weit verbreitet, große Community, viele Tutorials.
* Gut dokumentiert, viele Beispiele für typische Anwendungsfälle.

---

### **Zusammenfassung**

* Passport.js bietet **vorgefertigte Strategien**, eine **einheitliche Middleware-API**, ist **flexibel** (Sessions, JWT, OAuth2) und sorgt für **saubere Trennung der Authentifizierungslogik**.
* Dadurch ist es in Express der **De-facto-Standard** für Authentifizierung.

🔗 Quellen

* [Passport.js Dokumentation](http://www.passportjs.org/)
* [Express – Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)

---

  **[⬆ Наверх](#top)**      

239. ### <a name="239"></a> Unterschied zwischen lokaler Strategie und OAuth-Strategie in Passport.js?

### **Unterschied: Lokale Strategie vs. OAuth-Strategie in Passport.js**

---

### **Lokale Strategie (`passport-local`)**

* **Zweck:** Klassisches Login mit **Benutzername/E-Mail + Passwort**.
* **Ablauf:**

  1. User sendet Credentials an die App.
  2. Passport prüft sie mit DB (z. B. bcrypt/argon2-Hash).
  3. Bei Erfolg → `req.user` gesetzt.
* **Vorteil:** Vollständige Kontrolle (eigene Userdatenbank).
* **Nachteil:** App muss **Passwörter sicher speichern** und **Login-Schutzmechanismen** implementieren.

**Beispiel:**

```js
import { Strategy as LocalStrategy } from "passport-local";
import bcrypt from "bcrypt";

passport.use(new LocalStrategy(
  { usernameField: "email" },
  async (email, password, done) => {
    const user = await User.findOne({ where: { email } });
    if (!user) return done(null, false);
    const ok = await bcrypt.compare(password, user.passwordHash);
    return ok ? done(null, user) : done(null, false);
  }
));
```

---

### **OAuth-Strategie (z. B. `passport-google-oauth20`, `passport-github2`)**

* **Zweck:** Login über **externen Identity Provider (IdP)** wie Google, GitHub, Facebook.
* **Ablauf:**

  1. App leitet User zum IdP um.
  2. User loggt sich dort ein (ggf. MFA).
  3. IdP gibt Access Token/ID Token an die App zurück.
  4. Passport nutzt das Token, um Profildaten zu holen → `req.user`.
* **Vorteil:**

  * Keine Passwortverwaltung in der App.
  * Externe MFA/Policies nutzbar.
* **Nachteil:**

  * Abhängigkeit von externem Provider.
  * Einrichtung erfordert API-Keys, Callback-URLs.

**Beispiel:**

```js
import { Strategy as GoogleStrategy } from "passport-google-oauth20";

passport.use(new GoogleStrategy({
  clientID: process.env.GOOGLE_ID,
  clientSecret: process.env.GOOGLE_SECRET,
  callbackURL: "/auth/google/callback"
}, (_at, _rt, profile, done) => {
  const user = { id: profile.id, name: profile.displayName };
  done(null, user);
}));
```

---

### **Vergleich**

| Aspekt        | **Lokale Strategie**                     | **OAuth-Strategie**                           |
| ------------- | ---------------------------------------- | --------------------------------------------- |
| Login-Methode | Benutzername/E-Mail + Passwort           | Externer Provider (Google, GitHub, …)         |
| Credentials   | In eigener DB gespeichert & gehasht      | Bleiben beim Provider (App bekommt nur Token) |
| Sicherheit    | App muss Passwörter sicher managen       | Provider übernimmt Auth + MFA                 |
| UX            | Klassisch, Nutzer braucht Account in App | Bequem, „Login mit …“                         |
| Abhängigkeit  | Keine externe                            | Abhängig von IdP                              |

---

### **Zusammenfassung**

* **Lokale Strategie**: App verwaltet Credentials selbst (klassisches Passwort-Login).
* **OAuth-Strategie**: Login über externen IdP (Google, GitHub, etc.), App bekommt Tokens/Profildaten.
* Entscheidung: **Kontrolle & Unabhängigkeit** (Local) vs. **Komfort & Sicherheit** (OAuth).

🔗 Quellen

* [Passport Local](http://www.passportjs.org/packages/passport-local/)
* [Passport Google OAuth20](http://www.passportjs.org/packages/passport-google-oauth20/)
* [MDN – OAuth](https://developer.mozilla.org/en-US/docs/Glossary/OAuth)

---

  **[⬆ Наверх](#top)**      

240. ### <a name="240"></a> Wie testet man Authentifizierungs- und Autorisierungslogik in einer Express-App?

### **Strategie: AuthN/AuthZ testen in Express**

* **Ebenen trennen:**

  1. **Unit-Tests** für Krypto/Token (Passwort-Hash, JWT-Verify).
  2. **Middleware-Tests** (requireAuth/requireRole).
  3. **Integrationstests** der Routen mit **Supertest** (positiv/negativ, Cookies/Headers).
* **Fälle abdecken:** Happy-Path, fehlende/abgelaufene Tokens, falsche Rollen, Manipulation, Ratenbegrenzung (falls vorhanden).
* **Test-Daten:** Seed/Fixtures; für DB: separate Test-DB (z. B. PostgreSQL im Docker) oder In-Memory-Ansatz, Transaktionen je Test zurückrollen.

---

### **1) Unit: Passwort-Hash & JWT**

```js
// __tests__/crypto.test.mjs
import { test, expect } from "@jest/globals";
import bcrypt from "bcrypt";
import jwt from "jsonwebtoken";

const SECRET = "test_secret";

test("bcrypt verifiziert korrekt", async () => {
  const hash = await bcrypt.hash("s3cret", 12);
  await expect(bcrypt.compare("s3cret", hash)).resolves.toBe(true);
  await expect(bcrypt.compare("wrong", hash)).resolves.toBe(false);
});

test("JWT Sign/Verify + Ablauf", async () => {
  const token = jwt.sign({ sub: "u1", role: "user" }, SECRET, { expiresIn: "1s" });
  const payload = jwt.verify(token, SECRET);
  expect(payload.sub).toBe("u1");

  // Ablauf simulieren
  await new Promise(r => setTimeout(r, 1100));
  expect(() => jwt.verify(token, SECRET)).toThrow(/jwt expired/i);
});
```

---

### **2) Middleware: requireAuth (JWT)**

```js
// middleware/requireAuth.mjs
import jwt from "jsonwebtoken";
export const requireAuth = (req, res, next) => {
  const raw = req.headers.authorization ?? "";
  const token = raw.startsWith("Bearer ") ? raw.slice(7) : null;
  if (!token) return res.status(401).json({ error: "No token" });
  try {
    req.user = jwt.verify(token, process.env.JWT_SECRET, {
      algorithms: ["HS256"], issuer: "https://auth.example.com", audience: "example.api"
    });
    next();
  } catch { return res.status(403).json({ error: "Invalid/expired token" }); }
};
```

```js
// __tests__/requireAuth.test.mjs
import { test, expect } from "@jest/globals";
import express from "express";
import request from "supertest";
import jwt from "jsonwebtoken";
import { requireAuth } from "../middleware/requireAuth.mjs";

process.env.JWT_SECRET = "test_secret";

function mkApp() {
  const app = express();
  app.get("/private", requireAuth, (req, res) => res.json({ sub: req.user.sub }));
  return app;
}

test("401 ohne Token", async () => {
  const app = mkApp();
  const r = await request(app).get("/private");
  expect(r.status).toBe(401);
});

test("403 bei ungültigem Token", async () => {
  const app = mkApp();
  const r = await request(app).get("/private").set("Authorization", "Bearer bad");
  expect(r.status).toBe(403);
});

test("200 mit gültigem Token", async () => {
  const app = mkApp();
  const t = jwt.sign({ sub: "u1" }, process.env.JWT_SECRET, { issuer: "https://auth.example.com", audience: "example.api" });
  const r = await request(app).get("/private").set("Authorization", `Bearer ${t}`);
  expect(r.status).toBe(200);
  expect(r.body.sub).toBe("u1");
});
```

---

### **3) RBAC: Rollen prüfen**

```js
// middleware/rbac.mjs
export const requireRole = (...roles) => (req, res, next) =>
  req.user && roles.includes(req.user.role)
    ? next()
    : res.status(403).json({ error: "Forbidden" });
```

```js
// __tests__/rbac.test.mjs
import { test, expect } from "@jest/globals";
import express from "express";
import request from "supertest";
import { requireRole } from "../middleware/rbac.mjs";

test("403 wenn Rolle fehlt", async () => {
  const app = express();
  app.use((req, _res, next) => { req.user = { role: "user" }; next(); });
  app.delete("/admin", requireRole("admin"), (_req, res) => res.sendStatus(204));

  const r = await request(app).delete("/admin");
  expect(r.status).toBe(403);
});
```

---

### **4) Integration: Session-Auth (Cookies)**

```js
// __tests__/session-auth.test.mjs
import { test, expect } from "@jest/globals";
import express from "express";
import session from "express-session";
import request from "supertest";

function mkApp() {
  const app = express();
  app.use(express.json());
  app.use(session({ secret: "t", resave: false, saveUninitialized: false }));
  app.post("/login", (req, res) => { req.session.user = { id: "u1", role: "user" }; res.sendStatus(204); });
  const requireSession = (req, res, next) => req.session.user ? next() : res.sendStatus(401);
  app.get("/me", requireSession, (req, res) => res.json(req.session.user));
  return app;
}

test("persistente Session via supertest.agent()", async () => {
  const app = mkApp();
  const agent = request.agent(app);
  await agent.post("/login").send({ email: "a@b.c", password: "x" }).expect(204);
  const r = await agent.get("/me").expect(200);
  expect(r.body.id).toBe("u1");
});
```

---

### **5) DB-gestützte Tests (Sequelize/Postgres)**

* **Vor jedem Test:** Transaktion starten, Daten seeden.
* **Nach jedem Test:** Rollback → saubere Isolation.

```js
// jest.setup.mjs
import { sequelize } from "../src/db.mjs";
beforeEach(async () => { global.__tx = await sequelize.transaction(); });
afterEach(async () => { await global.__tx.rollback(); });

// In Repositories/Controller: Transaktion aus Context/CLS übernehmen (oder explizit injizieren).
```

---

### **6) Weitere Prüfungen**

* **CORS/Preflight** nur für erlaubte Origins.
* **Rate Limiting** auf `/auth/login` (z. B. 429 nach X Fehlversuchen).
* **CSRF** bei Session-Cookies: Token-Check in Tests simulieren (Hidden-Field/Header).
* **Security-Header** (Helmet) vorhanden? Minimaltest: `X-Content-Type-Options`, `X-Frame-Options`, `Content-Security-Policy` falls konfiguriert.

---

### **Tipps**

* **Supertest** für End-to-End über Express ohne echten Port.
* **Fake Timers** bei Ablauf/TTL-Logik (`jest.useFakeTimers()` → `advanceTimersByTimeAsync`).
* **Fixtures/Factories** für Nutzer/Rollen, eindeutige Seeds.
* **Mocking**: E-Mail/SMS/OAuth-Provider mit Mocks/Fakes testen, nicht real callen.

---

### **Zusammenfassung**

* **Unit**: Krypto & JWT separat prüfen.
* **Middleware**: `requireAuth`/`requireRole` direkt testen (401/403/200).
* **Integration**: komplette Flows mit **Supertest** (JWT-Header oder **Sessions mit `agent`**).
* **DB-Isolation**, **Ablauf/TTL** mit Fake Timern, externe Dienste mocken.

**Quellen**

* **Express**: [Using middleware](https://expressjs.com/de/guide/using-middleware.html) • [Security Best Practices](https://expressjs.com/de/advanced/best-practice-security.html)
* **Node.js**: [`crypto`](https://nodejs.org/docs/latest/api/crypto.html)
* **MDN**: [HTTP Status 401/403](https://developer.mozilla.org/ru/docs/Web/HTTP/Status)
* **Jest**: [Asynchronous Testing](https://jestjs.io/docs/asynchronous) • [Timer Mocks](https://jestjs.io/docs/timer-mocks)
* **Supertest**: [GitHub – supertest](https://github.com/ladjs/supertest)
* **Sequelize**: [Transactions](https://sequelize.org/docs/v6/other-topics/transactions/)


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
