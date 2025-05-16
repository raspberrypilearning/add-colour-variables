你可以在 `default.css` 中创建更多变量来存储更多颜色。

**提示：** 你可能想要添加一个新的背景颜色 **和** 一个新的文本颜色。

## --- code ---

language: html
filename: default.css
line_numbers: true
line_number_start: 4
line_highlights: 15-16
-----------------------------------------------------------

:root {
\--primary: #08586B;
\--onprimary:#4f4e4e;
\--secondary: #E0DB54;
\--onsecondary:#ffffff;
\--tertiary:#AF5C08;
\--ontertiary: #ffffff;
\--page:#ffffff;
\--onpage:#000000;
\--detail: #AB7C1C;
\--detail2: #38640D;
\--highlight: #DC9110;
\--onhighlight: #443C35;
}

\--- /code ---

你可以在 `style.css` 中创建一个使用新颜色的类。

## --- code ---

language: html
filename: style.css
line_numbers: true
line_number_start: 8
line_highlights: 18-21
-----------------------------------------------------------

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

\--- /code ---

然后，你随时可以在你的 `index.html` 文件中使用新类，以便元素可以使用你新配对颜色。

## --- code ---

language: html
filename: index.html
line_numbers: false
--------------------------------------------------------

<section class="highlight">

\--- /code ---
