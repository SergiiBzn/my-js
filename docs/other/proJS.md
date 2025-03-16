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
|41 | [Arrays und Pseudo-Arrays, Array-Destrukturierung](#41) |
|42 | [Methoden Array, Array.prototype](#42) |
|43 | [Kopieren von Arrays](#43) |
|44 | [Map, Set, WeakSet, WeakMap](#44) |
|45 | [Live Collections (lebendige Sammlungen)](#45) |
|46 | [](#46) |
|47 | [](#47) |
|48 | [](#48) |
|49 | [](#49) |
|50 | [](#50) |
|   | Moderne JavaScript-Funktionen |
|51 | [Spread-Operator (ES6-ES9)](#51) |
|52 | [Rest-Operator und Standardparameter (ES6)](#52) |
|53 | [Symbol](#53) |
|54 | [BigInt](#54) |
|55 | [Module import/export (ES6) & CommonJS](#55) |
|56 | [](#56) |
|57 | [](#57) |
|58 | [](#58) |
|59 | [](#59) |
|60 | [](#60) |
|   | Ereignisse und DOM-Manipulation |
|61 | [](#61) |
|62 | [](#62) |
|63 | [](#63) |
|64 | [](#64) |
|65 | [](#65) |
|66 | [](#66) |
|67 | [](#67) |
|68 | [](#68) |
|69 | [](#69) |
|70 | [](#70) |



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

In JavaScript sind **Konstruktor-Funktionen** spezielle Funktionen, die zur Erstellung von Objekten verwendet werden. Sie werden mit dem Schlüsselwort `new` aufgerufen und ermöglichen die Wiederverwendung von Objektstrukturen.

### **Syntax einer Konstruktor-Funktion**
```javascript
function Person(name, alter) {
  this.name = name; // Eigenschaft "name"
  this.alter = alter; // Eigenschaft "alter"

  this.greet = function() {
    console.log(`Hallo, mein Name ist ${this.name} und ich bin ${this.alter} Jahre alt.`);
  };
}

const person1 = new Person("Max", 30);
const person2 = new Person("Anna", 25);

person1.greet(); // Hallo, mein Name ist Max und ich bin 30 Jahre alt.
person2.greet(); // Hallo, mein Name ist Anna und ich bin 25 Jahre alt.
```
- Das Schlüsselwort `this` referenziert das erstellte Objekt.
- `new Person("Max", 30)` erzeugt ein neues Objekt mit den Eigenschaften `name` und `alter`.

### **Prototyp-Methode statt Direktdefinition**
Jede Instanz einer Konstruktor-Funktion erhält eine eigene Kopie der Methoden. Eine effizientere Lösung ist die Verwendung des **Prototyps**, da Methoden dann von allen Instanzen geteilt werden:

```javascript
function Person(name, alter) {
  this.name = name;
  this.alter = alter;
}

// Methode im Prototyp definieren (spart Speicherplatz)
Person.prototype.greet = function() {
  console.log(`Hallo, mein Name ist ${this.name} und ich bin ${this.alter} Jahre alt.`);
};

const person3 = new Person("Lena", 28);
person3.greet(); // Hallo, mein Name ist Lena und ich bin 28 Jahre alt.
```

### **Zusammenfassung**
- Konstruktor-Funktionen werden mit `new` aufgerufen.
- `this` verweist auf die erstellte Instanz.
- Methoden sollten über `prototype` hinzugefügt werden, um Speicher zu sparen.

🔗 [MDN-Dokumentation zu Konstruktor-Funktionen](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/new)

  **[⬆ Наверх](#top)**

26. ### <a name="26"></a> Aufrufkontext (this)

Der **Aufrufkontext (`this`)** in JavaScript bestimmt, auf welches Objekt sich `this` innerhalb einer Funktion oder Methode bezieht. Der Wert von `this` hängt davon ab, wie die Funktion aufgerufen wird.

### **1. Globaler Kontext (`this` in der obersten Ebene)**
Im globalen Kontext verweist `this`:
- Im **Browser** auf das `window`-Objekt.
- In **Node.js** auf `global`.

```javascript
console.log(this); // Im Browser: window, in Node.js: global
```

### **2. `this` in einer Funktion**
Ohne `use strict` verweist `this` in einer normalen Funktion auf das globale Objekt. Mit `"use strict"` ist `this` `undefined`.

```javascript
function test() {
  console.log(this);
}

test(); // Browser: window, Node.js: global (ohne strict)
```

Mit **strict mode**:

```javascript
"use strict";
function testStrict() {
  console.log(this);
}

testStrict(); // undefined
```

### **3. `this` in Objekten (Methoden)**
Wird eine Funktion als Methode eines Objekts aufgerufen, verweist `this` auf das Objekt selbst.

```javascript
const person = {
  name: "Max",
  greet: function() {
    console.log(`Hallo, ich bin ${this.name}`);
  }
};

person.greet(); // Hallo, ich bin Max
```

### **4. `this` in Konstruktor-Funktionen**
Bei Konstruktor-Funktionen verweist `this` auf die neu erstellte Instanz.

```javascript
function Person(name) {
  this.name = name;
}

const max = new Person("Max");
console.log(max.name); // Max
```

### **5. `this` in Arrow-Funktionen**
Arrow-Funktionen übernehmen `this` aus dem umgebenden Lexikalischen Kontext (kein eigenes `this`!).

```javascript
const person = {
  name: "Anna",
  greet: function() {
    const arrowFunction = () => console.log(this.name);
    arrowFunction(); // this bleibt auf `person` bezogen
  }
};

person.greet(); // Anna
```

### **6. Explizite Steuerung von `this` (`call`, `apply`, `bind`)**
Man kann `this` manuell setzen mit `call()`, `apply()` oder `bind()`.

```javascript
function greet() {
  console.log(`Hallo, ich bin ${this.name}`);
}

const user = { name: "Lisa" };

greet.call(user);  // Hallo, ich bin Lisa
greet.apply(user); // Hallo, ich bin Lisa

const boundGreet = greet.bind(user);
boundGreet(); // Hallo, ich bin Lisa
```

### **Zusammenfassung**
- `this` hängt vom **Aufrufkontext** ab.
- In einer **Funktion** (strict mode) ist `this` `undefined`, sonst `window/global`.
- In **Methoden** zeigt `this` auf das aufrufende Objekt.
- In **Konstruktoren** verweist `this` auf die erstellte Instanz.
- **Arrow-Funktionen** haben kein eigenes `this`, sondern übernehmen es aus der Umgebung.
- **`call`, `apply`, `bind`** erlauben das manuelle Setzen von `this`.

🔗 [MDN-Dokumentation zu `this`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/this)

  **[⬆ Наверх](#top)**

27. ### <a name="27"></a> Getter und Setter (Objekteigenschaften)

In JavaScript ermöglichen **Getter** und **Setter** den kontrollierten Zugriff auf Objekteigenschaften. Sie werden mit `get` und `set` innerhalb eines Objekts oder einer Klasse definiert.

---

### **1. Getter (`get`)**
Getter sind Methoden, die eine Eigenschaft abrufen, aber wie normale Eigenschaften verwendet werden.

```javascript
const person = {
  vorname: "Max",
  nachname: "Mustermann",
  
  get vollerName() {
    return `${this.vorname} ${this.nachname}`;
  }
};

console.log(person.vollerName); // Max Mustermann
```
- `vollerName` wird als Eigenschaft aufgerufen (`person.vollerName`), aber intern als Methode definiert.

---

### **2. Setter (`set`)**
Setter ermöglichen das Festlegen von Eigenschaftswerten und können Validierung oder Formatierung enthalten.

```javascript
const user = {
  _alter: 0, // Private Variable (Konvention: Unterstrich)

  get alter() {
    return this._alter;
  },

  set alter(value) {
    if (value < 0) {
      console.log("Alter kann nicht negativ sein!");
    } else {
      this._alter = value;
    }
  }
};

user.alter = 25;
console.log(user.alter); // 25

user.alter = -5; // Alter kann nicht negativ sein!
```
- Der `set`-Methodenaufruf `user.alter = -5` verhindert ungültige Werte.

---

### **3. Getter und Setter in Klassen**
In Klassen können Getter und Setter auf Instanzvariablen zugreifen.

```javascript
class Auto {
  constructor(marke, baujahr) {
    this.marke = marke;
    this._baujahr = baujahr; // Private Variable
  }

  get baujahr() {
    return this._baujahr;
  }

  set baujahr(value) {
    if (value < 1886) {
      console.log("Ungültiges Baujahr!");
    } else {
      this._baujahr = value;
    }
  }
}

const meinAuto = new Auto("Tesla", 2022);
console.log(meinAuto.baujahr); // 2022

meinAuto.baujahr = 1800; // Ungültiges Baujahr!
```

---

### **Zusammenfassung**
- **Getter (`get`)**: Erlauben den kontrollierten Zugriff auf Eigenschaften.
- **Setter (`set`)**: Ermöglichen das Setzen und Validieren von Werten.
- Werden oft für **Datenkapselung** verwendet.
- Können in **Objekten** und **Klassen** definiert werden.

🔗 [MDN-Dokumentation zu Getter und Setter](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Functions/get)

  **[⬆ Наверх](#top)**

28. ### <a name="28"></a> Generatorfunktionen in JavaScript

### **Generatorfunktionen in JavaScript**
Generatorfunktionen (`function*`) ermöglichen das **pausieren und fortsetzen** der Codeausführung mit `yield`. Sie sind besonders nützlich für iterative Prozesse und Lazy Evaluation.

---

### **1. Syntax einer Generatorfunktion**
```javascript
function* meineGeneratorFunktion() {
  yield 1;
  yield 2;
  yield 3;
}

const generator = meineGeneratorFunktion();

console.log(generator.next()); // { value: 1, done: false }
console.log(generator.next()); // { value: 2, done: false }
console.log(generator.next()); // { value: 3, done: false }
console.log(generator.next()); // { value: undefined, done: true }
```
- Das `yield`-Schlüsselwort pausiert die Funktion und gibt einen Wert zurück.
- `next()` setzt die Funktion an der letzten `yield`-Stelle fort.

---

### **2. Generator in einer Schleife**
Man kann Generatoren mit `for...of` durchlaufen:

```javascript
function* zahlenGenerator() {
  yield 10;
  yield 20;
  yield 30;
}

for (const zahl of zahlenGenerator()) {
  console.log(zahl);
}
// 10
// 20
// 30
```

---

### **3. Unendliche Generatoren**
Generatoren können **endlos laufen**, ohne den Speicher zu überlasten:

```javascript
function* unendlicherZähler() {
  let i = 1;
  while (true) {
    yield i++;
  }
}

const counter = unendlicherZähler();
console.log(counter.next().value); // 1
console.log(counter.next().value); // 2
console.log(counter.next().value); // 3
```

---

### **4. `yield` mit Parametern**
Man kann `next(value)` verwenden, um Werte an den Generator zurückzugeben:

```javascript
function* bidirektionalerGenerator() {
  const wert1 = yield "Erster Wert?";
  const wert2 = yield `Zweiter Wert ist ${wert1}`;
  return `Dritter Wert ist ${wert2}`;
}

const gen = bidirektionalerGenerator();
console.log(gen.next().value);      // "Erster Wert?"
console.log(gen.next(42).value);    // "Zweiter Wert ist 42"
console.log(gen.next(100).value);   // "Dritter Wert ist 100"
```

---

### **5. `yield*` für geschachtelte Generatoren**
Mit `yield*` kann man einen anderen Generator aufrufen:

```javascript
function* unterGenerator() {
  yield "A";
  yield "B";
}

function* hauptGenerator() {
  yield* unterGenerator();
  yield "C";
}

for (const wert of hauptGenerator()) {
  console.log(wert);
}
// A
// B
// C
```

---

### **Zusammenfassung**
- Generatorfunktionen (`function*`) erlauben das **pausieren und fortsetzen** der Codeausführung.
- `yield` gibt einen Wert zurück, `next()` setzt die Funktion fort.
- Generatoren eignen sich für **Lazy Evaluation, unendliche Sequenzen** und **asynchrone Verarbeitung**.
- `yield*` ermöglicht das Delegieren an andere Generatoren.

🔗 [MDN-Dokumentation zu Generatorfunktionen](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Statements/function*)

  **[⬆ Наверх](#top)**

29. ### <a name="29"></a> Rekursion in JavaScript

### **Rekursion in JavaScript**
Rekursion bedeutet, dass eine Funktion sich **selbst aufruft**, bis eine **Abbruchbedingung** erreicht ist. Sie wird oft für Probleme mit **natürlicher Teilung** verwendet, z. B. Baumstrukturen oder mathematische Berechnungen.

---

### **1. Einfaches Beispiel: Countdown**
```javascript
function countdown(n) {
  if (n <= 0) {
    console.log("Fertig!");
    return;
  }
  console.log(n);
  countdown(n - 1); // Rekursiver Aufruf
}

countdown(5);
/*
5
4
3
2
1
Fertig!
*/
```
- Die Funktion ruft sich mit `n - 1` selbst auf.
- Sobald `n <= 0`, stoppt die Rekursion (**Abbruchbedingung**).

---

### **2. Fakultät berechnen (n!)**
Die **Fakultät** eines Zahl `n` ist `n * (n-1) * (n-2) * ... * 1`.

```javascript
function fakultaet(n) {
  if (n === 0) return 1; // Abbruchbedingung
  return n * fakultaet(n - 1); // Rekursiver Aufruf
}

console.log(fakultaet(5)); // 120 (5*4*3*2*1)
```
- Ohne Abbruchbedingung würde die Funktion **unendlich laufen**.

---

### **3. Fibonacci-Folge**
Die **Fibonacci-Zahlen** sind definiert als:
- `fib(0) = 0`, `fib(1) = 1`
- `fib(n) = fib(n-1) + fib(n-2)`

```javascript
function fibonacci(n) {
  if (n <= 1) return n; // Basisfälle
  return fibonacci(n - 1) + fibonacci(n - 2);
}

console.log(fibonacci(6)); // 8 (0,1,1,2,3,5,8)
```
❌ **Problem:** Rekursion kann ineffizient sein, da viele Werte mehrfach berechnet werden.

✅ **Lösung:** **Memoization** zur Optimierung:

```javascript
function fibonacciMemo(n, memo = {}) {
  if (n in memo) return memo[n];
  if (n <= 1) return n;
  
  memo[n] = fibonacciMemo(n - 1, memo) + fibonacciMemo(n - 2, memo);
  return memo[n];
}

console.log(fibonacciMemo(50)); // Sehr schnelle Berechnung
```

---

### **4. Rekursion für verschachtelte Strukturen (Baum-Durchlauf)**
Rekursion ist ideal für **hierarchische Daten**, wie verschachtelte Objekte oder Bäume.

```javascript
const baum = {
  wert: 1,
  kinder: [
    { wert: 2, kinder: [{ wert: 4 }, { wert: 5 }] },
    { wert: 3, kinder: [{ wert: 6 }] }
  ]
};

function durchlaufeBaum(knoten) {
  console.log(knoten.wert);
  if (knoten.kinder) {
    knoten.kinder.forEach(durchlaufeBaum);
  }
}

durchlaufeBaum(baum);
/*
1
2
4
5
3
6
*/
```
- Die Funktion ruft sich **für jedes Kind** des Knotens auf.

---

### **5. Tail Call Optimization (TCO)**
Moderne JavaScript-Engines optimieren **Tail-Recursive-Funktionen** (wenn der letzte Ausdruck ein rekursiver Aufruf ist), um **Stack-Überläufe zu vermeiden**.

```javascript
function summe(n, akk = 0) {
  if (n === 0) return akk;
  return summe(n - 1, akk + n); // Tail Call (optimierbar)
}

console.log(summe(10000)); // Kein Stack Overflow in TCO-fähigen Umgebungen
```

---

### **Zusammenfassung**
- **Rekursion** bedeutet, dass eine Funktion sich **selbst aufruft**.
- **Wichtig:** Immer eine **Abbruchbedingung** (`if`) definieren, um Endlosschleifen zu vermeiden.
- **Memoization** kann ineffiziente Rekursion optimieren.
- **Ideal für:** Mathematische Probleme, hierarchische Strukturen (Bäume), Algorithmen wie Tiefensuche.
- **Tail Call Optimization (TCO)** reduziert Speicherverbrauch, aber nicht in allen JavaScript-Engines unterstützt.

🔗 [MDN-Dokumentation zu Rekursion](https://developer.mozilla.org/de/docs/Glossary/Rekursion)

  **[⬆ Наверх](#top)**

30. ### <a name="30"></a> 


  **[⬆ Наверх](#top)**

31. ### <a name="31"></a> Objekte, Destrukturierung von Objekten (ES6)

### **Objekte & Destrukturierung von Objekten (ES6) in JavaScript**  

---

## **1. Objekte in JavaScript**  
Ein **Objekt** ist eine Sammlung von **Schlüssel-Wert-Paaren**.

```javascript
const person = {
  name: "Max",
  alter: 30,
  beruf: "Entwickler"
};

console.log(person.name);  // Max
console.log(person["alter"]); // 30
```
✅ **Eigenschaften von Objekten**:  
- Werte können **beliebige Datentypen** sein (Strings, Arrays, andere Objekte).
- Zugriff über **Punkt-Notation (`.`)** oder **Array-Notation (`[]`)**.

---

## **2. ES6-Destrukturierung von Objekten**  
Mit **Destrukturierung** kann man **Eigenschaften direkt extrahieren**.

```javascript
const person = { name: "Anna", alter: 25, beruf: "Designer" };

const { name, alter } = person;

console.log(name); // Anna
console.log(alter); // 25
```
✅ **Vorteile**:  
- Spart **Schreibarbeit** (`person.name` → `name`).
- Einfachere **Funktionseingaben**.

---

## **3. Destrukturierung mit Standardwerten**
Falls eine Eigenschaft **nicht existiert**, kann ein **Standardwert** gesetzt werden.

```javascript
const user = { name: "Lisa" };

const { name, alter = 18 } = user;

console.log(alter); // 18 (Standardwert)
```

---

## **4. Umbenennung von Variablen bei der Destrukturierung**
Man kann Eigenschaftsnamen **umbenennen**.

```javascript
const auto = { marke: "Tesla", baujahr: 2023 };

const { marke: hersteller, baujahr } = auto;

console.log(hersteller); // Tesla
```

---

## **5. Destrukturierung in Funktionen**  
```javascript
function zeigeInfo({ name, alter }) {
  console.log(`${name} ist ${alter} Jahre alt.`);
}

const person = { name: "Tom", alter: 40 };
zeigeInfo(person); // Tom ist 40 Jahre alt.
```
✅ **Vorteile**:  
- Die Funktion erhält direkt die **relevanten Werte**.

---

## **6. Verschachtelte Objekte destrukturieren**
```javascript
const student = {
  name: "Sophia",
  adresse: {
    stadt: "Berlin",
    land: "Deutschland"
  }
};

const { adresse: { stadt, land } } = student;

console.log(stadt); // Berlin
console.log(land); // Deutschland
```
✅ **Hierbei wird `adresse` nicht als Variable erstellt!**  
Falls nötig, kann man `adresse` zusätzlich speichern:
```javascript
const { adresse, adresse: { stadt } } = student;
console.log(adresse); // { stadt: "Berlin", land: "Deutschland" }
```

---

### **Zusammenfassung**
- **Objekte** sind Sammlungen von Schlüssel-Wert-Paaren.
- **Destrukturierung** vereinfacht den Zugriff auf Eigenschaften.
- **Standardwerte** können gesetzt werden.
- **Eigenschaftsnamen können umbenannt werden**.
- **Verschachtelte Objekte** lassen sich destrukturieren.
- **Nützlich in Funktionen**, um nur relevante Daten zu extrahieren.

🔗 [MDN-Dokumentation zur Destrukturierung](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/Destrukturierende_Zuweisung)

  **[⬆ Наверх](#top)**

32. ### <a name="32"></a> Methoden Object, Object.prototype

### **Methoden von `Object` & `Object.prototype` in JavaScript**

In JavaScript gibt es zwei Kategorien von Methoden für Objekte:

1. **`Object`-Methoden** → Statische Methoden von `Object`
2. **`Object.prototype`-Methoden** → Methoden, die jedes Objekt erbt

---

## **1. `Object`-Methoden (statische Methoden)**
Diese Methoden werden direkt auf `Object` aufgerufen.

### **1.1 `Object.keys(obj)` – Alle Schlüssel eines Objekts**
```javascript
const person = { name: "Anna", alter: 28, beruf: "Designer" };

console.log(Object.keys(person)); // ["name", "alter", "beruf"]
```

### **1.2 `Object.values(obj)` – Alle Werte eines Objekts**
```javascript
console.log(Object.values(person)); // ["Anna", 28, "Designer"]
```

### **1.3 `Object.entries(obj)` – Schlüssel-Wert-Paare als Array**
```javascript
console.log(Object.entries(person));
// [["name", "Anna"], ["alter", 28], ["beruf", "Designer"]]
```

### **1.4 `Object.assign(target, source)` – Objekte zusammenführen**
```javascript
const obj1 = { a: 1 };
const obj2 = { b: 2 };
const merged = Object.assign({}, obj1, obj2);

console.log(merged); // { a: 1, b: 2 }
```

### **1.5 `Object.freeze(obj)` – Objekt unveränderlich machen**
```javascript
const buch = { titel: "JavaScript", preis: 30 };
Object.freeze(buch);

buch.preis = 40; // Fehler (im strikten Modus)
console.log(buch.preis); // 30 (unverändert)
```

### **1.6 `Object.seal(obj)` – Keine neuen Eigenschaften, aber Änderung erlaubt**
```javascript
const auto = { marke: "Tesla", farbe: "Rot" };
Object.seal(auto);

auto.farbe = "Blau"; // OK
auto.modell = "Model S"; // ❌ Fehler (Eigenschaft kann nicht hinzugefügt werden)
console.log(auto); // { marke: "Tesla", farbe: "Blau" }
```

### **1.7 `Object.create(proto)` – Neues Objekt mit bestimmtem Prototyp**
```javascript
const tier = { typ: "Säugetier" };
const hund = Object.create(tier);

console.log(hund.typ); // "Säugetier" (geerbt von `tier`)
```

---

## **2. `Object.prototype`-Methoden**
Diese Methoden sind für **alle Objekte verfügbar**, weil sie von `Object.prototype` erben.

### **2.1 `obj.hasOwnProperty(prop)` – Prüft, ob eine Eigenschaft direkt existiert**
```javascript
const person = { name: "Max" };

console.log(person.hasOwnProperty("name")); // true
console.log(person.hasOwnProperty("alter")); // false
```
🔹 **Warum wichtig?**  
Verhindert, dass geerbte Eigenschaften (`prototype`) fälschlicherweise als eigene Eigenschaften interpretiert werden.

---

### **2.2 `obj.toString()` – Objekt in String umwandeln**
```javascript
const zahl = 123;
console.log(zahl.toString()); // "123"

const array = [1, 2, 3];
console.log(array.toString()); // "1,2,3"
```

---

### **2.3 `obj.valueOf()` – Gibt den Primärwert eines Objekts zurück**
```javascript
const num = new Number(42);
console.log(num.valueOf()); // 42
```

---

### **2.4 `obj.isPrototypeOf(obj2)` – Prüft, ob ein Objekt Prototyp eines anderen ist**
```javascript
function Tier() {}
const hund = new Tier();

console.log(Tier.prototype.isPrototypeOf(hund)); // true
```

---

### **Zusammenfassung**
- **`Object.keys()`**, **`Object.values()`**, **`Object.entries()`** → Arbeiten mit Eigenschaften.
- **`Object.assign()`**, **`Object.create()`**, **`Object.freeze()`**, **`Object.seal()`** → Objektverwaltung.
- **`hasOwnProperty()`** → Prüft, ob eine Eigenschaft direkt im Objekt existiert.
- **`toString()`**, **`valueOf()`** → Umwandlung von Objekten in Strings oder primitive Werte.

🔗 [MDN-Dokumentation zu `Object`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object)

  **[⬆ Наверх](#top)**

33. ### <a name="33"></a> Möglichkeiten zur Objekterstellung

### **Möglichkeiten zur Objekterstellung in JavaScript**  

In JavaScript gibt es mehrere Möglichkeiten, ein Objekt zu erstellen. Jede Methode hat ihre eigenen **Anwendungsfälle und Vorteile**.

---

## **1. Objekt-Literal (`{}`)**
Die einfachste Methode, um ein Objekt zu erstellen.

```javascript
const person = {
  name: "Max",
  alter: 30,
  beruf: "Entwickler"
};

console.log(person.name); // Max
```
✅ **Vorteile**:  
- Schnell und einfach für kleine Objekte  
- Kein `new` oder Prototyp erforderlich  

---

## **2. `Object.create(prototype)`**
Erstellt ein neues Objekt mit einem bestimmten **Prototyp**.

```javascript
const tier = {
  typ: "Säugetier"
};

const hund = Object.create(tier);
hund.name = "Bello";

console.log(hund.typ); // "Säugetier" (geerbt von `tier`)
console.log(hund.hasOwnProperty("typ")); // false (kommt aus dem Prototyp)
```
✅ **Vorteile**:  
- Erlaubt direkte Kontrolle über den **Prototyp**  
- Gut für **Prototypen-Vererbung**  

---

## **3. `new Object()` (Konstruktor von `Object`)**
Alternative zu `{}`.

```javascript
const person = new Object();
person.name = "Anna";
person.alter = 25;

console.log(person.name); // Anna
```
❌ **Weniger gebräuchlich**, da `{}` kürzer und verständlicher ist.

---

## **4. Konstruktorfunktion**
Verwendet eine Funktion, um **mehrere Objekte mit ähnlicher Struktur** zu erstellen.

```javascript
function Person(name, alter) {
  this.name = name;
  this.alter = alter;
}

const person1 = new Person("Lisa", 28);
const person2 = new Person("Tom", 35);

console.log(person1.name); // Lisa
console.log(person2.alter); // 35
```
✅ **Vorteile**:  
- Ermöglicht das Erstellen **mehrerer Instanzen**  
- `this` verweist auf das erstellte Objekt  
❌ **Nachteile**:  
- Methoden werden bei jeder Instanz neu erstellt (besser `prototype` verwenden).  

---

## **5. Konstruktorfunktion mit `prototype` (Speichereffizienter)**
```javascript
function Auto(marke) {
  this.marke = marke;
}

Auto.prototype.fahren = function() {
  console.log(`${this.marke} fährt.`);
};

const meinAuto = new Auto("Tesla");
meinAuto.fahren(); // Tesla fährt.
```
✅ **Speichert Methoden im Prototyp, nicht bei jeder Instanz**.

---

## **6. ES6 Klassen (`class`)**
Klassen sind eine modernere Alternative zu Konstruktorfunktionen.

```javascript
class Fahrzeug {
  constructor(marke) {
    this.marke = marke;
  }

  fahren() {
    console.log(`${this.marke} fährt.`);
  }
}

const auto = new Fahrzeug("BMW");
auto.fahren(); // BMW fährt.
```
✅ **Vorteile**:  
- Klarere Syntax  
- Bessere Lesbarkeit für objektorientierte Programmierung  

---

## **7. Fabrikfunktion (Factory Function)**
Eine **Funktion, die Objekte zurückgibt**, ohne `new`.

```javascript
function erstellePerson(name, alter) {
  return {
    name,
    alter,
    sagHallo() {
      console.log(`Hallo, ich bin ${this.name}.`);
    }
  };
}

const person = erstellePerson("Markus", 40);
person.sagHallo(); // Hallo, ich bin Markus.
```
✅ **Vorteile**:  
- Kein `new` erforderlich  
- Gut für **geschlossene (private) Variablen**  

---

## **8. JSON (`JSON.parse()` & `JSON.stringify()`)**
### **Objekt aus JSON-String erstellen**
```javascript
const jsonString = '{"name": "Elena", "alter": 22}';
const person = JSON.parse(jsonString);

console.log(person.name); // Elena
```

### **Objekt in JSON umwandeln**
```javascript
const jsonDaten = JSON.stringify(person);
console.log(jsonDaten); // {"name":"Elena","alter":22}
```
✅ **Wichtig für:**  
- **Datenübertragung (APIs)**  
- **Speicherung in `localStorage`**  

---

### **Zusammenfassung**
| Methode | Vorteile | Nachteile |
|---------|---------|-----------|
| **`{}` (Objekt-Literal)** | Einfach, direkt | Nicht für viele Instanzen |
| **`Object.create(proto)`** | Direktes Prototyp-Handling | Komplexe Vererbung |
| **`new Object()`** | Alternative zu `{}` | Länger als `{}` |
| **Konstruktorfunktion (`new`)** | Strukturierte Erstellung | Methoden ineffizient ohne `prototype` |
| **Konstruktorfunktion mit `prototype`** | Speicheroptimiert | Weniger intuitiv als `class` |
| **`class` (ES6)** | Klarer, modernes OOP | Komplexer als einfache Objekte |
| **Fabrikfunktion (`Factory Function`)** | Kein `new`, einfach zu lesen | Kein direkter Prototypzugriff |
| **JSON (`JSON.parse()`)** | API-kompatibel | Kein Verhalten (Methoden) |

🔗 [MDN-Dokumentation zu Objekten](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object)

  **[⬆ Наверх](#top)**  

34. ### <a name="34"></a> Kopieren von Objekten

### **Kopieren von Objekten in JavaScript**  

Beim Kopieren von Objekten in JavaScript gibt es zwei Arten:  

1. **Shallow Copy (flache Kopie)** – Kopiert nur die erste Ebene der Eigenschaften (tiefer liegende Objekte bleiben referenziert).  
2. **Deep Copy (tiefe Kopie)** – Erstellt eine vollständige Kopie, auch von verschachtelten Objekten.  

---

## **1. Shallow Copy (Flache Kopie)**  

Flache Kopien duplizieren nur die **oberste Ebene** des Objekts. Falls das Objekt **verschachtelte Objekte** enthält, bleiben diese referenziert (Änderungen im Original wirken sich auf die Kopie aus).  

### **1.1 `Object.assign(target, source)`**
```javascript
const original = { a: 1, b: { c: 2 } };
const kopie = Object.assign({}, original);

kopie.a = 42;
kopie.b.c = 99; // Achtung: Referenzierte Objekte werden nicht kopiert!

console.log(original.b.c); // 99 (auch geändert!)
```

✅ **Schnelle flache Kopie**  
❌ **Nicht für verschachtelte Objekte geeignet**

---

### **1.2 Spread-Operator (`{ ...obj }`)**
```javascript
const original = { a: 1, b: { c: 2 } };
const kopie = { ...original };

kopie.a = 42;
kopie.b.c = 99; // Wieder nur eine Referenz!

console.log(original.b.c); // 99 (Original ebenfalls verändert!)
```
✅ **Einfacher als `Object.assign()`**  
❌ **Nur erste Ebene wird kopiert**

---

## **2. Deep Copy (Tiefe Kopie)**  

### **2.1 `JSON.parse(JSON.stringify(obj))` (einfache Lösung)**
```javascript
const original = { a: 1, b: { c: 2 } };
const kopie = JSON.parse(JSON.stringify(original));

kopie.b.c = 99;

console.log(original.b.c); // 2 (Original bleibt unverändert)
```
✅ **Einfache Methode für tiefe Kopien**  
❌ **Verliert Funktionen, `undefined`, Symbole**  

---

### **2.2 Rekursive Funktion für tiefe Kopie**
```javascript
function deepCopy(obj) {
  if (obj === null || typeof obj !== "object") return obj;

  const kopie = Array.isArray(obj) ? [] : {};

  for (let key in obj) {
    if (obj.hasOwnProperty(key)) {
      kopie[key] = deepCopy(obj[key]);
    }
  }
  return kopie;
}

const original = { a: 1, b: { c: 2 } };
const kopie = deepCopy(original);

kopie.b.c = 99;

console.log(original.b.c); // 2 (Original bleibt unverändert)
```
✅ **Kopiert auch Funktionen, Arrays, `undefined`**  
❌ **Aufwendiger als `JSON.parse()`**

---

### **2.3 `structuredClone(obj)` (Moderne Lösung)**
```javascript
const original = { a: 1, b: { c: 2 }, d: new Date() };
const kopie = structuredClone(original);

kopie.b.c = 99;

console.log(original.b.c); // 2 (Original bleibt unverändert)
console.log(kopie.d instanceof Date); // true (Kopiert auch `Date`!)
```
✅ **Unterstützt `Date`, Arrays, `Map`, `Set`**  
✅ **Schnell & sicher**  
❌ **Nicht in älteren Browsern verfügbar**  

---

### **Zusammenfassung**
| Methode | Typ | Vorteile | Nachteile |
|---------|-----|----------|------------|
| **`Object.assign({}, obj)`** | Flach | Schnell & einfach | Tiefe Objekte bleiben referenziert |
| **`{ ...obj }` (Spread)** | Flach | Kürzere Syntax | Keine tiefe Kopie |
| **`JSON.parse(JSON.stringify(obj))`** | Tief | Einfach & schnell | Verliert Methoden & `undefined` |
| **Rekursive Funktion** | Tief | Behandelt alle Datentypen | Komplexer |
| **`structuredClone(obj)`** | Tief | Beste moderne Lösung | Nicht überall unterstützt |

🔗 [MDN-Dokumentation zu `structuredClone()`](https://developer.mozilla.org/de/docs/Web/API/structuredClone)

  **[⬆ Наверх](#top)**

35. ### <a name="35"></a> Property Descriptors (Eigenschaftsbeschreibungen)

### **Property Descriptors (Eigenschaftsbeschreibungen) in JavaScript**  

Jede Eigenschaft eines Objekts hat **Eigenschaftsbeschreibungen** (**Property Descriptors**), die bestimmen, wie die Eigenschaft funktioniert. Diese können mit `Object.getOwnPropertyDescriptor()` und `Object.defineProperty()` verwaltet werden.

---

## **1. Property Descriptor auslesen**
Mit `Object.getOwnPropertyDescriptor(obj, prop)` kann man die Eigenschaften einer Eigenschaft abrufen.

```javascript
const person = { name: "Max" };

console.log(Object.getOwnPropertyDescriptor(person, "name"));
/*
{
  value: 'Max',
  writable: true,
  enumerable: true,
  configurable: true
}
*/
```

✅ **Standardwerte für eine Eigenschaft**:  
- `writable: true` → Wert kann geändert werden  
- `enumerable: true` → Eigenschaft wird in Schleifen (`for...in`, `Object.keys()`) angezeigt  
- `configurable: true` → Eigenschaft kann gelöscht oder verändert werden  

---

## **2. Eigenschaften mit `Object.defineProperty()` setzen**  
Mit `Object.defineProperty(obj, prop, descriptor)` kann man Eigenschaften **kontrollierter definieren**.

### **2.1 `writable: false` – Schreibschutz aktivieren**
```javascript
const auto = {};
Object.defineProperty(auto, "marke", {
  value: "Tesla",
  writable: false
});

auto.marke = "BMW"; // ❌ Keine Änderung möglich!
console.log(auto.marke); // "Tesla"
```

---

### **2.2 `enumerable: false` – Eigenschaft verstecken**
```javascript
const benutzer = { name: "Anna", passwort: "geheim" };

Object.defineProperty(benutzer, "passwort", {
  enumerable: false
});

console.log(Object.keys(benutzer)); // ["name"] (passwort wird nicht angezeigt)
```
✅ **Gut für sensible Daten!**

---

### **2.3 `configurable: false` – Eigenschaft gegen Änderungen sperren**
```javascript
const buch = { titel: "JavaScript Guide" };

Object.defineProperty(buch, "titel", {
  configurable: false
});

// Löschen schlägt fehl:
delete buch.titel; 
console.log(buch.titel); // "JavaScript Guide"

// `configurable: false` verhindert Neudefinition:
Object.defineProperty(buch, "titel", { writable: true }); // ❌ Fehler!
```
✅ **Schützt eine Eigenschaft vor Modifikationen oder Löschung**

---

## **3. Getter & Setter mit `defineProperty()`**
Man kann auch Getter und Setter definieren.

```javascript
const konto = {
  _saldo: 1000
};

Object.defineProperty(konto, "saldo", {
  get() {
    return `${this._saldo} EUR`;
  },
  set(value) {
    if (value < 0) {
      console.log("Saldo kann nicht negativ sein!");
    } else {
      this._saldo = value;
    }
  }
});

console.log(konto.saldo); // "1000 EUR"
konto.saldo = 500; 
console.log(konto.saldo); // "500 EUR"
konto.saldo = -200; // ❌ "Saldo kann nicht negativ sein!"
```
✅ **Steuert den Zugriff auf eine Eigenschaft durch Regeln**

---

### **Zusammenfassung**
| Eigenschaft | Bedeutung |
|------------|-----------|
| `value` | Der Wert der Eigenschaft |
| `writable` | Kann der Wert geändert werden? (`true` / `false`) |
| `enumerable` | Wird die Eigenschaft in `Object.keys()` und Schleifen (`for...in`) angezeigt? |
| `configurable` | Kann die Eigenschaft gelöscht oder verändert werden? |
| `get()` | Gibt einen Wert zurück (Getter) |
| `set(value)` | Setzt einen Wert mit Logik (Setter) |

🔗 [MDN-Dokumentation zu Property Descriptors](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty)

  **[⬆ Наверх](#top)**

36. ### <a name="36"></a> Private und geschützte Eigenschaften von Objekten

### **Private und geschützte Eigenschaften von Objekten in JavaScript**  

JavaScript bietet verschiedene Möglichkeiten, **private** oder **geschützte Eigenschaften** zu definieren, um Daten **vor direktem Zugriff zu schützen**.

---

## **1. Konvention: `_` für "geschützte" Eigenschaften**  
Es gibt **keine echte Privateigenschaft** in normalen Objekten, aber Konventionen helfen:

```javascript
class Nutzer {
  constructor(name) {
    this.name = name;
    this._passwort = "geheim"; // Geschützt (Konvention: `_`)
  }

  zeigePasswort() {
    return this._passwort;
  }
}

const user = new Nutzer("Anna");
console.log(user._passwort); // ❌ Sollte nicht direkt genutzt werden
console.log(user.zeigePasswort()); // ✅ "geheim"
```
✅ **Nützlich, aber nicht wirklich privat!**  
❌ **Jeder kann `_passwort` trotzdem lesen und ändern!**

---

## **2. Private Eigenschaften mit `#` (ES2020+)**
Seit ES2020 können **private Eigenschaften** mit `#` definiert werden. Sie sind **außerhalb der Klasse nicht zugänglich**.

```javascript
class Konto {
  #saldo = 1000; // Private Variable mit `#`

  getSaldo() {
    return this.#saldo;
  }

  einzahlen(betrag) {
    if (betrag > 0) this.#saldo += betrag;
  }
}

const meinKonto = new Konto();
console.log(meinKonto.getSaldo()); // ✅ 1000
meinKonto.einzahlen(500);
console.log(meinKonto.getSaldo()); // ✅ 1500

console.log(meinKonto.#saldo); // ❌ Fehler: Private Eigenschaft nicht zugänglich!
```
✅ **Echte Privateigenschaften** (nicht von außen sichtbar)  
❌ **Nicht kompatibel mit älteren JavaScript-Versionen**

---

## **3. Private Eigenschaften mit Closures (ältere Alternative)**
Vor ES2020 wurden Closures genutzt, um Eigenschaften **privat zu halten**:

```javascript
function erstelleKonto() {
  let saldo = 1000; // Private Variable

  return {
    getSaldo: () => saldo,
    einzahlen: (betrag) => { if (betrag > 0) saldo += betrag; }
  };
}

const konto = erstelleKonto();
console.log(konto.getSaldo()); // ✅ 1000
konto.einzahlen(500);
console.log(konto.getSaldo()); // ✅ 1500

console.log(konto.saldo); // ❌ `saldo` ist nicht zugänglich!
```
✅ **Private Daten sind geschützt**  
❌ **Nicht so intuitiv wie `class` mit `#`**

---

## **4. `WeakMap` für private Eigenschaften**
Eine andere Technik ist die Nutzung von `WeakMap`, um private Eigenschaften außerhalb des Objekts zu speichern.

```javascript
const privateDaten = new WeakMap();

class Benutzer {
  constructor(name) {
    privateDaten.set(this, { passwort: "geheim" });
    this.name = name;
  }

  getPasswort() {
    return privateDaten.get(this).passwort;
  }
}

const benutzer = new Benutzer("Tom");
console.log(benutzer.getPasswort()); // ✅ "geheim"

console.log(benutzer.passwort); // ❌ `undefined`
```
✅ **Sicherer als `_`-Konvention, aber komplexer**  
✅ **Privat, da `WeakMap`-Werte nicht direkt zugänglich sind**  
❌ **Mehr Overhead als `#`-Privateigenschaften**

---

### **Zusammenfassung**
| Methode | Privat? | Einfachheit | Kompatibilität |
|---------|---------|------------|---------------|
| `_geschützt` (Konvention) | ❌ Nein | ✅ Einfach | ✅ Überall |
| `#privat` (ES2020+) | ✅ Ja | ✅ Einfach | ❌ Nicht in älteren Browsern |
| **Closure (Funktion + `let`)** | ✅ Ja | ❌ Umständlich | ✅ Überall |
| `WeakMap` | ✅ Ja | ❌ Komplexer | ✅ Überall |

🔗 [MDN-Dokumentation zu privaten Feldern (`#`)](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Classes/Private_class_fields)

  **[⬆ Наверх](#top)**

37. ### <a name="37"></a> Prototypen, Prototypen-Kette

### **Prototypen und Prototypen-Kette in JavaScript**  

In JavaScript basiert die **Objektvererbung** auf **Prototypen**. Jedes Objekt hat eine **interne Verbindung zu einem Prototypen**, von dem es Eigenschaften und Methoden erben kann.

---

## **1. Prototyp eines Objekts**
Jedes JavaScript-Objekt hat eine versteckte Verbindung (`[[Prototype]]`) zu einem Prototyp-Objekt, das mit `Object.getPrototypeOf(obj)` oder `__proto__` sichtbar gemacht werden kann.

```javascript
const person = { name: "Max" };

console.log(Object.getPrototypeOf(person)); 
console.log(person.__proto__ === Object.prototype); // true
```
✅ **`Object.prototype` ist der Standard-Prototyp für Objekte.**  
✅ **`Object.getPrototypeOf(obj)` ist sicherer als `obj.__proto__`**  

---

## **2. Prototypen-Kette (Prototype Chain)**
Wenn eine Eigenschaft nicht im Objekt selbst gefunden wird, sucht JavaScript sie **im Prototypen**.

```javascript
const tier = {
  atmen() {
    console.log("Das Tier atmet.");
  }
};

const hund = Object.create(tier); // `hund` erbt von `tier`
hund.bellen = function() {
  console.log("Wuff!");
};

hund.bellen(); // "Wuff!"
hund.atmen(); // "Das Tier atmet." (geerbt von `tier`)
console.log(Object.getPrototypeOf(hund) === tier); // true
```
✅ **Eigenschaften werden über die Prototypen-Kette vererbt.**  
✅ **Wenn eine Eigenschaft fehlt, wird im nächsten Prototyp gesucht.**  

---

## **3. Eigene Prototypen mit Konstruktorfunktionen**
Jede Funktion hat eine `prototype`-Eigenschaft, die für die Vererbung genutzt wird.

```javascript
function Person(name) {
  this.name = name;
}

Person.prototype.greet = function() {
  console.log(`Hallo, ich bin ${this.name}.`);
};

const max = new Person("Max");
max.greet(); // "Hallo, ich bin Max."
console.log(max.__proto__ === Person.prototype); // true
```
✅ **Methoden werden nur einmal im Prototyp gespeichert, nicht in jeder Instanz.**  
❌ **Ohne `new` wird `this` nicht richtig gesetzt.**  

---

## **4. Prototyp-Kette mit Klassen (`class`)**
ES6 **Klassen (`class`)** sind eine modernere Syntax für Prototypen.

```javascript
class Tier {
  atmen() {
    console.log("Das Tier atmet.");
  }
}

class Hund extends Tier {
  bellen() {
    console.log("Wuff!");
  }
}

const bello = new Hund();
bello.bellen(); // "Wuff!"
bello.atmen(); // "Das Tier atmet." (geerbt von `Tier`)
```
✅ **Klarere Syntax für Vererbung.**  
✅ **Nutzen intern Prototypen (`extends`).**  

---

## **5. `Object.create(prototype)` für Prototypen**
```javascript
const katze = Object.create(tier);
katze.miauen = function() {
  console.log("Miau!");
};

katze.atmen(); // "Das Tier atmet." (geerbt)
```
✅ **Flexibel, kein `new` nötig.**  
❌ **Kein `instanceof`-Support.**  

---

### **Zusammenfassung**
| Methode | Beschreibung | Vorteile | Nachteile |
|---------|-------------|----------|-----------|
| `Object.create(proto)` | Erstellt ein Objekt mit bestimmtem Prototyp | Einfach, flexibel | Kein `instanceof` |
| **Konstruktorfunktion + `prototype`** | Klassische Methode zur Vererbung | Speicheroptimiert | Braucht `new` |
| **ES6 `class` + `extends`** | Modernere Syntax für Vererbung | Lesbar, `super()`-Support | Nur syntaktischer Zucker |
| **Prototyp-Kette** | Automatische Suche in `[[Prototype]]` | Ermöglicht Vererbung | Kann unübersichtlich werden |

🔗 [MDN-Dokumentation zu Prototypen](https://developer.mozilla.org/de/docs/Learn/JavaScript/Objects/Prototypes)

  **[⬆ Наверх](#top)**

38. ### <a name="38"></a> Object.create()

### **`Object.create()` in JavaScript**  

Die Methode `Object.create(proto)` erstellt ein neues Objekt mit einem bestimmten **Prototypen**. Dadurch kann man einfach Objekte **vererben**, ohne Konstruktorfunktionen oder Klassen zu verwenden.

---

## **1. Einfaches Beispiel: Objekt mit Prototyp**
```javascript
const tier = {
  atmen() {
    console.log("Das Tier atmet.");
  }
};

const hund = Object.create(tier);
hund.bellen = function() {
  console.log("Wuff!");
};

hund.atmen(); // "Das Tier atmet." (geerbt von `tier`)
hund.bellen(); // "Wuff!"
console.log(Object.getPrototypeOf(hund) === tier); // true
```
✅ **`hund` erbt die Methode `atmen()` von `tier`.**  
✅ **Prototype Chain wird genutzt.**  

---

## **2. `Object.create(proto, properties)` mit Eigenschaften**
Man kann Eigenschaften direkt definieren.

```javascript
const person = {
  beschreibung() {
    return `${this.name} ist ${this.alter} Jahre alt.`;
  }
};

const max = Object.create(person, {
  name: { value: "Max", writable: true, enumerable: true },
  alter: { value: 30, writable: true, enumerable: true }
});

console.log(max.beschreibung()); // "Max ist 30 Jahre alt."
console.log(Object.keys(max)); // ["name", "alter"] (enumerable: true)
```
✅ **Man kann `writable`, `enumerable`, `configurable` setzen.**  

---

## **3. `Object.create(null)` – Objekt ohne Prototyp**
Erstellt ein **komplett leeres Objekt** (kein `Object.prototype`).

```javascript
const obj = Object.create(null);
obj.name = "Test";

console.log(obj.name); // "Test"
console.log(obj.toString); // ❌ `undefined` (kein `Object.prototype`)
```
✅ **Gut für "reine" Key-Value-Maps (z. B. für Dictionary-Speicherung).**  
❌ **Keine Standardmethoden (`toString`, `hasOwnProperty`).**  

---

## **4. Vererbung mit `Object.create()`**
```javascript
const fahrzeug = {
  start() {
    console.log(`${this.marke} startet.`);
  }
};

const auto = Object.create(fahrzeug);
auto.marke = "Tesla";

auto.start(); // "Tesla startet."
```
✅ **Einfachere Alternative zu `class` oder Konstruktorfunktionen.**  

---

### **Zusammenfassung**
| Methode | Beschreibung | Vorteile | Nachteile |
|---------|-------------|----------|-----------|
| `Object.create(proto)` | Erstellt Objekt mit Prototyp `proto` | Speicheroptimiert, flexibel | Kein direkter `instanceof`-Support |
| `Object.create(proto, props)` | Erstellt Objekt + Eigenschaftsdefinition | Kontrolle über Eigenschaften | Komplexer |
| `Object.create(null)` | Objekt ohne Prototyp (`Object.prototype` fehlt) | Kein Overhead | Keine Standardmethoden |

🔗 [MDN-Dokumentation zu `Object.create()`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Object/create)

  **[⬆ Наверх](#top)**

39. ### <a name="39"></a> Unterschied zwischen klassischer und prototypischer Vererbung

### **Unterschied zwischen klassischer und prototypischer Vererbung in JavaScript**  

JavaScript nutzt **prototypische Vererbung**, während viele andere Sprachen wie Java oder C++ **klassische Vererbung** (klassenbasiert) verwenden. Ab **ES6** gibt es jedoch die `class`-Syntax, die auf Prototypen basiert, aber klassisches Verhalten nachahmt.

---

## **1. Klassische Vererbung (Klassenbasiert – ES6 `class`)**
In klassischer Vererbung erstellt man **eine Klasse**, die als Blaupause für Objekte dient. Subklassen können von einer Superklasse erben.

```javascript
class Tier {
  constructor(name) {
    this.name = name;
  }

  laufen() {
    console.log(`${this.name} läuft.`);
  }
}

class Hund extends Tier {
  bellen() {
    console.log(`${this.name} bellt: Wuff!`);
  }
}

const rex = new Hund("Rex");
rex.laufen(); // "Rex läuft."
rex.bellen(); // "Rex bellt: Wuff!"
```
✅ **Vorteile:**  
- Klare Struktur, leicht verständlich  
- `super()` ermöglicht Zugriff auf die Superklasse  
- Bessere Lesbarkeit für Entwickler mit OOP-Erfahrung  

❌ **Nachteile:**  
- Statischer als Prototypen  
- Weniger flexibel für dynamische Objekte  

---

## **2. Prototypische Vererbung (`Object.create()` oder `prototype`)**
Hier gibt es **keine Klassen**. Objekte erben direkt von anderen Objekten über die **Prototype Chain**.

```javascript
const tier = {
  laufen() {
    console.log("Das Tier läuft.");
  }
};

const hund = Object.create(tier);
hund.bellen = function() {
  console.log("Wuff!");
};

hund.laufen(); // "Das Tier läuft." (geerbt von `tier`)
hund.bellen(); // "Wuff!"
```
✅ **Vorteile:**  
- Mehr **Flexibilität** (dynamische Objekte, keine feste Klassendefinition)  
- **Direkte Vererbung von Objekten**  
- Speicherfreundlich (Methoden im Prototyp gespeichert)  

❌ **Nachteile:**  
- Weniger intuitiv für Entwickler mit OOP-Hintergrund  
- Keine direkte `instanceof`-Überprüfung  

---

## **3. Vergleich: Klassisch vs. Prototypisch**

| Merkmal | Klassische Vererbung (`class`) | Prototypische Vererbung (`Object.create()` / `prototype`) |
|---------|---------------------------------|---------------------------------|
| **Basis** | Klassen mit Konstruktoren | Objekte erben direkt von anderen Objekten |
| **Syntax** | `class` und `extends` | `Object.create()` oder `prototype` |
| **Methodenspeicher** | Im `prototype` der Klasse | Direkt im Prototyp-Objekt |
| **Flexibilität** | Statisch, festgelegte Struktur | Dynamisch, Objekte können geändert werden |
| **Performance** | Optimiert für OOP | Speicherfreundlich, da Prototypen gemeinsam genutzt werden |

---

### **Zusammenfassung**
- **`class` (ES6)** → Klassische Syntax, aber basiert intern auf **Prototypen**.
- **`Object.create(proto)` oder `prototype`** → Direktes Erben von Objekten, flexibler.
- **Prototypische Vererbung ist dynamischer**, klassisches OOP ist strukturierter.

🔗 [MDN-Dokumentation zu Vererbung](https://developer.mozilla.org/de/docs/Learn/JavaScript/Objects/Inheritance)

  **[⬆ Наверх](#top)**

40. ### <a name="40"></a> 


  **[⬆ Наверх](#top)**  

41. ### <a name="41"></a> Arrays und Pseudo-Arrays, Array-Destrukturierung

### **Arrays und Pseudo-Arrays, Array-Destrukturierung in JavaScript**  

---

## **1. Arrays in JavaScript**
Ein **Array** ist eine geordnete Liste von Werten, die mit Index (`0`-basiert) zugänglich sind.

```javascript
const zahlen = [10, 20, 30];
console.log(zahlen[0]); // 10
console.log(zahlen.length); // 3
```
✅ **Arrays sind dynamisch und können verschiedene Datentypen speichern.**  

---

## **2. Pseudo-Arrays (Array-ähnliche Objekte)**
Pseudo-Arrays haben **Längen- und Indexeigenschaften**, aber **nicht alle Array-Methoden**.

### **2.1 `arguments`-Objekt (funktionales Pseudo-Array)**
```javascript
function summe() {
  console.log(arguments); // Pseudo-Array
  return Array.from(arguments).reduce((acc, val) => acc + val, 0);
}

console.log(summe(1, 2, 3)); // 6
```
✅ `Array.from(arguments)` konvertiert ein Pseudo-Array in ein echtes Array.  

---

### **2.2 `NodeList` und `HTMLCollection` (DOM-Pseudo-Arrays)**
```javascript
const alleDivs = document.querySelectorAll("div");
console.log(alleDivs instanceof NodeList); // true

const echteArray = Array.from(alleDivs);
console.log(echteArray.map(div => div.innerText)); // Array-Methoden nutzbar
```
✅ **`NodeList` ist kein echtes Array → `Array.from()` oder Spread-Operator nutzen.**  

---

## **3. Array-Destrukturierung (ES6)**  
Mit **Destrukturierung** können Werte direkt aus einem Array extrahiert werden.

### **3.1 Grundlegende Destrukturierung**
```javascript
const zahlen = [10, 20, 30];
const [erstes, zweites] = zahlen;

console.log(erstes); // 10
console.log(zweites); // 20
```
✅ **Verkürzt den Code bei Wertzuweisungen.**  

---

### **3.2 Überspringen von Werten**
```javascript
const zahlen = [10, 20, 30, 40];
const [, , drittes] = zahlen;

console.log(drittes); // 30
```
✅ **Lässt bestimmte Elemente aus.**  

---

### **3.3 Destrukturierung mit Rest-Operator (`...`)**
```javascript
const [erstes, ...rest] = [1, 2, 3, 4, 5];

console.log(erstes); // 1
console.log(rest); // [2, 3, 4, 5]
```
✅ **Ideal für Variablen mit dynamischer Länge.**  

---

### **3.4 Werte tauschen mit Destrukturierung**
```javascript
let a = 5, b = 10;
[a, b] = [b, a];

console.log(a, b); // 10, 5
```
✅ **Kein temporärer Zwischenspeicher nötig.**  

---

### **3.5 Destrukturierung in Funktionsparametern**
```javascript
function zeigePerson([name, alter]) {
  console.log(`${name} ist ${alter} Jahre alt.`);
}

const daten = ["Lisa", 30];
zeigePerson(daten); // Lisa ist 30 Jahre alt.
```
✅ **Perfekt für Funktionen mit Array-Parametern.**  

---

### **Zusammenfassung**
| Thema | Beschreibung |
|-------|-------------|
| **Array** | Geordnete Liste von Werten (`[1, 2, 3]`) |
| **Pseudo-Arrays** | `arguments`, `NodeList` – Kein echtes Array |
| **Destrukturierung** | Extrahiert Werte aus Arrays |
| **Rest-Operator (`...`)** | Speichert den Rest der Werte |
| **Tauschen mit Destrukturierung** | `[a, b] = [b, a]` |

🔗 [MDN-Dokumentation zur Array-Destrukturierung](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Operators/Destrukturierende_Zuweisung#arrays)

  **[⬆ Наверх](#top)**

42. ### <a name="42"></a> Methoden Array, Array.prototype

### **Methoden für Arrays und `Array.prototype` in JavaScript**  

JavaScript-Arrays besitzen viele Methoden, die das Arbeiten mit Daten erleichtern. Sie sind in zwei Kategorien unterteilt:

1. **Statische Methoden** (`Array.method()`)
2. **Instanzmethoden** (`Array.prototype.method()` – für einzelne Arrays)

---

## **1. Statische Methoden (`Array.method()`)**
Diese Methoden werden direkt auf `Array` angewendet.

### **1.1 `Array.from(iterable)` – Pseudo-Array zu echtem Array konvertieren**
```javascript
const pseudoArray = document.querySelectorAll("div"); // NodeList (kein echtes Array)
const echtesArray = Array.from(pseudoArray);

console.log(echtesArray instanceof Array); // true
```
✅ **Konvertiert `NodeList`, `arguments`, `Set` in Arrays**  

---

### **1.2 `Array.isArray(value)` – Prüft, ob ein Wert ein echtes Array ist**
```javascript
console.log(Array.isArray([1, 2, 3])); // true
console.log(Array.isArray({ 0: "a", length: 1 })); // false
```
✅ **Sicherer als `instanceof Array`, weil auch für `iframes` funktioniert.**  

---

### **1.3 `Array.of(...values)` – Erstellt ein Array aus Argumenten**
```javascript
console.log(Array.of(1, 2, 3)); // [1, 2, 3]
console.log(Array(3)); // [empty × 3] (Sonderverhalten!)
```
✅ **Verhindert `Array(3)`-Problem (leeres Array mit Länge 3).**  

---

## **2. Instanzmethoden (`Array.prototype.method()`)**
Diese Methoden werden auf einzelne Arrays angewendet.

---

### **2.1 Mutierende Methoden (verändern das Array)**
#### **`push()` – Element(e) ans Ende hinzufügen**
```javascript
const zahlen = [1, 2];
zahlen.push(3, 4);
console.log(zahlen); // [1, 2, 3, 4]
```

#### **`pop()` – Letztes Element entfernen**
```javascript
const namen = ["Max", "Anna"];
namen.pop();
console.log(namen); // ["Max"]
```

#### **`shift()` – Erstes Element entfernen**
```javascript
const queue = ["Erster", "Zweiter"];
queue.shift();
console.log(queue); // ["Zweiter"]
```

#### **`unshift()` – Element(e) am Anfang hinzufügen**
```javascript
const liste = ["B"];
liste.unshift("A");
console.log(liste); // ["A", "B"]
```

#### **`splice(start, deleteCount, ...items)` – Elemente entfernen/hinzufügen**
```javascript
const farben = ["Rot", "Grün", "Blau"];
farben.splice(1, 1, "Gelb"); // 1 Element ab Index 1 ersetzen
console.log(farben); // ["Rot", "Gelb", "Blau"]
```
✅ **Vielseitig: Entfernen, Einfügen und Ersetzen von Elementen.**  

---

### **2.2 Nicht-mutierende Methoden (erstellt neue Arrays)**
#### **`slice(start, end)` – Teilausschnitt eines Arrays**
```javascript
const zahlen = [1, 2, 3, 4];
console.log(zahlen.slice(1, 3)); // [2, 3] (Index 1 bis 2)
```

#### **`concat(arr)` – Arrays verbinden**
```javascript
const a = [1, 2], b = [3, 4];
console.log(a.concat(b)); // [1, 2, 3, 4]
```

#### **`join(separator)` – Array zu String**
```javascript
const worte = ["Hallo", "Welt"];
console.log(worte.join(" ")); // "Hallo Welt"
```

---

### **2.3 Iterationsmethoden**
#### **`forEach(callback)` – Jedes Element durchlaufen**
```javascript
const zahlen = [1, 2, 3];
zahlen.forEach((zahl) => console.log(zahl * 2));
// 2
// 4
// 6
```
✅ **Ersetzt `for`-Schleife für Arrays.**  

---

### **2.4 Methoden für neue Arrays**
#### **`map(callback)` – Jedes Element transformieren**
```javascript
const zahlen = [1, 2, 3];
const verdoppelt = zahlen.map((zahl) => zahl * 2);
console.log(verdoppelt); // [2, 4, 6]
```
✅ **Ändert Werte ohne Original-Array zu modifizieren.**  

---

#### **`filter(callback)` – Elemente basierend auf Bedingung filtern**
```javascript
const zahlen = [10, 20, 30, 40];
const gefiltert = zahlen.filter((zahl) => zahl > 20);
console.log(gefiltert); // [30, 40]
```
✅ **Perfekt für Datenverarbeitung.**  

---

#### **`reduce(callback, startwert)` – Werte reduzieren (z. B. Summe)**
```javascript
const zahlen = [1, 2, 3, 4];
const summe = zahlen.reduce((acc, zahl) => acc + zahl, 0);
console.log(summe); // 10
```
✅ **Wird oft für Summen, Durchschnittswerte und Objektverarbeitung genutzt.**  

---

### **2.5 Suchen und Prüfen**
#### **`find(callback)` – Erstes passendes Element**
```javascript
const leute = [{ name: "Max", alter: 30 }, { name: "Anna", alter: 25 }];
const ergebnis = leute.find(person => person.alter > 28);
console.log(ergebnis); // { name: "Max", alter: 30 }
```

#### **`findIndex(callback)` – Index des ersten passenden Elements**
```javascript
const zahlen = [10, 20, 30];
console.log(zahlen.findIndex(n => n === 20)); // 1
```

#### **`some(callback)` – Prüft, ob mind. ein Element passt**
```javascript
const zahlen = [3, 7, 11];
console.log(zahlen.some(n => n > 5)); // true
```

#### **`every(callback)` – Prüft, ob ALLE Elemente passen**
```javascript
console.log(zahlen.every(n => n > 2)); // true
console.log(zahlen.every(n => n > 5)); // false
```

---

### **2.6 Sortieren**
#### **`sort([compareFunction])` – Sortiert das Array**
```javascript
const zahlen = [10, 2, 30, 4];
zahlen.sort((a, b) => a - b);
console.log(zahlen); // [2, 4, 10, 30]
```
❌ **Standard `sort()` sortiert alphabetisch – Immer `compareFunction` nutzen!**  

---

### **Zusammenfassung**
| Methode | Typ | Funktion |
|---------|-----|----------|
| `push()`, `pop()`, `shift()`, `unshift()` | Mutierend | Elemente hinzufügen/entfernen |
| `slice()`, `concat()`, `join()` | Nicht-mutierend | Neues Array/Strings erstellen |
| `map()`, `filter()`, `reduce()` | Iterativ | Transformation & Aggregation |
| `find()`, `some()`, `every()` | Suchmethoden | Elemente finden & prüfen |
| `sort()`, `reverse()` | Sortieren | Reihenfolge ändern |

🔗 [MDN-Dokumentation zu Arrays](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Array)

  **[⬆ Наверх](#top)**

43. ### <a name="43"></a> Kopieren von Arrays

### **Kopieren von Arrays in JavaScript**  

Beim Kopieren von Arrays gibt es zwei Methoden:  

1. **Shallow Copy (flache Kopie)** – Erstellt eine Kopie der obersten Ebene, verschachtelte Objekte/Arrays bleiben referenziert.  
2. **Deep Copy (tiefe Kopie)** – Erstellt eine komplette Kopie inklusive aller verschachtelten Werte.

---

## **1. Flache Kopie (Shallow Copy)**
Eine **flache Kopie** dupliziert nur die oberste Ebene des Arrays. **Verschachtelte Objekte bleiben referenziert**.

### **1.1 Spread-Operator (`[...]`)**
```javascript
const original = [1, 2, [3, 4]];
const kopie = [...original];

kopie[0] = 99;
kopie[2][0] = 999; // ⚠️ Änderung in verschachteltem Array!

console.log(original); // [1, 2, [999, 4]] (Änderung übernommen!)
console.log(kopie); // [99, 2, [999, 4]]
```
✅ **Kürzeste Methode**  
❌ **Tief verschachtelte Werte bleiben referenziert!**  

---

### **1.2 `Array.slice()` – Erstellt eine neue Kopie**
```javascript
const original = [1, 2, 3];
const kopie = original.slice();

kopie[0] = 99;

console.log(original); // [1, 2, 3] (unverändert)
console.log(kopie); // [99, 2, 3]
```
✅ **Gut für flache Arrays**  
❌ **Verschachtelte Werte bleiben referenziert**  

---

### **1.3 `Array.from()` – Erstellt eine Kopie**
```javascript
const original = [1, 2, { a: 3 }];
const kopie = Array.from(original);

kopie[2].a = 99; // ⚠️ Referenzierte Objekte werden nicht kopiert!

console.log(original); // [1, 2, { a: 99 }]
console.log(kopie); // [1, 2, { a: 99 }]
```
✅ **Nützlich für `arguments` oder `NodeList`**  
❌ **Verschachtelte Objekte bleiben referenziert**  

---

## **2. Tiefe Kopie (Deep Copy)**
Eine **tiefe Kopie** dupliziert **das gesamte Array und alle verschachtelten Werte**, sodass keine Referenz bestehen bleibt.

### **2.1 `JSON.parse(JSON.stringify(array))` (Einfache Lösung)**
```javascript
const original = [1, 2, { a: 3 }];
const kopie = JSON.parse(JSON.stringify(original));

kopie[2].a = 99;

console.log(original); // [1, 2, { a: 3 }] (unverändert)
console.log(kopie); // [1, 2, { a: 99 }]
```
✅ **Einfache Methode für tiefe Kopien**  
❌ **Verliert Methoden, `undefined`, `Symbol`, `Date`**  

---

### **2.2 `structuredClone(array)` (Moderne Lösung)**
```javascript
const original = [1, 2, { a: 3 }, new Date()];
const kopie = structuredClone(original);

kopie[2].a = 99;

console.log(original); // [1, 2, { a: 3 }, Date]
console.log(kopie); // [1, 2, { a: 99 }, Date]
```
✅ **Erhält `Date`, `Map`, `Set`**  
❌ **Nicht in älteren Browsern unterstützt**  

---

### **2.3 Rekursive Deep Copy-Funktion**
Falls `structuredClone()` nicht verfügbar ist, kann man eine **eigene Funktion** schreiben.

```javascript
function deepCopy(arr) {
  return arr.map(item => 
    Array.isArray(item) ? deepCopy(item) : 
    typeof item === "object" && item !== null ? {...item} : item
  );
}

const original = [1, 2, { a: 3 }, [4, 5]];
const kopie = deepCopy(original);

kopie[2].a = 99;
kopie[3][0] = 999;

console.log(original); // [1, 2, { a: 3 }, [4, 5]]
console.log(kopie); // [1, 2, { a: 99 }, [999, 5]]
```
✅ **Flexible und funktionale Lösung**  
❌ **Verliert Methoden und komplexe Objekte (`Date`, `Map`, `Set`)**  

---

### **Zusammenfassung**
| Methode | Typ | Vorteile | Nachteile |
|---------|-----|----------|-----------|
| **`slice()` / `[...arr]`** | Flach | Schnell, einfach | Tiefe Werte bleiben referenziert |
| **`JSON.parse(JSON.stringify(arr))`** | Tief | Einfach, gut für Objekte | Verliert `undefined`, Methoden, `Date` |
| **`structuredClone(arr)`** | Tief | Beste moderne Lösung | Nicht in älteren Browsern |
| **Rekursive Funktion (`deepCopy()`)** | Tief | Anpassbar | Kein `Date`, `Map`, `Set` |

🔗 [MDN-Dokumentation zu `structuredClone()`](https://developer.mozilla.org/de/docs/Web/API/structuredClone)

  **[⬆ Наверх](#top)**

44. ### <a name="44"></a> Map, Set, WeakSet, WeakMap

### **`Map`, `Set`, `WeakMap`, `WeakSet` in JavaScript**  

JavaScript bietet **`Map`** und **`Set`** als moderne Alternativen zu **Objekten (`{}`) und Arrays (`[]`)**, sowie **`WeakMap`** und **`WeakSet`** für schwache Referenzen.

---

## **1. `Map` – Schlüssel-Wert-Speicher mit beliebigen Schlüsseltypen**  

Ein **`Map`** ist eine geordnete Sammlung von **Schlüssel-Wert-Paaren**, bei der **beliebige Werte** als Schlüssel verwendet werden können (z. B. Objekte oder Funktionen).  

### **1.1 Erstellen & Befüllen einer Map**
```javascript
const benutzerMap = new Map();
benutzerMap.set("name", "Max");
benutzerMap.set(42, "Alter");
benutzerMap.set({ id: 1 }, "Objekt als Schlüssel");

console.log(benutzerMap.get("name")); // Max
console.log(benutzerMap.get(42)); // Alter
```
✅ **Beliebige Schlüssel möglich (Objekte, Zahlen, Strings, Funktionen)**  
✅ **Erhält Reihenfolge der Einträge**  

---

### **1.2 Methoden von `Map`**
```javascript
console.log(benutzerMap.has(42)); // true
benutzerMap.delete(42);
console.log(benutzerMap.size); // 2
benutzerMap.clear(); // Löscht alle Einträge
```

---

### **1.3 `forEach()`, `keys()`, `values()`, `entries()`**
```javascript
const map = new Map([
  ["name", "Anna"],
  ["stadt", "Berlin"]
]);

// Iteration
map.forEach((wert, schlüssel) => console.log(`${schlüssel}: ${wert}`));

console.log([...map.keys()]); // ["name", "stadt"]
console.log([...map.values()]); // ["Anna", "Berlin"]
console.log([...map.entries()]); // [["name", "Anna"], ["stadt", "Berlin"]]
```

---

## **2. `Set` – Sammlung eindeutiger Werte**  

Ein **`Set`** speichert **einzigartige Werte** (keine Duplikate).

### **2.1 Erstellen & Befüllen eines Sets**
```javascript
const zahlenSet = new Set([1, 2, 3, 3, 4]);

console.log(zahlenSet.size); // 4 (kein doppeltes 3)
```

---

### **2.2 Methoden von `Set`**
```javascript
zahlenSet.add(5);
console.log(zahlenSet.has(3)); // true
zahlenSet.delete(2);
zahlenSet.clear(); // Löscht alle Einträge
```

---

### **2.3 `forEach()`, `keys()`, `values()`, `entries()`**
```javascript
const set = new Set(["Apfel", "Banane", "Kirsche"]);
set.forEach((wert) => console.log(wert));

console.log([...set.keys()]); // ["Apfel", "Banane", "Kirsche"]
console.log([...set.values()]); // ["Apfel", "Banane", "Kirsche"]
console.log([...set.entries()]); // [["Apfel", "Apfel"], ["Banane", "Banane"], ["Kirsche", "Kirsche"]]
```
✅ **Perfekt für Listen ohne doppelte Werte**  

---

## **3. `WeakMap` – Schlüssel-Objekte mit automatischem Speicherfreigeben**  

Ein **`WeakMap`** speichert nur **Objekte als Schlüssel** und erlaubt **automatische Speicherbereinigung (Garbage Collection)**, wenn das Objekt nicht mehr verwendet wird.

### **3.1 Erstellen & Verwenden einer `WeakMap`**
```javascript
const weakMap = new WeakMap();
let obj = { id: 1 };

weakMap.set(obj, "Daten für das Objekt");
console.log(weakMap.get(obj)); // "Daten für das Objekt"

obj = null; // Das Objekt wird entfernt -> automatisch aus WeakMap gelöscht
```
✅ **Speichert nur Objekte als Schlüssel**  
✅ **Automatische Speicherfreigabe bei `null`**  
❌ **Hat keine `size`, `keys()`, `values()` oder Iterationsmethoden**  

---

## **4. `WeakSet` – Sammlung von Objekten mit automatischer Speicherfreigabe**  

Ein **`WeakSet`** speichert **nur Objekte** und entfernt sie automatisch, wenn sie nicht mehr referenziert werden.

### **4.1 Erstellen & Verwenden eines `WeakSet`**
```javascript
const weakSet = new WeakSet();
let obj1 = { name: "Max" };

weakSet.add(obj1);
console.log(weakSet.has(obj1)); // true

obj1 = null; // Objekt wird entfernt -> automatisch aus WeakSet gelöscht
```
✅ **Perfekt für "Markierungen" an Objekten**  
❌ **Keine Iterationsmethoden (`forEach()`, `keys()`, etc.)**  

---

### **Zusammenfassung**
| Struktur | Schlüsseltyp | Werte dürfen sein | Iterierbar? | Speicherbereinigung |
|----------|-------------|-------------------|-------------|---------------------|
| **Map** | Beliebig | Beliebig | ✅ Ja | ❌ Nein |
| **Set** | Keine Schlüssel | Einzigartige Werte | ✅ Ja | ❌ Nein |
| **WeakMap** | Nur Objekte | Beliebig | ❌ Nein | ✅ Ja |
| **WeakSet** | Keine Schlüssel | Nur Objekte | ❌ Nein | ✅ Ja |

🔗 [MDN-Dokumentation zu `Map`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Map)  
🔗 [MDN-Dokumentation zu `Set`](https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Set)  

  **[⬆ Наверх](#top)**

45. ### <a name="45"></a> Live Collections (lebendige Sammlungen)

### **Live Collections (lebendige Sammlungen) in JavaScript**  

**Live Collections** sind **Datenstrukturen im DOM**, die sich **automatisch aktualisieren**, wenn sich das Dokument ändert.  

---

## **1. Arten von Live Collections**
- **`HTMLCollection`** → Ergebnis von `getElementsByTagName()`, `getElementsByClassName()`
- **`NodeList` (manchmal live)** → Ergebnis von `querySelectorAll()` (statisch) oder `childNodes` (live)

---

## **2. `HTMLCollection` – Automatisch aktualisierbare Liste von Elementen**
Ein **`HTMLCollection`** wird live aktualisiert, wenn sich das DOM verändert.

```javascript
const divs = document.getElementsByTagName("div");
console.log(divs.length); // Anzahl der <div>-Elemente

const neuesDiv = document.createElement("div");
document.body.appendChild(neuesDiv); // Ein neues <div> wird hinzugefügt

console.log(divs.length); // Live-Collection zeigt automatisch die neue Anzahl!
```
✅ **Live (automatische Updates)**  
❌ **Hat keine Array-Methoden (`map()`, `filter()`, etc.)**  

---

## **3. `NodeList` – Live vs. Statische Liste**
Nicht alle `NodeList`-Sammlungen sind live!  

### **3.1 Live `NodeList` (z. B. `childNodes`)**
```javascript
const nodes = document.body.childNodes;
console.log(nodes.length);

const neuerText = document.createTextNode("Hallo!");
document.body.appendChild(neuerText);

console.log(nodes.length); // Wird automatisch aktualisiert!
```
✅ **Live-Updates bei Änderungen**  
❌ **Enthält auch `TextNodes` und `Comments`**  

---

### **3.2 Statische `NodeList` (`querySelectorAll()`)**
```javascript
const liste = document.querySelectorAll("li");
console.log(liste.length); // Anzahl der <li>-Elemente

const neuesLi = document.createElement("li");
document.querySelector("ul").appendChild(neuesLi);

console.log(liste.length); // ❌ Bleibt unverändert (statisch)!
```
✅ **Hat `forEach()` & andere Array-Methoden**  
❌ **Bleibt unverändert, wenn DOM geändert wird**  

---

## **4. Live Collection in einer Schleife (Problem!)**
Ein **großes Problem** mit Live Collections: Änderungen während einer Schleife führen zu unerwartetem Verhalten.

```javascript
const elemente = document.getElementsByTagName("p");

for (let i = 0; i < elemente.length; i++) {
  document.body.removeChild(elemente[i]); // ⚠️ Fehler: `elemente.length` ändert sich!
}
```
✅ **Lösung:** Rückwärts iterieren oder `Array.from()` verwenden.

```javascript
const elemente = Array.from(document.getElementsByTagName("p"));

elemente.forEach(p => document.body.removeChild(p)); // Funktioniert sicher
```

---

### **Zusammenfassung**
| Sammlung | Live? | Methoden verfügbar? | Typ |
|----------|------|----------------|------|
| **`HTMLCollection`** | ✅ Ja | ❌ Keine Array-Methoden | Elemente |
| **`NodeList` (z. B. `childNodes`)** | ✅ Ja | ❌ Nur `forEach()` | Knoten (Elemente, Text) |
| **`NodeList` (`querySelectorAll()`)** | ❌ Nein | ✅ Array-Methoden | Elemente |

🔗 [MDN-Dokumentation zu Live Collections](https://developer.mozilla.org/de/docs/Web/API/HTMLCollection)

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
