## 📘 Section 10  CSS Grid 

---

📦 CSS Grid ist ein CSS-Layout-System zur Erstellung von **zweidimensionalen (2D)** Layouts.  
Es ermöglicht die gleichzeitige Steuerung von **Zeilen (rows)** und **Spalten (columns)**.  
Besonders geeignet für komplexe Layouts wie Hauptseiten, Dashboards, Tabellen oder ein Schachbrett.

🔹 **Grid vs. Flexbox**

**Flexbox** → geeignet für **eindimensionale (1D)** Layouts  
z. B. horizontale **oder** vertikale Anordnung  

**Grid** → geeignet für **zweidimensionale (2D)** Layouts  
präzise Positionierung in Zeilen **und** Spalten  

👉 In der Praxis werden **Grid und Flexbox oft kombiniert**  
z. B. Grid für das Grundlayout und Flexbox innerhalb einzelner Bereiche

🔹 **Grundprinzipien von CSS Grid**

Container als Grid definieren  
`display: grid;`

Anzahl und Größe der Spalten festlegen  
`grid-template-columns: repeat(8, 100px);`

Anzahl und Größe der Zeilen festlegen  
`grid-template-rows: repeat(8, 100px);`

Abstände zwischen den Zellen definieren (optional)  
`gap: 10px;`

🔹 **Beispielhafte Anwendung**
- Ein 8×8-Schachbrett lässt sich einfach und exakt erstellen  
- Grid positioniert die Zellen automatisch anhand von Zeilen und Spalten  
- Sehr gut responsive, die Struktur bleibt auch bei kleineren Bildschirmen erhalten

  ---

## 📐 CSS Grid – Grid Sizing Zusammenfassung

Ein zentraler Punkt bei der Arbeit mit CSS Grid ist die Definition der Größen von  
**Zeilen (rows)** und **Spalten (columns)**, passend zum Design und für responsive Layouts.

🔹 **1. Feste Größen (px / rem)**

Definition fester Größen mit `px` oder `rem`

`grid-template-rows: 100px 200px;`  
`grid-template-columns: 400px 800px;`

❌ Nicht responsive  
- Größen passen sich nicht an die Bildschirmbreite an  
- `rem` bezieht sich auf die Root-Schriftgröße, nicht auf die Bildschirmgröße  

🔹 **2. Shorthand: grid-template**

Kombiniert Zeilen und Spalten in einer einzigen Zeile

`grid-template: 100px 200px / 400px 800px;`

- Funktioniert, aber nicht empfohlen für Einsteiger  
- Schwerer zu lesen und schwieriger zu debuggen  
- Wichtig zu kennen beim Lesen von Fremdcode  

🔹 **3. Auto Size**

Verwendung von `auto` für mehr Responsiveness

`grid-template-columns: 200px auto;`  
`grid-template-rows: 100px auto;`

- `auto` bei Columns → füllt den verbleibenden Platz  
- `auto` bei Rows → Höhe richtet sich nach dem Inhalt  
- ⚠️ Rows werden nicht automatisch so hoch wie der Viewport  

🔹 **4. Fractional Unit (fr)**

Größenangabe mit Verhältniswerten

`grid-template-rows: 1fr 2fr;`  
`grid-template-columns: 1fr 1fr;`

- Ideal für proportionale Layouts  
- Von Natur aus responsive  
- Passt sich dem verfügbaren Platz an  

🔹 **5. minmax()**

Definition von Minimal- und Maximalgrößen

`grid-template-columns: auto minmax(400px, 800px);`

- Verhindert zu kleine oder zu große Spalten  
- Besonders geeignet für Bilder oder wichtige Inhalte  
- Responsive innerhalb definierter Grenzen  

🔹 **6. repeat()**

Reduziert redundanten Code

`grid-template-columns: repeat(8, 1fr);`  
`grid-template-rows: repeat(2, 200px);`

- Spart Zeit  
- Verbessert die Lesbarkeit  
- Gleiches Ergebnis wie manuelles Wiederholen  

🔹 **7. Grid mit nicht passender Item-Anzahl**

- Grid größer als Items → leere Zellen bleiben sichtbar  
- Mehr Items als Grid → neue Zeilen/Spalten werden automatisch erzeugt  

Größe der automatisch erzeugten Bereiche steuerbar mit:

`grid-auto-rows: 50px;`  
`grid-auto-columns: 300px;`

🔹 **8. Grid Debugging mit Chrome DevTools**

- Klick auf `grid` im DevTools-Panel  
- Anzeige von Grid-Linien, Zeilen-/Spaltengrößen und Line-Nummern  
- Erleichtert das Verständnis des Layouts und die Fehlersuche  

✅ **Zusammenfassung**
- `px / rem` → fest, nicht responsive  
- `auto` → Column füllt Platz / Row folgt Inhalt  
- `fr` → flexibel, proportional, sehr empfehlenswert  
- `minmax()` → kontrollierte Responsiveness  
- `repeat()` → kürzerer, sauberer Code  
- `grid-auto-*` → Kontrolle über automatisch erzeugte Items

---

- 🧮 ****Projekt: Mondrian Painting****
  - 🧩 [Source Code](./section-10-grid/index.html)
  - 🌐 **Live Demo:**  
    https://punnatapat-dev.github.io/Full-Stack-Web-Development-Bootcamp/section-10-grid/
