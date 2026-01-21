# 📘 Section 3: Intermediate HTML

---

## 🔑 HTML List Elements — Zentrale Punkte

- 📋 **HTML kennt zwei Arten von Listen**
  - 🔹 **`<ul>` (ungeordnete Liste)**  
    Wird verwendet, wenn die Reihenfolge nicht wichtig ist → Darstellung als Aufzählungspunkte
  - 🔹 **`<ol>` (geordnete Liste)**  
    Wird verwendet, wenn die Reihenfolge wichtig ist → automatische Nummerierung

- 🧩 **Listenelemente**
  - Jedes Element muss in einem **`<li>` (List Item)** stehen
  - **`<ul>`** und **`<ol>`** sind Container  
    → ohne `<li>` werden sie nicht dargestellt
  - Die Reihenfolge der `<li>`-Elemente in einer `<ol>` bestimmt die angezeigten Nummern

- 🌐 **Praxisbezug**
  - Listen werden häufig in echten Webseiten verwendet  
    (z. B. Aufzählungen, Rezepte, Ranglisten)
  - `<ul>` für ungeordnete Inhalte  
  - `<ol>` für Anleitungen oder Schritt-für-Schritt-Prozesse

---

## 🔑 HTML Nesting & Indentation — Zentrale Punkte

- 🔁 **Verschachtelung (Nesting)**
  - Listen können verschachtelt werden, indem `<ul>` oder `<ol>` **innerhalb eines `<li>`** platziert werden
  - Eine verschachtelte Liste muss immer Teil eines Listenelements sein
  - Das `<li>` wird **erst nach der verschachtelten Liste** geschlossen

- 🧱 **Kombination von Listentypen**
  - `<ul>` in `<ul>`
  - `<ul>` in `<ol>`
  - `<ol>` in `<ul>` oder `<ol>`

- 📐 **Indentation (Einrückung)**
  - Beeinflusst nicht die Funktion von HTML
  - Ist aber entscheidend für:
    - bessere Lesbarkeit
    - klares Verständnis der Struktur
    - einfacheres Debugging

- 🛠️ **VS Code**
  - Formatiert den Code automatisch beim Speichern
  - Hilft, typische Fehler zu erkennen:
    - fehlende schließende Tags
    - falsche Verschachtelung

---

## 🔑 HTML Anchor Elements & Attribute — Zentrale Punkte

- 🔗 **Anchor-Element (`<a>`)**
  - Wird verwendet, um Hyperlinks zu erstellen
  - Besteht aus:
    - Opening Tag `<a>`
    - Content (Link-Text)
    - Closing Tag `</a>`

- ⚙️ **Attribute**
  - Werden im Opening Tag geschrieben
  - Aufbau: `attributname="wert"`

- ⭐ **Wichtigstes Attribut: `href`**
  - Definiert die Ziel-URL
  - Ohne `href`:
    - Text sichtbar
    - Link nicht klickbar
  - Mit `href`:
    - Aktiver Hyperlink
    - Klick führt zur Zielseite

- 🌍 **Attribut-Typen**
  - elementspezifisch (z. B. `href`)
  - global (z. B. `draggable`)
  - Mehrere Attribute werden durch Leerzeichen getrennt

- 🔢 **Ordered List Spezial**
  - `<ol start="5">` legt die Startnummer der Liste fest

---

## 🖼️ HTML Image Element — Zentrale Inhalte

- 🖼️ **Einbindung von Bildern**
  - Bilder werden mit dem `<img>`-Element eingebunden
  - Syntax:
    ```html
    <img src="url" alt="beschreibung" />
    ```

- ⚠️ **Void Element**
  - Kein Closing-Tag
  - Selbstschließend

- 🔗 **Attribut `src`**
  - Definiert die Bildquelle (URL oder Pfad)

- ♿ **Attribut `alt` (Alternative Text)**
  - Beschreibt den Bildinhalt
  - Essenziell für Accessibility
  - Wird von Screenreadern vorgelesen

- 🧪 **Platzhalterbilder**
  - z. B. `https://picsum.photos/200`
  - Vergleichbar mit Lorem Ipsum für Text

- 🎞️ **Unterstützte Formate**
  - JPEG, PNG, GIF
  - GIFs werden automatisch animiert

- ✅ **Best Practice**
  - `alt` immer setzen, wenn das Bild inhaltlich relevant ist
  - Dekorative Bilder können ein leeres `alt=""` haben
 
    
🌍 **Live Demo:**  
    https://punnatapat-dev.github.io/Full-Stack-Web-Development-Bootcamp/section-03-intermediate-html/
