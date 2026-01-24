📘 Section 05: Introduction to CSS
==================================================

🎨 **CSS (Cascading Style Sheets)** ist eine Stylesheet-Sprache, mit der das Aussehen und Layout von Webseiten gestaltet wird. Während **HTML** für die Struktur und den Inhalt zuständig ist, definiert **CSS** Farben, Schriftarten, Abstände und die Anordnung der Elemente.

🌊 Der Begriff **Cascading** beschreibt, dass CSS-Regeln von allgemein zu spezifisch angewendet werden. In den Anfängen des Internets gab es nur HTML, was die Gestaltung von Webseiten stark einschränkte und zu unübersichtlichem Code führte, da Inhalt und Design miteinander vermischt waren.

🧩 CSS wurde eingeführt, um Gestaltung und Inhalt klar voneinander zu trennen (**Separation of Concerns**). Dadurch wird der Code übersichtlicher, leichter wartbar und das Design einer Webseite kann geändert werden, ohne den HTML-Code anzupassen.

🚀 CSS ist daher eine grundlegende und unverzichtbare Technologie in der modernen Webentwicklung.

--------------------------------------------------
🎨 CSS in HTML einbinden
--------------------------------------------------

CSS kann auf drei verschiedene Arten in eine HTML-Datei eingebunden werden: **Inline**, **Internal** und **External CSS**.  
Jede Methode hat ihren eigenen Anwendungsbereich.

✏️ **1) Inline CSS**  
Inline CSS wird direkt im HTML-Element mit dem Attribut `style` geschrieben und gilt nur für dieses einzelne Element.

**Beispiel:**
```html
<h1 style="color: blue;">Style me in blue</h1>
```

✔️ Geeignet für einzelne Elemente oder schnelle Tests  
❌ Nicht empfehlenswert für größere Webseiten

🧩 **2) Internal CSS**  
Internal CSS wird innerhalb der HTML-Datei im `<style>`-Tag definiert, meistens im `<head>`-Bereich.  
Die Styles gelten nur für diese eine HTML-Seite.

**Beispiel:**
```html
<head>
  <style>
    h1 {
      color: red;
    }
  </style>
</head>
```

```html
<h1>Style me in red</h1>
```

✔️ Geeignet für eine einzelne Seite  
❌ Ungeeignet für Multi-Page-Websites

🌍 **3) External CSS**  
External CSS wird in einer separaten `.css`-Datei gespeichert und mit der HTML-Datei verknüpft.  
Dies ist die empfohlene und am häufigsten verwendete Methode in der Webentwicklung.

**Beispiel (style.css):**
```css
h1 {
  color: green;
}
```

**HTML:**
```html
<head>
  <link rel="stylesheet" href="./style.css">
</head>
```

```html
<h1>Style me in green</h1>
```

✔️ Ideal für Webseiten mit mehreren Seiten  
✔️ Sauberer, wartbarer Code (Best Practice)

📌 **Übersicht**
- ✏️ Inline CSS → einzelnes Element  
- 🧩 Internal CSS → eine HTML-Seite  
- 🌍 External CSS → mehrere Seiten (Best Practice)

--------------------------------------------------
🎯 CSS Selectors – Übersicht
--------------------------------------------------

CSS Selectors bestimmen, auf welche HTML-Elemente CSS-Regeln angewendet werden.  
Ein Selector legt fest, wo und wie ein Style eingesetzt wird.

🏷️ **Element Selector**  
Wählt alle HTML-Elemente eines bestimmten Tags aus.

**Beispiel:**
```css
h1 {
  color: blue;
}
```

→ Gilt für alle `<h1>`-Elemente.

🧩 **Class Selector**  
Wird mit einem Punkt (.) geschrieben und kann mehreren Elementen zugewiesen werden.

**Beispiel:**
```css
.red-text {
  color: red;
}
```

→ Gilt für alle Elemente mit `class="red-text"`.

🆔 **ID Selector**  
Wird mit einer Raute (#) geschrieben und darf nur einmal pro HTML-Datei verwendet werden.

**Beispiel:**
```css
#main {
  color: green;
}
```

→ Gilt nur für das Element mit `id="main"`.

🔗 **Attribute Selector**  
Wählt Elemente anhand eines bestimmten Attributs oder Attributwerts aus.

**Beispiel:**
```css
p[draggable="false"] {
  color: red;
}
```

→ Gilt nur für `<p>` mit `draggable="false"`.

🌐 **Universal Selector**  
Der Stern (*) wählt alle Elemente aus.

**Beispiel:**
```css
* {
  text-align: center;
}
```

→ Gilt für alle Elemente auf der Seite.

📌 **Kurzüberblick Selectors**
- 🏷️ Element → alle gleichen HTML-Tags  
- 🧩 Class → mehrere Elemente  
- 🆔 ID → ein eindeutiges Element  
- 🔗 Attribute → Auswahl nach Attribut(en)  
- 🌐 Universal → alle Elemente
  
🌍 **Live Demo:**  
https://punnatapat-dev.github.io/Full-Stack-Web-Development-Bootcamp/section-05-introduction-to-css/
