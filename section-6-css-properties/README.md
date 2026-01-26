## 📘 Section 6: CSS Properties  
### 🎨 CSS-Grundlagen für Farben
Eine CSS-Regel besteht immer aus:
- **Property** (Eigenschaft)
- **Value** (Wert)

Beispiel:
background-color: red;

### 🖌️ Wichtige Color-Properties
- **background-color** → setzt die Hintergrundfarbe eines Elements
- **color** → setzt die Textfarbe eines Elements

Beispiel:
body {
  background-color: red;
}

h1 {
  color: blue;
}

### 🌈 Named Colors
CSS bietet viele vordefinierte Farben mit Namen, z. B.:
- red, blue, green
- cornflowerblue, cadetblue, dimgrey, olivedrab

Diese Farben können direkt im Code verwendet werden.
Eine vollständige Liste findet man in den MDN Docs (Named Colors).

### 🎯 Hex Colors (Hex Codes)
Wenn man individuellere Farben möchte, kann man Hex Codes verwenden.

- Ein Hex Code beginnt mit #
- Er basiert auf RGB-Werten (Rot, Grün, Blau), jeweils von 0 bis 255

Beispiel:
h2 {
  color: #5D3891;
}

Hex Codes werden oft in Design-Tools wie Color Hunt verwendet und eignen sich gut für professionelle Farbpaletten.

### 🧪 Übung & Erkenntnisse
- Jedes HTML-Element kann eine Hintergrundfarbe haben
- h1 und h2 können sowohl Text- als auch Hintergrundfarben erhalten
- Named Colors und Hex Colors sind austauschbar
- Bei Unsicherheiten hilft immer ein Blick in die MDN Docs

➡️ Im nächsten Abschnitt geht es um die Formatierung von Schriftarten mit CSS.

