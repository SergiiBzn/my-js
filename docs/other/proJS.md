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
|21 | [](#21) |
|22 | [](#22) |
|23 | [](#23) |
|24 | [](#24) |
|25 | [](#25) |
|26 | [](#26) |
|27 | [](#27) |
|28 | [](#28) |
|29 | [](#29) |
|30 | [](#30) |


<a name="questions"></a>

## JavaScript Grundlagen

  **[⬆ Наверх](#top)**
  
1. ### <a name="1"></a> Klassifizierung von Datentypen, Typumwandlung

# Klassifizierung von Datentypen und Typumwandlung in JavaScript

## **Datentypen in JavaScript**
JavaScript unterteilt Datentypen in primitive Datentypen und komplexe (objektbasierte) Datentypen.

### **Primitive Datentypen**
Primitive Datentypen sind unveränderlich und enthalten nur einen einzelnen Wert:

- **Number**: Ganzzahlen und Gleitkommazahlen (`42`, `3.14`).
- **String**: Zeichenketten, die in Anführungszeichen gesetzt werden (`"Hallo"`, `'Welt'`).
- **Boolean**: Wahrheitswerte `true` oder `false`.
- **undefined**: Eine Variable wurde deklariert, aber nicht initialisiert.
- **null**: Eine explizite Absenz eines Wertes.
- **Symbol** (ES6): Einzigartige und unveränderliche Werte.
- **BigInt** (ES11): Für sehr große ganze Zahlen (`12345678901234567890n`).

### **Objektbasierte Datentypen**
Komplexe Datentypen, die mehrere Werte und Methoden enthalten können:

- **Object**: Sammlung von Schlüssel-Wert-Paaren (`{ key: "value" }`).
- **Array**: Geordnete Listen von Werten (`[1, 2, 3]`).
- **Function**: Wiederverwendbare Codeblöcke (`function() {}`).
- **Date**: Speichert Datums- und Zeitwerte.
- **RegExp**: Muster für die String-Suche (`/abc/`).
- **Weitere**: `Map`, `Set`, `WeakMap`, `WeakSet`, `Promise`, etc.

### **Spezielle Werte**
- **NaN (Not a Number)**: Ergebnis einer ungültigen mathematischen Operation (`Math.sqrt(-1)`).
- **Infinity / -Infinity**: Unendlich große Zahlen (`1 / 0`).

## **Typumwandlung in JavaScript**
JavaScript ist eine dynamisch und schwach typisierte Sprache. Datentypen können explizit oder implizit umgewandelt werden.

### **Explizite Typumwandlung (Type Casting)**
Manuelle Umwandlung von Datentypen mit eingebauten Funktionen.

#### **In eine Zeichenkette konvertieren**
```js
let num = 42;
let str = String(num); // Explizite Konvertierung
console.log(str); // "42"
```

#### **In eine Zahl konvertieren**
```js
let str = "42";
let num = Number(str);
console.log(num); // 42
```
Alternativ:
```js
let num2 = parseInt("42px"); // 42 (nur Ganzzahl wird extrahiert)
let num3 = parseFloat("3.14"); // 3.14
```

#### **In einen Boolean-Wert konvertieren**
```js
let value = "Hallo";
let bool = Boolean(value);
console.log(bool); // true
```

### **Implizite Typumwandlung (Type Coercion)**
JavaScript wandelt Typen automatisch um, je nach Kontext.

#### **Automatische Konvertierung zu einer Zeichenkette**
```js
let number = 42;
let str = "Die Antwort ist " + number;
console.log(str); // "Die Antwort ist 42"
```

#### **Automatische Konvertierung zu einer Zahl**
```js
let a = "42";
let b = "5";
let sum = a - b;
console.log(sum); // 37
```
(Achtung: `+` würde die Strings verketten, nicht subtrahieren.)

#### **Automatische Konvertierung zu einem Boolean**
```js
let value = "Hello";
if (value) {
  console.log("Wahrheitswert ist true"); // Wahrheitswert ist true
}
```

### **Achtung bei unerwarteten Typumwandlungen**
```js
console.log(1 + "1"); // "11" (String-Konkatenation)
console.log(1 - "1"); // 0 (numerische Berechnung)
console.log(true + false); // 1 (true = 1, false = 0)
console.log("5" * "2"); // 10 (automatische Zahlkonvertierung)
```

**Empfehlung**: Verwende explizite Typumwandlungen, um unerwartete Ergebnisse zu vermeiden.

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

5. ### <a name="5"></a> Unterschied zwischen null und undefined


  **[⬆ Наверх](#top)**

6. ### <a name="6"></a> Unterschied zwischen null und undefined


  **[⬆ Наверх](#top)**

7. ### <a name="7"></a> Unterschied zwischen null und undefined


  **[⬆ Наверх](#top)**

8. ### <a name="8"></a> Unterschied zwischen null und undefined


  **[⬆ Наверх](#top)**

9. ### <a name="9"></a> Unterschied zwischen null und undefined


  **[⬆ Наверх](#top)**

10. ### <a name="10"></a> Unterschied zwischen null und undefined


  **[⬆ Наверх](#top)**

11. ### <a name="11"></a> Unterschied zwischen null und undefined


  **[⬆ Наверх](#top)**
