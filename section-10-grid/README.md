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

✅ **Fazit**
- **Flexbox** verwenden für eindimensionale Anordnungen  
- **Grid** verwenden für tabellarische oder mehrdimensionale Layouts  
- Die Kombination beider Techniken ermöglicht flexible und professionelle Webseiten
