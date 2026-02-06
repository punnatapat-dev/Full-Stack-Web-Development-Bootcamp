## 📦 Section 11 Bootstrap Framework 

📌 **Was ist Bootstrap?**

Bootstrap ist ein **Open-Source CSS-Framework**,  
das im Jahr **2010 von Mark Otto und Jacob Thornton (Twitter-Team)** entwickelt wurde.  
Es wird verwendet, um Webseiten **schnell und effizient** mit vordefinierten CSS-Klassen  
und vorgefertigten UI-Komponenten zu erstellen.

📌 **Hauptmerkmale von Bootstrap**
- Vorgefertigte Komponenten (z. B. Button, Card, Navbar)
- 12-Spalten-Layout-System auf Basis von **Flexbox**
- Unterstützung für **Responsive Design** und das **Mobile-First-Prinzip**
- Einfache Nutzung durch Hinzufügen von Klassen im HTML
- Einheitliches, professionelles Design
- Unterstützung vieler Browser (Chrome, Safari, Brave usw.)

📌 **Wie funktioniert Bootstrap?**
- Einbindung von Bootstrap CSS über ein **CDN**
- Verwendung von Bootstrap-Klassen direkt im HTML
- Sofort ein ansprechendes UI, ohne alles selbst in CSS schreiben zu müssen

📌 **Vorteile**
- Schnelle Webentwicklung
- Reduzierter Design-Aufwand
- Viele sofort einsetzbare Komponenten
- Sehr gut geeignet für **responsive Webseiten**

📌 **Nachteile**
- **Class Bloat** (viele CSS-Klassen im HTML, schwerer lesbar)
- Tiefgehende Anpassungen sind schwieriger
- Weniger geeignet für Projekte mit sehr individuellem Design

📌 **Wann sollte man Bootstrap verwenden?**
✅ Responsive Webseiten  
✅ Wenn schnelle Entwicklung wichtig ist  
✅ Wenn ein standardisiertes, sauberes UI ausreicht  

❌ Sehr kleine Webseiten  
❌ Projekte, bei denen jedes Pixel manuell mit CSS kontrolliert werden muss  

📌 **CSS überschreiben (Override)**
- Eigenes CSS muss **nach Bootstrap** geladen werden
- Überschreiben ist möglich über:
  - internes CSS
  - externes CSS
  - Inline-Styles

📌 **Beispielhafte Verwendung**
- Einsatz der Bootstrap **Card-Komponente**
- Zentrierung mit Flexbox (`justify-content`, `align-items`, `height: 100vh`)
- Laden von Bootstrap über ein CDN

---

## 📦 Bootstrap Layout 
📌 **Grundidee**
Bootstrap verwendet ein **12-Spalten-Grid-System**,  
mit dem sich responsive Layouts einfach erstellen lassen,  
ohne eigenes CSS schreiben zu müssen.

📌 **Grundstruktur**
Das Bootstrap Grid besteht aus **drei Ebenen**:

<div class="container">
  <div class="row">
    <div class="col"></div>
  </div>
</div>

- `container` → umschließt das Layout (responsive)
- `row` → eine Zeile
- `col` → eine Spalte

📌 **Automatische Spalten**
- Wird nur `col` verwendet,
- verteilt Bootstrap den verfügbaren Platz **automatisch gleichmäßig**
- keine Zahlenangabe erforderlich

📌 **Feste Spalten (col-1 bis col-12)**
- Eine Row besteht aus **12 Spalten**
- Verhältnis wird über Klassen definiert

Beispiel:
<div class="col-2"></div>
<div class="col-4"></div>
<div class="col-6"></div>

- `col-6` = 50 %
- `col-4` = 4/12
- `col-2` = 2/12

📌 **Responsive Container**
- `container` → fester Rand links und rechts
- `container-fluid` → 100 % Breite auf allen Bildschirmgrößen
- `container-md / lg / xl` → Container wird erst ab bestimmten Breakpoints vollbreit

📌 **Bootstrap Breakpoints**
Bootstrap definiert feste Breakpoints:

| Breakpoint | Verwendung |
|-----------|-----------|
| xs | sehr kleine Bildschirme |
| sm | Smartphones |
| md | Tablets |
| lg | Laptops |
| xl | Desktop |
| xxl | sehr große Bildschirme |

📌 **Wichtig**
- Alle Breakpoints gelten nach dem Prinzip **„ab dieser Größe aufwärts (≥)“**

📌 **Responsive Spalten**
Spalten können je nach Breakpoint unterschiedlich definiert werden:

<div class="col-lg-4 col-md-8 col-sm-12"></div>

Bedeutung:
- Desktop → 4/12
- Tablet → 8/12
- Mobile → 12/12 (volle Breite)

📌 **Standardverhalten**
- Bei Bildschirmgrößen **kleiner als sm (<576px)**
- nehmen Columns automatisch **100 % der Breite** ein

📌 **Kombination aus festen und automatischen Spalten**
<div class="col-2"></div>
<div class="col-4"></div>
<div class="col"></div>

- `col` → nimmt den **verbleibenden Platz automatisch** ein

📌 **Vorteile des Grid-Systems**
- Kein eigenes CSS notwendig
- Keine Media Queries erforderlich
- Schnelle Umsetzung von Responsive Layouts
- Einheitliche Logik für alle Projekte

---

## 📦 Bootstrap Components

📌 **Was sind Bootstrap Components?**
Bootstrap Components sind **vorgefertigte UI-Bausteine**, die bereits gestaltet und gestylt sind,  
z. B. Buttons, Cards, Navbars, Carousels, Forms, Icons usw.  
Sie können **sofort verwendet** werden, indem man einfach Bootstrap-Klassen im HTML hinzufügt.

📌 **Button Component**
- Basisklasse: `btn`
- Farben werden über standardisierte Bootstrap-Farbnamen definiert

Beispiel:
`<button class="btn btn-success">Ok</button>`

Häufig verwendete Farben:
- `btn-primary` → Hauptaktion (Call to Action)
- `btn-success` → Erfolg / Bestätigung
- `btn-danger` → Kritische Aktion
- `btn-warning` → Warnung

📌 **Card Component**
- Wird verwendet, um Inhalte in **Boxen/Karten** darzustellen
- Struktur und Styling sind bereits vorhanden
- Inhalte wie Bilder, Texte und Buttons sind austauschbar

📌 **Nutzung**
- Code aus der offiziellen Dokumentation kopieren
- `src`, `alt` und Textinhalte anpassen

📌 **Navbar Component**
- Bootstrap Navbars sind **automatisch responsive**
- Auf kleinen Bildschirmen → **Hamburger-Menü**
- Für Dropdowns und Toggle-Funktionen ist **Bootstrap JavaScript** erforderlich

Erforderliches Script:
`<script src="bootstrap.bundle.min.js"></script>`

📌 **Bootstrap Icons (SVG)**
Bootstrap bietet **kostenlose Icons** an.

Zwei Nutzungsmöglichkeiten:
- SVG-Code direkt ins HTML kopieren
- Oder als Bild einbinden: `<img src="icon.svg">`

Geeignet für:
- Navbar-Brand
- Feature-Icons
- Buttons und Links

📌 **Bootstrap Examples & Snippets**
Bootstrap stellt eine **Examples-Seite** mit kompletten Layouts bereit.

Verwendbar für:
- Hero Sections
- Feature Sections
- Footer

→ Beschleunigt die Webentwicklung enorm, ohne bei Null anzufangen

📌 **Custom CSS mit Bootstrap**
- Bootstrap liefert das Grunddesign
- Eigenes CSS kann zur Feinabstimmung ergänzt werden
- Wichtig: **Eigenes CSS nach Bootstrap laden**

Beispiel:
`.feature-icon { background-color: #f8f9fa; border-radius: 0.75rem; }`

📌 **Carousel Component**
- Dient zur Anzeige von Bildern oder Inhalten als **Slideshow**
- Enthält:
  - Indicators
  - Navigationspfeile (links / rechts)
- Bilder müssen selbst eingebunden werden (`src`)

📌 **Layout-Tipp**
- Carousel am besten in einen `container` einbetten,
  um ein einheitliches Layout zu gewährleisten

📌 **Utility Classes (Abstände)**
Bootstrap bietet Utility-Klassen für Spacing:

Format:
`[property][side]-[size]`

Beispiele:
- `mt-3` → margin-top
- `mb-2` → margin-bottom
- `px-4` → padding links & rechts
- `my-5` → margin oben & unten

📌 **Größenbereich**
- `size` reicht von **0 bis 5**

📌 **Dark Mode**
Bootstrap unterstützt Dark Mode sehr einfach.

Aktivierung:
`<html data-bs-theme="dark">`

→ Das gesamte Design wechselt sofort in den Dark Mode  
→ Kann später mit JavaScript um einen Theme-Switch erweitert werden

📌 **Bootstrap Themes**
- Es gibt **kostenlose und kostenpflichtige Themes**
- Können als Basis-Template genutzt und weiter angepasst werden

Geeignet für:
- Startup-Websites
- Portfolios
- Blogs
- Business-Websites

