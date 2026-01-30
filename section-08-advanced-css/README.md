# 📘 Abschnitt 8: Advanced CSS & Responsive Design

## 📌 CSS Display Property 
Die CSS-Eigenschaft `display` bestimmt das Anzeigeverhalten und das Layout von Elementen auf einer Webseite.

Die wichtigsten und am häufigsten verwendeten Werte sind:

1. display: block  
- Nimmt die gesamte Breite einer Zeile ein  
- Das nächste Element beginnt in einer neuen Zeile  
- `width` und `height` können definiert werden  
- Beispiele: p, div, h1  

2. display: inline  
- Elemente werden in derselben Zeile angezeigt  
- Breite und Höhe können nicht definiert werden  
- Die Größe richtet sich nach dem Inhalt  
- Beispiele: span, a  

3. display: inline-block  
- Breite und Höhe können definiert werden  
- Elemente können nebeneinander stehen  
- Häufig verwendet für boxbasierte Layouts  

4. display: none  
- Das Element wird vollständig ausgeblendet  
- Es belegt keinen Platz im Layout  
- Wird zum Ein- und Ausblenden von Elementen verwendet  

Key Takeaways  
- block → vertikal, volle Zeile  
- inline → horizontal, nicht skalierbar  
- inline-block → skalierbar und horizontal  
- Durch Ändern von `display` lassen sich Layouts stark beeinflussen  

---

## 📌 CSS Float & Clear 

Die Eigenschaft `float` wird verwendet, um Text um andere Elemente (z. B. Bilder) fließen zu lassen.  
Sie wird häufig bei der Kombination von Bildern und Text eingesetzt, ähnlich wie im Zeitungsdesign.

Ergebnis von float  
- Bilder werden nach links oder rechts verschoben  
- Text umfließt das Bild  
- Das gefloatete Element verlässt den normalen Dokumentenfluss  

Häufig verwendete Werte  
- float: left  
- float: right  

Typische Probleme  
- Andere Elemente (z. B. Footer) können unbeabsichtigt nach oben gezogen werden  

Die Eigenschaft `clear` hebt die Wirkung von float auf  
Verwendete Werte  
- clear: left  
- clear: right  
- clear: both (am häufigsten verwendet)  

Key Takeaways  
- float eignet sich für Textumfluss um Bilder  
- clear ist notwendig, um Layout-Probleme zu vermeiden  
- float ist nicht für komplexe Layouts empfohlen  
- Moderne Layouts sollten mit Flexbox oder Grid umgesetzt werden  

---

## 📱 Responsive Web Design 

Responsive Web Design bedeutet, dass sich das Layout einer Website automatisch an verschiedene Bildschirmgrößen anpasst.  
So wird eine optimale Nutzung auf Desktop-, Tablet- und Mobilgeräten gewährleistet.

---

## 🔧 Methoden zur Erstellung responsiver Websites

1. Media Queries  
Ermöglichen es, CSS abhängig von Bildschirmgrößen (Breakpoints) anzuwenden.  
Ideal für den Einstieg und präzise Layout-Kontrolle.

2. CSS Grid  
Ein zweidimensionales Layout-System mit Zeilen und Spalten.  
Geeignet für komplexe Layouts wie Dashboards oder Kartenstrukturen.

3. CSS Flexbox  
Ein eindimensionales Layout-System (horizontal oder vertikal).  
Reagiert flexibel auf unterschiedliche Bildschirmgrößen durch Verhältniswerte.

4. Bootstrap Framework  
Ein externes Framework auf Basis von Flexbox.  
Verwendet ein 12-Spalten-System und bietet sofort responsive Komponenten.

Key Takeaways  
- Es gibt keine „beste“ Methode – alle sind Werkzeuge  
- Media Queries → Breakpoints steuern  
- Grid → komplexe 2D-Layouts  
- Flexbox → flexible 1D-Layouts  
- Bootstrap → schnell und einsatzbereit  

---

## 📐 Media Queries 

Media Queries ermöglichen es, CSS-Regeln abhängig von der Bildschirmgröße anzuwenden.

- max-width → für kleine Bildschirme (Mobile)  
- min-width → für große Bildschirme (Desktop)  

Typische Breakpoints  
- Mobile: ≤ 480px  
- Tablet: 481px – 1200px  
- Laptop: 1201px – 1600px  
- Desktop: ≥ 1601px  

Key Takeaways  
- Media Queries sind die Grundlage für Responsive Design  
- max-width für mobile Geräte  
- min-width für große Bildschirme  
- Kombinationen ermöglichen gezielte Layout-Steuerung  

---

## 🎨 Abschnittsprojekt – Responsive Web Design Agentur

Ziel des Projekts  
- Erstellung einer Web- oder Creative-Design-Agentur-Website  
- Schlichtes, sauberes und professionelles Design  
- Vollständig responsive auf allen Geräten  

Struktur der Website  
- Header mit Agenturname (Farbhervorhebung einzelner Wörter per span)  
- Zwei Content-Karten mit Bild und Text  
- Footer mit einem Motto  

Responsives Verhalten  
- Große Bildschirme → Karten nebeneinander  
- Kleine Bildschirme → Karten untereinander gestapelt  

Verwendete CSS-Techniken  
- display, float, clear  
- Media Queries  
- width: 100% auf mobilen Geräten  
- text-align: justify  
- object-fit für Bilder  

Key Takeaways  
- Responsive Design ist essenziell für moderne Websites  
- Das Layout muss nicht exakt der Musterlösung entsprechen  
- Entscheidend sind ein sauberes Layout und gute Responsivität  

---

## 🌍 Live Demo
https://punnatapat-dev.github.io/Full-Stack-Web-Development-Bootcamp/
