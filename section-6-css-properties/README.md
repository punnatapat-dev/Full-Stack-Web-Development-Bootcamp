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

---

## 🅰️ CSS Font Properties 


CSS bietet verschiedene Eigenschaften, um das Aussehen von Text auf Webseiten zu steuern. Zu den wichtigsten Font-Eigenschaften gehören font-size, font-weight, font-family und text-align.

### 🔤 font-size

Mit font-size wird die Größe des Textes festgelegt. Es gibt feste und relative Einheiten.

- px, pt → feste Größen (statisch)
- em → relative Größe zum Parent-Element
- rem → relative Größe zum Root-Element (html)

Beispiele:
font-size: 20px;   /* feste Größe */
font-size: 2em;    /* 2× Parent-Größe */
font-size: 2rem;   /* 2× Root-Größe */

Empfehlung: rem verwenden, da es übersichtlicher und konsistenter ist.


### ⚖️ font-weight

Mit font-weight wird die Schriftstärke bestimmt.

Mögliche Werte:
- normal
- bold
- lighter / bolder (relativ zum Parent)
- Zahlen von 100 bis 900 (z. B. 400 = normal, 700 = bold)

Beispiel:
font-weight: 700;


### 🆎 font-family

font-family bestimmt die Schriftart (Typeface).  
Es ist wichtig, immer eine generische Schriftart als Fallback anzugeben.

Beispiel:
font-family: Helvetica, sans-serif;

Bei Schriftarten mit Leerzeichen müssen Anführungszeichen verwendet werden:
font-family: "Times New Roman", serif;


### 🌐 Google Fonts

Für benutzerdefinierte Schriftarten können Google Fonts verwendet werden.

Vorgehen:
1. Schriftart auf fonts.google.com auswählen
2. <link>-Tag kopieren und im <head> einfügen
3. font-family in CSS verwenden

Dadurch sehen alle Nutzer dieselbe Schriftart, unabhängig vom Betriebssystem.


### 📐 text-align

Mit text-align wird die Ausrichtung des Textes festgelegt.

Mögliche Werte:
- left
- right
- center
- start / end (flexibel für verschiedene Schreibrichtungen)

Beispiel:
text-align: center;

--------------------------------------------------

## 🔍 CSS Inspection – Chrome Developer Tools

In dieser Lektion geht es um CSS Inspection und die Nutzung der Chrome Developer Tools, mit denen man CSS-Regeln analysieren, verstehen und Fehler finden kann. Die Developer Tools sind kostenlos und direkt im Chrome-Browser integriert.


### 🛠️ Chrome Developer Tools öffnen

Die Developer Tools können auf verschiedene Arten geöffnet werden:
- Menü (⋮) → More Tools → Developer Tools
- Rechtsklick auf ein Element → Inspect
- Tastenkürzel:
  - Mac: Cmd + Option + I
  - Windows: Ctrl + Shift + I
  - Alternativ: F12


### 🧩 Elements- und Styles-Bereich

Im Tab „Elements“ sieht man den HTML-Code der Seite.  
Der Bereich „Styles“ zeigt alle CSS-Regeln, die auf das ausgewählte Element angewendet werden, inklusive der Datei, aus der sie stammen (z. B. styles.css).

- Durchgestrichene Regeln → wurden überschrieben
- Eigene CSS-Regeln überschreiben Standard-Browser-Styles


### ✏️ CSS live bearbeiten

CSS kann direkt in den Developer Tools geändert oder hinzugefügt werden.  
Diese Änderungen wirken sich nur lokal und temporär aus und verändern nicht die eigentlichen HTML- oder CSS-Dateien.

Dies ist ideal, um Styles zu testen, bevor sie in den echten Code übernommen werden.


### 📊 Computed Tab

Der „Computed“-Tab zeigt die tatsächlich angewendeten CSS-Werte (z. B. Farben in RGB), ohne überschreibende oder deaktivierte Regeln.  
Er hilft dabei, schnell zu erkennen, welche Styles wirklich aktiv sind.


### 🎨 CSS Overview

Über:
Developer Tools (⋮) → More Tools → CSS Overview

kann eine Übersicht erstellt werden, die unter anderem zeigt:
- verwendete Farben
- verwendete Schriftarten
- allgemeine CSS-Informationen der Seite

Sehr hilfreich, um Farben oder Fonts auf fremden Webseiten zu analysieren.


### 🧠 Einsatz des Inspectors

Mit dem CSS Inspector kann man:
- CSS-Regeln anderer Webseiten verstehen
- eigene Styles debuggen
- vererbte Styles erkennen
- Probleme mit Überschreibungen finden

--------------------------------------------------
## 📦 CSS Box Model

Das CSS Box Model beschreibt, wie HTML-Elemente auf einer Webseite aufgebaut und dargestellt werden. Jedes Element wird als rechteckige Box betrachtet, die aus vier Bereichen besteht: Content, Padding, Border und Margin.


### 🧱 Bestandteile des Box Models

1) Content  
Der eigentliche Inhalt des Elements, z. B. Text oder Bilder.  
Die Größe wird durch width und height bestimmt.

2) Padding  
Der Abstand zwischen Content und Border.  
Padding vergrößert den Innenraum der Box, ohne die festgelegte width und height zu verändern.

3) Border  
Der Rand um das Element.  
Ein Border besteht aus drei Angaben:
- Breite (z. B. 10px)
- Stil (z. B. solid, dashed)
- Farbe (z. B. black)

Beispiel:
border: 10px solid black;

Der Border wächst nach außen und verändert nicht die Größe des Contents.

4) Margin  
Der äußere Abstand zwischen einem Element und anderen Elementen.  
Margins erzeugen Abstand zwischen Boxen auf der Seite.

### 📐 Reihenfolge im Box Model

Von innen nach außen:
Content → Padding → Border → Margin


### 🔢 Mehrere Werte für Padding, Margin und Border-Width

Diese Eigenschaften können 1, 2 oder 4 Werte annehmen:

- 1 Wert → alle Seiten gleich  
  padding: 10px;

- 2 Werte → oben/unten | links/rechts  
  margin: 10px 20px;

- 4 Werte → oben | rechts | unten | links (im Uhrzeigersinn)  
  border-width: 0px 10px 20px 30px;


### 📏 Width und Height

width und height bestimmen die Größe des Content-Bereichs.  
Padding, Border und Margin werden zusätzlich hinzugefügt und beeinflussen das Layout, nicht aber die eigentliche Content-Größe.


### 🧩 div als Container

Das `<div>`-Element wird verwendet, um Inhalte zu gruppieren.  
Ein div ist unsichtbar und dient als Container, um mehrere Elemente gemeinsam zu layouten oder zu stylen.


### 🛠️ Box Model im Browser inspecten

Im Chrome Developer Tool zeigt der Inspector das Box Model visuell an.  
Dort sind Margin, Border, Padding und Content farblich dargestellt und können live angepasst werden.

