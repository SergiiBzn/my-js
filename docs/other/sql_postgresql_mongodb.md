<a name="top"></a>

[На главную](../README.md)

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
|   | SQL |
|1 | [Was ist SQL und wofür wird es verwendet?](#1) |
|2 | [Unterschied zwischen SQL und NoSQL?](#2) |
|3 | [Was ist ein Primärschlüssel?](#3) |
|4 | [Was ist ein Fremdschlüssel?](#4) |
|5 | [Unterschied zwischen PRIMARY KEY, UNIQUE und INDEX?](#5) |
|6 | [Was sind Normalformen und warum sind sie wichtig?](#6) |
|7 | [Unterschied zwischen 1NF, 2NF und 3NF?](#7) |
|8 | [Was sind Transaktionen in SQL?](#8) |
|9 | [Was bedeutet ACID in Datenbanken?](#9) |
|10 | [Unterschied zwischen ACID und BASE Prinzipien?](#10) |
|11 | [Unterschied zwischen SELECT * und gezielten Spaltenabfragen?](#11) |
|12 | [Unterschied zwischen INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN?](#12) |
|13 | [Unterschied zwischen WHERE und HAVING?](#13) |
|14 | [Unterschied zwischen DISTINCT und GROUP BY?](#14) |
|15 | [Was sind Aggregatfunktionen (COUNT, SUM, AVG, MIN, MAX)?](#15) |
|16 | [Wie funktioniert ORDER BY und LIMIT?](#16) |
|17 | [Was ist ein Subquery (Unterabfrage)?](#17) |
|18 | [Unterschied zwischen korrelierter und nicht-korrelierter Unterabfrage?](#18) |
|19 | [Unterschied zwischen EXISTS und IN?](#19) |
|20 | [Unterschied zwischen UNION und UNION ALL?](#20) |
|   | PostgreSQL |
|21 | [Was ist PostgreSQL und welche Vorteile hat es gegenüber MySQL?](#21) |
|22 | [Was sind Datentypen in PostgreSQL (TEXT, VARCHAR, SERIAL, JSONB)?](#22) |
|23 | [Unterschied zwischen SERIAL und BIGSERIAL?](#23) |
|24 | [Wie arbeitet PostgreSQL mit Arrays?](#24) |
|25 | [Was ist der Unterschied zwischen JSON und JSONB in PostgreSQL?](#25) |
|26 | [Wie speichert und verarbeitet PostgreSQL Zeitstempel (TIMESTAMP, TIMESTAMPTZ)?](#26) |
|27 | [Was sind Sequences in PostgreSQL?](#27) |
|28 | [Wie implementiert man Auto-Increment in PostgreSQL?](#28) |
|29 | [Was sind Materialized Views?](#29) |
|30 | [Unterschied zwischen View und Materialized View?](#30) |
|31 | [Was ist ein Index in PostgreSQL?](#31) |
|32 | [Unterschied zwischen B-Tree, Hash und GIN Index?](#32) |
|33 | [Was ist ein Unique Index?](#33) |
|34 | [Nachteile von zu vielen Indexen?](#34) |
|35 | [Wie analysiert man eine Query mit EXPLAIN?](#35) |
|36 | [Unterschied zwischen EXPLAIN und EXPLAIN ANALYZE?](#36) |
|37 | [Wie vermeidet man Table Scans?](#37) |
|38 | [Was ist ein Partial Index?](#38) |
|39 | [Was ist ein Covering Index (INCLUDE)?](#39) |
|40 | [Wie funktioniert Vacuum in PostgreSQL?](#40) |
|41 | [Wie startet und beendet man eine Transaktion?](#41) |
|42 | [Unterschied zwischen COMMIT und ROLLBACK?](#42) |
|43 | [Was ist ein Savepoint in SQL?](#43) |
|44 | [Unterschied zwischen Deadlock und Race Condition?](#44) |
|45 | [Welche Isolation Levels gibt es in PostgreSQL (READ COMMITTED, SERIALIZABLE)?](#45) |
|46 | [Unterschied zwischen Optimistic Locking und Pessimistic Locking?](#46) |
|47 | [Wie erkennt PostgreSQL Deadlocks?](#47) |
|48 | [Welche Standard-Isolationsebene nutzt PostgreSQL?](#48) |
|49 | [Wie implementiert man Transaktionen in Node.js/Express mit PostgreSQL?](#49) |
|50 | [Unterschied zwischen BEGIN und START TRANSACTION?](#50) |
|51 | [Wie verwaltet man Benutzer und Rollen in PostgreSQL?](#51) |
|52 | [Unterschied zwischen Login-Rollen und Gruppen-Rollen?](#52) |
|53 | [Wie vergibt man Berechtigungen (GRANT, REVOKE)?](#53) |
|54 | [Was ist Row Level Security (RLS) in PostgreSQL?](#54) |
|55 | [Wie schützt man sensible Daten (z. B. Passwörter) in PostgreSQL?](#55) |
|56 | [Wie sichert man eine PostgreSQL-Datenbank (pg_dump)?](#56) |
|57 | [Wie stellt man ein Backup wieder her?](#57) |
|58 | [Unterschied zwischen pg_dump und pg_restore?](#58) |
|59 | [Wie konfiguriert man SSL für PostgreSQL-Verbindungen?](#59) |
|60 | [Was ist Connection Pooling und wie implementiert man es (z. B. mit pg-pool in Node.js)?](#60) |
|   | MongoDB |
|61 | [Was ist MongoDB und wofür wird es verwendet?](#61) |
|62 | [Unterschied zwischen SQL und NoSQL?](#62) |
|63 | [Was ist der Unterschied zwischen Dokument, Collection und Datenbank?](#63) |
|64 | [Was ist BSON und wie unterscheidet es sich von JSON?](#64) |
|65 | [Was ist ein ObjectId und warum wird es genutzt?](#65) |
|66 | [Wie fügt man Dokumente ein (insertOne, insertMany)?](#66) |
|67 | [Wie liest man Daten (find, findOne)?](#67) |
|68 | [Unterschied zwischen find(), findOne() und findById() in Mongoose?](#68) |
|69 | [Wie aktualisiert man Dokumente (updateOne, updateMany, findByIdAndUpdate)?](#69) |
|70 | [Wie löscht man Dokumente (deleteOne, deleteMany, findByIdAndDelete)?](#70) |
|71 | [Was ist Mongoose und warum wird es häufig in Node/Express-Projekten verwendet?](#71) |
|72 | [Unterschied zwischen Schema und Model in Mongoose?](#72) |
|73 | [Wie definiert man Validierungen in einem Schema?](#73) |
|74 | [Was sind Virtuals und Middleware (pre, post) in Mongoose?](#74) |
|75 | [Wie funktioniert populate in Mongoose (Beziehungen zwischen Dokumenten)?](#75) |
|76 | [Welche Vergleichsoperatoren gibt es ($gt, $lt, $in, $nin, $eq)?](#76) |
|77 | [Wie sucht man mit $and, $or, $nor?](#77) |
|78 | [Wie sucht man in Arrays ($elemMatch, $push, $pull)?](#78) |
|79 | [Unterschied zwischen sort, limit und skip?](#79) |
|80 | [Was ist der Unterschied zwischen countDocuments() und estimatedDocumentCount()?](#80) |
|81 | [Was ist eine Aggregation Pipeline und wofür wird sie verwendet?](#81) |
|82 | [Welche Stages gibt es ($match, $group, $project, $sort, $limit)?](#82) |
|83 | [Was sind Indexe und warum sind sie wichtig?](#83) |
|84 | [Unterschied zwischen Single-Field Index und Compound Index?](#84) |
|85 | [Was ist ein Unique-Index?](#85) |
|86 | [Was ist Sharding und Replikation in MongoDB?](#86) |
|87 | [Was ist ein Replica Set und warum ist es wichtig?](#87) |
|88 | [Wie optimiert man Queries in MongoDB (Explain, Indexe)?](#88) |
|89 | [Wie schützt man MongoDB vor unautorisiertem Zugriff?](#89) |
|90 | [Unterschied zwischen Rollen und Berechtigungen (z. B. read, readWrite)?](#90) |
|91 | [](#91) |
|92 | [](#92) |
|93 | [](#93) |
|94 | [](#94) |
|95 | [](#95) |
|96 | [](#96) |
|97 | [](#97) |
|98 | [](#98) |
|99 | [](#99) |
|100 | [](#100) |
|101 | [](#101) |
|102 | [](#102) |
|103 | [](#103) |
|104 | [](#104) |
|105 | [](#105) |
|106 | [](#106) |
|107 | [](#107) |
|108 | [](#108) |
|109 | [](#109) |
|110 | [](#110) |
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


  **[⬆ Наверх](#top)**
  
1. ### <a name="1"></a> Was ist SQL und wofür wird es verwendet?

**SQL (Structured Query Language)** ist eine standardisierte Sprache zur Arbeit mit relationalen Datenbanken.
Sie dient dazu:

* **Daten zu definieren** (Tabellen, Schemata) → *Data Definition Language (DDL)*
* **Daten zu manipulieren** (Einfügen, Aktualisieren, Löschen) → *Data Manipulation Language (DML)*
* **Daten abzufragen** (Selektieren, Filtern, Aggregieren) → *Data Query Language (DQL)*
* **Zugriffsrechte zu steuern** → *Data Control Language (DCL)*

### Beispiel:

```sql
-- Tabelle erstellen (DDL)
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100) UNIQUE
);

-- Daten einfügen (DML)
INSERT INTO users (name, email)
VALUES ('Max Mustermann', 'max@example.com');

-- Daten abfragen (DQL)
SELECT id, name
FROM users
WHERE email LIKE '%example.com';
```

SQL wird in relationalen Datenbanksystemen wie **PostgreSQL**, **MySQL**, **SQLite**, **Oracle DB** und **MS SQL Server** verwendet.

---

**Zusammenfassung:**
SQL ist die Standardsprache zur Definition, Abfrage und Manipulation von Daten in relationalen Datenbanken.

📖 Quellen:

* [PostgreSQL Dokumentation – SQL](https://www.postgresql.org/docs/current/sql.html)
* [MDN – SQL Einführung (RU)](https://developer.mozilla.org/ru/docs/Glossary/SQL)

---

  **[⬆ Наверх](#top)**

2. ### <a name="2"></a> Unterschied zwischen SQL und NoSQL?

**SQL (relational) vs. NoSQL (nicht-relational):**

### 1. **Datenmodell**

* **SQL:** Tabellenbasiert, mit Zeilen und Spalten. Starke Beziehungen (Relations).
* **NoSQL:** Flexible Modelle – Dokumente (MongoDB), Key-Value (Redis), Spalten (Cassandra), Graphen (Neo4j).

### 2. **Schema**

* **SQL:** Strenges, festes Schema (z. B. `VARCHAR(100)` für eine Spalte). Änderungen erfordern Migration.
* **NoSQL:** Schemafrei oder sehr flexibel. Neue Felder können einfach hinzugefügt werden.

### 3. **Skalierung**

* **SQL:** Vertikale Skalierung (stärkere Server). Horizontale Skalierung oft komplexer.
* **NoSQL:** Für horizontale Skalierung entworfen (Sharding, Replikation).

### 4. **Transaktionen**

* **SQL:** ACID-konform (Atomicity, Consistency, Isolation, Durability). Hohe Datenintegrität.
* **NoSQL:** Oft BASE-Prinzip (Basically Available, Soft state, Eventually consistent). Schneller, aber weniger strikt.

### 5. **Abfragesprache**

* **SQL:** Einheitliche Standardsprache (z. B. `SELECT`, `JOIN`).
* **NoSQL:** Unterschiedliche APIs oder abfrageähnliche Sprachen je nach DB (z. B. MongoDB mit `find()`).

---

### Beispiel SQL (PostgreSQL)

```sql
-- Benutzer mit Email abfragen
SELECT * FROM users WHERE email = 'max@example.com';
```

### Beispiel NoSQL (MongoDB)

```js
// Dokument aus der Collection users abfragen
db.users.find({ email: "max@example.com" });
```

---

**Zusammenfassung:**

* **SQL** → relational, streng, ACID, für komplexe Beziehungen und Integrität.
* **NoSQL** → flexibel, schemafrei, skalierbar, oft schneller für große unstrukturierte Datenmengen.

📖 Quellen:

* [PostgreSQL Docs – SQL](https://www.postgresql.org/docs/current/sql.html)
* [MongoDB – What is NoSQL?](https://www.mongodb.com/nosql-explained)
* [MDN – SQL Glossar (RU)](https://developer.mozilla.org/ru/docs/Glossary/SQL)

---

  **[⬆ Наверх](#top)**

3. ### <a name="3"></a> Was ist ein Primärschlüssel?

**Primärschlüssel (Primary Key)** ist ein Attribut oder eine Kombination von Attributen in einer Tabelle, das jeden Datensatz eindeutig identifiziert.

### Eigenschaften:

* **Eindeutigkeit:** Kein doppelter Wert erlaubt.
* **Nicht-Null:** Jeder Datensatz muss einen Primärschlüssel haben.
* **Stabilität:** Sollte sich nicht häufig ändern.
* **Nur ein Primärschlüssel pro Tabelle**, aber er kann aus mehreren Spalten bestehen (*komposit*).

---

### Beispiel in SQL (PostgreSQL)

```sql
-- Einfacher Primärschlüssel
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100)
);

-- Komposit-Schlüssel (zwei Spalten bilden den Primary Key)
CREATE TABLE orders (
  order_id INT,
  product_id INT,
  PRIMARY KEY (order_id, product_id)
);
```

---

### Warum wichtig?

* Sichert **Eindeutigkeit** der Daten.
* Ermöglicht effiziente **Indizierung und Suche**.
* Grundlage für **Beziehungen (FOREIGN KEYS)** zwischen Tabellen.

---

**Zusammenfassung:**
Ein Primärschlüssel ist ein eindeutiges Feld oder Feldkombination in einer Tabelle, das jeden Datensatz identifiziert und keine NULL-Werte zulässt.

📖 Quellen:

* [PostgreSQL Docs – Constraints](https://www.postgresql.org/docs/current/ddl-constraints.html)
* [MDN Glossar – Primary Key (RU)](https://developer.mozilla.org/ru/docs/Glossary/Primary_key)

---

  **[⬆ Наверх](#top)**

4. ### <a name="4"></a> Was ist ein Fremdschlüssel?

**Fremdschlüssel (Foreign Key)** ist eine Spalte oder eine Kombination von Spalten, die auf den **Primärschlüssel einer anderen Tabelle** verweist.
Er stellt eine **Beziehung zwischen zwei Tabellen** her und sorgt für **Datenintegrität**.

---

### Eigenschaften:

* Muss auf einen gültigen Wert im Primärschlüssel der referenzierten Tabelle zeigen.
* Verhindert das Einfügen von Werten, die nicht existieren.
* Kann mit **ON DELETE** oder **ON UPDATE** Regeln kombiniert werden (z. B. `CASCADE`, `SET NULL`).

---

### Beispiel in SQL (PostgreSQL)

```sql
-- Tabelle users
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100)
);

-- Tabelle orders mit Fremdschlüssel auf users.id
CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  user_id INT,
  product VARCHAR(100),
  CONSTRAINT fk_user FOREIGN KEY (user_id)
    REFERENCES users (id)
    ON DELETE CASCADE
);
```

* Wenn ein **User gelöscht wird**, werden durch `ON DELETE CASCADE` automatisch auch alle seine Bestellungen gelöscht.

---

### Nutzen:

* Sichert **Referenzielle Integrität**.
* Verbindet Daten logisch über Tabellen hinweg.
* Ermöglicht **Joins** zwischen Tabellen.

---

**Zusammenfassung:**
Ein Fremdschlüssel ist ein Attribut in einer Tabelle, das auf den Primärschlüssel einer anderen Tabelle verweist und so die Beziehung zwischen den Tabellen sicherstellt.

📖 Quellen:

* [PostgreSQL Docs – Foreign Keys](https://www.postgresql.org/docs/current/ddl-constraints.html#DDL-CONSTRAINTS-FK)
* [MDN Glossar – Foreign Key (RU)](https://developer.mozilla.org/ru/docs/Glossary/Foreign_key)

---

  **[⬆ Наверх](#top)**

5. ### <a name="5"></a> Unterschied zwischen PRIMARY KEY, UNIQUE und INDEX?

### **1. PRIMARY KEY**

* Eindeutiger Bezeichner für jede Zeile.
* Impliziert automatisch **NOT NULL** und **UNIQUE**.
* Nur **ein PRIMARY KEY pro Tabelle**, kann aber aus mehreren Spalten bestehen (*komposit*).
* Wird intern automatisch indiziert.

**Beispiel:**

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(100)
);
```

---

### **2. UNIQUE**

* Erzwingt, dass Werte in der Spalte oder Spaltenkombination **eindeutig** sind.
* Mehrere `UNIQUE`-Constraints pro Tabelle möglich.
* **NULL**-Werte sind erlaubt (abhängig vom DBMS, in PostgreSQL mehrfach `NULL`).

**Beispiel:**

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(100) UNIQUE
);
```

---

### **3. INDEX**

* Datenbankstruktur zur **Beschleunigung von Such- und Sortieroperationen**.
* Keine Einschränkung der Daten, nur Performance-Optimierung.
* Mehrere Indizes pro Tabelle möglich.
* Kann auch **auf nicht eindeutigen Spalten** erstellt werden.

**Beispiel:**

```sql
-- Index auf Spalte name
CREATE INDEX idx_users_name ON users (name);
```

---

### **Vergleich:**

| Merkmal            | PRIMARY KEY    | UNIQUE          | INDEX                     |
| ------------------ | -------------- | --------------- | ------------------------- |
| Eindeutigkeit      | Ja             | Ja              | Nein (außer UNIQUE Index) |
| NULL erlaubt       | Nein           | Ja (PostgreSQL) | Ja                        |
| Anzahl pro Tabelle | 1              | Beliebig viele  | Beliebig viele            |
| Hauptzweck         | Identifikation | Datenintegrität | Performance               |
| Automatisch Index? | Ja             | Ja              | Ja (aber nur manuell)     |

---

**Zusammenfassung:**

* **PRIMARY KEY** = eindeutiger Identifikator (einmal pro Tabelle).
* **UNIQUE** = verhindert Duplikate, aber erlaubt `NULL`.
* **INDEX** = dient nur der Performance, erzwingt keine Eindeutigkeit.

📖 Quellen:

* [PostgreSQL Docs – Constraints](https://www.postgresql.org/docs/current/ddl-constraints.html)
* [PostgreSQL Docs – Indexes](https://www.postgresql.org/docs/current/indexes.html)
* [MDN Glossar – Primary Key](https://developer.mozilla.org/ru/docs/Glossary/Primary_key)

---

  **[⬆ Наверх](#top)**

6. ### <a name="6"></a> Was sind Normalformen und warum sind sie wichtig?

### **Normalformen in relationalen Datenbanken**

**Definition:**
Normalformen sind Regeln zur **Strukturierung von Tabellen**, damit Redundanz, Inkonsistenzen und Anomalien beim Einfügen, Aktualisieren oder Löschen von Daten vermieden werden.

---

### **1. Normalform (1NF)**

* Alle Attribute enthalten **atomare Werte** (keine Listen oder Arrays).
* Keine mehrfachen oder wiederholenden Spalten.

**Beispiel – falsch (nicht 1NF):**

```sql
-- Spalte enthält mehrere Werte
CREATE TABLE customers (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  phones TEXT -- "12345, 67890"
);
```

**Korrekt (1NF):**

```sql
CREATE TABLE phones (
  id SERIAL PRIMARY KEY,
  customer_id INT REFERENCES customers(id),
  phone VARCHAR(20)
);
```

---

### **2. Normalform (2NF)**

* Erfüllt 1NF.
* Jedes Nicht-Schlüssel-Attribut hängt **vollständig vom Primärschlüssel** ab, nicht nur von einem Teil davon.
* Gilt nur für Tabellen mit **kompositem Primärschlüssel**.

---

### **3. Normalform (3NF)**

* Erfüllt 2NF.
* Keine **transitiven Abhängigkeiten** (ein Attribut hängt nicht von einem anderen Nicht-Schlüssel-Attribut ab).

**Beispiel – schlecht (nicht 3NF):**

```sql
CREATE TABLE orders (
  order_id SERIAL PRIMARY KEY,
  customer_id INT,
  customer_city VARCHAR(100) -- hängt vom Kunden, nicht von der Bestellung ab
);
```

**Besser (3NF):**

```sql
CREATE TABLE customers (
  id SERIAL PRIMARY KEY,
  city VARCHAR(100)
);

CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  customer_id INT REFERENCES customers(id)
);
```

---

### **Weitere Normalformen:**

* **BCNF (Boyce-Codd-Normalform):** Strengere Version von 3NF.
* **4NF/5NF:** Selten in der Praxis, behandeln mehrfache Abhängigkeiten und Join-Abhängigkeiten.

---

### **Warum wichtig?**

* **Vermeidung von Redundanz** → spart Speicherplatz.
* **Vermeidung von Anomalien** beim INSERT/UPDATE/DELETE.
* **Bessere Datenintegrität**.
* **Effiziente Abfragen** durch klare Beziehungen.

---

**Zusammenfassung:**
Normalformen sind Stufen der Datenbanknormalisierung, die sicherstellen, dass Tabellen logisch strukturiert sind, Redundanz vermeiden und Datenintegrität sichern. In der Praxis werden meist **1NF bis 3NF** umgesetzt.

📖 Quellen:

* [PostgreSQL Docs – Database Design](https://www.postgresql.org/docs/current/ddl.html)
* [MDN Glossar – Normalization (RU)](https://developer.mozilla.org/ru/docs/Glossary/Database_normalization)

---

  **[⬆ Наверх](#top)**

7. ### <a name="7"></a> Unterschied zwischen 1NF, 2NF und 3NF?

### **Unterschied zwischen 1NF, 2NF und 3NF**

---

### **1. Normalform (1NF)**

* Alle Attribute enthalten **atomare Werte** (keine Arrays oder mehrfachen Werte in einer Spalte).
* Keine wiederholenden Spalten.

**Beispiel (nicht 1NF):**

```sql
CREATE TABLE customers (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  phones TEXT -- "12345,67890"
);
```

**Korrekt (1NF):**

```sql
CREATE TABLE phones (
  id SERIAL PRIMARY KEY,
  customer_id INT REFERENCES customers(id),
  phone VARCHAR(20)
);
```

---

### **2. Normalform (2NF)**

* Erfüllt **1NF**.
* Alle Nicht-Schlüssel-Attribute hängen **vollständig vom gesamten Primärschlüssel** ab, nicht nur von einem Teil.
* Relevant bei **kompositem Primärschlüssel**.

**Beispiel (nicht 2NF):**

```sql
CREATE TABLE order_items (
  order_id INT,
  product_id INT,
  product_name VARCHAR(100), -- hängt nur von product_id ab
  PRIMARY KEY (order_id, product_id)
);
```

**Korrekt (2NF):**

```sql
CREATE TABLE products (
  id INT PRIMARY KEY,
  name VARCHAR(100)
);

CREATE TABLE order_items (
  order_id INT,
  product_id INT REFERENCES products(id),
  PRIMARY KEY (order_id, product_id)
);
```

---

### **3. Normalform (3NF)**

* Erfüllt **2NF**.
* Keine **transitiven Abhängigkeiten**: Ein Nicht-Schlüssel-Attribut darf nicht von einem anderen Nicht-Schlüssel-Attribut abhängen.

**Beispiel (nicht 3NF):**

```sql
CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  customer_id INT,
  customer_city VARCHAR(100) -- hängt von customer_id ab, nicht von der Bestellung
);
```

**Korrekt (3NF):**

```sql
CREATE TABLE customers (
  id SERIAL PRIMARY KEY,
  city VARCHAR(100)
);

CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  customer_id INT REFERENCES customers(id)
);
```

---

### **Vergleich in Kurzform**

| Normalform | Regel                                                                  | Fokus                            |
| ---------- | ---------------------------------------------------------------------- | -------------------------------- |
| **1NF**    | Nur atomare Werte, keine Wiederholungen                                | Struktur der Spalten             |
| **2NF**    | 1NF + keine partielle Abhängigkeit vom Teil eines zusammengesetzten PK | Abhängigkeit vom Primärschlüssel |
| **3NF**    | 2NF + keine transitive Abhängigkeit                                    | Trennung unabhängiger Infos      |

---

**Zusammenfassung:**

* **1NF** → Atomare Werte, keine Wiederholungen.
* **2NF** → Keine partielle Abhängigkeit von Teil-Schlüssel.
* **3NF** → Keine transitive Abhängigkeit von Nicht-Schlüssel-Attributen.

📖 Quellen:

* [PostgreSQL Docs – Database Design](https://www.postgresql.org/docs/current/ddl.html)
* [MDN Glossar – Normalization (RU)](https://developer.mozilla.org/ru/docs/Glossary/Database_normalization)

---

  **[⬆ Наверх](#top)**

8. ### <a name="8"></a> Was sind Transaktionen in SQL?

### **Transaktionen in SQL**

Eine **Transaktion** ist eine logische Einheit von Datenbankoperationen, die entweder **vollständig** oder **gar nicht** ausgeführt wird.
Sie sorgt für **Datenkonsistenz** und folgt den **ACID-Prinzipien**:

* **Atomicity** → Alles oder nichts wird ausgeführt.
* **Consistency** → Daten bleiben nach Transaktion in konsistentem Zustand.
* **Isolation** → Gleichzeitige Transaktionen beeinflussen sich nicht.
* **Durability** → Änderungen bleiben auch nach Systemabsturz erhalten.

---

### **Beispiel in SQL (PostgreSQL)**

```sql
BEGIN; -- Start der Transaktion

-- 1. Geld vom Konto A abbuchen
UPDATE accounts
SET balance = balance - 100
WHERE id = 1;

-- 2. Geld auf Konto B überweisen
UPDATE accounts
SET balance = balance + 100
WHERE id = 2;

COMMIT; -- Änderungen dauerhaft speichern
```

Falls während der Transaktion ein Fehler passiert:

```sql
ROLLBACK; -- Alle Änderungen rückgängig machen
```

---

### **Isolation Levels (PostgreSQL unterstützt 4 Stufen):**

1. **READ UNCOMMITTED** – unsichere Reads möglich.
2. **READ COMMITTED** – nur bestätigte Daten sichtbar (Standard in PostgreSQL).
3. **REPEATABLE READ** – gleiche Abfrage liefert immer identische Ergebnisse innerhalb der Transaktion.
4. **SERIALIZABLE** – maximale Isolation, Transaktionen wirken wie nacheinander ausgeführt.

---

**Zusammenfassung:**
Transaktionen sind logische Blöcke mehrerer SQL-Operationen, die mit **ACID-Sicherheit** ausgeführt werden. Sie stellen sicher, dass Daten konsistent bleiben, auch bei Fehlern oder parallelen Zugriffen.

📖 Quellen:

* [PostgreSQL Docs – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)
* [MDN Glossar – ACID (RU)](https://developer.mozilla.org/ru/docs/Glossary/ACID)

---

  **[⬆ Наверх](#top)**

9. ### <a name="9"></a> Was bedeutet ACID in Datenbanken?

### **ACID-Prinzip in Datenbanken**

ACID beschreibt die vier Kern­eigenschaften, die eine **Transaktion** in einem relationalen Datenbanksystem erfüllen muss:

---

### **1. Atomicity (Atomarität)**

* Eine Transaktion wird **vollständig oder gar nicht** ausgeführt.
* Fehler → alle Änderungen werden mit `ROLLBACK` rückgängig gemacht.

**Beispiel:** Geldüberweisung → entweder beide Konten werden angepasst, oder keins.

---

### **2. Consistency (Konsistenz)**

* Die Transaktion überführt die Datenbank von einem **konsistenten Zustand** in einen anderen.
* Regeln wie **Constraints, Datentypen, Trigger** werden eingehalten.

**Beispiel:** Ein negativer Kontostand ist nicht erlaubt → die Transaktion schlägt fehl.

---

### **3. Isolation (Isolation)**

* Gleichzeitige Transaktionen beeinflussen sich nicht gegenseitig.
* Isolation Levels (PostgreSQL):

  * **READ COMMITTED** (Standard)
  * **REPEATABLE READ**
  * **SERIALIZABLE**

**Beispiel:** Zwei Nutzer lesen und schreiben gleichzeitig denselben Datensatz, ohne dass Inkonsistenzen entstehen.

---

### **4. Durability (Dauerhaftigkeit)**

* Nach einem `COMMIT` bleiben Änderungen **dauerhaft gespeichert**, auch bei Absturz oder Stromausfall.
* Daten werden im **Write-Ahead-Log (WAL)** gesichert.

---

### **ACID in SQL-Beispiel**

```sql
BEGIN;

UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;

COMMIT; -- garantiert ACID-Sicherheit
```

---

**Zusammenfassung:**
ACID = **Atomicity, Consistency, Isolation, Durability**.
Diese Prinzipien garantieren sichere, konsistente und zuverlässige Transaktionen in Datenbanken.

📖 Quellen:

* [PostgreSQL Docs – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)
* [MDN Glossar – ACID (RU)](https://developer.mozilla.org/ru/docs/Glossary/ACID)

---

  **[⬆ Наверх](#top)**

10. ### <a name="10"></a> Unterschied zwischen ACID und BASE Prinzipien?

### **Unterschied zwischen ACID und BASE Prinzipien**

---

### **ACID (klassische SQL-Datenbanken)**

Fokus: **Korrektheit und Integrität der Daten**

1. **Atomicity** → Alles oder nichts wird ausgeführt
2. **Consistency** → Regeln und Constraints bleiben erhalten
3. **Isolation** → Parallele Transaktionen beeinflussen sich nicht
4. **Durability** → Änderungen sind dauerhaft gespeichert

➡️ Geeignet für **Banken, Finanzsysteme, Buchhaltung** – wo absolute Datenintegrität nötig ist.

---

### **BASE (häufig in NoSQL-Datenbanken)**

Fokus: **Verfügbarkeit und Skalierbarkeit**

1. **Basically Available** → Das System ist immer verfügbar, auch bei Teilfehlern
2. **Soft State** → Daten können sich ändern, auch ohne direkte Eingriffe (z. B. durch Replikation)
3. **Eventually Consistent** → Daten werden über Zeit konsistent, aber nicht sofort

➡️ Geeignet für **verteilte Systeme, Social Media, E-Commerce** – wo schnelle Antwortzeit wichtiger ist als sofortige Konsistenz.

---

### **Vergleich in Kurzform**

| Prinzip         | ACID (SQL)                                  | BASE (NoSQL)                           |
| --------------- | ------------------------------------------- | -------------------------------------- |
| Ziel            | Datenintegrität                             | Verfügbarkeit + Skalierbarkeit         |
| Konsistenz      | Streng, sofort                              | Eventual Consistency (zeitverzögert)   |
| Isolation       | Stark (Transaktionen sind getrennt)         | Locker, gleichzeitige Zugriffe erlaubt |
| Geschwindigkeit | Weniger performant bei vielen Transaktionen | Sehr performant bei großen Datenmengen |
| Beispiele       | PostgreSQL, MySQL, Oracle                   | MongoDB, Cassandra, DynamoDB           |

---

**Zusammenfassung:**

* **ACID** → strikte Konsistenz, sicher, aber weniger flexibel.
* **BASE** → hohe Verfügbarkeit und Skalierbarkeit, aber Daten können zeitweise inkonsistent sein.

📖 Quellen:

* [PostgreSQL Docs – Transactions (ACID)](https://www.postgresql.org/docs/current/tutorial-transactions.html)
* [MongoDB – NoSQL Explained (BASE)](https://www.mongodb.com/nosql-explained)
* [MDN Glossar – ACID (RU)](https://developer.mozilla.org/ru/docs/Glossary/ACID)

---

  **[⬆ Наверх](#top)**

11. ### <a name="11"></a> Unterschied zwischen SELECT * und gezielten Spaltenabfragen?

### **Unterschied zwischen `SELECT *` und gezielten Spaltenabfragen**

---

### **1. `SELECT *`**

* Wählt **alle Spalten** einer Tabelle aus.
* Praktisch für **schnelle Tests** oder kleine Tabellen.
* Nachteile:

  * **Performance**: Mehr Daten werden geladen, auch wenn nicht benötigt.
  * **Netzwerkbelastung**: Unnötige Datenübertragung.
  * **Instabilität**: Wenn sich das Schema ändert (neue Spalten), können Abfragen unvorhergesehen mehr Daten liefern.
  * **Schlechter für Index-Nutzung** → DB muss alle Spalten lesen.

**Beispiel:**

```sql
SELECT * FROM users;
```

---

### **2. Gezielte Spaltenabfragen**

* Nur die **benötigten Spalten** werden abgefragt.
* Vorteile:

  * **Effizienter** (schneller, weniger Speicherverbrauch).
  * **Klarheit**: Der Code zeigt, welche Daten wirklich gebraucht werden.
  * **Bessere Index-Nutzung** → DB kann Abfrage optimieren.

**Beispiel:**

```sql
SELECT id, name, email 
FROM users;
```

---

### **Vergleich**

| Merkmal           | `SELECT *`                        | Gezielte Spalten              |
| ----------------- | --------------------------------- | ----------------------------- |
| Performance       | Schwächer, lädt alles             | Besser, nur relevante Spalten |
| Lesbarkeit        | Unklar, was gebraucht wird        | Deutlich, selbsterklärend     |
| Schema-Änderungen | Kann ungewollt mehr Daten liefern | Stabiler                      |
| Nutzung in Praxis | Debugging, schnelle Tests         | Produktionscode, APIs         |

---

**Zusammenfassung:**

* `SELECT *` ist bequem, aber ineffizient und unsauber für produktiven Code.
* Gezielte Spaltenabfragen sind performanter, sicherer und besser lesbar.

📖 Quellen:

* [PostgreSQL Docs – SELECT](https://www.postgresql.org/docs/current/sql-select.html)
* [MDN Glossar – SQL SELECT (RU)](https://developer.mozilla.org/ru/docs/Web/SQL/SELECT)

---

  **[⬆ Наверх](#top)**

12. ### <a name="12"></a> Unterschied zwischen INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN?

### **JOIN-Arten in SQL**

Mit **JOINs** verbindet man Tabellen über gemeinsame Schlüssel (meist Fremdschlüssel). Unterschiedliche JOIN-Typen bestimmen, welche Datensätze zurückgegeben werden.

---

### **1. INNER JOIN**

* Liefert **nur die Datensätze**, bei denen in beiden Tabellen eine Übereinstimmung besteht.

```sql
SELECT u.id, u.name, o.product
FROM users u
INNER JOIN orders o ON u.id = o.user_id;
```

➡️ Nur Benutzer, die mindestens eine Bestellung haben.

---

### **2. LEFT JOIN (LEFT OUTER JOIN)**

* Alle Datensätze aus der **linken Tabelle** werden zurückgegeben.
* Falls keine Übereinstimmung in der rechten Tabelle → `NULL` in deren Spalten.

```sql
SELECT u.id, u.name, o.product
FROM users u
LEFT JOIN orders o ON u.id = o.user_id;
```

➡️ Alle Benutzer, auch die ohne Bestellungen (dort `product = NULL`).

---

### **3. RIGHT JOIN (RIGHT OUTER JOIN)**

* Alle Datensätze aus der **rechten Tabelle** werden zurückgegeben.
* Falls keine Übereinstimmung in der linken Tabelle → `NULL` in deren Spalten.

```sql
SELECT u.id, u.name, o.product
FROM users u
RIGHT JOIN orders o ON u.id = o.user_id;
```

➡️ Alle Bestellungen, auch ohne zugehörigen Benutzer (z. B. wenn ein User gelöscht wurde).

---

### **4. FULL JOIN (FULL OUTER JOIN)**

* Kombination aus LEFT JOIN + RIGHT JOIN.
* Alle Datensätze beider Tabellen, auch wenn keine Übereinstimmung vorliegt.

```sql
SELECT u.id, u.name, o.product
FROM users u
FULL JOIN orders o ON u.id = o.user_id;
```

➡️ Alle Benutzer und alle Bestellungen, auch wenn keine Zuordnung besteht (`NULL` auf einer Seite).

---

### **Vergleichsübersicht**

| JOIN-Typ   | Ergebnis                                                            |
| ---------- | ------------------------------------------------------------------- |
| INNER JOIN | Nur Datensätze mit Match in beiden Tabellen                         |
| LEFT JOIN  | Alle aus linker Tabelle + passende aus rechter Tabelle, Rest = NULL |
| RIGHT JOIN | Alle aus rechter Tabelle + passende aus linker Tabelle, Rest = NULL |
| FULL JOIN  | Alle Datensätze beider Tabellen, auch ohne Match                    |

---

**Zusammenfassung:**

* **INNER JOIN** → Schnittmenge
* **LEFT JOIN** → Alles aus links + Übereinstimmungen rechts
* **RIGHT JOIN** → Alles aus rechts + Übereinstimmungen links
* **FULL JOIN** → Vereinigung beider Tabellen

📖 Quellen:

* [PostgreSQL Docs – Joins](https://www.postgresql.org/docs/current/queries-table-expressions.html#QUERIES-JOIN)
* [MDN Glossar – JOIN (RU)](https://developer.mozilla.org/ru/docs/Glossary/Join)

---

  **[⬆ Наверх](#top)**

13. ### <a name="13"></a> Unterschied zwischen WHERE und HAVING?

### **Unterschied zwischen `WHERE` und `HAVING`**

---

### **1. WHERE**

* Filtert **Zeilen**, bevor Gruppierungen (`GROUP BY`) oder Aggregationen (`SUM`, `COUNT`, …) ausgeführt werden.
* Kann **nicht** direkt auf Aggregatfunktionen angewendet werden.

**Beispiel:**

```sql
-- Nur aktive Benutzer auswählen
SELECT id, name
FROM users
WHERE active = true;
```

---

### **2. HAVING**

* Filtert **Gruppen** nach einer Aggregation.
* Wird **nach GROUP BY** ausgeführt.
* Kann Bedingungen mit Aggregatfunktionen enthalten.

**Beispiel:**

```sql
-- Nur Benutzer anzeigen, die mehr als 2 Bestellungen haben
SELECT user_id, COUNT(*) AS total_orders
FROM orders
GROUP BY user_id
HAVING COUNT(*) > 2;
```

---

### **Vergleich in Kurzform**

| Merkmal       | WHERE                 | HAVING                             |
| ------------- | --------------------- | ---------------------------------- |
| Zeitpunkt     | Vor der Gruppierung   | Nach der Gruppierung               |
| Filtert       | Einzelne Zeilen       | Ganze Gruppen                      |
| Aggregatfunk. | Nicht erlaubt         | Erlaubt (z. B. `SUM()`, `COUNT()`) |
| Typischer Use | `WHERE active = true` | `HAVING COUNT(*) > 2`              |

---

**Zusammenfassung:**

* **WHERE** filtert Zeilen vor der Gruppierung.
* **HAVING** filtert Gruppen nach der Aggregation.

📖 Quellen:

* [PostgreSQL Docs – SELECT](https://www.postgresql.org/docs/current/sql-select.html)
* [MDN SQL HAVING (RU)](https://developer.mozilla.org/ru/docs/Web/SQL/HAVING)

---

  **[⬆ Наверх](#top)**

14. ### <a name="14"></a> Unterschied zwischen DISTINCT und GROUP BY?

### **Unterschied zwischen `DISTINCT` und `GROUP BY`**

---

### **1. DISTINCT**

* Entfernt **Duplikate** aus dem Ergebnis.
* Liefert eine **Liste einzigartiger Zeilen**.
* Keine Aggregatfunktionen erforderlich.

**Beispiel:**

```sql
-- Alle einzigartigen Städte aus der Kundentabelle
SELECT DISTINCT city
FROM customers;
```

➡️ Gibt jede Stadt nur **einmal** zurück.

---

### **2. GROUP BY**

* Fasst Zeilen zu **Gruppen** zusammen, basierend auf einer oder mehreren Spalten.
* Wird fast immer mit **Aggregatfunktionen** (`COUNT`, `SUM`, `AVG`, …) genutzt.
* Ohne Aggregatfunktion verhält es sich ähnlich wie DISTINCT, ist aber flexibler.

**Beispiel:**

```sql
-- Anzahl der Kunden pro Stadt
SELECT city, COUNT(*) AS customer_count
FROM customers
GROUP BY city;
```

➡️ Gibt pro Stadt **eine Zeile** zurück, zusätzlich mit Aggregatwerten.

---

### **Vergleich**

| Merkmal            | DISTINCT                               | GROUP BY                                     |
| ------------------ | -------------------------------------- | -------------------------------------------- |
| Zweck              | Entfernt Duplikate                     | Gruppiert Zeilen                             |
| Aggregatfunktionen | Nicht nötig                            | Typisch notwendig (`COUNT`, `SUM`, …)        |
| Ergebnis           | Einzigartige Kombinationen von Spalten | Eine Zeile pro Gruppe, oft mit Aggregaten    |
| Beispiel           | `SELECT DISTINCT city`                 | `SELECT city, COUNT(*) FROM … GROUP BY city` |

---

### **Beispiel mit gleichem Ergebnis**

```sql
-- DISTINCT
SELECT DISTINCT city FROM customers;

-- GROUP BY (ohne Aggregat)
SELECT city FROM customers GROUP BY city;
```

➡️ Beide geben eine Liste einzigartiger Städte zurück.
Aber: **GROUP BY** erlaubt zusätzlich Berechnungen pro Gruppe.

---

**Zusammenfassung:**

* **DISTINCT** entfernt nur Duplikate.
* **GROUP BY** gruppiert Daten und wird oft mit Aggregatfunktionen verwendet.

📖 Quellen:

* [PostgreSQL Docs – SELECT](https://www.postgresql.org/docs/current/sql-select.html)
* [MDN SQL DISTINCT (RU)](https://developer.mozilla.org/ru/docs/Web/SQL/Distinct)

---

  **[⬆ Наверх](#top)**

15. ### <a name="15"></a> Was sind Aggregatfunktionen (COUNT, SUM, AVG, MIN, MAX)?

### **Aggregatfunktionen in SQL**

Aggregatfunktionen fassen mehrere Zeilen zu einem einzigen Wert zusammen. Sie werden oft mit **`GROUP BY`** kombiniert.

---

### **1. COUNT()**

Zählt die Anzahl der Zeilen (oder nicht-NULL-Werte einer Spalte).

```sql
-- Anzahl aller Kunden
SELECT COUNT(*) FROM customers;

-- Anzahl der Kunden mit Email
SELECT COUNT(email) FROM customers;
```

---

### **2. SUM()**

Berechnet die Summe numerischer Werte.

```sql
-- Gesamtsumme aller Bestellungen
SELECT SUM(amount) AS total_sales
FROM orders;
```

---

### **3. AVG()**

Berechnet den Durchschnittswert.

```sql
-- Durchschnittlicher Bestellwert
SELECT AVG(amount) AS avg_order
FROM orders;
```

---

### **4. MIN()**

Gibt den kleinsten Wert zurück.

```sql
-- Günstigste Bestellung
SELECT MIN(amount) AS min_order
FROM orders;
```

---

### **5. MAX()**

Gibt den größten Wert zurück.

```sql
-- Teuerste Bestellung
SELECT MAX(amount) AS max_order
FROM orders;
```

---

### **Beispiel mit GROUP BY**

```sql
-- Anzahl und durchschnittlicher Umsatz pro Kunde
SELECT customer_id,
       COUNT(*) AS orders_count,
       SUM(amount) AS total_spent,
       AVG(amount) AS avg_spent,
       MIN(amount) AS min_order,
       MAX(amount) AS max_order
FROM orders
GROUP BY customer_id;
```

➡️ Ergebnis: eine Zeile pro Kunde mit Statistiken.

---

**Zusammenfassung:**

* **COUNT()** → Anzahl
* **SUM()** → Summe
* **AVG()** → Durchschnitt
* **MIN()** → Kleinster Wert
* **MAX()** → Größter Wert

📖 Quellen:

* [PostgreSQL Docs – Aggregate Functions](https://www.postgresql.org/docs/current/functions-aggregate.html)
* [MDN SQL Aggregate Functions (RU)](https://developer.mozilla.org/ru/docs/Web/SQL/Aggregate_functions)

---

  **[⬆ Наверх](#top)**

16. ### <a name="16"></a> Wie funktioniert ORDER BY und LIMIT?

### **ORDER BY**

* Sortiert die Ergebniszeilen einer Abfrage.
* Standardmäßig **aufsteigend (`ASC`)**, absteigend mit **`DESC`**.
* Kann nach mehreren Spalten sortieren.

**Beispiele:**

```sql
-- Alle Kunden nach Name (aufsteigend)
SELECT id, name FROM customers
ORDER BY name ASC;

-- Bestellungen nach Betrag (absteigend)
SELECT id, amount FROM orders
ORDER BY amount DESC;

-- Mehrfachsortierung: erst nach Stadt, dann nach Name
SELECT id, name, city FROM customers
ORDER BY city ASC, name ASC;
```

---

### **LIMIT**

* Begrenzt die Anzahl der zurückgegebenen Zeilen.
* Praktisch für **Pagination** oder Testabfragen.

**Beispiele:**

```sql
-- Nur die ersten 5 Kunden
SELECT * FROM customers
LIMIT 5;

-- Teuerste Bestellung (1 Ergebnis)
SELECT * FROM orders
ORDER BY amount DESC
LIMIT 1;
```

---

### **ORDER BY + LIMIT (Pagination)**

Mit `OFFSET` kann man Ergebnisse „überspringen“ → wichtig für **Seitenweise Anzeige**.

```sql
-- Seite 1: erste 10 Ergebnisse
SELECT * FROM products
ORDER BY name
LIMIT 10 OFFSET 0;

-- Seite 2: nächste 10 Ergebnisse
SELECT * FROM products
ORDER BY name
LIMIT 10 OFFSET 10;
```

---

### **Vergleich**

| Befehl   | Zweck                            |
| -------- | -------------------------------- |
| ORDER BY | Sortiert die Ergebnismenge       |
| LIMIT    | Beschränkt die Anzahl der Zeilen |
| OFFSET   | Überspringt bestimmte Zeilen     |

---

**Zusammenfassung:**

* **ORDER BY** → sortiert Ergebnisse.
* **LIMIT** → begrenzt Anzahl der Zeilen.
* Mit **OFFSET** → einfache Pagination möglich.

📖 Quellen:

* [PostgreSQL Docs – ORDER BY](https://www.postgresql.org/docs/current/queries-order.html)
* [PostgreSQL Docs – LIMIT/OFFSET](https://www.postgresql.org/docs/current/queries-limit.html)

---

  **[⬆ Наверх](#top)**

17. ### <a name="17"></a> Was ist ein Subquery (Unterabfrage)?

### **Subquery (Unterabfrage) in SQL**

Ein **Subquery** ist eine **verschachtelte Abfrage** innerhalb einer anderen SQL-Anweisung.
Die Unterabfrage wird zuerst ausgeführt, und ihr Ergebnis wird in der äußeren Abfrage verwendet.

---

### **Arten von Subqueries**

1. **Im `WHERE` oder `HAVING` (skalare oder Mengenabfrage)**

```sql
-- Kunden, die mindestens eine Bestellung gemacht haben
SELECT id, name
FROM customers
WHERE id IN (SELECT DISTINCT customer_id FROM orders);
```

2. **Im `FROM` (Subquery als virtuelle Tabelle)**

```sql
-- Durchschnittlicher Bestellwert pro Kunde
SELECT t.customer_id, AVG(t.amount) AS avg_amount
FROM (
  SELECT customer_id, amount
  FROM orders
) t
GROUP BY t.customer_id;
```

3. **Im `SELECT` (skalare Subquery)**

```sql
-- Kunden mit Anzahl ihrer Bestellungen
SELECT name,
       (SELECT COUNT(*) FROM orders o WHERE o.customer_id = c.id) AS total_orders
FROM customers c;
```

---

### **Eigenschaften**

* Kann **einen Wert** (skalare Subquery), **eine Liste** oder **eine Tabelle** zurückgeben.
* Kann mit Operatoren wie `IN`, `EXISTS`, `=`, `> ALL` usw. kombiniert werden.
* Können **korreliert** sein → Zugriff auf Spalten der äußeren Abfrage.

**Beispiel (korrelierte Subquery):**

```sql
-- Bestellungen, die über dem Durchschnittswert des jeweiligen Kunden liegen
SELECT o.id, o.amount
FROM orders o
WHERE o.amount > (
  SELECT AVG(amount)
  FROM orders
  WHERE customer_id = o.customer_id
);
```

---

**Zusammenfassung:**
Ein **Subquery** ist eine Abfrage in einer anderen Abfrage.

* Im `WHERE`/`HAVING`: Filterung.
* Im `FROM`: virtuelle Tabelle.
* Im `SELECT`: einzelner Wert.
* Kann **korreliert** oder **nicht korreliert** sein.

📖 Quellen:

* [PostgreSQL Docs – Subqueries](https://www.postgresql.org/docs/current/functions-subquery.html)
* [MDN Glossar – Subquery (RU)](https://developer.mozilla.org/ru/docs/Glossary/Subquery)

---

  **[⬆ Наверх](#top)**

18. ### <a name="18"></a> Unterschied zwischen korrelierter und nicht-korrelierter Unterabfrage?

### **Unterschied zwischen korrelierter und nicht-korrelierter Unterabfrage**

---

### **1. Nicht-korrelierte Unterabfrage**

* Wird **einmal** ausgeführt, unabhängig von der äußeren Abfrage.
* Ergebnis wird dann in der äußeren Abfrage verwendet.

**Beispiel:**

```sql
-- Alle Bestellungen, die über dem globalen Durchschnitt liegen
SELECT id, amount
FROM orders
WHERE amount > (SELECT AVG(amount) FROM orders);
```

➡️ Die Subquery `(SELECT AVG(amount) FROM orders)` wird **einmal berechnet**.

---

### **2. Korrelierte Unterabfrage**

* Wird **für jede Zeile der äußeren Abfrage erneut ausgeführt**.
* Bezieht sich auf Spalten der äußeren Abfrage.

**Beispiel:**

```sql
-- Bestellungen, die über dem Durchschnitt des jeweiligen Kunden liegen
SELECT o.id, o.amount
FROM orders o
WHERE o.amount > (
  SELECT AVG(amount)
  FROM orders
  WHERE customer_id = o.customer_id
);
```

➡️ Für jede Bestellung `o` wird die Subquery neu ausgeführt.

---

### **Vergleich**

| Merkmal      | Nicht-korreliert               | Korrelierte Unterabfrage                   |
| ------------ | ------------------------------ | ------------------------------------------ |
| Ausführung   | Einmal                         | Für jede Zeile der äußeren Abfrage         |
| Abhängigkeit | Unabhängig von äußerer Abfrage | Verweist auf Spalten der äußeren Abfrage   |
| Performance  | Meist effizienter              | Potenziell langsamer (mehrfach ausgeführt) |
| Beispiel     | Globaler Durchschnitt          | Durchschnitt pro Kunde                     |

---

**Zusammenfassung:**

* **Nicht-korrelierte Subquery**: unabhängig, einmal berechnet.
* **Korrelierte Subquery**: abhängig, mehrfach berechnet.

📖 Quellen:

* [PostgreSQL Docs – Subqueries](https://www.postgresql.org/docs/current/functions-subquery.html)
* [MDN Glossar – Subquery (RU)](https://developer.mozilla.org/ru/docs/Glossary/Subquery)

---

  **[⬆ Наверх](#top)**

19. ### <a name="19"></a> Unterschied zwischen EXISTS und IN?

### **Unterschied zwischen `EXISTS` und `IN`**

---

### **1. `IN`**

* Vergleicht einen Wert mit einer **Liste von Werten** oder dem Ergebnis einer Subquery.
* Subquery liefert eine **Liste von Werten** zurück.
* Eher geeignet, wenn wenige Werte zurückgegeben werden.

**Beispiel:**

```sql
-- Kunden, die Bestellungen gemacht haben
SELECT name
FROM customers
WHERE id IN (SELECT customer_id FROM orders);
```

---

### **2. `EXISTS`**

* Prüft, ob eine **Subquery mindestens eine Zeile** zurückgibt.
* Liefert `TRUE`, sobald ein Treffer gefunden wird (optimiert).
* Eher geeignet, wenn viele Werte zurückgegeben werden.

**Beispiel:**

```sql
-- Kunden, die Bestellungen gemacht haben
SELECT name
FROM customers c
WHERE EXISTS (
  SELECT 1
  FROM orders o
  WHERE o.customer_id = c.id
);
```

---

### **Technische Unterschiede**

| Merkmal      | `IN`                                           | `EXISTS`                             |
| ------------ | ---------------------------------------------- | ------------------------------------ |
| Rückgabewert | Vergleicht mit Liste von Werten                | Liefert TRUE/FALSE                   |
| Subquery-Typ | Muss Spalte(n) zurückgeben                     | Beliebige Abfrage (meist `SELECT 1`) |
| Performance  | Gut bei kleiner Ergebnismenge                  | Gut bei großer Ergebnismenge         |
| NULL-Werte   | Können zu Problemen führen (z. B. `IN (NULL)`) | Beeinträchtigen `EXISTS` nicht       |

---

### **Beispiel mit NULL-Problematik**

```sql
-- Problem mit IN, falls Subquery NULL enthält
SELECT name
FROM customers
WHERE id IN (SELECT customer_id FROM orders); -- Falls NULL dabei ist → Ergebnis kann leer sein

-- EXISTS vermeidet das Problem
SELECT name
FROM customers c
WHERE EXISTS (
  SELECT 1 FROM orders o WHERE o.customer_id = c.id
);
```

---

**Zusammenfassung:**

* **`IN`** → vergleicht mit Werteliste, gut für kleine Mengen.
* **`EXISTS`** → prüft nur Existenz, besser bei großen Datenmengen und sicherer bei NULL-Werten.

📖 Quellen:

* [PostgreSQL Docs – Subqueries with IN/EXISTS](https://www.postgresql.org/docs/current/functions-subquery.html)
* [MDN SQL Subquery (RU)](https://developer.mozilla.org/ru/docs/Glossary/Subquery)

---

  **[⬆ Наверх](#top)**

20. ### <a name="20"></a> Unterschied zwischen UNION und UNION ALL?

### **Unterschied zwischen `UNION` und `UNION ALL`**

---

### **1. UNION**

* Kombiniert Ergebnisse von zwei oder mehr `SELECT`-Abfragen.
* Entfernt **Duplikate** automatisch.
* Führt implizit ein **`DISTINCT`** auf allen zurückgegebenen Zeilen aus.
* Etwas langsamer, da ein Sortierschritt nötig ist.

**Beispiel:**

```sql
-- Gibt jede Stadt nur einmal zurück
SELECT city FROM customers
UNION
SELECT city FROM suppliers;
```

---

### **2. UNION ALL**

* Kombiniert Ergebnisse von zwei oder mehr `SELECT`-Abfragen.
* Behält **alle Duplikate** bei.
* Schneller, da keine zusätzliche Prüfung auf Duplikate erfolgt.

**Beispiel:**

```sql
-- Gibt auch doppelte Städte zurück
SELECT city FROM customers
UNION ALL
SELECT city FROM suppliers;
```

---

### **Vergleich**

| Merkmal       | UNION                                             | UNION ALL                            |
| ------------- | ------------------------------------------------- | ------------------------------------ |
| Duplikate     | Entfernt automatisch                              | Behält alle                          |
| Performance   | Langsamer (wegen DISTINCT)                        | Schneller                            |
| Typischer Use | Wenn nur **eindeutige Ergebnisse** gewünscht sind | Wenn **alle Daten** gebraucht werden |

---

**Zusammenfassung:**

* **`UNION`** = Kombination ohne Duplikate (langsamer).
* **`UNION ALL`** = Kombination mit allen Zeilen, inkl. Duplikaten (schneller).

📖 Quellen:

* [PostgreSQL Docs – UNION](https://www.postgresql.org/docs/current/queries-union.html)
* [MDN SQL UNION (RU)](https://developer.mozilla.org/ru/docs/Web/SQL/UNION)

---

  **[⬆ Наверх](#top)**

21. ### <a name="21"></a> Was ist PostgreSQL und welche Vorteile hat es gegenüber MySQL?

### **PostgreSQL**

PostgreSQL ist ein **objektrelationales Open-Source-Datenbankmanagementsystem (DBMS)**.
Es gilt als sehr stabil, ACID-konform und wird für kleine wie auch hochskalierte Anwendungen genutzt.

---

### **Vorteile von PostgreSQL gegenüber MySQL**

1. **Standardkonformität & Features**

* Vollständige ACID-Unterstützung.
* Mächtige SQL-Funktionen (z. B. CTEs, Window Functions, rekursive Abfragen).
* Unterstützung für komplexe Datentypen (JSONB, Arrays, HSTORE, Geodaten via PostGIS).

2. **Erweiterbarkeit**

* Eigene Funktionen, Operatoren und Datentypen definierbar.
* Erweiterungen wie **PostGIS**, **pg\_partman** (Partitionierung), **TimescaleDB** (Zeitreihen).

3. **Leistungsstärke bei komplexen Abfragen**

* Optimierter Query Planner.
* Bessere Performance bei **Joins, Aggregationen und OLAP**-ähnlichen Workloads.

4. **Transaktionen & Sicherheit**

* `SERIALIZABLE` Isolation Level voll implementiert.
* Starke Rolle-/Rechteverwaltung.
* Unterstützung für Row-Level Security (RLS).

5. **JSON-Unterstützung**

* **JSONB** mit Indizes, ideal für hybride SQL/NoSQL-Anwendungen.
* MySQL unterstützt JSON, aber weniger effizient und ohne so flexible Indexierung.

6. **Open-Source-Community & Stabilität**

* Sehr aktive Community, strenge Code-Qualität.
* Mehr als 30 Jahre Entwicklungsgeschichte.

---

### **Wann ist MySQL vorteilhaft?**

* Einfachere Einrichtung, oft **besser für kleinere Webanwendungen**.
* Breite Unterstützung durch viele Hosting-Anbieter (z. B. WordPress, PHP-Umgebungen).
* Performance-Vorteile bei **simplen Lese-lastigen Workloads**.

---

### **Vergleichsübersicht**

| Merkmal            | PostgreSQL                                | MySQL                               |
| ------------------ | ----------------------------------------- | ----------------------------------- |
| ACID               | Vollständig implementiert                 | Teilweise (InnoDB notwendig)        |
| JSON-Unterstützung | JSON + JSONB mit Indizes                  | JSON (eingeschränkt)                |
| Erweiterbarkeit    | Sehr hoch (Extensions, eigene Datentypen) | Begrenzt                            |
| Komplexe Abfragen  | Sehr stark (Window, CTE, rekursiv)        | Weniger leistungsfähig              |
| Performance        | Stärker bei komplexen Queries             | Oft schneller bei einfachen Queries |
| Community          | Stark, akademisch & professionell         | Sehr groß im Web-Bereich            |

---

**Zusammenfassung:**

* **PostgreSQL** ist mächtiger, erweiterbarer und besser für komplexe Anwendungen.
* **MySQL** ist einfacher, weit verbreitet und besser für kleine bis mittlere Webprojekte.

📖 Quellen:

* [PostgreSQL Docs](https://www.postgresql.org/docs/)
* [MySQL Docs](https://dev.mysql.com/doc/)
* [Vergleich PostgreSQL vs. MySQL (MDN RU)](https://developer.mozilla.org/ru/docs/Glossary/SQL)

---

  **[⬆ Наверх](#top)**

22. ### <a name="22"></a> Was sind Datentypen in PostgreSQL (TEXT, VARCHAR, SERIAL, JSONB)?

### **Datentypen in PostgreSQL (TEXT, VARCHAR, SERIAL, JSONB)**

PostgreSQL bietet eine große Vielfalt an Datentypen. Einige der wichtigsten sind:

---

### **1. TEXT**

* Speichert Zeichenketten beliebiger Länge (theoretisch bis 1 GB).
* Kein Längenlimit erforderlich.
* Praktisch identisch zu `VARCHAR` ohne Längenbeschränkung.

**Beispiel:**

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  bio TEXT
);
```

---

### **2. VARCHAR(n)**

* Variable Länge, aber mit **maximaler Zeichenanzahl n**.
* Bei Überschreiten → Fehler.
* In PostgreSQL gibt es **keinen Performance-Unterschied** zu `TEXT`.

**Beispiel:**

```sql
CREATE TABLE products (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100) -- max. 100 Zeichen
);
```

---

### **3. SERIAL**

* Pseudotyp für **Auto-Increment Integer**.
* Erstellt automatisch eine **Sequenz** und setzt sie als Default für die Spalte.
* Typisch für Primärschlüssel.
* In modernen PostgreSQL-Versionen ersetzt durch `GENERATED AS IDENTITY`.

**Beispiel:**

```sql
CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  amount NUMERIC(10,2)
);
```

---

### **4. JSONB**

* Binäre Form von JSON, effizienter als `JSON`.
* Vorteile:

  * Kompakter Speicher.
  * Unterstützt **Indexierung** (`GIN`-Index).
  * Schnelle Abfragen innerhalb von JSON-Daten.

**Beispiel:**

```sql
CREATE TABLE events (
  id SERIAL PRIMARY KEY,
  data JSONB
);

-- Einfügen
INSERT INTO events (data)
VALUES ('{"type": "login", "user": "max"}');

-- Abfragen
SELECT data->>'user'
FROM events
WHERE data->>'type' = 'login';
```

---

### **Vergleich**

| Datentyp    | Beschreibung                         | Typische Nutzung                |
| ----------- | ------------------------------------ | ------------------------------- |
| **TEXT**    | Zeichenketten beliebiger Länge       | Freitext, lange Texte           |
| **VARCHAR** | Zeichenkette mit Längenlimit         | Namen, Codes, begrenzte Strings |
| **SERIAL**  | Auto-Increment Ganzzahl              | Primärschlüssel                 |
| **JSONB**   | JSON in binärer Form mit Indexierung | Semi-strukturierte Daten, Logs  |

---

**Zusammenfassung:**

* **TEXT** und **VARCHAR** sind für Strings → praktisch gleichwertig in PostgreSQL.
* **SERIAL** = Auto-Increment für Primärschlüssel (heute: `IDENTITY`).
* **JSONB** = flexibler, indexierbarer Datentyp für semi-strukturierte Daten.

📖 Quellen:

* [PostgreSQL Docs – Data Types](https://www.postgresql.org/docs/current/datatype.html)
* [PostgreSQL Docs – JSON Types](https://www.postgresql.org/docs/current/datatype-json.html)

---

  **[⬆ Наверх](#top)**

23. ### <a name="23"></a> Unterschied zwischen SERIAL und BIGSERIAL?

### **Unterschied zwischen `SERIAL` und `BIGSERIAL` in PostgreSQL**

---

### **1. SERIAL**

* Alias für `INTEGER` + automatische Sequenz.
* Wertebereich: **-2.147.483.648 bis 2.147.483.647** (\~2,1 Mrd).
* Für kleine bis mittlere Tabellen geeignet.

**Beispiel:**

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT
);
```

---

### **2. BIGSERIAL**

* Alias für `BIGINT` + automatische Sequenz.
* Wertebereich: **-9.223.372.036.854.775.808 bis 9.223.372.036.854.775.807** (\~9 Quintillionen).
* Für sehr große Tabellen mit extrem vielen Zeilen.

**Beispiel:**

```sql
CREATE TABLE logs (
  id BIGSERIAL PRIMARY KEY,
  message TEXT
);
```

---

### **Vergleich**

| Merkmal        | SERIAL (INTEGER)                     | BIGSERIAL (BIGINT)                           |
| -------------- | ------------------------------------ | -------------------------------------------- |
| Speichergröße  | 4 Byte                               | 8 Byte                                       |
| Max. Wert      | \~ 2,1 Milliarden                    | \~ 9,2 Quintillionen                         |
| Performance    | Minimal schneller (kleiner Datentyp) | Minimal langsamer (größerer Datentyp)        |
| Anwendungsfall | Normale Tabellen                     | Sehr große Tabellen (Milliarden+ Datensätze) |

---

**Zusammenfassung:**

* **SERIAL** → 32-Bit, reicht für die meisten Anwendungen.
* **BIGSERIAL** → 64-Bit, für extrem große Tabellen.

📖 Quellen:

* [PostgreSQL Docs – SERIAL Types](https://www.postgresql.org/docs/current/datatype-numeric.html#DATATYPE-SERIAL)

---

  **[⬆ Наверх](#top)**

24. ### <a name="24"></a> Wie arbeitet PostgreSQL mit Arrays?

### **Arrays in PostgreSQL**

PostgreSQL unterstützt **Arrays als Datentyp**. Eine Spalte kann mehrere Werte desselben Typs speichern (z. B. `INTEGER[]`, `TEXT[]`).

---

### **1. Array-Datentyp definieren**

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT,
  tags TEXT[] -- Array von Textwerten
);
```

---

### **2. Array-Werte einfügen**

```sql
INSERT INTO users (name, tags)
VALUES ('Max', ARRAY['admin', 'editor']),
       ('Anna', '{"guest","beta"}'); -- alternative Syntax
```

---

### **3. Zugriff auf Array-Elemente**

* Einzelnes Element mit Index (1-basiert!).
* Slice mit Bereich.

```sql
-- Erstes Tag von Max
SELECT tags[1] FROM users WHERE name = 'Max';

-- Erstes bis zweites Element
SELECT tags[1:2] FROM users WHERE name = 'Max';
```

---

### **4. Array-Funktionen und Operatoren**

* **Mit Element vergleichen:** `= ANY(array)`
* **Array enthält Wert:** `array @> array`
* **Array ist enthalten in:** `array <@ array`
* **Überschneidung prüfen:** `&&`

```sql
-- Alle User mit Tag 'admin'
SELECT name
FROM users
WHERE 'admin' = ANY(tags);

-- User, deren Tags 'admin' enthalten
SELECT name
FROM users
WHERE tags @> ARRAY['admin'];
```

---

### **5. Nützliche Funktionen**

* `unnest()` → Array in mehrere Zeilen auflösen
* `array_length()` → Länge bestimmen
* `array_append()` / `array_remove()`

```sql
-- Array in Zeilen umwandeln
SELECT unnest(tags) FROM users WHERE name = 'Max';

-- Länge des Arrays
SELECT array_length(tags, 1) FROM users WHERE name = 'Max';
```

---

**Zusammenfassung:**
PostgreSQL bietet Arrays als nativen Datentyp mit flexiblem Zugriff, Vergleichsoperatoren und nützlichen Funktionen wie `unnest()`. Arrays sind praktisch für Tags, Labels oder kleine Listen, aber bei stark relationalen Daten sind **separate Tabellen + JOINs** oft die bessere Wahl.

📖 Quellen:

* [PostgreSQL Docs – Arrays](https://www.postgresql.org/docs/current/arrays.html)


  **[⬆ Наверх](#top)**

25. ### <a name="25"></a> Was ist der Unterschied zwischen JSON und JSONB in PostgreSQL?

### **Unterschied zwischen `JSON` und `JSONB` in PostgreSQL**

---

### **1. JSON**

* Speichert Daten als **reinen Text** im JSON-Format.
* Speicherung erfolgt genau so, wie die Eingabe ist (inkl. Whitespaces, Keys-Reihenfolge).
* Vorteile:

  * Originalformat bleibt unverändert.
  * Weniger Rechenaufwand beim Einfügen.
* Nachteile:

  * Keine Indexierung möglich.
  * Langsamer bei Abfragen und Filtern.

**Beispiel:**

```sql
CREATE TABLE events (
  id SERIAL PRIMARY KEY,
  data JSON
);

INSERT INTO events (data)
VALUES ('{ "user": "Max", "role": "admin" }');
```

---

### **2. JSONB**

* Speichert JSON-Daten im **binären Format**.
* Entfernt unnötige Whitespaces, sortiert Keys.
* Vorteile:

  * Unterstützt **Indizes** (z. B. GIN-Index).
  * Schnellere Abfragen und Vergleiche.
  * Bessere Operatoren und Funktionen.
* Nachteile:

  * Etwas langsamer beim Einfügen (wegen Konvertierung in Binärformat).

**Beispiel:**

```sql
CREATE TABLE events_b (
  id SERIAL PRIMARY KEY,
  data JSONB
);

-- Abfrage mit Filter
SELECT data->>'user'
FROM events_b
WHERE data @> '{"role": "admin"}';
```

Mit Index:

```sql
CREATE INDEX idx_events_data ON events_b USING gin (data);
```

---

### **Vergleich**

| Merkmal            | JSON                         | JSONB                         |
| ------------------ | ---------------------------- | ----------------------------- |
| Speicherung        | Text (wie eingegeben)        | Binär, normalisiert           |
| Whitespaces / Keys | Werden gespeichert           | Ignoriert, Keys sortiert      |
| Einfügen           | Schneller                    | Etwas langsamer               |
| Abfragen           | Langsamer                    | Schneller, da binär           |
| Indexierung        | Nicht möglich                | Möglich (z. B. GIN-Index)     |
| Nutzung            | Archivierung, Originalformat | Aktive Queries, Filter, Suche |

---

**Zusammenfassung:**

* **JSON** → schneller beim Schreiben, speichert Originalformat, keine Indizes.
* **JSONB** → optimal für Abfragen und Suche, unterstützt Indizes, braucht aber mehr beim Einfügen.

📖 Quellen:

* [PostgreSQL Docs – JSON Types](https://www.postgresql.org/docs/current/datatype-json.html)


  **[⬆ Наверх](#top)**

26. ### <a name="26"></a> Wie speichert und verarbeitet PostgreSQL Zeitstempel (TIMESTAMP, TIMESTAMPTZ)?

### **Zeitstempel in PostgreSQL: `TIMESTAMP` vs. `TIMESTAMPTZ`**

---

### **1. TIMESTAMP (without time zone)**

* Speichert **Datum + Uhrzeit**, aber **ohne Zeitzonen-Information**.
* Werte werden so gespeichert, wie sie eingegeben werden.
* Keine automatische Anpassung an Zeitzonen.

**Beispiel:**

```sql
CREATE TABLE events (
  id SERIAL PRIMARY KEY,
  created_at TIMESTAMP
);

INSERT INTO events (created_at)
VALUES ('2025-09-06 15:00:00'); -- bleibt exakt so gespeichert
```

---

### **2. TIMESTAMPTZ (TIMESTAMP WITH TIME ZONE)**

* Speichert **Zeitpunkt in UTC**, zeigt ihn aber abhängig von der Session-Zeitzone an.
* Bei Eingabe wird automatisch nach UTC konvertiert.
* Sicherer für globale Anwendungen.

**Beispiel:**

```sql
CREATE TABLE events_tz (
  id SERIAL PRIMARY KEY,
  created_at TIMESTAMPTZ
);

-- Eingabe mit Zeitzone
INSERT INTO events_tz (created_at)
VALUES ('2025-09-06 15:00:00+02'); -- wird in UTC gespeichert

-- Anzeige in aktueller Session-Zeitzone
SET TIMEZONE = 'Europe/Berlin';
SELECT created_at FROM events_tz;
```

➡️ Wenn Session-Zeitzone `UTC` ist → `2025-09-06 13:00:00+00`
➡️ Wenn Session-Zeitzone `Europe/Berlin` ist → `2025-09-06 15:00:00+02`

---

### **Vergleich**

| Merkmal    | TIMESTAMP             | TIMESTAMPTZ                        |
| ---------- | --------------------- | ---------------------------------- |
| Zeitzone   | Keine Speicherung     | Speicherung in UTC + Konvertierung |
| Konsistenz | Lokal gültig          | Global eindeutig                   |
| Verwendung | Für rein lokale Daten | Für globale Systeme, APIs, Logs    |

---

### **Best Practices**

* Für **globale Anwendungen** (Web, APIs, Logs) → **TIMESTAMPTZ** verwenden.
* Für **rein lokale Daten** (z. B. Öffnungszeiten) → **TIMESTAMP** reicht.

---

**Zusammenfassung:**

* **TIMESTAMP** = Datum + Uhrzeit ohne Zeitzone.
* **TIMESTAMPTZ** = Datum + Uhrzeit mit Zeitzonenunterstützung (intern UTC).
* Empfehlung: Standardmäßig **TIMESTAMPTZ** nutzen, da es konsistenter für globale Systeme ist.

📖 Quellen:

* [PostgreSQL Docs – Date/Time Types](https://www.postgresql.org/docs/current/datatype-datetime.html)


  **[⬆ Наверх](#top)**

27. ### <a name="27"></a> Was sind Sequences in PostgreSQL?

### **Sequences in PostgreSQL**

Eine **Sequence** ist ein spezielles Datenbankobjekt, das fortlaufende **Zahlenwerte** generiert.
Sie wird oft für **Primärschlüssel (Auto-Increment)** verwendet.

---

### **1. Sequence erstellen**

```sql
CREATE SEQUENCE user_id_seq
  START 1      -- Startwert
  INCREMENT 1  -- Schrittweite
  MINVALUE 1
  MAXVALUE 1000000
  CYCLE;       -- optional: nach MAXVALUE wieder von vorne beginnen
```

---

### **2. Werte abrufen**

```sql
-- Nächster Wert
SELECT nextval('user_id_seq');

-- Aktueller Wert (ohne Erhöhung)
SELECT currval('user_id_seq');

-- Wert zurücksetzen
ALTER SEQUENCE user_id_seq RESTART WITH 1;
```

---

### **3. Nutzung in Tabellen**

```sql
CREATE TABLE users (
  id INT DEFAULT nextval('user_id_seq') PRIMARY KEY,
  name TEXT
);
```

Oder direkt mit **SERIAL / BIGSERIAL / IDENTITY** (nutzt intern auch Sequences):

```sql
CREATE TABLE orders (
  id SERIAL PRIMARY KEY,
  amount NUMERIC
);
```

---

### **4. Vorteile**

* Garantierte eindeutige Werte.
* Unabhängig von Tabellen nutzbar.
* Flexibel (kann mit beliebigen INCREMENT, START, CYCLE konfiguriert werden).

---

### **Unterschied zu `SERIAL` / `IDENTITY`**

* `SERIAL` / `IDENTITY` sind nur **Convenience-Shortcuts**, die intern automatisch eine Sequence anlegen.
* Mit einer **manuell definierten Sequence** hat man mehr Kontrolle (z. B. mehrere Tabellen nutzen dieselbe Sequence).

---

**Zusammenfassung:**
Sequences sind Objekte in PostgreSQL zur Erzeugung fortlaufender eindeutiger Zahlen.
Sie werden oft für Auto-Increment-Spalten verwendet und bilden die Basis für `SERIAL` und `IDENTITY`.

📖 Quellen:

* [PostgreSQL Docs – Sequences](https://www.postgresql.org/docs/current/sql-createsequence.html)


  **[⬆ Наверх](#top)**

28. ### <a name="28"></a> Wie implementiert man Auto-Increment in PostgreSQL?

### **Auto-Increment in PostgreSQL**

PostgreSQL unterstützt mehrere Möglichkeiten, automatisch fortlaufende IDs zu erzeugen.

---

### **1. SERIAL (klassisch, älterer Ansatz)**

* Kürzel für: `INTEGER` + `DEFAULT nextval(sequence)`
* Legt im Hintergrund automatisch eine **Sequence** an.

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name TEXT
);
```

➡️ `id` wird bei jedem `INSERT` automatisch erhöht.

---

### **2. BIGSERIAL**

* Wie `SERIAL`, aber auf `BIGINT`-Basis (für sehr große Tabellen).

```sql
CREATE TABLE logs (
  id BIGSERIAL PRIMARY KEY,
  message TEXT
);
```

---

### **3. IDENTITY (moderner Standard, SQL:2003)**

* Ab PostgreSQL 10 verfügbar.
* Empfohlen, da **Standard-konform** und flexibler.

```sql
CREATE TABLE products (
  id INT GENERATED ALWAYS AS IDENTITY PRIMARY KEY,
  name TEXT
);
```

Varianten:

* `GENERATED ALWAYS AS IDENTITY` → DB verwaltet die Werte strikt (manuelles Insert nicht möglich ohne Override).
* `GENERATED BY DEFAULT AS IDENTITY` → erlaubt manuelles Setzen, wenn nötig.

---

### **4. Manuelle Sequence** (volle Kontrolle)

```sql
CREATE SEQUENCE order_seq START 1;

CREATE TABLE orders (
  id INT DEFAULT nextval('order_seq') PRIMARY KEY,
  amount NUMERIC
);
```

---

### **Vergleich**

| Methode          | Datentyp       | Standard-konform | Empfehlung                                                      |
| ---------------- | -------------- | ---------------- | --------------------------------------------------------------- |
| SERIAL           | INTEGER        | Nein             | Legacy, noch häufig genutzt                                     |
| BIGSERIAL        | BIGINT         | Nein             | Für sehr große Tabellen                                         |
| IDENTITY         | INTEGER/BIGINT | Ja               | Moderne Best Practice                                           |
| Sequence manuell | Flexibel       | Ja               | Spezialfälle (z. B. mehrere Tabellen teilen sich eine Sequence) |

---

**Zusammenfassung:**

* **`SERIAL`/`BIGSERIAL`** → älter, praktisch, aber nicht Standard.
* **`IDENTITY`** → moderner, SQL-konform, empfohlen ab PostgreSQL 10.
* **Manuelle Sequence** → maximale Flexibilität.

📖 Quellen:

* [PostgreSQL Docs – SERIAL Types](https://www.postgresql.org/docs/current/datatype-numeric.html#DATATYPE-SERIAL)
* [PostgreSQL Docs – Identity Columns](https://www.postgresql.org/docs/current/ddl-generated-columns.html#DDL-IDENTITY-COLUMNS)
* [PostgreSQL Docs – Sequences](https://www.postgresql.org/docs/current/sql-createsequence.html)


  **[⬆ Наверх](#top)**

29. ### <a name="29"></a> Was sind Materialized Views?

### **Materialized Views in PostgreSQL**

Eine **Materialized View** ist eine gespeicherte Abfrage, deren Ergebnis **physisch in der Datenbank gespeichert** wird.
Sie ähnelt einer normalen View, wird aber nicht bei jeder Abfrage neu berechnet, sondern als **statische Tabelle** abgelegt.

---

### **1. Erstellung**

```sql
CREATE MATERIALIZED VIEW sales_summary AS
SELECT customer_id, SUM(amount) AS total_sales
FROM orders
GROUP BY customer_id;
```

➡️ Ergebnis wird gespeichert wie in einer Tabelle.

---

### **2. Nutzung**

```sql
-- Abfrage wie bei einer normalen Tabelle
SELECT * FROM sales_summary;
```

---

### **3. Aktualisierung**

* Daten sind **nicht automatisch aktuell**.
* Müssen manuell oder über Cron/Trigger mit `REFRESH` aktualisiert werden.

```sql
REFRESH MATERIALIZED VIEW sales_summary;
```

Optional:

```sql
REFRESH MATERIALIZED VIEW CONCURRENTLY sales_summary;
```

➡️ Ermöglicht gleichzeitige Lesezugriffe während des Refreshs (erfordert Unique Index).

---

### **4. Vorteile**

* Schnelle Abfragen für komplexe Berechnungen (z. B. Aggregationen, Joins).
* Reduziert Datenbanklast bei häufig wiederholten komplexen Queries.

---

### **5. Nachteile**

* Daten sind nicht „live“, sondern nur so aktuell wie der letzte `REFRESH`.
* Benötigen zusätzlichen Speicherplatz.

---

### **Vergleich: View vs. Materialized View**

| Merkmal        | View                          | Materialized View                      |
| -------------- | ----------------------------- | -------------------------------------- |
| Speicherung    | Nur Abfrage gespeichert       | Ergebnis der Abfrage gespeichert       |
| Aktualität     | Immer aktuell                 | Muss mit `REFRESH` aktualisiert werden |
| Performance    | Langsam bei komplexen Queries | Schnell, da vorgerechnet               |
| Speicherbedarf | Kein zusätzlicher Speicher    | Braucht Speicherplatz                  |

---

**Zusammenfassung:**
Eine **Materialized View** ist eine gespeicherte Abfrage mit persistenten Ergebnissen.
Sie beschleunigt komplexe Abfragen, muss aber regelmäßig mit `REFRESH` aktualisiert werden.

📖 Quellen:

* [PostgreSQL Docs – Materialized Views](https://www.postgresql.org/docs/current/rules-materializedviews.html)


  **[⬆ Наверх](#top)**

30. ### <a name="30"></a> Unterschied zwischen View und Materialized View?

### **Unterschied zwischen View und Materialized View in PostgreSQL**

---

### **1. View**

* Eine **gespeicherte Abfrage** (virtuelle Tabelle).
* Ergebnis wird **nicht gespeichert**, sondern **bei jeder Abfrage neu berechnet**.
* Immer **aktuell**, aber langsamer bei komplexen Abfragen.

**Beispiel:**

```sql
CREATE VIEW active_users AS
SELECT id, name
FROM users
WHERE active = true;

SELECT * FROM active_users;
```

➡️ Berechnet sich jedes Mal neu.

---

### **2. Materialized View**

* Speichert das Ergebnis der Abfrage **physisch in der Datenbank**.
* Ergebnis bleibt erhalten und wird wie eine Tabelle abgefragt.
* Muss manuell mit `REFRESH MATERIALIZED VIEW` aktualisiert werden.

**Beispiel:**

```sql
CREATE MATERIALIZED VIEW sales_summary AS
SELECT customer_id, SUM(amount) AS total_sales
FROM orders
GROUP BY customer_id;

-- später aktualisieren
REFRESH MATERIALIZED VIEW sales_summary;
```

➡️ Schneller bei Abfragen, aber nicht automatisch aktuell.

---

### **Vergleichstabelle**

| Merkmal             | View                            | Materialized View                |
| ------------------- | ------------------------------- | -------------------------------- |
| Speicherung         | Keine Daten gespeichert         | Ergebnis wird gespeichert        |
| Aktualität          | Immer aktuell                   | Muss manuell aktualisiert werden |
| Performance         | Langsamer bei komplexen Queries | Schnell, da vorgerechnet         |
| Speicherplatzbedarf | Kein zusätzlicher Speicher      | Benötigt Speicherplatz           |

---

**Zusammenfassung:**

* **View** = immer aktuell, aber langsamer.
* **Materialized View** = schneller, aber erfordert manuelles Aktualisieren.

📖 Quellen:

* [PostgreSQL Docs – Views](https://www.postgresql.org/docs/current/sql-createview.html)
* [PostgreSQL Docs – Materialized Views](https://www.postgresql.org/docs/current/rules-materializedviews.html)


  **[⬆ Наверх](#top)**  

31. ### <a name="31"></a> Was ist ein Index in PostgreSQL?

### **Index in PostgreSQL**

Ein **Index** ist eine zusätzliche Datenstruktur, die PostgreSQL anlegt, um **Datenbankabfragen zu beschleunigen**.
Er funktioniert ähnlich wie ein Inhaltsverzeichnis in einem Buch: Statt jede Seite zu durchsuchen, springt die Datenbank direkt an die richtige Stelle.

---

### **1. Erstellung eines Index**

```sql
-- Einfacher Index auf Spalte email
CREATE INDEX idx_users_email
ON users (email);
```

➡️ Abfragen wie

```sql
SELECT * FROM users WHERE email = 'max@example.com';
```

werden dadurch wesentlich schneller.

---

### **2. Arten von Indizes**

* **B-Tree (Standard):** Für Gleichheits- und Bereichsabfragen (`=`, `<`, `>`, `BETWEEN`).
* **Hash:** Nur für Gleichheitsvergleiche.
* **GIN (Generalized Inverted Index):** Für Arrays, JSONB, Volltextsuche.
* **GiST (Generalized Search Tree):** Für Geodaten, komplexe Datentypen.
* **BRIN (Block Range Index):** Für sehr große Tabellen mit sequenziellen Daten (z. B. Zeitserien).
* **Unique Index:** Erzwingt Eindeutigkeit (z. B. Emails).

---

### **3. Wartung**

* Indizes brauchen **Speicherplatz** und müssen beim `INSERT`, `UPDATE`, `DELETE` aktualisiert werden.
* Zu viele Indizes können Schreiboperationen verlangsamen.

---

### **4. Beispiel: Unique Index**

```sql
CREATE UNIQUE INDEX idx_users_email_unique
ON users (email);
```

➡️ Kein Nutzer kann doppelte Email eintragen.

---

### **5. Index bei JSONB**

```sql
CREATE INDEX idx_events_data
ON events USING gin (data);
```

➡️ Ermöglicht schnelle Suche in JSONB-Feldern:

```sql
SELECT * FROM events WHERE data @> '{"type": "login"}';
```

---

### **Vergleich: Index vs. kein Index**

| Merkmal            | Ohne Index                | Mit Index                            |
| ------------------ | ------------------------- | ------------------------------------ |
| SELECT-Abfragen    | Langsam (Full Table Scan) | Schnell (direkter Zugriff)           |
| Speicherbedarf     | Wenig                     | Mehr (Index-Struktur zusätzlich)     |
| Schreiboperationen | Schneller                 | Etwas langsamer (Index-Update nötig) |

---

**Zusammenfassung:**
Ein **Index** in PostgreSQL beschleunigt Lesezugriffe auf Tabellen, indem er eine optimierte Datenstruktur anlegt. Er erhöht aber den Speicherbedarf und verlangsamt Schreiboperationen leicht.

📖 Quellen:

* [PostgreSQL Docs – Indexes](https://www.postgresql.org/docs/current/indexes.html)


  **[⬆ Наверх](#top)**

32. ### <a name="32"></a> Unterschied zwischen B-Tree, Hash und GIN Index?

### **Unterschied zwischen B-Tree, Hash und GIN Index in PostgreSQL**

---

### **1. B-Tree Index (Standard)**

* **Default-Index-Typ** in PostgreSQL.
* Optimiert für **Vergleiche und Sortierungen**:

  * `=`, `<`, `>`, `<=`, `>=`, `BETWEEN`, `ORDER BY`.
* Unterstützt auch **Prefix-Suche** bei Strings (`LIKE 'abc%'`).
* Sehr universell, für die meisten Fälle geeignet.

**Beispiel:**

```sql
CREATE INDEX idx_users_email
ON users (email);
```

➡️ Schnell für:

```sql
SELECT * FROM users WHERE email = 'max@example.com';
```

---

### **2. Hash Index**

* Optimiert für **Gleichheitsabfragen (`=`)**.
* Früher weniger stabil, seit PostgreSQL 10 **WAL-gesichert** und produktionsreif.
* Kein Vorteil gegenüber B-Tree, außer in speziellen Fällen.

**Beispiel:**

```sql
CREATE INDEX idx_users_hash
ON users USING hash (email);
```

➡️ Schnell für:

```sql
SELECT * FROM users WHERE email = 'anna@example.com';
```

Aber nicht für `<`, `>`, `ORDER BY` geeignet.

---

### **3. GIN (Generalized Inverted Index)**

* Speziell für **Sammlungen von Werten** innerhalb einer Spalte.
* Ideal für **Arrays, JSONB, Full-Text-Suche**.
* Unterstützt Operatoren wie `@>`, `<@`, `&&`.

**Beispiel für JSONB:**

```sql
CREATE INDEX idx_events_data
ON events USING gin (data);
```

```sql
SELECT * FROM events
WHERE data @> '{"role": "admin"}';
```

➡️ Ohne GIN-Index → sehr langsam (Full Table Scan).
➡️ Mit GIN-Index → extrem schnell.

---

### **Vergleichstabelle**

| Merkmal               | B-Tree                         | Hash                   | GIN                                           |
| --------------------- | ------------------------------ | ---------------------- | --------------------------------------------- |
| Standard              | Ja                             | Nein                   | Nein                                          |
| Unterstützte Abfragen | `=`, `<`, `>`, `BETWEEN`, Sort | Nur `=`                | JSONB, Arrays, Volltext                       |
| Stärken               | Universell, sehr flexibel      | Gleichheitsvergleiche  | Suche in komplexen Datentypen                 |
| Schwächen             | Nicht optimal für Arrays/JSONB | Keine Bereichsabfragen | Hoher Speicherbedarf, langsamer Insert/Update |

---

**Zusammenfassung:**

* **B-Tree** → Standard, universell für Vergleiche und Sortierungen.
* **Hash** → Nur für Gleichheit (`=`), selten sinnvoller als B-Tree.
* **GIN** → Speziell für JSONB, Arrays und Volltextsuche.

📖 Quellen:

* [PostgreSQL Docs – Index Types](https://www.postgresql.org/docs/current/indexes-types.html)


  **[⬆ Наверх](#top)**

33. ### <a name="33"></a> Was ist ein Unique Index?

### **Unique Index in PostgreSQL**

Ein **Unique Index** stellt sicher, dass die Werte in einer oder mehreren Spalten **eindeutig** sind.
Dadurch wird verhindert, dass doppelte Werte eingefügt werden.

---

### **1. Erstellung eines Unique Index**

```sql
CREATE UNIQUE INDEX idx_users_email_unique
ON users (email);
```

➡️ Kein Benutzer kann zweimal dieselbe Email eintragen.

---

### **2. Unique Constraint vs. Unique Index**

* `UNIQUE CONSTRAINT` (z. B. in `CREATE TABLE`) erzeugt intern automatisch einen **Unique Index**.
* Unterschied:

  * **Unique Constraint** = Teil der Datenintegrität (Schema-Level).
  * **Unique Index** = Index-Objekt, kann auch unabhängig erstellt werden.

**Beispiel mit Constraint:**

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email TEXT UNIQUE
);
```

➡️ PostgreSQL erzeugt dabei automatisch einen Unique Index.

---

### **3. Mehrspaltige Unique Indizes**

Man kann auch Kombinationen von Spalten eindeutig machen.

```sql
CREATE UNIQUE INDEX idx_orders_user_product
ON orders (user_id, product_id);
```

➡️ Ein Benutzer kann jedes Produkt nur **einmal** bestellen.

---

### **4. Vorteile**

* Verhindert doppelte Werte → **Datenintegrität**.
* Schnelle Suche durch Indexierung.

### **5. Nachteile**

* **Einfügen/Update langsamer**, weil PostgreSQL prüfen muss, ob der Wert schon existiert.

---

**Zusammenfassung:**
Ein **Unique Index** garantiert Eindeutigkeit in einer oder mehreren Spalten. Er wird automatisch bei `UNIQUE`-Constraints angelegt oder kann manuell erstellt werden.

📖 Quellen:

* [PostgreSQL Docs – Indexes: Unique Indexes](https://www.postgresql.org/docs/current/indexes-unique.html)
* [PostgreSQL Docs – Constraints](https://www.postgresql.org/docs/current/ddl-constraints.html)


  **[⬆ Наверх](#top)**

34. ### <a name="34"></a> Nachteile von zu vielen Indexen?

### **Nachteile von zu vielen Indizes in PostgreSQL**

Indizes verbessern die **Lesegeschwindigkeit**, haben aber auch Nachteile, wenn man zu viele davon anlegt:

---

### **1. Speicherverbrauch**

* Jeder Index benötigt zusätzlichen **Platz auf der Festplatte**.
* Große Tabellen mit vielen Indizes können deutlich mehr Speicher belegen.

---

### **2. Langsamere Schreiboperationen**

* Bei **INSERT, UPDATE, DELETE** muss PostgreSQL alle relevanten Indizes **mitaktualisieren**.
* Je mehr Indizes → desto langsamer werden Schreibvorgänge.

---

### **3. Komplexere Wartung**

* Indizes müssen regelmäßig **neu aufgebaut oder analysiert** werden (`REINDEX`, `VACUUM ANALYZE`).
* Viele Indizes machen das aufwändiger.

---

### **4. Suboptimale Query-Pläne**

* Der Query Planner kann bei zu vielen Indizes schlechter entscheiden, welcher Index am besten ist.
* Risiko: PostgreSQL wählt einen ineffizienten Index → schlechtere Performance.

---

### **5. Redundanz und Overhead**

* Gleiche oder ähnliche Indizes (z. B. auf `email` und zusätzlich auf `LOWER(email)`) können sich überlappen.
* Das führt zu unnötigem Overhead ohne zusätzlichen Nutzen.

---

### **Beispiel**

```sql
-- Übertrieben viele Indizes
CREATE INDEX idx_users_name ON users(name);
CREATE INDEX idx_users_name_lower ON users(LOWER(name));
CREATE INDEX idx_users_name_text_pattern ON users(name text_pattern_ops);
```

➡️ Diese Indizes könnten teilweise überflüssig sein und die Schreibperformance stark verschlechtern.

---

**Zusammenfassung:**
Zu viele Indizes führen zu **mehr Speicherverbrauch**, **langsamen Schreiboperationen**, **aufwendiger Wartung** und manchmal sogar zu **schlechterer Query-Performance**.
Empfehlung: Nur Indizes anlegen, die **konkret von Abfragen genutzt** werden.

📖 Quellen:

* [PostgreSQL Docs – Indexes](https://www.postgresql.org/docs/current/indexes.html)
* [PostgreSQL Performance Tuning Guide](https://www.postgresql.org/docs/current/performance-tips.html)


  **[⬆ Наверх](#top)**

35. ### <a name="35"></a> Wie analysiert man eine Query mit EXPLAIN?

### **Query-Analyse mit `EXPLAIN` in PostgreSQL**

Mit **`EXPLAIN`** zeigt PostgreSQL, **wie** eine Abfrage vom Query Planner ausgeführt wird.
So kann man Performanceprobleme erkennen (z. B. fehlende Indizes, Full Table Scans).

---

### **1. Einfaches `EXPLAIN`**

```sql
EXPLAIN
SELECT * FROM users WHERE email = 'max@example.com';
```

➡️ Gibt den **geplanten Ausführungsplan** zurück (z. B. „Seq Scan“ oder „Index Scan“).

---

### **2. `EXPLAIN ANALYZE`**

```sql
EXPLAIN ANALYZE
SELECT * FROM users WHERE email = 'max@example.com';
```

➡️ Führt die Abfrage **wirklich aus** und zeigt:

* Tatsächliche Laufzeit
* Anzahl der gescannten Zeilen
* Unterschied zwischen geschätzten und realen Werten

---

### **3. Typische Scan-Arten**

* **Seq Scan (Sequential Scan)** → Tabelle wird komplett gelesen (teuer bei großen Tabellen).
* **Index Scan** → Daten werden über einen Index gesucht (viel schneller).
* **Bitmap Index Scan** → Hybrid-Ansatz, nützlich bei vielen Treffern.
* **Nested Loop / Hash Join / Merge Join** → verschiedene Join-Strategien.

---

### **4. Beispielvergleich**

Ohne Index:

```sql
EXPLAIN ANALYZE
SELECT * FROM users WHERE email = 'max@example.com';
```

Ausgabe (gekürzt):

```
Seq Scan on users  (cost=0.00..35.50 rows=1 width=50)
  Filter: (email = 'max@example.com')
```

Mit Index:

```sql
CREATE INDEX idx_users_email ON users(email);

EXPLAIN ANALYZE
SELECT * FROM users WHERE email = 'max@example.com';
```

Ausgabe (gekürzt):

```
Index Scan using idx_users_email on users  (cost=0.15..8.17 rows=1 width=50)
  Index Cond: (email = 'max@example.com')
```

➡️ Deutlich effizienter.

---

### **5. Erweiterungen**

* `EXPLAIN (BUFFERS, ANALYZE)` → zeigt auch Lese-/Schreibzugriffe auf Datenblöcken.
* `EXPLAIN (FORMAT JSON)` → strukturierte Ausgabe für Tools.

---

**Zusammenfassung:**

* **`EXPLAIN`** → zeigt geplanten Ausführungsplan.
* **`EXPLAIN ANALYZE`** → zeigt zusätzlich echte Laufzeiten.
* Wichtig zur Optimierung von Abfragen (z. B. Einsatz von Indizes, Join-Strategien).

📖 Quellen:

* [PostgreSQL Docs – EXPLAIN](https://www.postgresql.org/docs/current/using-explain.html)


  **[⬆ Наверх](#top)**

36. ### <a name="36"></a> Unterschied zwischen EXPLAIN und EXPLAIN ANALYZE?

### **Unterschied zwischen `EXPLAIN` und `EXPLAIN ANALYZE` in PostgreSQL**

---

### **1. `EXPLAIN`**

* Zeigt den **geplanten Ausführungsplan** des Query Planners.
* Führt die Abfrage **nicht aus**.
* Liefert **geschätzte Kosten** (cost), Zeilenanzahl (rows) und Breite (width).
* Gut für eine schnelle **theoretische Analyse**.

**Beispiel:**

```sql
EXPLAIN
SELECT * FROM users WHERE email = 'max@example.com';
```

Ausgabe (gekürzt):

```
Seq Scan on users  (cost=0.00..35.50 rows=1 width=50)
  Filter: (email = 'max@example.com')
```

---

### **2. `EXPLAIN ANALYZE`**

* Führt die Abfrage **wirklich aus**.
* Zeigt zusätzlich **tatsächliche Laufzeiten** und die **wirklich gelesene Zeilenanzahl**.
* Hilfreich, um zu prüfen, ob die **Schätzungen des Planners korrekt** sind.
* Kann Änderungen an Daten (z. B. `INSERT`, `UPDATE`, `DELETE`) wirklich ausführen → Vorsicht in Produktion.

**Beispiel:**

```sql
EXPLAIN ANALYZE
SELECT * FROM users WHERE email = 'max@example.com';
```

Ausgabe (gekürzt):

```
Index Scan using idx_users_email on users  (cost=0.15..8.17 rows=1 width=50)
  Index Cond: (email = 'max@example.com')
  Actual time=0.020..0.022 rows=1 loops=1
```

---

### **Vergleich**

| Merkmal              | `EXPLAIN`        | `EXPLAIN ANALYZE`                           |
| -------------------- | ---------------- | ------------------------------------------- |
| Führt Query aus?     | Nein             | Ja                                          |
| Kosten / Schätzungen | Ja               | Ja                                          |
| Tatsächliche Zeiten  | Nein             | Ja                                          |
| Zeilenanzahl (real)  | Nein             | Ja                                          |
| Risiko               | Keine Änderungen | Führt Query wirklich aus (Vorsicht bei DML) |

---

**Zusammenfassung:**

* **`EXPLAIN`** → nur Plan, keine Ausführung.
* **`EXPLAIN ANALYZE`** → Plan + echte Laufzeiten (führt Query wirklich aus).

📖 Quellen:

* [PostgreSQL Docs – Using EXPLAIN](https://www.postgresql.org/docs/current/using-explain.html)


  **[⬆ Наверх](#top)**

37. ### <a name="37"></a> Wie vermeidet man Table Scans?

### **Table Scans in PostgreSQL vermeiden**

Ein **Sequential Scan (Table Scan)** bedeutet, dass PostgreSQL die komplette Tabelle Zeile für Zeile durchsucht.
Das ist bei großen Tabellen teuer. Ziel: Möglichst einen **Index Scan** nutzen.

---

### **1. Indexe anlegen**

* **B-Tree-Index** für Gleichheits- und Bereichsabfragen:

```sql
CREATE INDEX idx_users_email ON users(email);
```

➡️ Beschleunigt:

```sql
SELECT * FROM users WHERE email = 'max@example.com';
```

* **GIN-Index** für JSONB, Arrays, Volltextsuche:

```sql
CREATE INDEX idx_events_data ON events USING gin (data);
```

---

### **2. Geeignete Bedingungen schreiben**

* Abfragen so formulieren, dass der Index genutzt werden kann.
  ❌ Schlecht (kein Index-Use):

```sql
WHERE LOWER(email) = 'max@example.com'
```

✅ Besser (funktionaler Index):

```sql
CREATE INDEX idx_users_lower_email ON users(LOWER(email));
WHERE LOWER(email) = 'max@example.com';
```

---

### **3. Nur benötigte Spalten abfragen**

* `SELECT *` zwingt die DB oft zu mehr Arbeit.
* Lieber gezielt:

```sql
SELECT id, email FROM users WHERE email = 'max@example.com';
```

---

### **4. Statistiken aktuell halten**

* Query Planner verlässt sich auf Statistiken.
* Regelmäßig:

```sql
ANALYZE users;
```

Oder Auto-VACUUM aktivieren.

---

### **5. Partitionierung nutzen**

* Große Tabellen in **Partitionen** aufteilen, z. B. nach Datum.
* PostgreSQL durchsucht dann nur die relevante Partition.

```sql
CREATE TABLE logs (
  id SERIAL,
  created_at DATE,
  message TEXT
) PARTITION BY RANGE (created_at);
```

---

### **6. EXPLAIN verwenden**

* Prüfen, ob wirklich ein Index genutzt wird:

```sql
EXPLAIN ANALYZE
SELECT * FROM users WHERE email = 'max@example.com';
```

➡️ Statt `Seq Scan` sollte `Index Scan` erscheinen.

---

**Zusammenfassung:**
Table Scans vermeidet man durch **geeignete Indizes, optimierte Abfragen, aktuelle Statistiken und Partitionierung**. Mit `EXPLAIN` überprüft man den Query Plan.

📖 Quellen:

* [PostgreSQL Docs – Indexes](https://www.postgresql.org/docs/current/indexes.html)
* [PostgreSQL Docs – Performance Tips](https://www.postgresql.org/docs/current/performance-tips.html)


  **[⬆ Наверх](#top)**

38. ### <a name="38"></a> Was ist ein Partial Index?

### **Partial Index in PostgreSQL**

Ein **Partial Index** ist ein Index, der **nur für einen Teil der Zeilen einer Tabelle** erstellt wird – basierend auf einer **WHERE-Bedingung**.
Dadurch spart man **Speicherplatz** und beschleunigt Abfragen, die genau diese Bedingung nutzen.

---

### **1. Erstellung**

```sql
-- Index nur für aktive Benutzer
CREATE INDEX idx_users_active
ON users (email)
WHERE active = true;
```

---

### **2. Nutzung**

Dieser Index wird nur bei Abfragen verwendet, die dieselbe Bedingung enthalten:

```sql
SELECT * FROM users WHERE active = true AND email = 'max@example.com';
```

➡️ Schneller, weil nur ein Teil der Tabelle indexiert ist.

---

### **3. Vorteile**

* **Weniger Speicherplatz** als ein vollständiger Index.
* **Schnelleres Schreiben** (INSERT/UPDATE), da weniger Zeilen indexiert werden.
* Ideal bei **Tabellen mit vielen NULLs oder selten genutzten Werten**.

---

### **4. Einschränkungen**

* Nur effektiv, wenn Abfragen **die Bedingung des Index exakt enthalten**.
* Falsche Bedingung → Index wird nicht genutzt.

---

### **5. Beispiel für häufige Anwendung**

* Nur **nicht gelöschte Zeilen** indexieren (Soft Deletes):

```sql
CREATE INDEX idx_orders_not_deleted
ON orders (customer_id)
WHERE deleted_at IS NULL;
```

➡️ Abfragen nach aktiven Bestellungen sind schnell, gelöschte Daten werden ignoriert.

---

**Zusammenfassung:**
Ein **Partial Index** ist ein Index über eine Teilmenge der Daten, definiert durch eine WHERE-Bedingung. Er spart Speicher und verbessert Performance bei spezifischen Abfragen.

📖 Quellen:

* [PostgreSQL Docs – Partial Indexes](https://www.postgresql.org/docs/current/indexes-partial.html)


  **[⬆ Наверх](#top)**

39. ### <a name="39"></a> Was ist ein Covering Index (INCLUDE)?

### **Covering Index (INCLUDE) in PostgreSQL**

Ein **Covering Index** ist ein Index, der neben den indexierten Spalten auch **zusätzliche Spalten** speichert.
Diese zusätzlichen Spalten werden mit dem Schlüssel gespeichert, sind aber **nicht Teil der Index-Sortierung**.
In PostgreSQL wird das mit **`INCLUDE`** umgesetzt.

---

### **1. Zweck**

* Verhindert, dass PostgreSQL die Tabelle selbst (Heap) lesen muss.
* Die Abfrage kann vollständig aus dem Index beantwortet werden → **Index-only Scan**.
* Spart **I/O und Zeit**.

---

### **2. Beispiel**

```sql
-- Index auf email, zusätzlich name speichern
CREATE INDEX idx_users_email_include
ON users (email)
INCLUDE (name);
```

**Abfrage:**

```sql
SELECT email, name
FROM users
WHERE email = 'max@example.com';
```

➡️ PostgreSQL kann die Abfrage **nur mit dem Index** beantworten, ohne die Tabelle zu lesen.

---

### **3. Vorteile**

* **Schneller** bei häufigen SELECTs mit mehreren Spalten.
* Spart Speicher, da nicht alle Spalten im Index sortiert werden müssen.
* Besonders nützlich bei **breiten Tabellen**.

---

### **4. Einschränkungen**

* `INCLUDE`-Spalten können nicht für Sortierung oder Bedingungen (`WHERE`) genutzt werden.
* Sie dienen nur der **Abdeckung von SELECT-Ausgaben**.

---

### **5. Beispiel für typische Nutzung**

```sql
-- Eindeutigkeit nach user_id, aber zusätzlich Spalte created_at abdecken
CREATE UNIQUE INDEX idx_orders_user_product
ON orders (user_id, product_id)
INCLUDE (created_at);
```

➡️ Queries wie

```sql
SELECT user_id, product_id, created_at
FROM orders
WHERE user_id = 1 AND product_id = 5;
```

können komplett über den Index laufen.

---

**Zusammenfassung:**
Ein **Covering Index (INCLUDE)** speichert zusätzliche Spalten im Index, die nicht Teil der Schlüsseldefinition sind. Dadurch können Abfragen vollständig aus dem Index beantwortet werden (**Index-only Scan**) und werden schneller.

📖 Quellen:

* [PostgreSQL Docs – Indexes with INCLUDE](https://www.postgresql.org/docs/current/sql-createindex.html#SQL-CREATEINDEX-INCLUDE)


  **[⬆ Наверх](#top)**

40. ### <a name="40"></a> Wie funktioniert Vacuum in PostgreSQL?

### **VACUUM in PostgreSQL**

PostgreSQL nutzt ein **MVCC-Modell (Multi-Version Concurrency Control)**.
Dabei werden alte Versionen von Zeilen nicht sofort gelöscht, sondern als **tote Tupel** (dead tuples) markiert.
Das Kommando **`VACUUM`** bereinigt diese toten Tupel und hält Tabellen und Indizes effizient.

---

### **1. Aufgaben von VACUUM**

* Entfernt **nicht mehr benötigte Zeilen** (dead tuples).
* Gibt Speicherplatz **innerhalb der Tabelle** wieder frei.
* Hält **Index-Einträge** aktuell.
* Verhindert das Überschreiten des **Transaction ID Wraparound** (sonst Datenbankstop).

---

### **2. Arten von VACUUM**

#### 🔹 **VACUUM (Standard)**

* Bereinigt tote Tupel.
* Gibt Speicher nur intern wieder frei (nicht sofort an das Betriebssystem).
* Schnell, nicht blockierend.

```sql
VACUUM users;
```

#### 🔹 **VACUUM FULL**

* Kompaktet Tabellen komplett neu.
* Gibt Speicher **an das Betriebssystem** zurück.
* **Blockiert** die Tabelle während der Ausführung.
* Sehr ressourcenintensiv.

```sql
VACUUM FULL users;
```

#### 🔹 **AUTOVACUUM**

* Läuft automatisch im Hintergrund.
* Startet, wenn eine bestimmte Menge an Änderungen in einer Tabelle überschritten wird.
* Konfigurierbar über `postgresql.conf`.

---

### **3. Ergänzende Befehle**

* `ANALYZE` → aktualisiert Statistiken für den Query Planner.

```sql
VACUUM ANALYZE users;
```

* `REINDEX` → neuaufbau von Indizes, wenn diese zu groß oder fragmentiert sind.

---

### **4. Beispiel**

```sql
-- Standard-Vacuum für alle Tabellen
VACUUM;

-- Tabelle bereinigen + Statistiken aktualisieren
VACUUM ANALYZE orders;

-- Komplette Neuorganisation (teuer!)
VACUUM FULL orders;
```

---

### **5. Nachteile, wenn man VACUUM nicht nutzt**

* Tabellen und Indizes wachsen unnötig („bloating“).
* Abfragen werden langsamer.
* Gefahr des **Transaction ID Wraparound**, was die Datenbank unbenutzbar machen kann.

---

**Zusammenfassung:**
`VACUUM` entfernt alte Zeilen (dead tuples), hält Tabellen kompakt und schützt PostgreSQL vor Transaction-ID-Überlauf.

* **VACUUM** = leicht, regelmäßig.
* **VACUUM FULL** = schwer, blockierend, nur bei starkem Bloating nötig.
* **AUTOVACUUM** = läuft automatisch und sollte fast immer aktiviert bleiben.

📖 Quellen:

* [PostgreSQL Docs – VACUUM](https://www.postgresql.org/docs/current/sql-vacuum.html)
* [PostgreSQL Docs – Routine Vacuuming](https://www.postgresql.org/docs/current/routine-vacuuming.html)


  **[⬆ Наверх](#top)**  

41. ### <a name="41"></a> Wie startet und beendet man eine Transaktion?

### **Transaktionen in PostgreSQL starten und beenden**

Eine Transaktion ist ein Block von SQL-Anweisungen, die als **eine Einheit** ausgeführt werden.
In PostgreSQL gibt es dafür spezielle Befehle.

---

### **1. Start einer Transaktion**

```sql
BEGIN;   -- oder START TRANSACTION;
```

---

### **2. SQL-Befehle innerhalb der Transaktion**

```sql
UPDATE accounts
SET balance = balance - 100
WHERE id = 1;

UPDATE accounts
SET balance = balance + 100
WHERE id = 2;
```

---

### **3. Transaktion beenden**

* **Erfolgreich abschließen:**

```sql
COMMIT;
```

➡️ Alle Änderungen werden dauerhaft gespeichert.

* **Abbrechen:**

```sql
ROLLBACK;
```

➡️ Alle Änderungen seit `BEGIN` werden verworfen.

---

### **4. Komplettes Beispiel**

```sql
BEGIN;

UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;

COMMIT; -- oder ROLLBACK bei Fehler
```

---

### **5. Automatisches Verhalten**

* Standardmäßig läuft PostgreSQL im **Autocommit-Modus** → jede einzelne Query ist automatisch eine Transaktion.
* Mit `BEGIN` deaktiviert man Autocommit, bis `COMMIT` oder `ROLLBACK` ausgeführt wird.

---

**Zusammenfassung:**

* **BEGIN / START TRANSACTION** → Start
* **COMMIT** → Änderungen speichern
* **ROLLBACK** → Änderungen verwerfen
* Standard = Autocommit, explizite Transaktionen für mehrere zusammengehörige Befehle.

📖 Quellen:

* [PostgreSQL Docs – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)


  **[⬆ Наверх](#top)**

42. ### <a name="42"></a> Unterschied zwischen COMMIT und ROLLBACK?

### **Unterschied zwischen `COMMIT` und `ROLLBACK` in PostgreSQL**

---

### **1. COMMIT**

* Beendet eine Transaktion **erfolgreich**.
* Alle Änderungen (INSERT, UPDATE, DELETE) werden **dauerhaft gespeichert**.
* Andere Sessions sehen die Änderungen erst nach `COMMIT`.

**Beispiel:**

```sql
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT; -- Änderungen gespeichert
```

---

### **2. ROLLBACK**

* Bricht eine Transaktion **ab**.
* Alle Änderungen seit `BEGIN` werden **zurückgesetzt**.
* Datenbankzustand = wie vor Beginn der Transaktion.

**Beispiel:**

```sql
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
-- Fehler passiert hier
ROLLBACK; -- Änderungen rückgängig gemacht
```

---

### **Vergleich**

| Merkmal            | COMMIT                        | ROLLBACK             |
| ------------------ | ----------------------------- | -------------------- |
| Wirkung            | Änderungen speichern          | Änderungen verwerfen |
| Zeitpunkt sichtbar | Nach COMMIT für alle Sessions | Nie                  |
| Typischer Einsatz  | Erfolgreiche Transaktion      | Fehler oder Abbruch  |

---

**Zusammenfassung:**

* **COMMIT** → speichert Änderungen dauerhaft.
* **ROLLBACK** → macht Änderungen rückgängig.

📖 Quellen:

* [PostgreSQL Docs – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)


  **[⬆ Наверх](#top)**

43. ### <a name="43"></a> Was ist ein Savepoint in SQL?

### **Savepoint in SQL (PostgreSQL)**

Ein **Savepoint** ist ein **Zwischenpunkt innerhalb einer Transaktion**, auf den man mit `ROLLBACK TO` zurückspringen kann, ohne die ganze Transaktion abzubrechen.
Er erlaubt eine **feinere Kontrolle** über Fehlerbehandlung in langen oder komplexen Transaktionen.

---

### **1. Savepoint setzen**

```sql
BEGIN;

UPDATE accounts SET balance = balance - 100 WHERE id = 1;

SAVEPOINT sp1; -- Zwischenpunkt
```

---

### **2. Weiterarbeiten und ggf. zurückspringen**

```sql
UPDATE accounts SET balance = balance + 100 WHERE id = 2;

-- Fehler passiert, zurück zum Savepoint
ROLLBACK TO sp1;
```

➡️ Die Änderung an `account 2` wird verworfen, aber die vorherige Änderung (`account 1`) bleibt bestehen.

---

### **3. Transaktion fortsetzen**

```sql
UPDATE accounts SET balance = balance + 50 WHERE id = 3;

COMMIT; -- speichert die Änderungen endgültig
```

---

### **4. Savepoint löschen (optional)**

```sql
RELEASE SAVEPOINT sp1;
```

➡️ Entfernt den Savepoint, ohne die Transaktion zu beenden.

---

### **Vorteile**

* Ermöglicht **Teil-Rollbacks** innerhalb einer Transaktion.
* Nützlich bei komplexen Operationen mit mehreren Schritten.
* Verhindert unnötige Komplettabbrüche der Transaktion.

---

**Zusammenfassung:**
Ein **Savepoint** ist ein Marker in einer Transaktion, zu dem man mit `ROLLBACK TO` zurückspringen kann, ohne die ganze Transaktion zu verlieren.

📖 Quellen:

* [PostgreSQL Docs – Savepoints](https://www.postgresql.org/docs/current/sql-savepoint.html)


  **[⬆ Наверх](#top)**

44. ### <a name="44"></a> Unterschied zwischen Deadlock und Race Condition?

### **Unterschied zwischen Deadlock und Race Condition**

---

### **1. Deadlock**

* Situation, in der sich **zwei oder mehr Transaktionen gegenseitig blockieren**.
* Keine der Transaktionen kann fortfahren, weil jede auf eine Ressource wartet, die von der anderen gehalten wird.
* Führt zu einem Stillstand, den PostgreSQL automatisch erkennt → eine Transaktion wird abgebrochen.

**Beispiel:**

```sql
-- Transaktion A
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;

-- Transaktion B
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 2;

-- A will id=2 updaten, B will id=1 updaten → Deadlock
```

➡️ Ergebnis: PostgreSQL bricht eine Transaktion mit `ERROR: deadlock detected` ab.

---

### **2. Race Condition**

* Tritt auf, wenn mehrere Transaktionen **gleichzeitig auf dieselben Daten zugreifen** und das Ergebnis von der **Reihenfolge der Ausführung** abhängt.
* Kann zu **inkonsistenten Daten** führen, wenn keine Synchronisation erfolgt.

**Beispiel:**

```sql
-- Kontostand = 100

-- Transaktion A liest balance = 100
-- Transaktion B liest balance = 100

-- A zieht 30 ab → schreibt 70
-- B zieht 50 ab → schreibt 50

-- Endergebnis = 50 (statt 20!)
```

➡️ Das passiert durch **fehlende Isolation** (Lost Update).

---

### **Vergleich**

| Merkmal   | Deadlock                                  | Race Condition                                   |
| --------- | ----------------------------------------- | ------------------------------------------------ |
| Ursache   | Gegenseitige Sperren auf Ressourcen       | Gleichzeitiger Zugriff ohne Kontrolle            |
| Wirkung   | Vollständiger Stillstand (Blockade)       | Falsche oder unerwartete Ergebnisse              |
| Erkennung | DB erkennt und bricht eine Transaktion ab | Schwerer zu erkennen, erfordert Isolation Levels |
| Lösung    | Sperr-Reihenfolge konsistent halten       | Geeignete Isolation (`SERIALIZABLE`, Locks)      |

---

**Zusammenfassung:**

* **Deadlock** = gegenseitige Blockade → Stillstand, DB löst es durch Abbruch.
* **Race Condition** = parallele Zugriffe führen zu falschen Ergebnissen → verhindert durch Isolation oder Locks.

📖 Quellen:

* [PostgreSQL Docs – Concurrency Control](https://www.postgresql.org/docs/current/mvcc.html)
* [MDN Glossar – Race Condition (RU)](https://developer.mozilla.org/ru/docs/Glossary/Race_condition)


  **[⬆ Наверх](#top)**

45. ### <a name="45"></a> Welche Isolation Levels gibt es in PostgreSQL (READ COMMITTED, SERIALIZABLE)?

### **Isolation Levels in PostgreSQL**

Isolation Levels bestimmen, wie stark Transaktionen voneinander abgeschirmt werden. PostgreSQL unterstützt gemäß **SQL-Standard** drei Stufen:

---

### **1. READ COMMITTED (Standard in PostgreSQL)**

* Jede Abfrage innerhalb einer Transaktion sieht nur **bereits bestätigte Änderungen (COMMIT)**.
* Wenn eine andere Transaktion währenddessen Daten ändert, sieht die nächste Abfrage innerhalb derselben Transaktion **den neuen Stand**.
* Verhindert **Dirty Reads**, erlaubt aber **Non-Repeatable Reads** und **Phantom Reads**.

**Beispiel:**

```sql
BEGIN; -- Transaktion A
SELECT balance FROM accounts WHERE id = 1; -- Ergebnis: 100

-- Transaktion B führt UPDATE + COMMIT aus (balance = 200)

SELECT balance FROM accounts WHERE id = 1; -- Ergebnis: 200
COMMIT;
```

➡️ Wert hat sich während der Transaktion geändert → **Non-Repeatable Read** möglich.

---

### **2. REPEATABLE READ**

* Alle Abfragen innerhalb einer Transaktion sehen einen **konsistenten Schnappschuss** vom Start der Transaktion.
* Andere Commits sind währenddessen **nicht sichtbar**.
* Verhindert **Dirty Reads** und **Non-Repeatable Reads**.
* Aber **Phantom Reads** sind noch möglich.

---

### **3. SERIALIZABLE**

* Stärkste Isolation.
* Transaktionen werden so ausgeführt, als ob sie **nacheinander (seriell)** gelaufen wären.
* Verhindert **Dirty Reads, Non-Repeatable Reads und Phantom Reads**.
* Kann bei Konflikten zu Fehlern führen:

  ```text
  ERROR: could not serialize access due to concurrent update
  ```
* Lösung: Transaktion wiederholen.

---

### **Vergleich**

| Isolation Level | Dirty Read | Non-Repeatable Read | Phantom Read |
| --------------- | ---------- | ------------------- | ------------ |
| READ COMMITTED  | Nein       | Ja                  | Ja           |
| REPEATABLE READ | Nein       | Nein                | Ja           |
| SERIALIZABLE    | Nein       | Nein                | Nein         |

---

### **Setzen des Isolation Levels**

```sql
SET TRANSACTION ISOLATION LEVEL SERIALIZABLE;

BEGIN;
-- Transaktionslogik
COMMIT;
```

---

**Zusammenfassung:**

* **READ COMMITTED** = Standard, schnell, aber schwächere Isolation.
* **REPEATABLE READ** = konsistenter Snapshot, verhindert Non-Repeatable Reads.
* **SERIALIZABLE** = höchste Isolation, garantiert korrekte Ergebnisse, kann aber zu Rollbacks führen.

📖 Quellen:

* [PostgreSQL Docs – Transaction Isolation](https://www.postgresql.org/docs/current/transaction-iso.html)


  **[⬆ Наверх](#top)**

46. ### <a name="46"></a> Unterschied zwischen Optimistic Locking und Pessimistic Locking?

### **Unterschied zwischen Optimistic Locking und Pessimistic Locking**

---

### **1. Optimistic Locking**

* Annahme: **Konflikte treten selten auf**.
* Mehrere Transaktionen dürfen **gleichzeitig lesen und bearbeiten**.
* Beim Speichern wird geprüft, ob sich die Daten zwischenzeitlich geändert haben → wenn ja → Fehler / Wiederholung nötig.
* Technisch oft mit einer **Versionsspalte (`version`, `updated_at`)** umgesetzt.

**Beispiel:**

```sql
-- Tabelle mit Versionsspalte
CREATE TABLE accounts (
  id SERIAL PRIMARY KEY,
  balance NUMERIC,
  version INT DEFAULT 0
);

-- Update mit Optimistic Locking
UPDATE accounts
SET balance = balance - 100,
    version = version + 1
WHERE id = 1 AND version = 0;
```

➡️ Nur erfolgreich, wenn kein anderer die Zeile verändert hat.

**Vorteile:** Hohe Parallelität, kein Locking nötig.
**Nachteile:** Fehler beim Commit möglich → Transaktion muss wiederholt werden.

---

### **2. Pessimistic Locking**

* Annahme: **Konflikte treten häufig auf**.
* Eine Transaktion sperrt die Daten sofort → andere Transaktionen müssen warten.
* Verhindert Konflikte, aber reduziert Parallelität.

**Beispiel in PostgreSQL:**

```sql
BEGIN;

-- Sperrt die Zeile für andere Transaktionen (exclusive lock)
SELECT * FROM accounts
WHERE id = 1
FOR UPDATE;

-- Änderungen vornehmen
UPDATE accounts SET balance = balance - 100 WHERE id = 1;

COMMIT;
```

➡️ Andere Transaktionen können erst nach Freigabe weitermachen.

**Vorteile:** Keine Konflikte beim Commit.
**Nachteile:** Weniger parallel, Gefahr von Deadlocks.

---

### **Vergleich**

| Merkmal          | Optimistic Locking                             | Pessimistic Locking                              |
| ---------------- | ---------------------------------------------- | ------------------------------------------------ |
| Annahme          | Konflikte sind selten                          | Konflikte sind wahrscheinlich                    |
| Sperren          | Keine direkten Locks                           | Zeilen/Tabelle werden gesperrt                   |
| Performance      | Hohe Parallelität, effizient                   | Weniger parallel, langsamer bei vielen Zugriffen |
| Risiko           | Konflikte beim Commit, Wiederholung nötig      | Deadlocks, lange Wartezeiten möglich             |
| Typische Nutzung | Web-Apps, verteilte Systeme, seltene Konflikte | Banking, kritische Konsistenz, viele Konflikte   |

---

**Zusammenfassung:**

* **Optimistic Locking** → keine Sperren, Konflikte erst beim Commit erkannt.
* **Pessimistic Locking** → sofortige Sperre, Konflikte werden verhindert, aber weniger parallel.

📖 Quellen:

* [PostgreSQL Docs – Concurrency Control](https://www.postgresql.org/docs/current/mvcc.html)
* [MDN Glossar – Race Condition (RU)](https://developer.mozilla.org/ru/docs/Glossary/Race_condition)


  **[⬆ Наверх](#top)**

47. ### <a name="47"></a> Wie erkennt PostgreSQL Deadlocks?

### **Deadlock-Erkennung in PostgreSQL**

PostgreSQL arbeitet mit **Locks** (Sperren) auf Tabellen- oder Zeilenebene, um Konsistenz sicherzustellen.
Ein **Deadlock** entsteht, wenn zwei oder mehr Transaktionen sich gegenseitig blockieren:

* Transaktion A hält Sperre X und will Sperre Y.
* Transaktion B hält Sperre Y und will Sperre X.

Keiner kann fortfahren → Deadlock.

---

### **1. Deadlock Detection Mechanismus**

* PostgreSQL verwaltet intern ein **Lock-Wait-Graph**:

  * Knoten = Transaktionen
  * Kanten = Abhängigkeiten („wartet auf Sperre“)
* Bei jedem **Lock-Wait** prüft PostgreSQL, ob ein **Zyklus** im Graphen entsteht.
* Wenn Zyklus erkannt → **Deadlock**.

---

### **2. Verhalten bei Deadlock**

* PostgreSQL bricht **sofort eine der beteiligten Transaktionen** ab (die „billigste“ laut Heuristik → meist die mit weniger Ressourcenverbrauch).
* Die andere Transaktion darf weiterlaufen.

**Fehlermeldung:**

```text
ERROR: deadlock detected
DETAIL: Process 12345 waits for ShareLock on transaction 67890; blocked by process 67890.
```

---

### **3. Beispiel für Deadlock**

```sql
-- Transaktion A
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;

-- Transaktion B
BEGIN;
UPDATE accounts SET balance = balance - 200 WHERE id = 2;

-- A versucht nun id=2 zu sperren
UPDATE accounts SET balance = balance - 50 WHERE id = 2;

-- B versucht id=1 zu sperren → Deadlock
UPDATE accounts SET balance = balance - 30 WHERE id = 1;
```

➡️ PostgreSQL erkennt den Zyklus und bricht eine Transaktion ab.

---

### **4. Vermeidung von Deadlocks**

* **Konsistente Sperr-Reihenfolge** einhalten (immer gleiche Reihenfolge von Ressourcen sperren).
* Möglichst kleine Transaktionen.
* Sperren explizit mit `SELECT ... FOR UPDATE` setzen.

---

**Zusammenfassung:**
PostgreSQL erkennt Deadlocks durch Analyse des Lock-Wait-Graphen.
Bei einem Zyklus wird eine Transaktion automatisch abgebrochen, um das System zu entlasten.

📖 Quellen:

* [PostgreSQL Docs – Deadlocks](https://www.postgresql.org/docs/current/explicit-locking.html#LOCKING-DEADLOCKS)


  **[⬆ Наверх](#top)**

48. ### <a name="48"></a> Welche Standard-Isolationsebene nutzt PostgreSQL?

### **Standard-Isolationsebene in PostgreSQL**

PostgreSQL verwendet standardmäßig die Isolationsebene:

👉 **READ COMMITTED**

---

### **Eigenschaften von READ COMMITTED**

* Jede Anweisung innerhalb einer Transaktion sieht nur **bereits bestätigte Daten** (kein Dirty Read).
* Jede Anweisung liest einen **neuen Snapshot** der Daten → Änderungen anderer Transaktionen nach deren COMMIT sind sofort sichtbar.
* Zulässig sind aber:

  * **Non-Repeatable Reads** (derselbe SELECT kann verschiedene Ergebnisse liefern).
  * **Phantom Reads** (neue Zeilen können „auftauchen“).

---

### **Beispiel**

```sql
BEGIN; -- Transaktion A
SELECT balance FROM accounts WHERE id = 1; -- Ergebnis: 100

-- Parallel: Transaktion B
UPDATE accounts SET balance = 200 WHERE id = 1;
COMMIT;

-- Transaktion A fragt erneut ab
SELECT balance FROM accounts WHERE id = 1; -- Ergebnis: 200
COMMIT;
```

➡️ In derselben Transaktion sieht man beim zweiten SELECT den **geänderten Wert** → typisch für READ COMMITTED.

---

**Zusammenfassung:**
Die Standard-Isolationsebene in PostgreSQL ist **READ COMMITTED**.
Sie verhindert Dirty Reads, erlaubt aber Non-Repeatable Reads und Phantom Reads.

📖 Quellen:

* [PostgreSQL Docs – Transaction Isolation](https://www.postgresql.org/docs/current/transaction-iso.html)


  **[⬆ Наверх](#top)**

49. ### <a name="49"></a> Wie implementiert man Transaktionen in Node.js/Express mit PostgreSQL?

### **Transaktionen in Node.js/Express mit PostgreSQL**

---

#### **A) Mit `node-postgres` (`pg`) – manuell `BEGIN/COMMIT/ROLLBACK`**

```js
// ESM-Imports
import express from "express";
import pg from "pg";

const { Pool } = pg;
const app = express();
app.use(express.json());

const pool = new Pool({
  connectionString: process.env.DATABASE_URL,
  // ssl: { rejectUnauthorized: false } // falls nötig (Cloud)
});

// Transaktions-Wrapper (Hilfsfunktion)
async function withTransaction(fn, { isolation = "READ COMMITTED" } = {}) {
  const client = await pool.connect();
  try {
    await client.query("BEGIN");
    await client.query(`SET TRANSACTION ISOLATION LEVEL ${isolation}`);
    const result = await fn(client);            // alle Queries über denselben Client!
    await client.query("COMMIT");
    return result;
  } catch (err) {
    await client.query("ROLLBACK");
    throw err;
  } finally {
    client.release();
  }
}

// Beispiel-Route: Geld überweisen (ACID-sicher)
app.post("/transfer", async (req, res) => {
  const { fromId, toId, amount } = req.body;

  try {
    const result = await withTransaction(async (client) => {
      // 1) Abbuchen (mit Plausibilitätscheck)
      const { rows: [from] } = await client.query(
        `UPDATE accounts
           SET balance = balance - $1
         WHERE id = $2
         RETURNING id, balance`,
        [amount, fromId]
      );
      if (!from || from.balance < 0) {
        throw new Error("Unzureichendes Guthaben oder Konto nicht gefunden");
      }

      // 2) Gutschrift
      const { rows: [to] } = await client.query(
        `UPDATE accounts
           SET balance = balance + $1
         WHERE id = $2
         RETURNING id, balance`,
        [amount, toId]
      );
      if (!to) throw new Error("Zielkonto nicht gefunden");

      return { from, to };
    }, { isolation: "SERIALIZABLE" }); // optional: stärkeres Isolation Level

    res.json({ ok: true, result });
  } catch (e) {
    res.status(400).json({ ok: false, error: e.message });
  }
});

app.listen(3000);
```

**Hinweise:**

* **Immer denselben `client`** innerhalb der Transaktion verwenden.
* Bei Fehlern: `ROLLBACK` im `catch`.
* Optional: **Savepoints** für Teil-Rollbacks:

  ```js
  await client.query("SAVEPOINT sp1");
  // … riskante Operation …
  await client.query("ROLLBACK TO sp1"); // nur Teil zurücknehmen
  ```

---

#### **B) Mit Sequelize (ORM) – Transaktionen als API**

```js
// ESM-Imports
import { Sequelize, Transaction, DataTypes } from "sequelize";

export const sequelize = new Sequelize(process.env.DATABASE_URL, {
  dialect: "postgres"
});

const Account = sequelize.define("Account", {
  balance: { type: DataTypes.DECIMAL(12,2), allowNull: false }
}, { tableName: "accounts", timestamps: false });

// Muster: Manuelle Transaktion
async function transferSequelize(fromId, toId, amount) {
  const t = await sequelize.transaction({
    isolationLevel: Transaction.ISOLATION_LEVELS.SERIALIZABLE
  });

  try {
    const from = await Account.findByPk(fromId, { transaction: t, lock: t.LOCK.UPDATE });
    const to   = await Account.findByPk(toId,   { transaction: t, lock: t.LOCK.UPDATE });

    if (!from || !to) throw new Error("Konto nicht gefunden");
    if (Number(from.balance) < amount) throw new Error("Unzureichendes Guthaben");

    await from.update({ balance: Number(from.balance) - amount }, { transaction: t });
    await to.update({ balance: Number(to.balance) + amount }, { transaction: t });

    await t.commit();
    return { from, to };
  } catch (err) {
    await t.rollback();
    throw err;
  }
}
```

**Hinweise:**

* `transaction`-Objekt **überall weitergeben** (`find/update/create`).
* Optional: **`lock: t.LOCK.UPDATE`** für pessimistisches Locking (verhindert Race Conditions).
* Isolation Level je nach Bedarf wählen (z. B. `READ COMMITTED` vs. `SERIALIZABLE`).

---

#### **Best Practices**

* **Kleine, fokussierte Transaktionen** (kurze Sperrzeiten).
* **Konsistente Reihenfolge** beim Zugriff auf Ressourcen → Deadlocks vermeiden.
* **Explizite Fehlerbehandlung** und **Retry** bei `SERIALIZABLE`-Konflikten.
* **Parameterisierte Queries** (`$1, $2, …`) gegen SQL-Injection.
* **`EXPLAIN (ANALYZE, BUFFERS)`** nutzen, wenn Performance leidet.

---

**Zusammenfassung:**
Transaktionen in Node.js/Express mit PostgreSQL implementiert man entweder **niedrigschwellig mit `pg`** über `BEGIN/COMMIT/ROLLBACK` (ein Client pro Transaktion, Fehler → Rollback) oder **höherstufig mit Sequelize** via `sequelize.transaction(...)`. Isolation Level und optionales Locking/Savepoints sichern Korrektheit unter Parallelität.

📖 **Quellen:**

* [PostgreSQL – Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html)
* [PostgreSQL – Transaction Isolation](https://www.postgresql.org/docs/current/transaction-iso.html)
* [Express.js Offizielle Doku](https://expressjs.com/de/)
* [Node.js Dokumentation](https://nodejs.org/docs)
* [Sequelize – Transactions](https://sequelize.org/docs/v6/other-topics/transactions/)


  **[⬆ Наверх](#top)**

50. ### <a name="50"></a> Unterschied zwischen BEGIN und START TRANSACTION?

### **Unterschied zwischen `BEGIN` und `START TRANSACTION` in PostgreSQL**

---

### **1. BEGIN**

* Kürzere Schreibweise für den Transaktionsstart.
* Von PostgreSQL als Alias für `START TRANSACTION` implementiert.
* In PostgreSQL gängig, wird oft im Alltag verwendet.

**Beispiel:**

```sql
BEGIN;
UPDATE accounts SET balance = balance - 100 WHERE id = 1;
COMMIT;
```

---

### **2. START TRANSACTION**

* Standardkonforme SQL-Syntax (SQL-92).
* Bietet **mehr Optionen direkt beim Start**, z. B. Isolation Level oder Read/Write-Modus.

**Beispiel:**

```sql
START TRANSACTION ISOLATION LEVEL SERIALIZABLE READ WRITE;
UPDATE accounts SET balance = balance + 100 WHERE id = 2;
COMMIT;
```

---

### **3. Technischer Unterschied in PostgreSQL**

* Funktional **kein Unterschied** → beide starten eine Transaktion.
* Nur bei **zusätzlichen Optionen** ist `START TRANSACTION` nötig.
* PostgreSQL-Doku empfiehlt `START TRANSACTION`, wenn man **Isolation Levels oder Modus** setzen möchte.

---

### **Vergleich**

| Merkmal              | `BEGIN`                      | `START TRANSACTION`           |
| -------------------- | ---------------------------- | ----------------------------- |
| SQL-Standard         | Nein (PostgreSQL-spezifisch) | Ja (SQL-konform)              |
| Optionen (Isolation) | Nicht möglich                | Direkt beim Start möglich     |
| Nutzung              | Kürzer, häufiger             | Formeller, für komplexe Fälle |

---

**Zusammenfassung:**

* **`BEGIN`** = PostgreSQL-Kurzform.
* **`START TRANSACTION`** = Standard-SQL, mit Optionen wie Isolation Level und Read/Write-Modus.
* In PostgreSQL sind beide im Alltag gleichwertig, außer man will spezielle Einstellungen setzen.

📖 Quellen:

* [PostgreSQL Docs – Transaction Control](https://www.postgresql.org/docs/current/sql-begin.html)
* [PostgreSQL Docs – START TRANSACTION](https://www.postgresql.org/docs/current/sql-start-transaction.html)


  **[⬆ Наверх](#top)**  

51. ### <a name="51"></a> Wie verwaltet man Benutzer und Rollen in PostgreSQL?

### **Benutzer- und Rollenverwaltung in PostgreSQL**

In PostgreSQL sind **Benutzer und Rollen dasselbe Konzept**:

* **Benutzer** = Rolle mit **Login-Recht**.
* **Rolle** = Kann Berechtigungen haben und Mitglied anderer Rollen sein.

---

### **1. Benutzer/Rollen erstellen**

```sql
-- Benutzer mit Login-Recht
CREATE ROLE max LOGIN PASSWORD 'geheim';

-- Nur Rolle ohne Login
CREATE ROLE read_only;
```

---

### **2. Rechte vergeben**

```sql
-- Rechte für eine Tabelle
GRANT SELECT, INSERT ON users TO max;

-- Rolle als Gruppe nutzen
GRANT read_only TO max; -- Benutzer max ist jetzt Mitglied von read_only
```

---

### **3. Attribute von Rollen**

* `LOGIN` → erlaubt Anmeldung.
* `SUPERUSER` → uneingeschränkte Rechte.
* `CREATEDB` → darf neue Datenbanken anlegen.
* `CREATEROLE` → darf neue Rollen erstellen.
* `REPLICATION` → für Streaming-Replikation.
* `INHERIT` → erbt Rechte von Rollen, in denen sie Mitglied ist.

**Beispiel:**

```sql
CREATE ROLE admin LOGIN PASSWORD 'admin123'
  CREATEDB CREATEROLE;
```

---

### **4. Rollen ändern**

```sql
ALTER ROLE max WITH PASSWORD 'neuPasswort';
ALTER ROLE max WITH LOGIN;
```

---

### **5. Rollen löschen**

```sql
DROP ROLE max;
```

---

### **6. Aktuelle Rollen anzeigen**

```sql
\du   -- im psql-Client
```

Beispielausgabe:

```
 Role name | Attributes                 | Member of
-----------+----------------------------+-----------
 postgres  | Superuser, Create DB       | {}
 max       |                            | {read_only}
```

---

### **7. Best Practices**

* Für **jeden Entwickler/Service eigenen Benutzer** anlegen.
* Rechte so restriktiv wie möglich vergeben (**Principle of Least Privilege**).
* Rollen als Gruppen nutzen (z. B. `read_only`, `read_write`).

---

**Zusammenfassung:**
PostgreSQL verwaltet Benutzer und Rollen über das gleiche Konzept: Rollen können **Login-Rechte** haben und Berechtigungen übernehmen. Man vergibt Rechte über `GRANT`, organisiert Nutzer in Rollen-Gruppen und nutzt Attribute wie `CREATEDB` oder `CREATEROLE` für erweiterte Privilegien.

📖 Quellen:

* [PostgreSQL Docs – Database Roles](https://www.postgresql.org/docs/current/user-manag.html)
* [PostgreSQL Docs – GRANT](https://www.postgresql.org/docs/current/sql-grant.html)


  **[⬆ Наверх](#top)**

52. ### <a name="52"></a> Unterschied zwischen Login-Rollen und Gruppen-Rollen?

### **Unterschied zwischen Login-Rollen und Gruppen-Rollen in PostgreSQL**

PostgreSQL kennt nur **Rollen** – diese können unterschiedliche Attribute haben.
Der Unterschied zwischen **Login-Rollen** und **Gruppen-Rollen** ergibt sich aus deren Rechten.

---

### **1. Login-Rollen**

* Rollen mit dem Attribut **`LOGIN`**.
* Können sich **anmelden** (z. B. per `psql`, Anwendung, Benutzerkonto).
* Werden als **Benutzer** verstanden.

**Beispiel:**

```sql
CREATE ROLE max LOGIN PASSWORD 'geheim';
```

➡️ `max` kann sich direkt an der Datenbank anmelden.

---

### **2. Gruppen-Rollen**

* Rollen **ohne `LOGIN`**.
* Dienen als **Sammelrollen**, um Berechtigungen zu bündeln.
* Können an Login-Rollen vergeben werden.

**Beispiel:**

```sql
CREATE ROLE read_only; -- ohne LOGIN
GRANT SELECT ON ALL TABLES IN SCHEMA public TO read_only;

-- Benutzer max erhält die Gruppenrolle
GRANT read_only TO max;
```

➡️ `max` kann sich einloggen und hat zusätzlich **READ-ONLY-Rechte**.

---

### **3. Vergleich**

| Merkmal       | Login-Rolle                  | Gruppen-Rolle                 |
| ------------- | ---------------------------- | ----------------------------- |
| LOGIN möglich | ✅ Ja                         | ❌ Nein                        |
| Zweck         | Benutzerkonto                | Rechtebündel (Gruppe)         |
| Beispiel      | `CREATE ROLE anna LOGIN ...` | `CREATE ROLE reporting;`      |
| Nutzung       | Verbindung zur DB            | Verwaltung von Berechtigungen |

---

**Zusammenfassung:**

* **Login-Rolle** = tatsächlicher Benutzer (kann sich anmelden).
* **Gruppen-Rolle** = Sammlung von Berechtigungen (wird Benutzern zugewiesen).
  Best Practice: **Benutzer = Login-Rollen**, **Gruppen = Rollen ohne Login** für Rechteverwaltung.

📖 Quellen:

* [PostgreSQL Docs – Database Roles](https://www.postgresql.org/docs/current/user-manag.html)


  **[⬆ Наверх](#top)**

53. ### <a name="53"></a> Wie vergibt man Berechtigungen (GRANT, REVOKE)?

### **Berechtigungen in PostgreSQL mit `GRANT` und `REVOKE`**

PostgreSQL steuert den Zugriff auf Objekte (Tabellen, Schemata, Funktionen usw.) über **Privileges**.
Man vergibt (`GRANT`) oder entzieht (`REVOKE`) diese an Rollen oder Benutzer.

---

### **1. GRANT – Rechte vergeben**

```sql
-- SELECT-Recht auf Tabelle users an Rolle read_only
GRANT SELECT ON users TO read_only;

-- Alle Rechte auf Tabelle users an Benutzer max
GRANT ALL PRIVILEGES ON users TO max;

-- Nutzung eines Schemas erlauben
GRANT USAGE ON SCHEMA public TO read_only;
```

➡️ `GRANT` ermöglicht Rollen/Benutzern den Zugriff.

---

### **2. REVOKE – Rechte entziehen**

```sql
-- SELECT-Recht entziehen
REVOKE SELECT ON users FROM read_only;

-- Alle Rechte entziehen
REVOKE ALL PRIVILEGES ON users FROM max;
```

➡️ `REVOKE` entfernt bestimmte oder alle Rechte.

---

### **3. Verfügbare Privilegien (häufig genutzt)**

* **SELECT** → Lesen von Tabellen/Views.
* **INSERT** → Neue Zeilen einfügen.
* **UPDATE** → Daten ändern.
* **DELETE** → Daten löschen.
* **TRUNCATE** → Tabelle leeren.
* **REFERENCES** → Fremdschlüssel auf Tabelle setzen.
* **USAGE** → Nutzung von Schema oder Sequenz.
* **EXECUTE** → Funktionen/Prozeduren ausführen.
* **ALL PRIVILEGES** → alle verfügbaren Rechte.

---

### **4. Beispiel: Kombinierte Nutzung**

```sql
-- Neue Gruppe mit Lese-Rechten
CREATE ROLE read_only;

-- Lesezugriff auf alle Tabellen im Schema public
GRANT CONNECT ON DATABASE mydb TO read_only;
GRANT USAGE ON SCHEMA public TO read_only;
GRANT SELECT ON ALL TABLES IN SCHEMA public TO read_only;

-- Benutzer max bekommt die Rolle
GRANT read_only TO max;
```

---

### **5. Rechte entziehen**

```sql
-- Benutzer max darf nicht mehr lesen
REVOKE read_only FROM max;
```

---

### **6. Aktuelle Berechtigungen anzeigen**

```sql
\z users   -- im psql-Client: zeigt Privilegien für Tabelle users
```

---

**Zusammenfassung:**

* **`GRANT`** → Rechte vergeben.
* **`REVOKE`** → Rechte entziehen.
* Typische Rechte: `SELECT`, `INSERT`, `UPDATE`, `DELETE`, `USAGE`, `EXECUTE`.
* Best Practice: **Gruppenrollen für Berechtigungen**, **Login-Rollen für Benutzer**.

📖 Quellen:

* [PostgreSQL Docs – GRANT](https://www.postgresql.org/docs/current/sql-grant.html)
* [PostgreSQL Docs – REVOKE](https://www.postgresql.org/docs/current/sql-revoke.html)


  **[⬆ Наверх](#top)**

54. ### <a name="54"></a> Was ist Row Level Security (RLS) in PostgreSQL?

### **Row Level Security (RLS) in PostgreSQL**

**Row Level Security (RLS)** ist ein Sicherheitsmechanismus, mit dem man **Zugriffsrechte auf Zeilenebene** steuern kann.
Damit wird festgelegt, **welche Zeilen einer Tabelle ein Benutzer sehen oder ändern darf**.

---

### **1. Aktivierung von RLS**

```sql
ALTER TABLE accounts ENABLE ROW LEVEL SECURITY;
```

---

### **2. Policies definieren**

Eine **Policy** beschreibt die Bedingungen, unter denen ein Benutzer Zeilen lesen, einfügen oder ändern darf.

**Beispiel: Benutzer darf nur seine eigenen Konten sehen**

```sql
CREATE POLICY user_can_select_own_rows
ON accounts
FOR SELECT
USING (owner_id = current_user::int);
```

➡️ `USING` definiert, welche Zeilen bei `SELECT` sichtbar sind.

---

### **3. Policies für andere Operationen**

* **SELECT** → Zugriff auf Zeilen beim Lesen
* **INSERT** → Bedingungen für neue Zeilen
* **UPDATE** → Welche Zeilen aktualisiert werden dürfen
* **DELETE** → Welche Zeilen gelöscht werden dürfen

**Beispiel: Benutzer darf nur eigene Zeilen ändern**

```sql
CREATE POLICY user_can_update_own_rows
ON accounts
FOR UPDATE
USING (owner_id = current_user::int);
```

---

### **4. Zugriff für alle Benutzer (optional)**

Falls auch Superuser-Rollen oder bestimmte Gruppen Zugriff haben sollen:

```sql
ALTER TABLE accounts FORCE ROW LEVEL SECURITY; -- erzwingt RLS
```

---

### **5. Kombination mit GRANT**

* RLS ersetzt nicht `GRANT`/`REVOKE`.
* Erst **Basisrechte** (z. B. `SELECT`, `UPDATE`) vergeben, dann über Policies fein steuern.

---

### **6. Beispiel komplett**

```sql
-- Tabelle mit Konten
CREATE TABLE accounts (
  id SERIAL PRIMARY KEY,
  owner_id INT NOT NULL,
  balance NUMERIC NOT NULL
);

-- RLS aktivieren
ALTER TABLE accounts ENABLE ROW LEVEL SECURITY;

-- Policy: jeder Benutzer sieht nur seine eigenen Zeilen
CREATE POLICY own_rows_only
ON accounts
FOR SELECT
USING (owner_id = current_user::int);

-- Rechte vergeben
GRANT SELECT ON accounts TO public;
```

---

### **Vorteile von RLS**

* Sehr fein granulierte Sicherheit.
* Besonders nützlich für **Multi-Tenant-Apps** (z. B. SaaS-Systeme).
* Regeln liegen **direkt in der Datenbank** → weniger Logik im Code.

---

**Zusammenfassung:**
Row Level Security (RLS) ermöglicht Zugriffskontrolle **auf Zeilenebene** in PostgreSQL. Mit Policies legt man fest, welche Zeilen ein Benutzer lesen, einfügen, ändern oder löschen darf.

📖 Quellen:

* [PostgreSQL Docs – Row Security Policies](https://www.postgresql.org/docs/current/ddl-rowsecurity.html)


  **[⬆ Наверх](#top)**

55. ### <a name="55"></a> Wie schützt man sensible Daten (z. B. Passwörter) in PostgreSQL?

### **Schutz sensibler Daten (z. B. Passwörter) in PostgreSQL**

---

#### **1) Passwörter: niemals im Klartext**

* **Hash + Salt** verwenden (empfohlen: **Argon2id**, alternativ **bcrypt**).
* Hashing **in der Applikation** durchführen; DB speichert nur den Hash.
* In PostgreSQL-Only-Setups kann `pgcrypto` genutzt werden.

**Node.js (ESM) mit Argon2id**

```js
import argon2 from "argon2";

// Hashen
const hash = await argon2.hash(plaintextPassword, {
  type: argon2.argon2id,
  memoryCost: 2 ** 16,  // z. B. 64 MiB
  timeCost: 3,
  parallelism: 1
});

// Prüfen
const ok = await argon2.verify(hash, loginPassword);
```

**PostgreSQL (pgcrypto, falls Hashing in der DB)**

```sql
CREATE EXTENSION IF NOT EXISTS pgcrypto;

-- bcrypt-Hash erstellen/prüfen
UPDATE users SET password_hash = crypt($1, gen_salt('bf'));
SELECT crypt($1, password_hash) = password_hash AS valid FROM users WHERE email=$2;
```

---

#### **2) Transport & Zugriff**

* **TLS aktivieren** (Client↔Server): `ssl = on`, Zertifikate nutzen.
* **Least Privilege**: separate **Login-Rollen** pro Service, nur benötigte Rechte (`GRANT/REVOKE`).
* **RLS** (Row Level Security) für mandantenfähige/zeilengranulare Zugriffe.
* **Sensible Spalten abschirmen**: nur über **Views** freigeben; direkte Spaltenrechte entziehen.

---

#### **3) Daten „at rest“**

* **Festplatten-/Volume-Verschlüsselung** (OS/Cloud) für das Cluster.
* **Spaltenweise Verschlüsselung** für besonders sensible Felder mit `pgcrypto`.

```sql
CREATE EXTENSION IF NOT EXISTS pgcrypto;

-- symmetrisch verschlüsseln (z. B. Steuer-ID)
INSERT INTO persons(ssn_enc)
VALUES (pgp_sym_encrypt('123-45-6789', current_setting('app.encryption_key')));

-- entschlüsseln
SELECT pgp_sym_decrypt(ssn_enc, current_setting('app.encryption_key')) AS ssn
FROM persons;
```

> Schlüssel **nie** hartkodieren; via **Server-Var/Secret-Manager** injizieren (z. B. `ALTER DATABASE SET app.encryption_key TO '...';` nur zur Laufzeit setzen).

---

#### **4) Server-Authentifizierung**

* **SCRAM-SHA-256** für DB-Rollen aktivieren:

```sql
ALTER SYSTEM SET password_encryption = 'scram-sha-256';
SELECT pg_reload_conf();
```

* Alte `md5`-Passwörter migrieren.

---

#### **5) Auditing & Betrieb**

* **Logging** sensibler Spalten verhindern (kein PII in Logs).
* **Backups** verschlüsseln (z. B. `pg_dump` → verschlüsselte Speicherung).
* **EXPLAIN/Parameterization**: Nur **parametrisierte Queries** verwenden, kein SQL-Injection.
* **Regelmäßige Updates** (PostgreSQL/OS), **Rechte-Review**, **Rotation** von Secrets/Keys.

---

#### **6) Wann DB-seitiges Hashing sinnvoll ist**

* Zentralisierte Passwortlogik ohne Applikationszugriff auf Klartext.
* Beachte: Funktionsumfang (Argon2) ist in DB begrenzt; moderne KDFs besser **in der App**.

---

**Zusammenfassung:**

* Passwörter stets mit **Argon2id/bcrypt** hashen (idealerweise in der App); nur Hash speichern.
* **TLS**, **Least Privilege**, **RLS** und **Views** für Zugriffskontrolle.
* **At-rest-Schutz** via Volume-Verschlüsselung und gezielte **Spaltenverschlüsselung** mit `pgcrypto`.
* **SCRAM-SHA-256** für Rollenpasswörter aktivieren; Backups/Logs sicher handhaben.

📖 **Quellen:**

* [PostgreSQL Docs – Data Types / `pgcrypto`](https://www.postgresql.org/docs/current/pgcrypto.html)
* [PostgreSQL Docs – Row Security](https://www.postgresql.org/docs/current/ddl-rowsecurity.html)
* [PostgreSQL Docs – GRANT/REVOKE](https://www.postgresql.org/docs/current/sql-grant.html)
* [PostgreSQL Docs – Authentication / `password_encryption`](https://www.postgresql.org/docs/current/auth-password.html)
* [MDN (RU) – Пароли и аутентификация (общие рекомендации)](https://developer.mozilla.org/ru/)


  **[⬆ Наверх](#top)**

56. ### <a name="56"></a> Wie sichert man eine PostgreSQL-Datenbank (pg_dump)?

### **Backup einer PostgreSQL-Datenbank mit `pg_dump`**

Das Standardwerkzeug für Backups in PostgreSQL ist **`pg_dump`**. Es erstellt **logische Backups**, d. h. SQL-Skripte oder portierbare Dumps, die unabhängig von der PostgreSQL-Version sind.

---

### **1. Einfache Sicherung (SQL-Skript)**

```bash
pg_dump -U username -d mydb > backup.sql
```

* Enthält alle `CREATE TABLE`, `INSERT` usw.
* Kann mit `psql` wiederhergestellt werden:

```bash
psql -U username -d mydb < backup.sql
```

---

### **2. Backup mit Schema + Daten**

* **Nur Schema (ohne Daten):**

```bash
pg_dump -U username -s mydb > schema.sql
```

* **Nur Daten (ohne Schema):**

```bash
pg_dump -U username -a mydb > data.sql
```

---

### **3. Komprimierte / Custom Backups**

`pg_dump` kann auch im **Custom-Format** sichern (`-Fc`):

```bash
pg_dump -U username -d mydb -Fc > backup.dump
```

Wiederherstellung mit `pg_restore`:

```bash
pg_restore -U username -d mydb backup.dump
```

---

### **4. Parallele Backups (schneller bei großen DBs)**

Nur im **Custom/Directory-Format** möglich:

```bash
pg_dump -U username -d mydb -Fd -j 4 -f /backups/mydb_dir
```

* `-Fd` = Directory-Format
* `-j 4` = 4 parallele Jobs

Wiederherstellung:

```bash
pg_restore -U username -d mydb -j 4 /backups/mydb_dir
```

---

### **5. Ganze Cluster sichern (alle DBs)**

Dafür nutzt man **`pg_dumpall`**:

```bash
pg_dumpall -U username > cluster_backup.sql
```

➡️ Enthält auch Rollen und globale Objekte.

---

### **6. Best Practices**

* **Automatisieren** (z. B. via Cronjob):

```bash
0 2 * * * pg_dump -U username -Fc mydb > /backups/mydb_$(date +\%F).dump
```

* **Backups verschlüsseln** (z. B. mit `gpg`).
* **Regelmäßig testen** (`restore` auf Testsystem prüfen).
* Für sehr große DBs: zusätzlich **physische Backups** mit **`pg_basebackup`** oder Replikation.

---

**Zusammenfassung:**

* `pg_dump` → Backup einer einzelnen DB (Schema + Daten).
* Formate: **SQL (Standard)**, **Custom/Directory (schnell, parallel, flexibel)**.
* Wiederherstellung: `psql` (SQL) oder `pg_restore` (Custom/Dir).
* **pg\_dumpall** → Backup des gesamten Clusters inkl. Rollen.

📖 Quellen:

* [PostgreSQL Docs – pg\_dump](https://www.postgresql.org/docs/current/app-pgdump.html)
* [PostgreSQL Docs – pg\_restore](https://www.postgresql.org/docs/current/app-pgrestore.html)
* [PostgreSQL Docs – pg\_dumpall](https://www.postgresql.org/docs/current/app-pgdumpall.html)


  **[⬆ Наверх](#top)**

57. ### <a name="57"></a> Wie stellt man ein Backup wieder her?

### **Wiederherstellung eines PostgreSQL-Backups**

Die Wiederherstellung hängt vom Format des Backups ab, das mit `pg_dump` oder `pg_dumpall` erstellt wurde.

---

### **1. SQL-Backup (Plain Text)**

* Enthält `CREATE TABLE`, `INSERT`, … → direkt mit `psql` einspielen.

```bash
psql -U username -d mydb < backup.sql
```

➡️ Vorher sicherstellen, dass die Datenbank **existiert**:

```bash
createdb -U username mydb
```

---

### **2. Custom- oder Directory-Format (`-Fc`, `-Fd`)**

* Muss mit **pg\_restore** wiederhergestellt werden.

**Einfaches Restore in bestehende DB:**

```bash
pg_restore -U username -d mydb backup.dump
```

**Vorherige Datenbank ersetzen (DROP + CREATE):**

```bash
pg_restore -U username -C -d postgres backup.dump
```

➡️ `-C` erstellt die Datenbank automatisch.

**Paralleles Restore (schneller):**

```bash
pg_restore -U username -d mydb -j 4 /backups/mydb_dir
```

---

### **3. Komplettes Cluster-Backup (`pg_dumpall`)**

```bash
psql -U username -f cluster_backup.sql postgres
```

➡️ Spielt **alle Datenbanken + Rollen** wieder ein.

---

### **4. Best Practices**

* Immer **auf Testsystem prüfen**, bevor man ein Backup in Produktion einspielt.
* Gegebenenfalls vorher DB löschen/leeren:

```bash
dropdb -U username mydb
createdb -U username mydb
```

* Bei großen DBs: besser **pg\_restore im Directory-Format mit -j (parallel)** nutzen.
* Für Rollen/Rechte: `pg_dumpall --globals-only` sichern und mit `psql` zurückspielen.

---

**Zusammenfassung:**

* **SQL-Backups** → mit `psql` einspielen.
* **Custom/Directory-Backups** → mit `pg_restore`.
* **pg\_dumpall-Backups** → mit `psql` auf `postgres` zurückspielen.

📖 Quellen:

* [PostgreSQL Docs – Restoring the Dump](https://www.postgresql.org/docs/current/backup-dump.html#BACKUP-DUMP-RESTORE)
* [PostgreSQL Docs – pg\_restore](https://www.postgresql.org/docs/current/app-pgrestore.html)


  **[⬆ Наверх](#top)**

58. ### <a name="58"></a> Unterschied zwischen pg_dump und pg_restore?

### **Unterschied zwischen `pg_dump` und `pg_restore` in PostgreSQL**

---

### **1. `pg_dump`**

* Werkzeug zum **Erstellen von Backups**.
* Erzeugt ein **logisches Backup** (Daten + Schema).
* Unterstützte Formate:

  * **Plain SQL** (`.sql`) → direkt mit `psql` einspielbar.
  * **Custom** (`-Fc`) → komprimiert, für `pg_restore`.
  * **Directory** (`-Fd`) → Ordnerstruktur, parallele Dumps möglich.
  * **Tar** (`-Ft`).

**Beispiel:**

```bash
pg_dump -U username -d mydb > backup.sql      # Plain SQL
pg_dump -U username -Fc mydb > backup.dump    # Custom Format
```

---

### **2. `pg_restore`**

* Werkzeug zum **Wiederherstellen von Backups**, die mit `pg_dump` im **Custom/Directory/Tar-Format** erstellt wurden.
* Vorteile gegenüber `psql` (bei Plain SQL):

  * Selektives Restore (z. B. nur bestimmte Tabellen/Funktionen).
  * Paralleles Restore (`-j`).
  * Kontrolle über Reihenfolge und Objekte.

**Beispiel:**

```bash
pg_restore -U username -d mydb backup.dump        # Restore Custom-Backup
pg_restore -U username -d mydb -j 4 mydb_dir      # Restore Directory-Backup parallel
pg_restore -l backup.dump                         # Liste der enthaltenen Objekte
pg_restore -t users -d mydb backup.dump           # Nur Tabelle "users" wiederherstellen
```

---

### **3. Vergleich**

| Merkmal            | `pg_dump`                       | `pg_restore`                            |
| ------------------ | ------------------------------- | --------------------------------------- |
| Zweck              | Backup erstellen                | Backup wiederherstellen                 |
| Input              | Datenbank                       | Dump-Datei (Custom/Dir/Tar)             |
| Output             | Dump-Datei (SQL/Custom/Dir/Tar) | Datenbank (oder SQL)                    |
| Plain-SQL nutzbar? | Ja                              | Nein (dafür `psql`)                     |
| Selektives Restore | Nein                            | Ja (z. B. einzelne Tabellen/Funktionen) |
| Parallelisierung   | Beim Dump mit `-Fd`             | Beim Restore mit `-j`                   |

---

**Zusammenfassung:**

* **`pg_dump`** → erstellt ein Backup (SQL oder spezielles Format).
* **`pg_restore`** → spielt Backups im **Custom/Directory/Tar-Format** wieder ein und erlaubt selektives, paralleles Restore.
* Für **Plain SQL Dumps** nutzt man direkt `psql` zum Wiederherstellen.

📖 Quellen:

* [PostgreSQL Docs – pg\_dump](https://www.postgresql.org/docs/current/app-pgdump.html)
* [PostgreSQL Docs – pg\_restore](https://www.postgresql.org/docs/current/app-pgrestore.html)


  **[⬆ Наверх](#top)**

59. ### <a name="59"></a> Wie konfiguriert man SSL für PostgreSQL-Verbindungen?

### **SSL/TLS für PostgreSQL-Verbindungen konfigurieren**

---

#### **1) Server-Zertifikate erstellen/ablegen**

```bash
# Self-signed (Test)
openssl req -new -x509 -days 365 -nodes \
  -out server.crt -keyout server.key -subj "/CN=db.example.com"

# Rechte setzen (wichtig!)
chmod 600 server.key
chown postgres:postgres server.crt server.key

# In PG-Datenverzeichnis verschieben (z. B. /var/lib/postgresql/data)
mv server.crt server.key $PGDATA/
```

> Produktion: **CA-signiertes** Zertifikat (z. B. via Let’s Encrypt). Chain korrekt ablegen (server.crt inkl. Intermediate).

---

#### **2) `postgresql.conf`**

```conf
ssl = on
ssl_cert_file = 'server.crt'
ssl_key_file  = 'server.key'
# optional: ssl_ciphers, ssl_min_protocol_version = 'TLSv1.2'
```

---

#### **3) `pg_hba.conf` (nur SSL erlauben)**

```conf
# Nur SSL-Verbindungen akzeptieren:
hostssl all all 0.0.0.0/0 scram-sha-256
hostssl all all ::0/0       scram-sha-256

# (Optional) Non-SSL explizit ablehnen:
hostnossl all all 0.0.0.0/0 reject
hostnossl all all ::0/0     reject
```

> Optional: **Client-Zertifikate** erzwingen (`clientcert=verify-full`) bei hostssl-Zeilen.

---

#### **4) Server neu laden**

```bash
pg_ctl reload   # oder: SELECT pg_reload_conf();
```

---

#### **5) Clientseite – `psql` testen**

```bash
# Mindestens SSL verwenden
psql "host=db.example.com dbname=mydb user=myuser sslmode=require"

# Server gegen CA prüfen (empfohlen)
# Root-CA lokal speichern: ~/.postgresql/root.crt
psql "host=db.example.com dbname=mydb user=myuser sslmode=verify-full"
```

**sslmode-Übersicht:**

* `require` → verschlüsselt, prüft Zertifikat **nicht**
* `verify-ca` → CA geprüft, **Hostnamen nicht**
* `verify-full` → CA **und** Hostname geprüft (**empfohlen**)

---

#### **6) Node.js/Express (`pg`)**

```js
import pg from "pg";
import fs from "node:fs";

const pool = new pg.Pool({
  host: "db.example.com",
  user: "myuser",
  database: "mydb",
  password: process.env.DB_PASSWORD,
  port: 5432,
  ssl: {
    rejectUnauthorized: true,                   // wie verify-full
    ca:   fs.readFileSync("/etc/ssl/rootCA.pem").toString(),
    // optional bei mTLS (Client-Zertifikate):
    // key:  fs.readFileSync("/etc/ssl/client.key").toString(),
    // cert: fs.readFileSync("/etc/ssl/client.crt").toString(),
  },
});
```

---

#### **7) Verifikation & Betrieb**

* **Überprüfen:** `SHOW ssl;` (sollte `on` sein), `\conninfo` in `psql` (zeigt TLS).
* **Schlüssel schützen:** `server.key` ausschließlich für `postgres` lesbar.
* **Nur starke Protokolle/Cipher:** `ssl_min_protocol_version = 'TLSv1.2'` oder höher.
* **Hostname passend zum Zertifikat** (CN/SAN = `db.example.com`).
* **Backups/HA:** Zertifikate/Keys sicher versionieren/rotieren (kein Git!).

---

**Zusammenfassung:**
SSL aktivieren (`ssl=on`), Zertifikat/Key mit restriktiven Rechten ins Datenverzeichnis legen, in `pg_hba.conf` **hostssl** nutzen (optional non-SSL blockieren), Server neu laden. Clients mit `sslmode=verify-full` und korrekter CA verbinden; in Node.js `ssl.rejectUnauthorized=true` plus `ca` verwenden. Produktion: CA-signierte Zertifikate und starke TLS-Einstellungen.

📖 **Quellen:**

* [PostgreSQL Docs – SSL Support](https://www.postgresql.org/docs/current/ssl-tcp.html)
* [PostgreSQL Docs – Client Authentication (`pg_hba.conf`)](https://www.postgresql.org/docs/current/auth-pg-hba-conf.html)
* [PostgreSQL Docs – libpq SSL Modes](https://www.postgresql.org/docs/current/libpq-ssl.html)


  **[⬆ Наверх](#top)**

60. ### <a name="60"></a> Was ist Connection Pooling und wie implementiert man es (z. B. mit pg-pool in Node.js)?

### **Connection Pooling in PostgreSQL & Implementierung mit `pg` (pg-pool) in Node.js**

**Definition:**
Connection Pooling hält **wiederverwendbare DB-Verbindungen** offen, statt pro Request eine neue TCP/SSL-/Auth-Verbindung aufzubauen. Ziel: **Latenz reduzieren**, **Ressourcen begrenzen**, **Durchsatz erhöhen**.

---

### **Warum Pooling?**

* Neue Verbindungen sind teuer (Handshake, Auth, TLS).
* PostgreSQL hat **Begrenzungen pro Server**; zu viele parallele Sessions schaden der Performance.
* Gleichmäßige Lastverteilung und Backpressure (max. Verbindungen).

---

### **Implementierung mit `pg` (ESM)**

```js
// pool.js
import pg from "pg";
const { Pool } = pg;

export const pool = new Pool({
  connectionString: process.env.DATABASE_URL,
  max: 10,                 // maximale gleichzeitige Verbindungen im Pool
  idleTimeoutMillis: 30_000, // Idle-Verbindung schließen nach 30s
  connectionTimeoutMillis: 5_000, // Wartezeit bis Verbindungsaufbau fehlschlägt
  // ssl: { rejectUnauthorized: true, ca: '...'} // falls nötig
});

// optional: sauberes Herunterfahren (z. B. bei SIGTERM/K8s)
process.on("SIGTERM", async () => {
  await pool.end();
  process.exit(0);
});
```

```js
// app.js
import express from "express";
import { pool } from "./pool.js";

const app = express();
app.use(express.json());

// Einfache Query (Pool verwaltet Verbindungen)
app.get("/users", async (_req, res) => {
  try {
    const { rows } = await pool.query("SELECT id, email FROM users ORDER BY id LIMIT 100");
    res.json(rows);
  } catch (e) {
    res.status(500).json({ error: e.message });
  }
});

// Transaktion: immer denselben Client verwenden!
app.post("/transfer", async (req, res) => {
  const { fromId, toId, amount } = req.body;
  const client = await pool.connect();
  try {
    await client.query("BEGIN");
    const { rows: [from] } = await client.query(
      "UPDATE accounts SET balance = balance - $1 WHERE id = $2 RETURNING id,balance",
      [amount, fromId]
    );
    if (!from || Number(from.balance) < 0) throw new Error("Unzureichendes Guthaben");
    await client.query(
      "UPDATE accounts SET balance = balance + $1 WHERE id = $2",
      [amount, toId]
    );
    await client.query("COMMIT");
    res.json({ ok: true });
  } catch (err) {
    await client.query("ROLLBACK");
    res.status(400).json({ ok: false, error: err.message });
  } finally {
    client.release(); // sehr wichtig: sonst Verbindungs-Leak!
  }
});

app.listen(3000);
```

---

### **Best Practices**

* **Ein Pool pro Prozess**, nicht pro Request/Route erstellen.
* **`max`** sinnvoll setzen (z. B. Anzahl CPU-Worker × 5–10) und **Serverlimit** beachten (`max_connections` bzw. PgBouncer-Limit).
* **Transaktionen:** denselben **`client`** durchreichen; nach Nutzung **`release()`**.
* **Timeouts**/**Backpressure** konfigurieren (z. B. `connectionTimeoutMillis`).
* **SSL/TLS** korrekt konfigurieren in produktiven Umgebungen.
* **Pooling auf Infrastruktur-Ebene:** Für viele Services/Server **PgBouncer** nutzen (Modus *transaction pooling* für hohe Parallelität, *session pooling* wenn Session-Features nötig, z. B. Temp-Tables, CTE-cursors).

---

### **Typische Fehler**

* Pool in jeder Funktion neu erzeugen → **Verbindungsflut**.
* `client.release()` vergessen → **Pool erschöpft** (Hänger).
* Zu hohes `max` → Server thrashen (zu viele gleichzeitige Queries).
* PgBouncer im *transaction pooling* mit **Session-State** (z. B. `SET LOCAL`, Temp-Tables) kombinieren → unerwartetes Verhalten.

---

**Zusammenfassung:**
Connection Pooling hält eine begrenzte Anzahl wiederverwendbarer Verbindungen und reduziert Verbindungs-Overhead. In Node.js nutzt man einen **zentralen `Pool` aus `pg`**, gibt bei Transaktionen denselben Client weiter und released ihn zuverlässig. Für viele App-Instanzen empfiehlt sich zusätzlich **PgBouncer**.

📖 **Quellen:**

* [Node-Postgres (`pg`) – Pool](https://node-postgres.com/features/pooling)
* [PostgreSQL Docs – libpq / Verbindungen](https://www.postgresql.org/docs/current/libpq-connect.html)
* [Express.js Offizielle Doku](https://expressjs.com/de/)
* [PostgreSQL Performance-Tipps](https://www.postgresql.org/docs/current/performance-tips.html)


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
