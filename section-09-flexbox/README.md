## 📘 Day 9📦 CSS Flexbox

✅ **Flexbox** ist ein modernes Layout-System in CSS, das entwickelt wurde, um flexible, übersichtliche und responsive Webseiten-Strukturen zu erstellen.  
Durch das Setzen des Containers auf `display: flex;` werden alle enthaltenen Elemente standardmäßig horizontal angeordnet.

🔧 **Wichtige Eigenschaften von Flexbox**
- 🎯 Einfache Kontrolle über das Layout ohne komplizierte Hacks
- 🚫 Frühere `display`-Werte der Kindelemente (`block` / `inline`) werden ignoriert
- 📐 Die Breite der Elemente richtet sich automatisch nach dem Inhalt
- 📏 Abstände zwischen Elementen können bequem mit `gap` definiert werden

🧩 **Zwei Varianten des Flex-Containers**
- `flex` → nimmt die volle Breite ein
- `inline-flex` → nimmt nur so viel Platz ein wie nötig

🧪 **Praxisübung**
Eine Liste (`list items`) wird mithilfe von Flexbox in eine Navigationsleiste umgewandelt.  
Dafür reichen bereits folgende CSS-Eigenschaften aus:

```css
display: flex;
gap: 1rem;
