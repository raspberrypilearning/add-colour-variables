Tu peux créer des variables supplémentaires dans `default.css` pour stocker plus de couleurs.

**Astuce :** tu peux ajouter une nouvelle couleur d'arrière-plan **et** une nouvelle couleur de texte à utiliser avec elle.

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

Tu peux créer une classe dans `style.css` qui utilise tes nouvelles couleurs.

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

Ta nouvelle classe peut ensuite être utilisée dans ton fichier `index.html` à tout moment pour qu'un élément puisse utiliser ta nouvelle association de couleurs.

--- code ---
---
language: html
filename: index.html
line_numbers: false
---

<section class="highlight">

--- /code ---
