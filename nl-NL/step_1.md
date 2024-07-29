Je kunt extra variabelen maken in `default.css` om meer kleuren op te slaan.

**Tip:** Je wilt misschien een nieuwe achtergrondkleur **en** een nieuwe tekstkleur toevoegen.

--- code ---
---
language: html
filename: default.css
line_numbers: true
line_number_start: 4
line_highlights: 15-16
---

:root {
  --primary: #08586B;
  --onprimary:#4f4e4e;
  --secondary: #E0DB54;
  --onsecondary:#ffffff;
  --tertiary:#AF5C08;
  --ontertiary: #ffffff;
  --page:#ffffff;
  --onpage:#000000;
  --detail: #AB7C1C;
  --detail2: #38640D;
  --highlight: #DC9110;
  --onhighlight: #443C35;
}

--- /code ---

Je kunt een class maken in `style.css` die je nieuwe kleuren gebruikt.

--- code ---
---
language: html
filename: style.css
line_numbers: true
line_number_start: 8
line_highlights: 18-21
---

.secondary {
  background: var(--secondary);
  color: var(--onsecondary);
}

.tertiary {
  background: var(--tertiary);
  color: var(--ontertiary);
}

.highlight {
  background: var(--highlight);
  color: var(--onhighlight);
}

--- /code ---

Je nieuwe class kan dan op elk moment in je `index.html` bestand gebruikt worden, zodat een element je nieuwe kleur kan gebruiken.

--- code ---
---
language: html
filename: index.html
line_numbers: false
---

<section class="highlight">

--- /code ---
