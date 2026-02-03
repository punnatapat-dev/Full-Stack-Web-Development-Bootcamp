📘 Day 9 📦 CSS Flexbox

✅ **Flexbox** ist ein modernes Layout-System in CSS, das entwickelt wurde, um flexible, übersichtliche und responsive Webseiten-Strukturen zu erstellen.  
Durch das Setzen des Containers auf `display: flex;` werden alle enthaltenen Elemente standardmäßig horizontal angeordnet.

🔧 **Wichtige Eigenschaften von Flexbox**
- 🎯 Einfache Kontrolle über das Layout ohne komplizierte Hacks
- 🚫 Frühere `display`-Werte der Kindelemente (`block` / `inline`) werden ignoriert
- 📐 Die Breite der Elemente richtet sich automatisch nach dem Inhalt
- 📏 Abstände zwischen Elementen können bequem mit `gap` definiert werden

🧩 **Zwei Varianten des Flex-Containers**
- `flex` → nimmt die volle Breite ein
- `inline-flex` → nimmt nur so viel Platz ein wie nötig

🧪 **Praxisübung**
Eine Liste (`list items`) wird mithilfe von Flexbox in eine Navigationsleiste umgewandelt.  
Dafür reichen bereits folgende CSS-Eigenschaften aus:

display: flex;  
gap: 1rem;

---

## 🔁 Flex Direction & Axis 

Standardmäßig verwendet Flexbox `flex-direction: row;`  
→ Elemente werden horizontal von links nach rechts angeordnet.

🔧 **flex-direction**
`flex-direction` bestimmt die Anordnung der Flexbox-Items:
- `row` → horizontale Anordnung
- `column` → vertikale Anordnung

🧭 **Achsen in Flexbox**
In Flexbox gibt es zwei wichtige Achsen:
- **Main Axis** → Hauptrichtung der Anordnung
- **Cross Axis** → Achse, die senkrecht zur Main Axis verläuft

🔄 **Zusammenhang zwischen flex-direction und Achsen**

`flex-direction: row`  
- Main Axis → links ↔ rechts  
- Cross Axis → oben ↕ unten  

`flex-direction: column`  
- Main Axis → oben ↕ unten  
- Cross Axis → links ↔ rechts  

📏 **flex-basis**
`flex-basis` definiert die Anfangsgröße eines Flex-Items entlang der Main Axis:
- bei `row` → flex-basis = Breite
- bei `column` → flex-basis = Höhe  

`flex-basis` wird auf die **Child-Elemente**, nicht auf den Container angewendet.

Beispiel für alle direkten Kinder eines Containers:  
.container > * { flex-basis: 100px; }

📦 **display: inline-flex**  
`display: inline-flex` → Der Container nimmt nur so viel Platz ein wie nötig  
(im Gegensatz zu `display: flex`, das die volle Breite nutzt)

---
## 🧩 Flexbox Layout 

Flexbox besitzt Properties, die entweder auf den **Parent (Container)** oder auf die **Child-Elemente (Flex Items)** angewendet werden.  
Diese Unterscheidung ist sehr wichtig, da Properties nicht funktionieren, wenn sie am falschen Element gesetzt werden.

🔢 **Properties für Child (Flex Item)**

**order**  
Ändert die Reihenfolge der Flex Items  
- Standardwert: `0` → Reihenfolge gemäß HTML  
- Höherer Wert → Element wird weiter nach hinten verschoben  

**align-self**  
- Richtet ein einzelnes Flex Item unabhängig von den anderen aus  
- Überschreibt die Einstellung von `align-items`

📦 **Properties für Parent (Container)**

**flex-wrap**
- `nowrap` (Standard) → Kein Zeilenumbruch  
- `wrap` → Items, die keinen Platz haben, umbrechen in die nächste Zeile  
- `wrap-reverse` → Umbruch mit umgekehrter Richtung  

**justify-content (Main Axis)**  
Steuert die Verteilung der Items entlang der Hauptachse  
Beispiele:  
`flex-start`, `flex-end`, `center`,  
`space-between`, `space-around`, `space-evenly`

**align-items (Cross Axis)**  
- Richtet Items entlang der Querachse aus  
- Die Höhe des Containers muss gesetzt sein, damit der Effekt sichtbar wird  
Beispiele:  
`flex-start`, `flex-end`, `center`, `stretch`

**align-content**  
- Richtet mehrere Zeilen von Flex Items aus  
- Funktioniert nur, wenn `flex-wrap: wrap` aktiviert ist

🧠 **Wichtige Konzepte**
- `justify-content` → Ausrichtung entlang der **Main Axis**  
- `align-items` → Ausrichtung der Items entlang der **Cross Axis**  
- `align-content` → Ausrichtung von Item-Gruppen / Zeilen (nur mit Wrap)

---

## 🧩 Flexbox Layout 
Flexbox bietet viele Eigenschaften zur Erstellung flexibler und responsiver Layouts.  
Dabei ist es sehr wichtig, zwischen **Properties für den Parent (Container)** und **Properties für die Child-Elemente (Flex Items)** zu unterscheiden, da sie sonst nicht korrekt funktionieren.

🔢 **Properties für Child (Flex Items)**

**order**  
Ändert die Reihenfolge der Flex Items  
- Standardwert: `0` → Reihenfolge gemäß HTML  
- Höherer Wert → Element wird weiter nach hinten verschoben  

**align-self**  
- Richtet ein einzelnes Flex Item unabhängig von den anderen aus  
- Überschreibt die Einstellung von `align-items`

📦 **Properties für Parent (Container)**

**flex-wrap**
- `nowrap` (Standard) → Kein Zeilenumbruch  
- `wrap` → Items umbrechen in die nächste Zeile  
- `wrap-reverse` → Umbruch mit umgekehrter Richtung  

**justify-content (Main Axis)**  
Steuert die Verteilung der Items entlang der Hauptachse  
Häufige Werte:  
`flex-start`, `flex-end`, `center`,  
`space-between`, `space-around`, `space-evenly`

**align-items (Cross Axis)**  
- Richtet Items entlang der Querachse aus  
- Die Höhe des Containers muss gesetzt sein, damit der Effekt sichtbar wird  
Beispiele:  
`flex-start`, `flex-end`, `center`, `stretch`

**align-content**  
- Richtet mehrere Zeilen von Flex Items aus  
- Funktioniert nur, wenn `flex-wrap: wrap` aktiviert ist

🧠 **Wichtige Konzepte**
- `justify-content` → Ausrichtung entlang der **Main Axis**  
- `align-items` → Ausrichtung einzelner Items entlang der **Cross Axis**  
- `align-content` → Ausrichtung von Zeilengruppen (nur bei Wrap)

---

## 📐 Flexbox Sizing

Flexbox ermöglicht eine flexible Größensteuerung von Elementen durch **Wachsen (grow)** und **Schrumpfen (shrink)**  
und eignet sich ideal für responsive Layouts.

🧮 **Priorität bei der Größenberechnung**

Flexbox bestimmt die Größe eines Flex-Items in folgender Reihenfolge:
1. `min-width` / `max-width`
2. `flex-basis`
3. `width` / `height`
4. Größe des Inhalts (Content Size)

📦 **Standardverhalten**
- Flex Items richten sich standardmäßig nach der Inhaltsgröße
- Elemente können schrumpfen, aber nicht automatisch wachsen
- Die minimale Größe wird durch das längste Wort bestimmt

📏 **width vs. flex-basis**
- `width` definiert eine feste Größe
- `flex-basis` definiert die Startgröße entlang der **Main Axis**
- Ist `flex-basis` gesetzt, wird `width` ignoriert

🔒 **max-width / 🔓 min-width**
- `max-width` begrenzt die maximale Wachstumsgröße
- `min-width` begrenzt die minimale Schrumpfgröße
- Wenn `min-width` > `flex-basis` → `min-width` wird verwendet
- Wenn `max-width` < `flex-basis` → `max-width` wird verwendet

🌱 **flex-grow / flex-shrink**
- `flex-grow` → erlaubt das Wachsen eines Items
- `flex-shrink` → erlaubt das Schrumpfen eines Items

Standardwerte:
- `flex-grow: 0;`
- `flex-shrink: 1;`

Häufige Kombinationen:

`flex-grow: 1;`  
`flex-shrink: 1;`  
→ Item wächst und schrumpft flexibel

`flex-grow: 0;`  
`flex-shrink: 0;`  
→ Feste Größe, keine Flexibilität

⚙️ **flex-basis: auto vs. 0**
- `auto` (Standard) → Items mit mehr Inhalt erhalten mehr Platz
- `0` → Alle Items starten gleich breit (sehr gebräuchlich)

✨ **Shorthand für Flex**

`flex: 1;`

entspricht:
- `flex-grow: 1;`
- `flex-shrink: 1;`
- `flex-basis: 0;`

Ideal zur Definition von Layout-Verhältnissen  
(z. B. `flex: 1`, `flex: 2`, `flex: 3`)

🧠 **Wichtige Konzepte**
- Die Stärke von Flexbox liegt im **Wachsen und Schrumpfen**
- `flex-basis` bestimmt die Startgröße eines Elements
- Das `flex`-Shorthand ist das wichtigste Werkzeug für responsive Flexbox-Layouts
- 
---

🌐 Live Demo:
https://punnatapat-dev.github.io/Full-Stack-Web-Development-Bootcamp/section-09-flexbox/

