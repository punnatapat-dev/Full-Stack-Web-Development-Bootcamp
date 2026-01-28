# 📘 Section 7: Intermediate CSS

---

## 🔑 CSS Cascade 

## Was ist die CSS Cascade?
Die CSS Cascade ist ein Regelwerk, das bestimmt,
welche CSS-Regel angewendet wird, wenn mehrere Regeln
dasselbe Element betreffen und sich gegenseitig widersprechen.

## 🔄 Wie funktioniert die Cascade?
Der Browser prüft CSS-Regeln Schritt für Schritt
von oben nach unten – ähnlich wie Wasser in einem Wasserfall.
Die Regel mit der höchsten Priorität nach allen Prüfungen
wird schließlich im Browser angezeigt.

## 🧩 Die 4 wichtigsten Faktoren der CSS Cascade
Von niedriger zu höherer Priorität

### 1️⃣ Position (Reihenfolge)
Wenn Selektor und Property gleich sind,
gewinnt die CSS-Regel, die weiter unten in der Datei steht.

p { color: red; }
p { color: blue; }

### 2️⃣ Spezifität (Specificity)
Reihenfolge der Selektor-Priorität:

1. Element-Selektor → p
2. Klassen-Selektor → .class
3. Attribut-Selektor → [attr]
4. ID-Selektor → #id

Beispiel:
p { color: green; }
.text { color: blue; }
[draggable] { color: purple; }
#title { color: orange; }

🍊 Endergebnis: orange

### 3️⃣ Typ der CSS-Regel
Prioritätsreihenfolge:

1. Externes CSS (style.css)
2. Internes CSS (<style>)
3. Inline-CSS (style="") → gewinnt

Inline-CSS ist wichtiger als ID-Selektoren.

### 4️⃣ Wichtigkeit (!important)
Eine Regel mit !important überschreibt alle anderen Regeln,
unabhängig von Position, Spezifität oder Typ.

Beispiel:
color: red !important;

!important sollte nur sparsam verwendet werden.

## 🏆 Gesamte Prioritätsreihenfolge der Cascade
1. Position
2. Spezifität
3. Typ
4. !important

Innerhalb jeder Kategorie gibt es zusätzliche Prioritätsstufen.

## 🧪 Quiz – Merkhilfen
ID vs. Klasse → ID gewinnt
Klasse vs. Klasse → die untere Regel gewinnt
ID vs. Inline → Inline gewinnt
Alles vs. !important → !important gewinnt

## ✅ Fazit
Wenn CSS nicht wie erwartet funktioniert,
nicht raten – sondern die Cascade systematisch prüfen:

Position → Spezifität → Typ → !important

---
# 📘 CSS Selector-Kombinationen 

## ❓ Warum Selektoren kombinieren?
- `p {}` stylt **alle** Absätze
- Für jedes Element eine eigene Klasse zu vergeben → HTML wird unübersichtlich
- Lösung: **HTML-Struktur + kombinierte Selektoren nutzen**

## 1️⃣ Gruppierungsselektor (,)
Wird verwendet, um mehreren Selektoren **denselben Stil** zuzuweisen.

Beispiel:
h1, h2 {
  color: blueviolet;
}

✔ Spart Code  
✔ Funktioniert mit Elementen, Klassen und IDs

## 2️⃣ Child-Selektor (>)
Wählt **nur direkte Kindelemente (1 Ebene tief)** aus.

Syntax:
parent > child

Beispiel:
.box > p {
  color: firebrick;
}

✔ Nur direkte Kinder  
✖ Keine Enkel-Elemente

## 3️⃣ Descendant-Selektor (Leerzeichen)
Wählt **alle Nachfahren**, egal wie tief verschachtelt.

Syntax:
ancestor descendant

Beispiel:
.box li {
  color: blue;
}

✔ Ideal bei tieferen HTML-Strukturen  
✔ Flexibler als der Child-Selektor

## 4️⃣ Chaining-Selektoren (ohne Leerzeichen)
Wird verwendet, wenn **alle Bedingungen gleichzeitig** zutreffen müssen.

Syntax:
element.class
element#id
element.class1.class2

Beispiel:
li.done {
  color: seagreen;
}

✔ Sehr präzise Auswahl  
✔ Unterscheidet z.B. `li.done` von `p.done`  
⚠ Immer mit dem Element beginnen

## 5️⃣ Kombination mehrerer Methoden
Selektoren können kombiniert werden:
- Descendant + Chaining
- Child + Chaining

Beispiel:
ul p.done {
  font-size: 0.5rem;
}

Bedeutung:
Wählt ein `p`-Element mit der Klasse `done`,
das sich innerhalb eines `ul` befindet.

## 🧠 Wichtige Merkhilfen
- Kein Leerzeichen → Chaining (alles im selben Element)
- Leerzeichen → Descendant
- `>` → Child (nur eine Ebene)
- `,` → Gruppierung
- HTML-Struktur ist wichtiger als viele Klassen

---

# 📘 CSS Positioning 
## Ziel der Lektion
Diese Lektion erklärt, wie Elemente auf dem Bildschirm positioniert werden
und wie die vier wichtigsten CSS-Positionierungsarten funktionieren:
static, relative, absolute und fixed.

## 🧭 Die vier Position-Werte in CSS
- static (Standard)
- relative
- absolute
- fixed

Die Positionierung wird mit den Eigenschaften
top, right, bottom und left gesteuert.

## 1️⃣ position: static
- Standardverhalten aller HTML-Elemente
- Elemente folgen dem normalen HTML-Fluss
- top, left, right, bottom haben keine Wirkung

Beispiel:
position: static;

## 2️⃣ position: relative
- Element wird relativ zu seiner ursprünglichen Position verschoben
- Der Platz im Layout bleibt erhalten

Beispiel:
position: relative;
top: 50px;
left: 50px;

Wichtig:
„relative“ bedeutet nicht relativ zu anderen Elementen,
sondern relativ zur eigenen Ausgangsposition.

## 3️⃣ position: absolute
- Element wird aus dem normalen HTML-Fluss entfernt
- Positionierung relativ zum nächsten positionierten Vorfahren
- Gibt es keinen positionierten Vorfahren,
  erfolgt die Positionierung relativ zur linken oberen Ecke der Webseite

Beispiel:
position: absolute;
top: 50px;
left: 50px;

Wichtig:
Der gewünschte Eltern-Container sollte position: relative haben.

## 🔢 z-index
- Steuert die Stapelreihenfolge auf der Z-Achse (vorne / hinten)
- Standardwert ist 0
- Höherer Wert liegt weiter vorne
- Negative Werte sind möglich

Beispiel:
z-index: 100;

Hinweis:
Absolute Positionierung legt Elemente auf eine eigene Ebene.

## 4️⃣ position: fixed
- Position relativ zum Browserfenster
- Element bleibt beim Scrollen an derselben Stelle sichtbar

Beispiel:
position: fixed;
top: 50px;
left: 50px;

Geeignet für:
Navigationen, Header, Floating Buttons.

## 📦 Position und Box-Modell
- position wirkt außerhalb von margin
- Reihenfolge:
content → padding → border → margin → position

Position berechnet Abstände automatisch,
um feste Abstände (z. B. 50px von oben) beizubehalten.

## ⚪ Kreis mit CSS erstellen
Ein Kreis ist ein normales Rechteck mit border-radius: 50 %

Beispiel:
width: 200px;
height: 200px;
border-radius: 50%;

Erklärung:
Absolute Positionierung bezieht sich immer auf den nächsten
positionierten Vorfahren.

## 🧠 Merkhilfen
- static → normaler HTML-Fluss
- relative → Verschiebung vom eigenen Platz
- absolute → relativ zum nächsten positionierten Elternteil
- fixed → relativ zum Browserfenster
- absolute entfernt das Element aus dem Flow
- relative behält den Platz im Layout

## ✅ Fazit
CSS-Positionierung bedeutet nicht Auswendiglernen,
sondern das Verstehen von Beziehungen zwischen Elementen.
Wer weiß, wozu ein Element relativ ist,
kann Layout-Probleme gezielt und sicher lösen.

🌍 **Live Demo:**  
    https://punnatapat-dev.github.io/Full-Stack-Web-Development-Bootcamp/section-07-intermediate-css/
