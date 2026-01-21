# Section 2

## 🧱 HTML Heading Elements  

### 📌 Anatomie eines HTML-Elements
Ein HTML-Element definiert sich durch:
- den **Opening Tag** (z. B. `<h1>`)
- den **Content** (eingebetteter Inhalt)
- den **Closing Tag** (z. B. `</h1>`)

---

### 🔍 Differenzierung: Tag vs. Element
- Ein **Tag** bezeichnet lediglich die syntaktische Markierung innerhalb der spitzen Klammern `< >`
- Ein **Element** umfasst das gesamte Konstrukt und besteht aus Start-Tag, Inhalt und End-Tag

---

### 🧩 Semantische Hierarchie (h1–h6)
- Headings dienen der logischen Strukturierung eines Dokuments  
  (vergleichbar mit einem Inhaltsverzeichnis)
- **`<h1>`** ist die Hauptüberschrift mit der höchsten Priorität  
  → sollte pro Seite **idealerweise nur einmal** verwendet werden
- **`<h2>` bis `<h6>`** werden für untergeordnete Sektionen genutzt
- Syntaktisch existiert kein Tag oberhalb von `<h6>`  
  → ein `<h7>` gibt es nicht

---

### 🖥️ Browser-Rendering
- Browser stellen Headings standardmäßig in absteigender Größe dar
- `<h1>` wird am größten, `<h6>` am kleinsten angezeigt

---

## 🧱 HTML Paragraph-Element  

- 📄 Einführung in das **Paragraph-Element (`<p>`)**, das zur Formatierung und Trennung von Text auf Webseiten verwendet wird

### 🏗️ Aufbau eines Paragraph-Elements
- 🔓 Öffnender Tag: `<p>`
- 🔒 Schließender Tag: `</p>`
- ✍️ Inhalt befindet sich zwischen den Tags

### ❌ Ohne Verwendung von `<p>`
- Texte werden in einer einzigen Zeile dargestellt
- Absätze sind nicht klar voneinander getrennt

### ✅ Durch die Verwendung von `<p>`
- Absätze werden klar voneinander getrennt
- Die Webseite wird besser lesbar

### ♿ Bedeutung für Accessibility
- Screenreader nutzen Paragraph-Elemente
- Erleichtert sehbehinderten Nutzern das Navigieren zwischen Absätzen

### 🛠️ Praktische Übung
- Anwendung des Paragraph-Elements im `index.html`
- Strukturierung von Texten in mehrere Absätze

### 🧪 Verwendung von Lorem Ipsum
- Platzhaltertext (Placeholder Text) für Webdesign und Layout
- Ersatz für echten Inhalt während der Entwicklungsphase
- Erzeugt natürlich wirkende Textblöcke

### 🌐 Quellen für Lorem Ipsum
- `lipsum.com`
- Spaßige Varianten wie `baconipsum.com` oder `broipsum.com`

---

## 🧱 HTML Void Elements — Zusammenfassung  

Diese Lektion führt in **HTML Void Elements** ein.  
Dabei handelt es sich um Elemente, die **keinen Content enthalten dürfen** und **keinen separaten Closing-Tag** besitzen.

### 🔹 Void Elements in dieser Einheit
- **`<hr />`**  
  → Erstellt eine horizontale Trennlinie zur visuellen Abgrenzung von Inhalten
- **`<br />`**  
  → Erzeugt einen Zeilenumbruch innerhalb eines Absatzes  
  → Geeignet für Gedichte, Adressen oder strukturierte Texte  
  → **Nicht** als Ersatz für `<p>` verwenden

### 🧠 Wichtige Konzepte zu Void Elements
- Void Elements enthalten keinen Content
- Sie werden als selbstschließende Tags verwendet (z. B. `<hr />`, `<br />`)
- Es muss ein **Forward Slash (`/`)** verwendet werden, kein Backslash (`\`)
- In HTML5 sind `<hr>` und `<br>` ohne Slash erlaubt  
  → die Variante mit `/` wird jedoch empfohlen, da sie besser lesbar ist

---

## 🎬 Projekt: Movie Ranking List  

### 📋 Erforderliche HTML-Struktur
Das Projekt muss mindestens folgende Elemente enthalten:
- `<h1>` für den Website-Titel
- `<h2>` für Untertitel oder Beschreibung
- `<hr />` als visuelle Trennlinie
- `<h3>` für mindestens drei Filmtitel
- `<p>` zur Beschreibung der Filme

### 🛠️ Lernziele des Projekts
- Anwendung von Heading-Elementen zur strukturierten Gliederung
- Nutzung des Paragraph-Elements zur inhaltlichen Beschreibung
- Einsatz von Void Elements zur visuellen Strukturierung
- Erstellung einer einfachen HTML-Webseite von Grund auf
- Selbstständige Erweiterung und Weiterentwicklung der Seite

🌍 **Live Demo:**  
    https://punnatapat-dev.github.io/Full-Stack-Web-Development-Bootcamp/section-02-html/
