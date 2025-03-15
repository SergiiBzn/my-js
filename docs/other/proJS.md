<a name="top"></a>

[На главную](../README.md)

[Перейти к вопросам](#questions)

| №. | Вопрос |
| --- | --------- |
|   | JavaScript Grundlagen |
|1 | [Klassifizierung von Datentypen, Typumwandlung](#1) |
|2 | [Unterschied zwischen null und undefined](#2) |
|3 | [Variablen let, const, var. Strikter Modus](#3) |
|4 | [Interaktion mit dem Benutzer: alert(), prompt(), confirm()](#4) |
|5 | [Interpolation (ES6)](#5) |
|6 | [Operatoren in JavaScript](#6) |
|7 | [Bedingungen](#7) |
|8 | [Schleifen, verschachtelte Schleifen, Labels](#8) |
|9 | [Hoisting (Hochheben von Variablen und Funktionen)](#9) |
|10 | [Ausführungskontext, Lexikalische Umgebung](#10) |
|11 | [Temporäre Totzone (Temporal Dead Zone)](#11) |
|12 | [typeof – wie erkennt man den Typ eines Werts?](#12) |
|13 | [Warum haben primitive Datentypen Methoden? Was ist Autoboxing?](#13) |
|14 | [Garbage Collector in JavaScript](#14) |
|15 | [](#15) |
|16 | [](#16) |
|17 | [](#17) |
|18 | [](#18) |
|19 | [](#19) |
|20 | [](#20) |
|   | Funktionen und ihre Besonderheiten |
|21 | [Funktionen, Pfeilfunktionen, IIFE](#21) |
|22 | [Methoden zur Kontextbindung (call, apply, bind)](#22) |
|23 | [Closures (Abschlüsse)](#23) |
|24 | [Callback-Funktionen](#24) |
|25 | [Konstruktor-Funktionen](#25) |
|26 | [Aufrufkontext (this)](#26) |
|27 | [Getter und Setter (Objekteigenschaften)](#27) |
|28 | [Generatorfunktionen](#28) |
|29 | [Rekursion](#29) |
|30 | [](#30) |
|   | Arbeiten mit Objekten |
|31 | [Objekte, Destrukturierung von Objekten (ES6)](#31) |
|32 | [Methoden Object, Object.prototype](#32) |
|33 | [Möglichkeiten zur Objekterstellung](#33) |
|34 | [Kopieren von Objekten](#34) |
|35 | [Property Descriptors (Eigenschaftsbeschreibungen)](#35) |
|36 | [Private und geschützte Eigenschaften von Objekten](#36) |
|37 | [Prototypen, Prototypen-Kette](#37) |
|38 | [Object.create()](#38) |
|39 | [Unterschied zwischen klassischer und prototypischer Vererbung](#39) |
|40 | [](#40) |
|   | Arrays und Sammlungen |
|41 | [](#41) |
|42 | [](#42) |
|43 | [](#43) |
|44 | [](#44) |
|45 | [](#45) |
|46 | [](#46) |
|47 | [](#47) |
|48 | [](#48) |
|49 | [](#49) |
|50 | [](#50) |



<a name="questions"></a>

## JavaScript Grundlagen

  **[⬆ Наверх](#top)**
  
1. ### <a name="1"></a> Klassifizierung von Datentypen, Typumwandlung

### **Datentypen in JavaScript**  

In JavaScript gibt es **primitive Datentypen** und **Referenztypen**.  

---

## **1. Primitive Datentypen (Werte werden direkt gespeichert)**  
Primitive Datentypen sind **immutable** (unveränderlich) und speichern Werte direkt im Speicher.

| Datentyp   | Beschreibung | Beispiel |
|------------|-------------|-----------|
| **`string`** | Zeichenkette | `"Hallo"`, `'Test'`, `` `Template` `` |
| **`number`** | Zahlen (Ganzzahlen, Dezimal, `NaN`, `Infinity`) | `42`, `3.14`, `NaN`, `Infinity` |
| **`bigint`** | Sehr große Ganzzahlen | `123456789012345678901234567890n` |
| **`boolean`** | Wahrheitswerte | `true`, `false` |
| **`undefined`** | Variable wurde deklariert, aber nicht zugewiesen | `let x; console.log(x); // undefined` |
| **`null`** | Bewusste "leere" Variable | `let y = null;` |
| **`symbol`** | Einzigartige, unveränderliche Identifikatoren | `let id = Symbol("id");` |

```js
let name = "Max"; // string
let alter = 25; // number
let isStudent = true; // boolean
let nichts = null; // null
let unbestimmt; // undefined
let großeZahl = 123456789012345678901n; // bigint
let uniqueKey = Symbol("key"); // symbol
```

---

## **2. Referenztypen (Speichern Verweise auf Objekte im Speicher)**
Referenztypen speichern **Referenzen** auf Speicherorte, nicht die Werte direkt.

| Datentyp   | Beschreibung | Beispiel |
|------------|-------------|-----------|
| **`object`** | Sammlungen von Werten als Key-Value-Paare | `{name: "Max", alter: 25}` |
| **`array`** | Listen von Werten | `[1, 2, 3, "Test"]` |
| **`function`** | Funktionen sind Objekte | `function add(a, b) { return a + b; }` |
| **`date`** | Datum und Zeit | `new Date()` |
| **`RegExp`** | Reguläre Ausdrücke | `/abc/i` |

```js
let person = { name: "Max", alter: 25 }; // Objekt
let zahlen = [1, 2, 3, 4]; // Array
function sagHallo() { console.log("Hallo!"); } // Funktion
let heute = new Date(); // Datum
let regex = /abc/i; // Regulärer Ausdruck
```

---

## **3. Unterschiede zwischen Primitiven und Referenztypen**
| Eigenschaft | Primitive Typen | Referenztypen |
|------------|----------------|--------------|
| Speicherort | Direkt im Stack gespeichert | Verweis auf Speicheradresse im Heap |
| Vergleich | Vergleicht Werte (`===` und `==` gleich) | Vergleicht Speicherreferenzen (`{}` !== `{}`) |
| Veränderbarkeit | **Immutable** (Wert kann nicht direkt geändert werden) | **Mutable** (Werte innerhalb des Objekts/Arrays können geändert werden) |

```js
let a = 5;
let b = a;
b = 10;
console.log(a); // 5 (unverändert)

let obj1 = { name: "Max" };
let obj2 = obj1; // Referenz auf dasselbe Objekt
obj2.name = "Anna";
console.log(obj1.name); // "Anna" (beide verweisen auf dasselbe Objekt)
```

---

## **4. Sonderfälle**
### **Falsy und Truthy Werte**
#### **Falsy-Werte (`Boolean(wert) → false`)**
Diese Werte werden als `false` interpretiert:
```js
false, 0, "", null, undefined, NaN
```

#### **Truthy-Werte (`Boolean(wert) → true`)**
Alle anderen Werte sind `true`, z. B.:
```js
"0", "false", [], {}, function() {}, Infinity
```

```js
console.log(Boolean(0)); // false
console.log(Boolean("")); // false
console.log(Boolean([])); // true (leeres Array ist truthy)
console.log(Boolean({})); // true (leeres Objekt ist truthy)
```

---

## **5. Dynamische Typisierung in JavaScript**
JavaScript ist eine **dynamisch typisierte** Sprache, d. h., eine Variable kann den Typ zur Laufzeit ändern:
```js
let x = "Hallo"; // String
x = 42; // Jetzt eine Zahl
x = true; // Jetzt ein Boolean
console.log(x); // true
```

---

### **Zusammenfassung**
✅ **Primitive Typen** speichern Werte direkt und sind immutable.  
✅ **Referenztypen** speichern Verweise auf Objekte und sind veränderbar.  
✅ **Vergleich von Referenztypen** erfolgt über Speicherreferenzen.  
✅ **Falsy-Werte** sind `0, "", null, undefined, NaN`.  
✅ **Dynamische Typisierung** erlaubt das Ändern von Typen zur Laufzeit.


### **Typumwandlung in JavaScript (Type Conversion)**

In JavaScript gibt es zwei Arten der Typumwandlung:
1. **Implizite Typumwandlung (Type Coercion)** → Automatische Konvertierung durch JavaScript  
2. **Explizite Typumwandlung (Type Casting)** → Manuelle Konvertierung durch den Entwickler

---

## **1. Implizite Typumwandlung (Automatische Umwandlung)**
JavaScript wandelt Werte automatisch um, wenn sie in bestimmten Operationen verwendet werden.

### **String-Konkatenation mit `+` (Zahl → String)**
```js
console.log("10" + 5); // "105" (Zahl wird zu String)
console.log(5 + "10"); // "510"
console.log("Hello " + true); // "Hello true"
```

### **Arithmetische Operationen (`-`, `*`, `/`) (String → Zahl)**
```js
console.log("10" - 5); // 5 ("10" wird zu 10)
console.log("6" * "2"); // 12
console.log("100" / "10"); // 10
console.log("5" - true); // 4 (true → 1)
console.log("5" - false); // 5 (false → 0)
```

### **Vergleiche mit `==` (Typumwandlung vor dem Vergleich)**
```js
console.log(0 == "0");  // true (String wird zu Zahl)
console.log(false == ""); // true ("" wird zu false)
console.log(null == undefined); // true
```
👉 **Verwende `===`, um ohne Typumwandlung zu vergleichen!**
```js
console.log(0 === "0"); // false
console.log(false === ""); // false
```

---

## **2. Explizite Typumwandlung (Manuelle Umwandlung)**
Hier erfolgt die Umwandlung durch Methoden wie `Number()`, `String()`, `Boolean()`.

### **String → Number**
```js
console.log(Number("42")); // 42
console.log(Number("3.14")); // 3.14
console.log(Number("10abc")); // NaN (Fehler, da "abc" keine Zahl ist)
console.log(parseInt("42px")); // 42 (ignoriert "px")
console.log(parseFloat("3.14abc")); // 3.14
```

### **Number → String**
```js
console.log(String(100)); // "100"
console.log((42).toString()); // "42"
console.log((3.14).toFixed(1)); // "3.1" (Rundet und gibt String zurück)
```

### **Beliebiger Wert → Boolean**
```js
console.log(Boolean(1)); // true
console.log(Boolean(0)); // false
console.log(Boolean("Hello")); // true
console.log(Boolean("")); // false
console.log(Boolean(null)); // false
console.log(Boolean(undefined)); // false
console.log(Boolean([])); // true (leeres Array ist truthy!)
console.log(Boolean({})); // true (leeres Objekt ist truthy!)
```

---

## **Spezialfälle und Fallstricke**
### **1. `NaN` (Not-a-Number)**
```js
console.log(Number("abc")); // NaN
console.log(0 / 0); // NaN
console.log(NaN == NaN); // false (NaN ist nicht gleich NaN!)
```

### **2. `null` und `undefined` Verhalten**
```js
console.log(Number(null)); // 0
console.log(Number(undefined)); // NaN
console.log(Boolean(null)); // false
console.log(Boolean(undefined)); // false
```

---

## **Fazit**
- **Implizite Typumwandlung** passiert automatisch, kann aber zu unerwarteten Ergebnissen führen.
- **Explizite Typumwandlung** ist sicherer und kontrollierter.
- **Nutze `===` statt `==`**, um unerwartete Konvertierungen zu vermeiden.

---
📖 Weitere Informationen findest du in der offiziellen [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Data_structures).

  **[⬆ Наверх](#top)**

2. ### <a name="2"></a> Unterschied zwischen null und undefined

# Unterschied zwischen `null` und `undefined` in JavaScript

In JavaScript stehen `null` und `undefined` für das Fehlen eines Wertes, aber sie unterscheiden sich in ihrer Bedeutung und Verwendung.

## **`undefined`**
- Eine Variable wurde deklariert, aber nicht initialisiert.
- Ist der Standardwert für nicht zugewiesene Variablen.
- Wird zurückgegeben, wenn eine Funktion kein explizites `return` hat.
- Wird zurückgegeben, wenn auf eine nicht existierende Objekt-Eigenschaft oder ein nicht existierendes Array-Element zugegriffen wird.

### **Beispiele für `undefined`**
```js
let x;
console.log(x); // undefined
```

```js
function doSomething() {
  // Keine Rückgabe
}
console.log(doSomething()); // undefined
```

```js
let obj = {};
console.log(obj.nonExistentProperty); // undefined
```

## **`null`**
- `null` ist ein expliziter Wert, der anzeigt, dass eine Variable bewusst leer oder nicht gesetzt ist.
- Wird vom Entwickler zugewiesen, um eine Variable als „ohne Wert“ zu markieren.

### **Beispiel für `null`**
```js
let y = null;
console.log(y); // null
```

## **Unterschiede zusammengefasst**
| Eigenschaft   | `undefined` | `null` |
|--------------|------------|--------|
| Standardwert | Ja (bei nicht zugewiesenen Variablen) | Nein (muss explizit gesetzt werden) |
| Rückgabewert | Funktionen ohne `return`, fehlende Objekteigenschaften | Muss manuell zugewiesen werden |
| Typ          | `undefined` | `object` (bekannter JavaScript-Bug) |

## **Wann `null` oder `undefined` verwenden?**
- **Verwende `null`**, wenn du eine Variable explizit auf „kein Wert“ setzen möchtest.
- **Lass `undefined`** dem System überlassen (z. B. nicht initialisierte Variablen, fehlende Eigenschaften).

---
📖 Weitere Informationen findest du in der offiziellen [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/null).

  **[⬆ Наверх](#top)**

3. ### <a name="3"></a> Variablen let, const, var. Strikter Modus

# `let`, `const`, `var` und der strikte Modus in JavaScript

## **Unterschiede zwischen `let`, `const` und `var`**
JavaScript bietet drei Möglichkeiten, Variablen zu deklarieren: `let`, `const` und `var`. Hier sind ihre Unterschiede:

### **`let`** – Blockscope und Neu-Zuweisung erlaubt
- Hat **Block-Scope** (gültig innerhalb `{}`).
- Kann neu zugewiesen werden.
- **Hoisting:** Wird hochgehoben, aber nicht initialisiert.

**Beispiel:**
```js
let x = 5;
if (true) {
  let x = 10;
  console.log(x); // 10 (innerhalb des Blocks)
}
console.log(x); // 5 (außerhalb des Blocks)
```

### **`const`** – Blockscope und unveränderlich
- Hat ebenfalls **Block-Scope**.
- Muss **direkt initialisiert** werden.
- Kann **nicht** neu zugewiesen werden.

**Beispiel:**
```js
const y = 7;
// y = 10; // ❌ Fehler: `const`-Variablen können nicht neu zugewiesen werden.
```

### **`var`** – Funktionaler Scope und Hoisting
- Hat **funktionalen Scope** (sichtbar in der gesamten Funktion, in der sie deklariert wurde).
- Wird **gehoistet** und erhält beim Hoisting den Wert `undefined`.
- Kann überschrieben und neu deklariert werden.

**Beispiel:**
```js
var z = 3;
if (true) {
  var z = 6;
  console.log(z); // 6
}
console.log(z); // 6 (da `var` global oder funktionsweit gültig ist)
```

🚀 **Empfehlung:** Verwende **`let`** oder **`const`**, da sie sicherer sind. **`var`** sollte vermieden werden.

---

## **Strikter Modus (`"use strict"`)**
Der **strikte Modus** (`"use strict";`) aktiviert eine strengere Interpretation von JavaScript und hilft, Fehler frühzeitig zu erkennen.

### **Aktivierung des strikten Modus**
```js
"use strict";
function myFunction() {
  x = 10; // ❌ Fehler: `x` wurde nicht mit `let`, `const` oder `var` deklariert.
}
```

### **Wichtige Änderungen durch `"use strict"`**
1. **Keine impliziten globalen Variablen**
   ```js
   "use strict";
   myVar = 10; // ❌ Fehler: Variable wurde nicht deklariert.
   ```

2. **Kein mehrfaches Deklarieren von Parametern**
   ```js
   "use strict";
   function sum(a, a) { // ❌ Fehler: Doppelte Parameter-Namen nicht erlaubt.
       return a + a;
   }
   ```

3. **Kein Löschen von Variablen und Funktionen**
   ```js
   "use strict";
   let myVar = 10;
   delete myVar; // ❌ Fehler: Variablen können nicht gelöscht werden.
   ```

4. **`this` ist `undefined` in einer Funktion**
   ```js
   "use strict";
   function show() {
       console.log(this); // `undefined` statt `window`
   }
   show();
   ```

### **Warum `"use strict"` verwenden?**
✅ Verhindert häufige Fehler.  
✅ Erhöht die Code-Sicherheit.  
✅ Hilft, modernen JavaScript-Standards zu entsprechen.

📖 Weitere Informationen findest du in der offiziellen [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Strict_mode).

  **[⬆ Наверх](#top)**

4. ### <a name="4"></a> Interaktion mit dem Benutzer: alert(), prompt(), confirm()

# Benutzerinteraktion in JavaScript: `alert()`, `prompt()`, `confirm()`

JavaScript bietet drei eingebaute Funktionen zur Benutzerinteraktion über modale Dialoge im Browser: `alert()`, `prompt()` und `confirm()`. Diese blockieren die weitere Ausführung des Skripts, bis der Benutzer eine Aktion ausführt.

## **`alert()` – Anzeige einer einfachen Nachricht**
Verwendet, um eine Nachricht in einem Dialogfeld mit einer **OK-Schaltfläche** anzuzeigen. 

**Beispiel:**
```js
alert("Hallo, Welt!"); // Zeigt eine Meldung an.
```

📌 **Eigenschaften:**
- Blockiert den Code, bis der Benutzer auf **OK** klickt.
- Hat **keine** Rückgabe (immer `undefined`).

---

## **`prompt()` – Benutzereingabe anfordern**
Zeigt ein Dialogfeld mit einer Nachricht, einem **Eingabefeld** und den Schaltflächen **OK / Abbrechen**.

**Beispiel:**
```js
let name = prompt("Wie heißt du?");
console.log("Hallo, " + name + "!");
```

📌 **Eigenschaften:**
- Gibt den **eingegebenen Text** als `string` zurück.
- Gibt `null` zurück, wenn der Benutzer **Abbrechen** klickt.
- Standardmäßig wird alles als `string` gespeichert (auch Zahlen!).

👉 **Achtung:** Wenn eine Zahl benötigt wird, sollte `Number()` verwendet werden:
```js
let age = Number(prompt("Gib dein Alter ein:"));
console.log(age + 1); // Falls eine Zahl eingegeben wurde, wird sie korrekt erhöht.
```

---

## **`confirm()` – Benutzerentscheidung abfragen**
Zeigt ein Dialogfeld mit einer Nachricht und zwei Schaltflächen: **OK / Abbrechen**.

**Beispiel:**
```js
let result = confirm("Bist du sicher?");
if (result) {
  console.log("Benutzer hat OK geklickt");
} else {
  console.log("Benutzer hat Abbrechen geklickt");
}
```

📌 **Eigenschaften:**
- Gibt `true` zurück, wenn der Benutzer **OK** klickt.
- Gibt `false` zurück, wenn der Benutzer **Abbrechen** klickt.

---

## **Einschränkungen der Modalfenster**
❌ Können nicht gestylt oder angepasst werden.  
❌ Unterbrechen den Codefluss (synchron).  
❌ Können in modernen Web-Apps störend sein, daher sind **benutzerdefinierte Dialoge** (`<dialog>`-Element oder modale Fenster mit JavaScript/CSS) oft besser.

📖 Weitere Informationen findest du in der offiziellen [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/API/Window/alert).

  **[⬆ Наверх](#top)**

5. ### <a name="5"></a> Interpolation (ES6)

### **Interpolation in JavaScript (ES6)**

Interpolation in JavaScript refers to embedding variables or expressions inside a string literal dynamically. This is done using **template literals**, introduced in **ES6**.

#### **Syntax of Template Literals**
Template literals are enclosed in **backticks** (`` ` ``) instead of quotes. The placeholders for variables or expressions are written inside **`${}`**.

```js
let variable = "Wert";
let expression = 2 + 2;

let interpolatedString = `Text: ${variable}, Ausdruck: ${expression}`;
console.log(interpolatedString); // "Text: Wert, Ausdruck: 4"
```

#### **Example: Dynamic String Construction**
```js
let name = "Alice";
let age = 25;

let message = `Hallo, mein Name ist ${name} und ich bin ${age} Jahre alt.`;
console.log(message);
// Ausgabe: "Hallo, mein Name ist Alice und ich bin 25 Jahre alt."
```

#### **Advantages of Template Literals**
✅ **Better Readability**: No need to concatenate strings using `+`.  
✅ **Expression Embedding**: Mathematical operations or function calls can be directly embedded.  
✅ **Multiline Strings**: Supports **multiline strings** without `\n`.  

**Example with Multiline String:**
```js
let text = `Das ist eine mehrzeilige
Zeichenkette ohne Escape-Sequenzen.`;
console.log(text);
```

📌 **Use Case:** Template literals make it easier to build dynamic messages, queries, or HTML content.

Weitere Details findest du in den [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Template_literals). 🚀

  **[⬆ Наверх](#top)**

6. ### <a name="6"></a> Operatoren in JavaScript

### **Operatoren in JavaScript**  

JavaScript bietet verschiedene Operatoren, die in mehrere Kategorien unterteilt werden können:  

---

## **1. Arithmetische Operatoren**
Diese Operatoren führen mathematische Berechnungen durch.  

| Operator | Beschreibung  | Beispiel | Ergebnis |
|----------|--------------|----------|----------|
| `+`      | Addition     | `5 + 2`  | `7` |
| `-`      | Subtraktion  | `5 - 2`  | `3` |
| `*`      | Multiplikation | `5 * 2` | `10` |
| `/`      | Division     | `5 / 2`  | `2.5` |
| `%`      | Modulo (Rest) | `5 % 2`  | `1` |
| `++`     | Inkrement    | `let a = 5; a++` | `6` |
| `--`     | Dekrement    | `let b = 2; b--` | `1` |

**Beispiel:**  
```js
let a = 5;
let b = 2;

console.log(a + b); // 7
console.log(a - b); // 3
console.log(a * b); // 10
console.log(a / b); // 2.5
console.log(a % b); // 1
```

---

## **2. Zuweisungsoperatoren**
Diese Operatoren weisen Werte zu und können eine Kombination aus Rechenoperationen und Zuweisung sein.

| Operator | Beschreibung | Beispiel | Ergebnis |
|----------|-------------|----------|----------|
| `=`      | Zuweisung    | `x = 10` | `x = 10` |
| `+=`     | Addition und Zuweisung | `x += 5` | `x = x + 5` |
| `-=`     | Subtraktion und Zuweisung | `x -= 3` | `x = x - 3` |
| `*=`     | Multiplikation und Zuweisung | `x *= 2` | `x = x * 2` |
| `/=`     | Division und Zuweisung | `x /= 4` | `x = x / 4` |

**Beispiel:**  
```js
let x = 10;
x += 5;  // x = 15
x -= 3;  // x = 12
x *= 2;  // x = 24
x /= 4;  // x = 6
console.log(x);
```

---

## **3. Vergleichsoperatoren**
Vergleichsoperatoren vergleichen zwei Werte und geben ein Boolean-Ergebnis (`true` oder `false`) zurück.

| Operator | Bedeutung | Beispiel | Ergebnis |
|----------|------------|----------|----------|
| `==`     | Gleich (Wert) | `5 == "5"` | `true` |
| `===`    | Strikt gleich (Wert und Typ) | `5 === "5"` | `false` |
| `!=`     | Ungleich | `5 != 3` | `true` |
| `!==`    | Strikt ungleich | `5 !== "5"` | `true` |
| `>`      | Größer als | `5 > 3` | `true` |
| `<`      | Kleiner als | `5 < 3` | `false` |
| `>=`     | Größer oder gleich | `5 >= 5` | `true` |
| `<=`     | Kleiner oder gleich | `3 <= 5` | `true` |

**Beispiel:**  
```js
let a = 5;
let b = "5";

console.log(a == b);  // true
console.log(a === b); // false
console.log(a !== b); // true
console.log(a > 3);   // true
```

---

## **4. Logische Operatoren**
Werden für logische Ausdrücke verwendet.

| Operator | Bedeutung | Beispiel | Ergebnis |
|----------|------------|----------|----------|
| `&&`     | Logisches UND | `true && false` | `false` |
| `||`     | Logisches ODER | `true || false` | `true` |
| `!`      | Logisches NICHT | `!true` | `false` |

**Beispiel:**  
```js
let x = 5;
let y = 10;

console.log(x > 0 && y > 0); // true
console.log(x > 0 || y < 0); // true
console.log(!(x > 0));       // false
```

---

## **5. Nullish Coalescing Operator (`??`)**
Gibt den **ersten definierten Wert** zurück (wenn der linke Wert `null` oder `undefined` ist, wird der rechte verwendet).

**Beispiel:**  
```js
let username = null;
let defaultUsername = "Gast";

let finalUsername = username ?? defaultUsername;
console.log(finalUsername); // "Gast"

let count = 0;
let finalCount = count ?? 10;
console.log(finalCount); // 0 (weil `count` nicht `null` oder `undefined` ist)
```

---

## **6. Optionale Verkettung (`?.`)**
Ermöglicht den **sicheren Zugriff** auf Eigenschaften oder Methoden von `null` oder `undefined`, ohne einen Fehler auszulösen.

**Beispiel:**  
```js
let user = {
  name: "John",
  address: {
    city: "Berlin"
  }
};

console.log(user?.name);         // "John"
console.log(user?.address?.city); // "Berlin"
console.log(user?.age);          // undefined (statt Fehler)
```

---

## **7. Bitweise Operatoren**
Arbeiten direkt auf den Binärwerten von Zahlen.

| Operator | Beschreibung | Beispiel | Ergebnis |
|----------|-------------|----------|----------|
| `&`      | Bitweises UND | `5 & 3`  | `1` |
| `|`      | Bitweises ODER | `5 | 3`  | `7` |
| `^`      | Bitweises XOR | `5 ^ 3`  | `6` |
| `~`      | Bitweises NOT | `~5` | `-6` |
| `<<`     | Linksverschiebung | `5 << 1` | `10` |
| `>>`     | Rechtsverschiebung | `5 >> 1` | `2` |

**Beispiel:**  
```js
let a = 5;  // Binär: 101
let b = 3;  // Binär: 011

console.log(a & b); // 1 (001)
console.log(a | b); // 7 (111)
console.log(a ^ b); // 6 (110)
console.log(~a);    // -6
console.log(a << 1); // 10
console.log(b >> 1); // 1
```

---

## **8. Unterschied zwischen unärem und binärem `+`**
- **Binärer `+`**: Führt Addition oder String-Konkatenation durch.
- **Unärer `+`**: Wandelt einen Wert in eine Zahl um.

**Beispiel:**  
```js
let a = "10";
let b = 5;

console.log(a + b);  // "105" (String-Konkatenation)
console.log(+a + b); // 15 (Addition)

console.log(+"123"); // 123 (String → Zahl)
console.log(+true);  // 1 (Boolean → Zahl)
console.log(+"abc"); // NaN (ungültige Umwandlung)
```

---

### **Zusammenfassung**
- Verwende `===` für verlässliche Vergleiche.
- Nutze `??` für Standardwerte bei `null` oder `undefined`.
- Die **optionale Verkettung (`?.`)** ist hilfreich für den sicheren Zugriff auf Objekte.
- **Unärer `+`** kann nützlich sein, um Strings in Zahlen zu konvertieren.

📖 Weitere Details findest du in den [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators). 🚀

  **[⬆ Наверх](#top)**

7. ### <a name="7"></a> Bedingungen

### **Bedingungen in JavaScript**

In JavaScript gibt es verschiedene Möglichkeiten, Bedingungen zu prüfen und Code auszuführen, wenn bestimmte Kriterien erfüllt sind.  

---

## **1. Truthy- und Falsy-Werte**
Bestimmte Werte werden als **falsch** (`false`) behandelt, wenn sie in einer Bedingung überprüft werden:
- `0`
- `""` (leerer String)
- `null`
- `undefined`
- `NaN`

Alle anderen Werte sind **wahr** (`true`), einschließlich:
- `"0"` (String mit Null)
- `"false"` (String mit "false")
- `[]` (leeres Array)
- `{}` (leeres Objekt)
- `function() {}` (leere Funktion)

**Beispiel:**  
```js
if (0) {
  console.log("Dies wird nicht ausgeführt.");
} else {
  console.log("0 ist ein falsy Wert.");
}
```
---

## **2. `if`-`else`-Bedingungen**
Der `if`-Befehl prüft eine Bedingung und führt den zugehörigen Codeblock aus.

### **Syntax:**
```js
if (Bedingung) {
  // Code wird ausgeführt, wenn die Bedingung true ist
} else if (weitere Bedingung) {
  // Code für eine alternative Bedingung
} else {
  // Code für den Fall, dass keine Bedingung wahr ist
}
```

### **Beispiel:**
```js
let x = 5;

if (x > 0) {
  console.log("Die Zahl ist positiv.");
} else if (x < 0) {
  console.log("Die Zahl ist negativ.");
} else {
  console.log("Die Zahl ist null.");
}
```

---

## **3. Logische Operatoren in Bedingungen**
Logische Operatoren werden verwendet, um mehrere Bedingungen zu kombinieren.

| Operator | Bedeutung | Beispiel |
|----------|------------|-------------|
| `&&`     | UND       | `true && false // false` |
| `||`     | ODER      | `true || false // true` |
| `!`      | NICHT     | `!true // false` |

**Beispiel mit `&&` (UND):**  
```js
let age = 25;
let hasDriverLicense = true;

if (age >= 18 && hasDriverLicense) {
  console.log("Du kannst Auto fahren.");
} else {
  console.log("Du darfst nicht fahren.");
}
```

**Beispiel mit `||` (ODER):**  
```js
let isWeekend = false;
let isHoliday = true;

if (isWeekend || isHoliday) {
  console.log("Du hast frei!");
} else {
  console.log("Arbeitstag!");
}
```

---

## **4. Ternärer Operator (`? :`)**
Der **ternäre Operator** ist eine Kurzform für `if`-`else`.

### **Syntax:**
```js
Bedingung ? Ausdruck_wenn_wahr : Ausdruck_wenn_falsch;
```

### **Beispiel:**
```js
let x = 10;
let isEven = x % 2 === 0 ? "Gerade Zahl" : "Ungerade Zahl";
console.log(isEven); // "Gerade Zahl"
```

---

## **5. `switch`-Bedingungen**
Der `switch`-Operator wird verwendet, wenn ein Wert mit mehreren Möglichkeiten verglichen werden soll.  
🔹 **Vergleich ist strikt (`===`)** – Datentypen müssen übereinstimmen.  
🔹 **`break` nicht vergessen**, um zu verhindern, dass alle weiteren `case`-Blöcke ausgeführt werden.  

### **Syntax:**
```js
switch (Ausdruck) {
  case Wert1:
    // Code wenn Ausdruck === Wert1
    break;
  case Wert2:
    // Code wenn Ausdruck === Wert2
    break;
  default:
    // Code wenn kein Fall zutrifft
}
```

### **Beispiel:**
```js
let day = 2;
let dayName;

switch (day) {
  case 1:
    dayName = "Montag";
    break;
  case 2:
    dayName = "Dienstag";
    break;
  case 3:
    dayName = "Mittwoch";
    break;
  case 4:
    dayName = "Donnerstag";
    break;
  case 5:
    dayName = "Freitag";
    break;
  default:
    dayName = "Wochenende";
}

console.log(dayName); // "Dienstag"
```

### **Mehrere `case`-Werte gruppieren:**
```js
let char = "a";

switch (char) {
  case "a":
  case "e":
  case "i":
  case "o":
  case "u":
    console.log("Vokal");
    break;
  default:
    console.log("Konsonant");
}
```

---

### **Wann `if-else` und wann `switch` verwenden?**
| Situation | Empfohlene Struktur |
|-----------|----------------------|
| Vergleich von Zahlen-/Booleschen Werten | `if-else` |
| Komplexe Bedingungen mit `&&` oder `||` | `if-else` |
| Vergleich einer Variable mit mehreren festen Werten | `switch` |

---

## **Zusammenfassung**
✅ **Falsy-Werte**: `0, "", null, undefined, NaN`  
✅ **`if-else`** für allgemeine Bedingungen  
✅ **Logische Operatoren (`&&`, `||`, `!`)** für kombinierte Bedingungen  
✅ **Ternärer Operator (`? :`)** für kurze Bedingungen  
✅ **`switch`** für mehrere mögliche Werte einer Variablen  

📖 Weitere Infos: [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Statements/if...else) 🚀

  **[⬆ Наверх](#top)**

8. ### <a name="8"></a> Schleifen, verschachtelte Schleifen, Labels

### **Schleifen in JavaScript: `for`, `while`, `do...while`**
Schleifen ermöglichen es, Codeblöcke mehrfach auszuführen, solange eine Bedingung erfüllt ist.

---

## **1. `for`-Schleife**
Die `for`-Schleife ist ideal, wenn die Anzahl der Durchläufe bekannt ist.

### **Syntax:**
```js
for (Start; Bedingung; Inkrement) {
  // Code, der in jeder Iteration ausgeführt wird
}
```

### **Beispiel:**
```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
// Ausgabe: 0, 1, 2, 3, 4
```

---

## **2. `while`-Schleife**
Die `while`-Schleife wird ausgeführt, solange die Bedingung `true` ist.

### **Beispiel:**
```js
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

Falls die Bedingung von Anfang an `false` ist, wird die Schleife **keinmal** ausgeführt.

---

## **3. `do...while`-Schleife**
Diese Schleife wird **mindestens einmal** ausgeführt, da die Bedingung erst nach dem ersten Durchlauf geprüft wird.

### **Beispiel:**
```js
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

---

## **4. Verschachtelte Schleifen (Nested Loops)**
Eine Schleife kann innerhalb einer anderen ausgeführt werden.

### **Beispiel:**
```js
for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
    console.log(`i: ${i}, j: ${j}`);
  }
}
```
👉 Dies wird für `i = 0` dreimal ausgeführt (`j = 0, 1, 2`), dann für `i = 1` usw.

---

## **5. `break` und `continue`**
- **`break`** → Bricht die Schleife ab.
- **`continue`** → Überspringt den aktuellen Durchlauf und fährt mit der nächsten Iteration fort.

### **Beispiel für `break`:**
```js
for (let i = 0; i < 5; i++) {
  if (i === 3) {
    break; // Schleife wird bei i = 3 abgebrochen
  }
  console.log(i);
}
// Ausgabe: 0, 1, 2
```

### **Beispiel für `continue`:**
```js
for (let i = 0; i < 5; i++) {
  if (i === 3) {
    continue; // i = 3 wird übersprungen
  }
  console.log(i);
}
// Ausgabe: 0, 1, 2, 4
```

---

## **6. Labels in Schleifen**
Labels helfen, **verschachtelte Schleifen gezielt zu unterbrechen**.

### **Beispiel:**
```js
outerLoop: for (let i = 0; i < 3; i++) {
  for (let j = 0; j < 3; j++) {
    if (i === 1 && j === 1) {
      break outerLoop; // Beendet die äußere Schleife komplett
    }
    console.log(`i: ${i}, j: ${j}`);
  }
}
```
👉 Hier würde der `break` normalerweise nur die innere Schleife abbrechen. Durch das **Label `outerLoop`** wird jedoch die äußere Schleife gestoppt.

---

### **Zusammenfassung**
✅ **`for`** → Wenn die Anzahl der Durchläufe bekannt ist.  
✅ **`while`** → Solange eine Bedingung wahr ist.  
✅ **`do...while`** → Wird **mindestens einmal** ausgeführt.  
✅ **Verschachtelte Schleifen** für komplexe Strukturen.  
✅ **`break` & `continue`** zur Steuerung des Ablaufs.  
✅ **Labels** ermöglichen gezieltes Unterbrechen von verschachtelten Schleifen.

📖 Mehr Infos: [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Statements/for) 🚀

  **[⬆ Наверх](#top)**

9. ### <a name="9"></a> Hoisting (Hochheben von Variablen und Funktionen)

### **Hoisting in JavaScript (Hochheben von Variablen und Funktionen)**

**Hoisting** ist ein Mechanismus in JavaScript, bei dem **Deklarationen von Variablen und Funktionen** vor der Codeausführung an den Anfang ihres Gültigkeitsbereichs (Scope) **verschoben** werden.

---

## **1. Hoisting von Variablen**
### **1.1 `var` (Hoisting mit `undefined`)**
- Deklaration wird **hochgehoben**, aber die Initialisierung bleibt an der ursprünglichen Stelle.
- Zugriff vor der Initialisierung gibt `undefined` zurück.

```js
console.log(x); // undefined
var x = 10;
console.log(x); // 10
```
🔹 **Warum?** JavaScript behandelt es so:
```js
var x;
console.log(x); // undefined
x = 10;
console.log(x);
```

---

### **1.2 `let` und `const` (Hoisting mit TDZ)**
- `let` und `const` werden ebenfalls hochgehoben, aber sie bleiben in der **Temporal Dead Zone (TDZ)**.
- Zugriff vor der Deklaration führt zu **ReferenceError**.

```js
console.log(y); // ❌ ReferenceError
let y = 20;
console.log(y); // ✅ 20

console.log(z); // ❌ ReferenceError
const z = 30;
console.log(z); // ✅ 30
```
🔹 **Warum?** JavaScript behandelt es so:
```js
// Variablen existieren in der TDZ (keine Nutzung möglich)
let y;
const z;
console.log(y, z); // ReferenceError
y = 20;
z = 30;
```
📌 **Empfehlung:** Nutze `let` oder `const` statt `var`, um unerwartetes Verhalten zu vermeiden.

---

## **2. Hoisting von Funktionen**
### **2.1 `function` (Function Declaration)**
- **Wird vollständig hochgehoben**, d.h. Funktionen können **vor ihrer Definition** aufgerufen werden.

```js
myFunction(); // ✅ "Hello, world!"

function myFunction() {
  console.log("Hello, world!");
}
```
🔹 **JavaScript behandelt es so:**
```js
function myFunction() {
  console.log("Hello, world!");
}
myFunction();
```

---

### **2.2 `function` als `const` oder `let` (Function Expression)**
- Wenn eine Funktion als **Variable (`let` oder `const`) gespeichert wird**, gilt **TDZ**.
- Zugriff vor der Definition führt zu **ReferenceError**.

```js
myFunc(); // ❌ ReferenceError
const myFunc = function () {
  console.log("Hello!");
};
```
📌 **Warum?** `const myFunc` wird hochgehoben, aber bleibt in der **Temporal Dead Zone**.

---

## **3. Hoisting: Zusammenfassung**
| Typ | Wird hochgehoben? | Zugriff vor Deklaration? |
|------|----------------|----------------|
| `var` | ✅ Ja | `undefined` |
| `let` | ✅ Ja (aber in TDZ) | ❌ ReferenceError |
| `const` | ✅ Ja (aber in TDZ) | ❌ ReferenceError |
| Function Declaration | ✅ Ja | ✅ Funktion kann vorher aufgerufen werden |
| Function Expression (`let/const`) | ✅ Ja (aber in TDZ) | ❌ ReferenceError |

---

📖 **Empfohlene Praxis**:
✅ **Immer `let` oder `const` verwenden**  
✅ **Variablen immer am Anfang des Scopes deklarieren**  
✅ **Funktionen bevorzugt mit `function myFunc()` deklarieren, wenn sie vor Nutzung verfügbar sein sollen**  

🔗 **Mehr Infos**: [MDN Web Docs](https://developer.mozilla.org/de/docs/Glossary/Hoisting) 🚀

  **[⬆ Наверх](#top)**

10. ### <a name="10"></a> Ausführungskontext, Lexikalische Umgebung

### **Ausführungskontext und Lexikalische Umgebung in JavaScript**  

JavaScript verwaltet die Ausführung von Code mithilfe von **Ausführungskontexten (Execution Contexts)** und **lexikalischen Umgebungen (Lexical Environments)**. Diese Mechanismen bestimmen, welche Variablen und Funktionen an einer bestimmten Stelle im Code zugänglich sind.

---

## **1. Ausführungskontext (Execution Context)**  
Ein **Ausführungskontext** ist die Umgebung, in der JavaScript-Code ausgeführt wird. Er enthält:
- **Variablen** und **Funktionen**, die im aktuellen Kontext definiert sind.
- Eine **Referenz zur äußeren Umgebung** für den Zugriff auf äußere Variablen.

### **Arten von Ausführungskontexten**  
1. **Globaler Kontext**:  
   - Wird automatisch beim Start des Skripts erstellt.
   - Enthält globale Variablen und Funktionen.
   - Im Browser ist das `window`-Objekt der globale Kontext.

2. **Funktionskontext**:  
   - Wird für jede aufgerufene Funktion erstellt.
   - Jede Funktion hat ihren eigenen lokalen Kontext.

3. **Eval-Kontext** *(selten verwendet)*:  
   - Entsteht beim Ausführen von Code mit `eval()`.

---

## **2. Lexikalische Umgebung (Lexical Environment)**  
Eine **lexikalische Umgebung** speichert **Variablen und Funktionen** im aktuellen Scope und enthält eine **Referenz zum äußeren Scope**.

### **Bestandteile der lexikalischen Umgebung**
1. **Environment Record** (Speicher für Variablen und Funktionen).
2. **Outer Environment Reference** (Referenz zur äußeren Umgebung).

🔹 **Lexikalische Umgebung wird beim Parsen (Code-Analyse) erstellt**, bevor der Code ausgeführt wird.

---

## **3. Beispiel für Ausführungskontext & Lexikalische Umgebung**
```js
function outer() {
  const x = 10; // x gehört zur Lexical Environment von outer()

  function inner() {
    const y = 20; // y gehört zur Lexical Environment von inner()
    console.log(x + y); // Zugriff auf x durch "Outer Environment Reference"
  }

  inner();
}

outer();
```

### **Ablauf des Codes**
1. **Global Execution Context wird erstellt** (`outer` wird definiert).
2. `outer()` wird aufgerufen:
   - Neuer **Funktionskontext für `outer()`** wird erstellt.
   - `x = 10` wird gespeichert.
3. `inner()` wird aufgerufen:
   - Neuer **Funktionskontext für `inner()`** wird erstellt.
   - `y = 20` wird gespeichert.
   - Zugriff auf `x` durch **Outer Environment Reference**.
4. Nach der Ausführung werden die **inneren Kontexte gelöscht**, der **globale Kontext bleibt**.

---

## **4. Call Stack (Ausführungsstapel)**
JavaScript verwaltet mehrere Ausführungskontexte mit einem **Stack (Stapelprinzip: LIFO - Last In, First Out)**.

**Beispiel Call Stack für obigen Code:**
1. **Global Execution Context (wird zuerst geladen)**  
2. `outer()` wird aufgerufen → Neuer **Funktionskontext für `outer()`**  
3. `inner()` wird aufgerufen → Neuer **Funktionskontext für `inner()`**  
4. `inner()` beendet → **Wird aus dem Stack entfernt**  
5. `outer()` beendet → **Wird aus dem Stack entfernt**  
6. Globaler Kontext bleibt.

---

## **5. Temporal Dead Zone (TDZ) und Scope Chain**
- **Variablen mit `let` oder `const` befinden sich vor ihrer Initialisierung in der Temporal Dead Zone (TDZ)**.
- **Scope Chain:** Falls eine Variable nicht im aktuellen Scope gefunden wird, sucht JavaScript in den äußeren Scopes weiter.

**Beispiel für TDZ:**
```js
console.log(a); // ❌ ReferenceError (TDZ)
let a = 5;
```

**Beispiel für Scope Chain:**
```js
const globalVar = "Ich bin global";

function outerFunction() {
  const outerVar = "Ich bin in outer";

  function innerFunction() {
    console.log(globalVar); // Zugriff auf globale Variable
    console.log(outerVar);  // Zugriff auf äußere Funktion
  }

  innerFunction();
}

outerFunction();
```

🔹 **Hier greift `innerFunction` auf `outerVar` zu, weil es im äußeren Scope existiert.**  

---

### **Zusammenfassung**
✅ **Execution Context (Ausführungskontext)** verwaltet Codeausführung.  
✅ **Lexikalische Umgebung (Lexical Environment)** speichert Variablen und Funktionen.  
✅ **Call Stack (Ausführungsstapel)** verwaltet, welche Funktion gerade läuft.  
✅ **Scope Chain** bestimmt, wo JavaScript nach Variablen sucht.  
✅ **TDZ (Temporal Dead Zone)** tritt bei `let` und `const` auf.

📖 Weitere Infos: [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/LexicalEnvironment) 🚀

  **[⬆ Наверх](#top)**

11. ### <a name="11"></a> Temporäre Totzone (Temporal Dead Zone)

### **Temporäre Totzone (Temporal Dead Zone, TDZ) in JavaScript**  

Die **Temporäre Totzone (TDZ)** ist eine Phase, in der eine Variable existiert, aber **noch nicht zugänglich** ist.  

---

## **1. Wann tritt die TDZ auf?**  
### **⚠️ Die TDZ tritt bei `let` und `const` auf, aber nicht bei `var`.**  
```js
console.log(x); // ❌ ReferenceError: x is not defined
let x = 10;
```
Hier existiert `x` technisch bereits im **Scope**, ist aber noch **nicht nutzbar**, bis die Deklaration tatsächlich erreicht wird.

---

## **2. Beispiele für TDZ**
### **2.1 TDZ in `let` und `const`**
```js
{
  console.log(a); // ❌ ReferenceError: a is not defined
  let a = 5;
  console.log(a); // ✅ 5 (ab hier nutzbar)
}
```
**Erklärung:**  
- `a` existiert im Scope des `{}`-Blocks.
- Aber **vor der Deklaration (`let a = 5`) befindet sich `a` in der TDZ**.

---

### **2.2 TDZ in `if`, `for` oder anderen Blöcken**
```js
if (true) {
  console.log(b); // ❌ ReferenceError
  let b = 20;
}
```
**Warum?**  
- `b` wird erst **nach der Deklaration (`let b = 20;`) verwendbar**.

---

### **2.3 TDZ bei Funktionsparametern**
**⚠️ Parameter können auch in der TDZ sein, wenn sie sich auf spätere Parameter beziehen.**  
```js
function myFunction(x = y, y = 2) {
  console.log(x); // ❌ ReferenceError: y is not defined
  console.log(y); // ✅ 2
}
myFunction();
```
**Warum?**  
- `x = y` wird ausgeführt, **bevor** `y` einen Wert erhält → **TDZ für `y`**.

---

## **3. Unterschiede zwischen `var`, `let` und `const`**
| Deklaration | Wird hochgehoben? | Zugriff vor Initialisierung? | Wert in TDZ? |
|------------|----------------|----------------|-------------|
| `var`      | ✅ Ja           | ✅ `undefined` | ❌ Keine TDZ |
| `let`      | ✅ Ja           | ❌ ReferenceError | ✅ TDZ vorhanden |
| `const`    | ✅ Ja           | ❌ ReferenceError | ✅ TDZ vorhanden |

---

## **4. Wie vermeide ich TDZ-Fehler?**
✅ **Immer `let` oder `const` direkt am Anfang eines Scopes deklarieren.**  
✅ **Keinen Code schreiben, der auf eine Variable zugreift, bevor sie definiert ist.**  

**🔹 Falsch:**
```js
console.log(x); // ❌ ReferenceError
let x = 5;
```

**✅ Richtig:**
```js
let x = 5;
console.log(x); // ✅ 5
```

📖 Weitere Infos: [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Statements/let#temporal_dead_zone_tdz) 🚀

  **[⬆ Наверх](#top)**

12. ### <a name="12"></a> typeof – wie erkennt man den Typ eines Werts?

### **`typeof` – Den Typ eines Werts in JavaScript erkennen**  

Der `typeof`-Operator wird in JavaScript verwendet, um den **Datentyp** einer Variablen oder eines Werts als **String** zurückzugeben.

---

## **1. Syntax**  
```js
typeof Wert;
typeof (Wert);
```

📌 **Hinweis:** Klammern sind optional, können aber zur besseren Lesbarkeit genutzt werden.

---

## **2. Rückgabewerte von `typeof`**  
| Datentyp | `typeof` Rückgabe |
|----------|------------------|
| `undefined` | `"undefined"` |
| `null` | `"object"` ❌ (JavaScript-Bug) |
| `boolean` | `"boolean"` |
| `number` | `"number"` |
| `bigint` | `"bigint"` (ab ES11) |
| `string` | `"string"` |
| `symbol` | `"symbol"` |
| `function` | `"function"` |
| `object` | `"object"` (Objekte, Arrays) |

---

## **3. Beispiele**
```js
console.log(typeof 42);         // "number"
console.log(typeof "Hello");    // "string"
console.log(typeof true);       // "boolean"
console.log(typeof undefined);  // "undefined"
console.log(typeof null);       // "object" ❌ (Bug in JavaScript)
console.log(typeof {});         // "object"
console.log(typeof []);         // "object" (Arrays sind Objekte!)
console.log(typeof function(){}); // "function"
console.log(typeof Symbol("id")); // "symbol"
console.log(typeof BigInt(9007199254740991)); // "bigint"
```

---

## **4. Besonderheiten und Fallstricke**
### ❌ **`typeof null` gibt `"object"` zurück**
```js
console.log(typeof null); // "object"
```
📌 **Grund:** Dies ist ein **historischer Bug** in JavaScript. `null` ist **kein** Objekt, sondern ein eigener Datentyp.

**Richtige Prüfung auf `null`:**
```js
let value = null;
console.log(value === null); // ✅ true
```

---

### ❌ **Arrays geben `"object"` zurück**
```js
console.log(typeof [1, 2, 3]); // "object"
```
📌 **Arrays sind eine spezielle Art von Objekten.**  
**Richtige Prüfung:**  
```js
console.log(Array.isArray([1, 2, 3])); // ✅ true
```

---

### **`typeof` bei `functions`**
```js
console.log(typeof function() {}); // "function"
```
📌 **Obwohl Funktionen Objekte sind, gibt `typeof` "function" zurück.**  

---

## **5. Praktische Anwendungsfälle**
### ✅ **Datentyp prüfen, bevor Operationen ausgeführt werden**
```js
function add(a, b) {
  if (typeof a !== "number" || typeof b !== "number") {
    return "Fehler: Beide Werte müssen Zahlen sein!";
  }
  return a + b;
}

console.log(add(5, "10")); // "Fehler: Beide Werte müssen Zahlen sein!"
```

### ✅ **Prüfung auf `null`**
```js
let obj = null;

if (obj === null) {
  console.log("obj ist null");
}
```

### ✅ **Unterschied zwischen `object` und `array` prüfen**
```js
let data = [1, 2, 3];

if (Array.isArray(data)) {
  console.log("data ist ein Array!");
} else {
  console.log("data ist ein Objekt!");
}
```

---

### **6. Zusammenfassung**
✅ `typeof` gibt den Datentyp eines Werts als **String** zurück.  
✅ **Achtung bei `typeof null` → gibt `"object"` zurück (Bug).**  
✅ **Arrays** sind `typeof "object"` → `Array.isArray()` zur Prüfung verwenden.  
✅ **Funktionen** sind `typeof "function"` (aber intern Objekte).  

📖 Weitere Infos: [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/typeof) 🚀

  **[⬆ Наверх](#top)**

13. ### <a name="13"></a> Warum haben primitive Datentypen Methoden? Was ist Autoboxing?

### **Warum haben primitive Datentypen Methoden? Was ist Autoboxing?**  

In JavaScript sind **primitive Datentypen** (`string`, `number`, `boolean`, `symbol`, `bigint`, `null`, `undefined`) **keine Objekte** und haben normalerweise keine Methoden. Dennoch können wir Methoden wie `.toUpperCase()` für Strings oder `.toFixed()` für Zahlen aufrufen.  

📌 **Grund:** **JavaScript nutzt "Autoboxing"**, um primitive Werte in **Objekt-Wrapper** umzuwandeln, wenn Methoden aufgerufen werden.

---

## **1. Was ist Autoboxing?**
📌 **Autoboxing** bedeutet, dass ein primitiver Wert **automatisch in ein entsprechendes Objekt umgewandelt** wird, wenn eine Methode oder Eigenschaft aufgerufen wird.  

| Primitiver Typ | Entsprechendes Wrapper-Objekt |
|---------------|------------------------------|
| `string`      | `String` |
| `number`      | `Number` |
| `boolean`     | `Boolean` |

Nach der **Nutzung des Objekts wird es sofort wieder verworfen**, und die Variable bleibt ein primitiver Wert.

---

## **2. Beispiel für Autoboxing**
```js
const str = "hello";
console.log(str.toUpperCase()); // "HELLO"
```
👉 **Was passiert intern?**
1. JavaScript erstellt **temporär** ein `String`-Objekt:  
   ```js
   new String("hello");
   ```
2. Führt `.toUpperCase()` darauf aus.  
3. Gibt `"HELLO"` zurück und verwirft das Objekt.

---

## **3. Beispiel mit `Number`**
```js
const num = 42;
console.log(num.toFixed(2)); // "42.00"
```
👉 **Intern passiert Folgendes:**
1. `num` ist ein primitiver `number`-Wert.
2. JavaScript wandelt `num` temporär in ein `Number`-Objekt um.
3. Führt `.toFixed(2)` aus.
4. Gibt das Ergebnis zurück und verwirft das `Number`-Objekt.

---

## **4. Was passiert, wenn wir ein echtes Wrapper-Objekt nutzen?**
```js
const strObj = new String("hello");
console.log(typeof strObj); // "object"
console.log(strObj === "hello"); // false (Objekt ≠ primitiver Wert)
```
📌 **Achtung:** Ein `new String("hello")` ist **kein** primitiver `string`, sondern ein Objekt!  
Deshalb sollte man `new String()`, `new Number()` oder `new Boolean()` **nicht verwenden**.

---

## **5. Warum sind primitive Werte unveränderlich?**
```js
const str = "hello";
str[0] = "H"; // ❌ Keine Änderung möglich
console.log(str); // "hello" bleibt unverändert
```
📌 **Warum?** Weil **primitive Werte keine veränderbaren Objekte sind**. Methoden wie `.toUpperCase()` oder `.slice()` **geben eine neue Zeichenkette zurück, anstatt die ursprüngliche zu ändern**.

---

### **Zusammenfassung**
✅ **Autoboxing** ermöglicht Methodenaufrufe auf primitiven Werten.  
✅ **Primitive Werte bleiben unverändert** – Methoden erzeugen neue Werte.  
✅ **Nach der Methode wird das temporäre Objekt sofort verworfen.**  
✅ **Vermeide `new String()`, `new Number()` und `new Boolean()`** – sie erzeugen unnötige Objekte.

📖 Mehr Infos: [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/String) 🚀

  **[⬆ Наверх](#top)**

14. ### <a name="14"></a> Garbage Collector in JavaScript

### **Garbage Collector in JavaScript**  

JavaScript hat einen **automatischen Garbage Collector**, der **nicht mehr verwendete Objekte aus dem Speicher entfernt**. Dies verhindert manuelles Speichermanagement wie in C oder C++.  

---

## **1. Wie funktioniert der Garbage Collector?**  
Der **Garbage Collector** entfernt Objekte aus dem Speicher, die **nicht mehr erreichbar** sind.  
Ein Objekt gilt als **"nicht mehr erreichbar"**, wenn **keine Referenz mehr darauf existiert**.

🔹 **Beispiel für ein erreichbares Objekt:**  
```js
let obj = { name: "Max" }; // "obj" hält eine Referenz auf das Objekt
```
👉 **Dieses Objekt wird NICHT gelöscht**, weil `obj` darauf verweist.

🔹 **Objekt wird unerreichbar und gelöscht:**  
```js
let obj = { name: "Max" };
obj = null; // Keine Referenz mehr → Speicher wird freigegeben
```
👉 **Nach `obj = null;` gibt es keine Referenz mehr → Objekt wird gelöscht.**

---

## **2. Hauptstrategie des Garbage Collectors: Mark-and-Sweep (Markierung & Löschung)**  
Der **häufigste Algorithmus** in modernen JavaScript-Engines ist **"Mark-and-Sweep"**:
1. **Mark (Markieren)**: Der Garbage Collector markiert **alle erreichbaren Objekte**.
2. **Sweep (Löschen)**: Alle **nicht markierten (unerreichbaren) Objekte werden gelöscht**.

📌 **Beispiel für Mark-and-Sweep:**
```js
function createObject() {
  let obj = { value: 42 }; // Erreichbar innerhalb der Funktion
}
createObject(); 
// Nach dem Funktionsaufruf ist "obj" nicht mehr erreichbar → Es wird gelöscht.
```

---

## **3. Memory Leaks (Speicherlecks) vermeiden**
Obwohl der Garbage Collector automatisch arbeitet, können **Speicherlecks** auftreten.

### **Typische Ursachen für Memory Leaks**  
1. **Unnötige globale Variablen**  
   ```js
   var globalVar = {}; // Bleibt für die gesamte Laufzeit erhalten
   ```
   **Lösung:** **Vermeide `var`, nutze `let` oder `const`.**  
   
2. **Vergessene Timer (`setInterval`)**
   ```js
   let interval = setInterval(() => console.log("läuft"), 1000);
   // clearInterval(interval); // Muss gestoppt werden, sonst bleibt es im Speicher!
   ```

3. **DOM-Referenzen behalten**  
   ```js
   let button = document.getElementById("btn");
   button.addEventListener("click", () => console.log("geklickt"));
   // Falls "button" entfernt wird, bleibt die Referenz bestehen und blockiert Speicher.
   ```

   **Lösung:** `removeEventListener()` nutzen:  
   ```js
   button.removeEventListener("click", handler);
   ```

---

## **4. Zusammenfassung**
✅ **Garbage Collector entfernt ungenutzte Objekte automatisch**.  
✅ **"Mark-and-Sweep" ist der wichtigste Algorithmus**.  
✅ **Speicherlecks vermeiden:** `setInterval` stoppen, Event-Listener entfernen, keine unnötigen globalen Variablen.  

📖 **Mehr Infos:** [MDN Web Docs](https://developer.mozilla.org/de/docs/Web/JavaScript/Memory_Management) 🚀

  **[⬆ Наверх](#top)**

15. ### <a name="15"></a> 


  **[⬆ Наверх](#top)**

16. ### <a name="16"></a> 


  **[⬆ Наверх](#top)**

17. ### <a name="17"></a> 


  **[⬆ Наверх](#top)**

18. ### <a name="18"></a> 


  **[⬆ Наверх](#top)**

19. ### <a name="19"></a> 


  **[⬆ Наверх](#top)**

20. ### <a name="20"></a> 


  **[⬆ Наверх](#top)**

21. ### <a name="21"></a> Funktionen, Pfeilfunktionen, IIFE

### **Funktionen, Pfeilfunktionen und IIFE in JavaScript**

JavaScript bietet verschiedene Arten von Funktionen, die sich in **Syntax, `this`-Bindung und Anwendungsfällen** unterscheiden.

---

## **1. Klassische Funktionsdeklaration**
Die **Funktionsdeklaration** ist die traditionelle Methode zur Definition von Funktionen.

```javascript
function addiere(a, b) {
  return a + b;
}

console.log(addiere(3, 5)); // 8
```
✅ **Eigenschaften**:
- Kann **vor der Definition** aufgerufen werden (Hoisting).
- Hat eine eigene `this`-Bindung.

---

## **2. Funktionsausdruck**
Ein **Funktionsausdruck** speichert eine Funktion in einer Variable.

```javascript
const subtrahiere = function (a, b) {
  return a - b;
};

console.log(subtrahiere(10, 4)); // 6
```
✅ **Eigenschaften**:
- Muss **nach der Definition** aufgerufen werden.
- Ist nützlich für **anonyme Funktionen**.

---

## **3. Pfeilfunktionen (`=>`)**
Pfeilfunktionen bieten eine **kürzere Syntax** und übernehmen `this` aus dem umgebenden Kontext.

```javascript
const multipliziere = (a, b) => a * b;

console.log(multipliziere(3, 4)); // 12
```

📌 **Besonderheiten von Pfeilfunktionen**:
- **Kein eigenes `this`** (übernimmt `this` vom äußeren Kontext).
- **Kein `arguments`-Objekt**.
- Kürzere Syntax, **besonders für Callbacks**.

### **Beispiel: `this` in Pfeilfunktionen**
```javascript
const person = {
  name: "Max",
  sagHallo: function() {
    setTimeout(() => {
      console.log(`Hallo, ich bin ${this.name}`);
    }, 1000);
  }
};

person.sagHallo(); // Hallo, ich bin Max (weil `this` von `person` kommt)
```
- **Normale Funktionen** würden `this` verlieren (`undefined` oder `window`).
- **Pfeilfunktionen** behalten `this` vom äußeren Scope.

---

## **4. Immediately Invoked Function Expression (IIFE)**
Ein **IIFE** (Sofort ausgeführter Funktionsausdruck) wird **direkt nach der Definition** ausgeführt.

```javascript
(function() {
  console.log("Ich bin ein IIFE!");
})(); // Ich bin ein IIFE!
```
Oder mit **Pfeilfunktion**:

```javascript
(() => {
  console.log("IIFE mit Pfeilfunktion!");
})(); // IIFE mit Pfeilfunktion!
```

📌 **Anwendungsfälle für IIFE**:
- Um **Variablen vor dem globalen Scope zu schützen**.
- Einmalige Initialisierungen oder Konfigurationen.

---

## **Zusammenfassung**
- **Funktionsdeklarationen** (`function name()`) sind **hoistbar** und haben ein eigenes `this`.
- **Funktionsausdrücke** (`const name = function() {}`) müssen zuerst definiert werden.
- **Pfeilfunktionen** (`const name = () => {}`) haben **kein eigenes `this`** und sind ideal für Callbacks.
- **IIFE (`(function() {})()`)** werden sofort ausgeführt und kapseln Variablen.

🔗 [MDN-Dokumentation zu Funktionen](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Functions)

  **[⬆ Наверх](#top)**

22. ### <a name="22"></a> Methoden zur Kontextbindung (call, apply, bind)

### **Methoden zur Kontextbindung (`call`, `apply`, `bind`) in JavaScript**

In JavaScript kann das `this`-Binding einer Funktion dynamisch verändert werden. Dafür gibt es drei Methoden:  
- `call()`
- `apply()`
- `bind()`

Diese Methoden werden verwendet, um **Funktionen mit einem bestimmten `this`-Wert auszuführen**.

---

## **1. `call()` – Funktion mit explizitem `this`-Wert aufrufen**
Die Methode `call()` ruft eine Funktion mit einem bestimmten `this`-Wert und einzelnen Argumenten auf.

```javascript
function begruessen(land, sprache) {
  console.log(`Hallo, ich bin ${this.name} aus ${land}, und ich spreche ${sprache}.`);
}

const person = { name: "Max" };

begruessen.call(person, "Deutschland", "Deutsch");
// Hallo, ich bin Max aus Deutschland, und ich spreche Deutsch.
```
✅ **Eigenschaften**:
- `this` wird auf `person` gesetzt.
- Die Argumente werden **einzeln übergeben**.

---

## **2. `apply()` – Ähnlich wie `call()`, aber mit Array als Argumente**
Die Methode `apply()` funktioniert wie `call()`, aber Argumente werden als **Array** übergeben.

```javascript
begruessen.apply(person, ["Frankreich", "Französisch"]);
// Hallo, ich bin Max aus Frankreich, und ich spreche Französisch.
```
✅ **Unterschied zu `call()`**:
- Argumente werden **als Array** (`[]`) übergeben, nicht einzeln.

---

## **3. `bind()` – Neue Funktion mit festem `this` erstellen**
Die Methode `bind()` gibt eine **neue Funktion** zurück, in der `this` dauerhaft an ein Objekt gebunden ist.

```javascript
const begruessungMax = begruessen.bind(person);
begruessungMax("Spanien", "Spanisch");
// Hallo, ich bin Max aus Spanien, und ich spreche Spanisch.
```
✅ **Eigenschaften**:
- `this` bleibt dauerhaft auf `person` gebunden.
- Gibt eine **neue Funktion** zurück, die später aufgerufen werden kann.

---

## **4. `bind()` für Methoden in Objekten**
Ein häufiges Problem: **`this`-Verlust in Event-Handlern**.

```javascript
const user = {
  name: "Lisa",
  sagHallo() {
    console.log(`Hallo, ich bin ${this.name}`);
  }
};

const hallo = user.sagHallo;
hallo(); // Fehler: `this` ist `undefined` oder `window`
```
✅ **Lösung: `bind()` verwenden**:
```javascript
const halloGebunden = user.sagHallo.bind(user);
halloGebunden(); // Hallo, ich bin Lisa
```
- `bind()` sorgt dafür, dass `this` auf `user` bleibt.

---

## **5. `bind()` in Event-Handlern**
Beim Event-Handling in DOM-Elementen verliert `this` oft die Verbindung zum Objekt.

```javascript
const button = document.querySelector("button");

const handler = {
  text: "Geklickt!",
  clickHandler() {
    console.log(this.text);
  }
};

// Funktion ohne Bindung (Fehlverhalten)
button.addEventListener("click", handler.clickHandler); // `this` ist nicht `handler`

// Lösung: `bind()`
button.addEventListener("click", handler.clickHandler.bind(handler));
```

---

### **Zusammenfassung**
- **`call(obj, arg1, arg2, ...)`** → Führt die Funktion sofort mit `this = obj` aus (Argumente einzeln).
- **`apply(obj, [arg1, arg2, ...])`** → Wie `call()`, aber Argumente als Array.
- **`bind(obj)`** → Erstellt eine neue Funktion mit festem `this`, die später aufgerufen wird.

🔗 [MDN-Dokumentation zu `call`, `apply` und `bind`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Function/bind)

  **[⬆ Наверх](#top)**

23. ### <a name="23"></a> Closures (Abschlüsse)

### **Closures (Abschlüsse) in JavaScript**  

Ein **Closure** entsteht, wenn eine **innere Funktion** auf die **Variablen einer äußeren Funktion** zugreift, auch nach dem Abschluss der äußeren Funktion. Dadurch bleibt der Zugriff auf **private Daten** erhalten.

---

## **1. Einfaches Beispiel für ein Closure**  
```javascript
function begruessung(name) {
  return function() {
    console.log(`Hallo, ${name}!`);
  };
}

const sagHallo = begruessung("Max");
sagHallo(); // Hallo, Max!
```
✅ **Erklärung**:  
- `begruessung("Max")` gibt eine **innere Funktion** zurück.  
- Diese Funktion merkt sich `name`, selbst nachdem `begruessung` beendet wurde.

---

## **2. Datenkapselung mit Closures**  
Closures können **private Variablen** simulieren:

```javascript
function zaehler() {
  let count = 0; // Private Variable

  return {
    hoch: function() { count++; console.log(count); },
    runter: function() { count--; console.log(count); },
    wert: function() { return count; }
  };
}

const meinZaehler = zaehler();
meinZaehler.hoch(); // 1
meinZaehler.hoch(); // 2
meinZaehler.runter(); // 1
console.log(meinZaehler.wert()); // 1
```
✅ **Vorteile**:
- `count` ist **nicht direkt zugänglich** (private Variable).
- Zugriff nur über die bereitgestellten Methoden.

---

## **3. Closures in `setTimeout` und Event-Handlern**  
```javascript
function verzögerteNachricht(nachricht, delay) {
  setTimeout(function() {
    console.log(nachricht);
  }, delay);
}

verzögerteNachricht("Hallo nach 2 Sekunden!", 2000);
```
- Die innere Funktion speichert `nachricht` und `delay`, bis `setTimeout` sie ausführt.

---

## **4. Closure in einer Schleife (Problem & Lösung)**  
❌ **Problem mit `var` (kein Block-Scope)**  
```javascript
for (var i = 1; i <= 3; i++) {
  setTimeout(function() {
    console.log(i);
  }, i * 1000);
}
// Ausgabe nach 3 Sekunden: 4, 4, 4 (falsche Werte!)
```
✅ **Lösung mit `let` (Block-Scope)**  
```javascript
for (let i = 1; i <= 3; i++) {
  setTimeout(function() {
    console.log(i);
  }, i * 1000);
}
// Ausgabe: 1, 2, 3 (korrekt)
```
✅ **Alternative Lösung mit Closure (`var`)**  
```javascript
for (var i = 1; i <= 3; i++) {
  (function(j) {
    setTimeout(function() {
      console.log(j);
    }, j * 1000);
  })(i);
}
```
- Hier wird `i` als Parameter (`j`) an eine sofort ausgeführte Funktion (`IIFE`) übergeben.

---

### **Zusammenfassung**  
- **Closures** ermöglichen Zugriff auf Variablen einer äußeren Funktion, auch nach deren Ausführung.  
- **Nützlich für**:
  - **Datenkapselung** (private Variablen).
  - **Callbacks und Event-Handler**.
  - **Speicherung von Werten über Zeit** (z. B. `setTimeout`).  
- **Probleme mit `var`** → Verwende `let` oder eine IIFE-Lösung.

🔗 [MDN-Dokumentation zu Closures](https://developer.mozilla.org/de/docs/Web/JavaScript/Closures)

  **[⬆ Наверх](#top)**

24. ### <a name="24"></a> Callback-Funktionen in JavaScript

### **Callback-Funktionen in JavaScript**  

Eine **Callback-Funktion** ist eine Funktion, die als Argument an eine andere Funktion übergeben wird und **zu einem späteren Zeitpunkt** aufgerufen wird. Callbacks sind essenziell für **asynchrone Operationen** (z. B. `setTimeout`, Event-Handling, HTTP-Anfragen).

---

## **1. Einfaches Beispiel für Callbacks**  
```javascript
function begruessen(name, callback) {
  console.log(`Hallo, ${name}!`);
  callback();
}

function verabschieden() {
  console.log("Tschüss!");
}

begruessen("Max", verabschieden);
// Hallo, Max!
// Tschüss!
```
✅ **Erklärung**:
- `verabschieden` wird als **Callback** an `begruessen` übergeben.
- Nach der Begrüßung wird `callback()` ausgeführt.

---

## **2. Callbacks mit `setTimeout` (asynchrones Verhalten)**  
```javascript
function ladeDaten(callback) {
  console.log("Daten werden geladen...");
  setTimeout(() => {
    console.log("Daten erfolgreich geladen.");
    callback();
  }, 2000);
}

function verarbeiteDaten() {
  console.log("Daten werden verarbeitet...");
}

ladeDaten(verarbeiteDaten);
/*
Daten werden geladen...
(Daten werden nach 2 Sekunden geladen)
Daten erfolgreich geladen.
Daten werden verarbeitet...
*/
```
✅ **Erklärung**:
- `ladeDaten()` simuliert eine **asynchrone Operation**.
- Nach 2 Sekunden wird `callback()` (`verarbeiteDaten()`) ausgeführt.

---

## **3. Callbacks in Arrays (z. B. `forEach`, `map`, `filter`)**
```javascript
const zahlen = [1, 2, 3, 4, 5];

zahlen.forEach((zahl) => {
  console.log(zahl * 2);
});
/*
2
4
6
8
10
*/
```
- `forEach()` nimmt eine **Callback-Funktion** als Argument.
- Die Callback-Funktion wird für jedes Element des Arrays ausgeführt.

---

## **4. Callback Hell (verschachtelte Callbacks)**
**Problem**: Wenn Callbacks tief verschachtelt werden, entsteht **"Callback Hell"** (schwer lesbarer Code).

```javascript
function schritt1(callback) {
  setTimeout(() => {
    console.log("Schritt 1 erledigt");
    callback();
  }, 1000);
}

function schritt2(callback) {
  setTimeout(() => {
    console.log("Schritt 2 erledigt");
    callback();
  }, 1000);
}

function schritt3(callback) {
  setTimeout(() => {
    console.log("Schritt 3 erledigt");
    callback();
  }, 1000);
}

schritt1(() => {
  schritt2(() => {
    schritt3(() => {
      console.log("Alle Schritte erledigt!");
    });
  });
});
```
❌ **Problem:** Der Code ist schwer zu lesen und zu warten.

✅ **Lösung:** Verwende **Promises** oder **async/await** statt Callbacks.

---

### **Zusammenfassung**  
- **Callback-Funktionen** werden als Argumente an andere Funktionen übergeben und später ausgeführt.  
- Nützlich für **asynchrone Operationen** (z. B. `setTimeout`, HTTP-Anfragen, Events).  
- **Array-Methoden** wie `forEach`, `map`, `filter` verwenden Callbacks.  
- **Callback Hell** (tiefe Verschachtelung) → Ersetze Callbacks durch **Promises** oder **async/await**.

🔗 [MDN-Dokumentation zu Callbacks](https://developer.mozilla.org/de/docs/Glossary/Callback-Funktion)  

  **[⬆ Наверх](#top)**

25. ### <a name="25"></a> Konstruktor-Funktionen


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
