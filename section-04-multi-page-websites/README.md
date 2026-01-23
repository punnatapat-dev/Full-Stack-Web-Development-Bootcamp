# 📘 Section 4: Multi-Page Websites

---

🔗 Multi-Page Websites  
• 🌐 Eine Multi-Page Website besteht aus mehreren HTML-Dateien  
• 📂 Jede Seite ist eine eigene Datei (z. B. "index.html", "about.html", "contact.html")

---

🧭 Navigation zwischen Seiten  
- Seiten werden mit dem Anchor-Element <a> verlinkt  
- Das Attribut "href" verweist auf eine andere HTML-Datei  
- Meist werden Relative File Paths verwendet  

Beispiel:  
<a href="./about.html">Über uns</a>

---

📁 Ordnerstruktur  
- Eine saubere Ordnerstruktur ist entscheidend  
- HTML-Dateien können im gleichen Ordner oder in Unterordnern liegen  
- Der File Path muss immer relativ zur aktuellen Datei stimmen  

---

🔁 Relative File Paths zwischen Seiten  
- "./seite.html" → Datei im gleichen Ordner  
- "../seite.html" → Datei eine Ebene höher  
- "./ordner/seite.html" → Datei in einem Unterordner  

---

🛠️ Best Practices  
- Einheitliche Navigation auf allen Seiten verwenden  
- Relative Paths statt Absolute Paths nutzen  
- Dateinamen klein und konsistent halten (z. B. "about.html")  
- Navigation nach jeder Änderung testen  

---

🌐 Was ist eine Multi-Page Website?  
- Eine Website besteht aus mehreren HTML-Dateien  
- Jede Seite ist eine eigene Datei (z. B. "index.html", "about.html", "contact.html")  
- Alle Seiten liegen im gleichen Projektordner  

---

🔗 Navigation zwischen Seiten  
- Seiten werden mit dem Anchor-Element <a> verlinkt  
- Das Attribut "href" verweist auf eine andere HTML-Datei  
- Nutzer wechseln Seiten durch Klicken auf Links oder Bilder  

Beispiel:  
<a href="./about.html">About</a>

---

📁 Ordner- & Dateistruktur  
- "index.html" ist die Startseite (Home)  
- Weitere Seiten liegen oft in einem Unterordner (z. B. "public")  
- Assets (Bilder) liegen meist in "assets/images"  

---

🧭 Relative File Paths (entscheidend)  
- "./datei.html" → Datei im gleichen Ordner  
- "./public/contact.html" → Datei im Unterordner  
- "../" → eine Ordner-Ebene nach oben  
- Relative Paths sind Standard im Web Development  

---

🖼️ Bild als Link  
- Ein Bild kann in ein <a>-Element eingebettet werden  
- Klick auf das Bild führt zu einer anderen Seite  

Beispiel:  
<a href="./contact.html">
  <img src="./assets/picme.png" alt="Profilbild" width="200">
</a>


---

🛠️ Best Practices  
- Relative Paths statt Absolute Paths verwenden  
- Einheitliche Navigation auf allen Seiten  
- Ordnerstruktur sauber und logisch halten  
- Links und Bilder nach jeder Änderung testen  

---

📄 Was ist ein HTML Boilerplate?  
- Der HTML Boilerplate ist die Grundstruktur jeder HTML-Datei  
- Er ist der Startpunkt für jede Webseite  
- Definiert Aufbau, Sprache und wichtige Meta-Informationen  

---

📌 Doctype Declaration  
- <!DOCTYPE html>  
- Gibt dem Browser an, dass HTML5 verwendet wird  
- Muss immer ganz oben im Dokument stehen  

---

🌍 Das <html>-Element  
- Root-Element des Dokuments  
- Enthält den gesamten Code der Webseite  
- Attribut lang definiert die Sprache (z. B. lang="en" oder lang="de")  
- Wichtig für Screenreader & Accessibility  

---

🧠 Das <head>-Element  
- Enthält Metadaten (nicht sichtbar für Nutzer)  
- Wichtige Inhalte:  
  - <meta charset="UTF-8"> → korrekte Zeichendarstellung (inkl. Emojis)  
  - <title> → Titel im Browser-Tab  
- Keine sichtbaren Inhalte wie Text oder Bilder  

---

👁️ Das <body>-Element  
- Enthält den gesamten sichtbaren Inhalt der Webseite  
- Hier kommen:  
  - Überschriften  
  - Texte  
  - Bilder  
  - Links  
  - Listen  

---

🧩 Nesting & Indentation  
- HTML-Elemente werden ineinander verschachtelt (nested)  
- Saubere Einrückung macht die Struktur sofort verständlich  
- Erleichtert Lesen des Codes, Fehlersuche (Debugging) und Wartung  

---

⚡ VS Code Shortcut  
- In einer .html-Datei:  
  - ! + Enter  
- VS Code erzeugt automatisch den kompletten HTML Boilerplate  
- Spart Zeit bei neuen Dateien  

---

🛠️ Zusätzliche Meta-Tags  
- viewport → wichtig für responsive Darstellung  
- X-UA-Compatible → veraltet (Internet Explorer), kann entfernt werden  

---

