Section 2

##  HTML Heading Elements  
📌 Anatomie eines Elements
Ein HTML-Element definiert sich durch den Opening Tag (z. B. <h1>), den Content (eingebetteter Inhalt) und den Closing Tag (z. B. </h1>).
🔍 Differenzierung
Ein Tag bezeichnet lediglich die syntaktische Markierung innerhalb der spitzen Klammern < >. Ein Element umfasst das gesamte Konstrukt und besteht aus Start-Tag, Inhalt und End-Tag.
🧩 Semantische Hierarchie (h1–h6)
Headings dienen der logischen Strukturierung eines Dokuments und sind vergleichbar mit einem Inhaltsverzeichnis. <h1> ist die Hauptüberschrift mit der höchsten Priorität und sollte pro Seite idealerweise nur einmal verwendet werden. <h2> bis <h6> werden für untergeordnete Sektionen zur Abbildung der Informationsarchitektur genutzt. Syntaktisch existiert kein Tag oberhalb von <h6>, ein <h7> gibt es nicht.
🖥️ Browser-Rendering
Standardmäßig stellt der Browser Headings absteigend dar, wobei <h1> die größte und <h6> die kleinste Darstellung hat.

## HTML Paragraph-Element 
- 📄 Einführung in das **Paragraph-Element (`<p>`)**, das zur Formatierung und Trennung von Text auf Webseiten verwendet wird
- 🏗️ Aufbau eines Paragraph-Elements:
  - 🔓 Öffnender Tag: `<p>`
  - 🔒 Schließender Tag: `</p>`
  - ✍️ Inhalt befindet sich zwischen den Tags
- ❌ Ohne Verwendung von `<p>`:
  - Texte werden in einer einzigen Zeile dargestellt
  - Absätze sind nicht klar voneinander getrennt
- ✅ Durch die Verwendung von `<p>`:
  - Absätze werden klar voneinander getrennt
  - Die Webseite wird besser lesbar
- ♿ Bedeutung für **Accessibility**:
  - Screenreader nutzen Paragraph-Elemente, um sehbehinderten Nutzern das Navigieren zwischen Absätzen zu erleichtern
- 🛠️ Praktische Übung:
  - Anwendung des Paragraph-Elements im `index.html`
  - Strukturierung von Texten in mehrere Absätze
- 🧪 Verwendung von **Lorem Ipsum**:
  - Platzhaltertext (Placeholder Text) für Webdesign und Layout
  - Dient als Ersatz für echten Inhalt während der Entwicklungsphase
  - Erzeugt natürlich wirkende Textblöcke
- 🌐 Quellen für Lorem Ipsum:   - `lipsum.com`
  - Spaßige Varianten wie `baconipsum.com` oder `broipsum.com`
- 📝 Einsatz von Lorem Ipsum zur Übung beim Erstellen von Artikeln mit dem `<p>`-Element

## HTML Void Elements — Zusammenfassung
Diese Lektion führt in HTML Void Elements ein. Dabei handelt es sich um Elemente, die keinen Inhalt (Content) enthalten dürfen und nicht aus einem separaten Opening- und Closing-Tag bestehen wie Non-Void-Elemente (z. B. <p>, <h1>). Stattdessen werden Void Elements als einzelnes, selbstschließendes Tag verwendet.
🔹 Void Elements in dieser Einheit
<hr /> dient zur Erstellung einer horizontalen Trennlinie, mit der inhaltlich nicht zusammengehörige Bereiche visuell voneinander abgegrenzt werden.
<br /> wird verwendet, um innerhalb eines Absatzes einen Zeilenumbruch zu erzeugen. Es eignet sich unter anderem für Gedichte, Adressen oder Texte, die zwar einen Absatz bilden, aber in mehrere Zeilen unterteilt werden müssen. <br /> sollte nicht als Ersatz für <p> zur Erstellung neuer Absätze verwendet werden.
🧠 Wichtige Konzepte zu Void Elements
Void Elements enthalten keinen Content und besitzen keinen separaten Closing-Tag. Üblicherweise werden sie mit einem Forward Slash geschrieben, zum Beispiel <hr /> oder <br />. Dabei ist darauf zu achten, dass ein Forward Slash (/) und kein Backslash (\) verwendet wird. In HTML5 ist es zwar erlaubt, <hr> oder <br> ohne Slash zu schreiben, die Verwendung von / wird jedoch empfohlen, da sie den Code für Menschen besser lesbar und verständlicher macht.

🎬 Project: Movie Ranking List
## Erforderliche HTML-Struktur für das Projekt
Dieses Projekt muss mindestens die folgenden HTML-Elemente enthalten:
<h1> zur Darstellung des Website-Titels als Hauptüberschrift,
<h2> für eine kurze Beschreibung oder einen Untertitel,
<hr /> als Trennlinie (Void Element) zur visuellen Abgrenzung von Inhalten,
<h3> zur Auflistung von mindestens drei Filmtiteln,
<p> zur Erklärung der Gründe, warum die jeweiligen Filme gefallen.
🛠️ Lernziele dieses Projekts
In diesem Projekt wird der Einsatz von Heading-Elementen (<h1>, <h2>, <h3>) zur strukturierten Gliederung von Inhalten geübt. Außerdem wird das Paragraph-Element (<p>) verwendet, um Inhalte verständlich zu beschreiben. Das Void Element <hr /> dient zur Trennung verschiedener Bereiche der Webseite. Ziel ist es, eine einfache HTML-Webseite von Grund auf zu erstellen sowie diese anschließend selbstständig zu bearbeiten und weiterzuentwickeln.


