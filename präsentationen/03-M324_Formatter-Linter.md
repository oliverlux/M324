---
marp: false
theme: gaia
paginate: true
_class: lead

backgroundImage: url('https://res.cloudinary.com/luggs/image/upload/v1634832661/GBS/bg1.png')
---

<!-- _backgroundImage: url('https://res.cloudinary.com/luggs/image/upload/v1622877578/GBS/gbs.jpg') 
_color: black;

_footer: ""
_paginate: false
-->

<style scoped>
h1 {
    background-color: #222;
    margin: 0;
    padding: 0 10px 0 20px;
    font-weight: 800;
    transform: rotate(-5deg);
    color: #fff;
    text-align: left;
}

h1::after {
    font-family: Arial, Helvetica, sans-serif;
    bottom: 0;
    color: #CCCC00;
    content: '.';
    position: absolute;
    margin-left: 25px;
    transform: translate(-100%, 0);
}

h3 {
    background-color: #222;
    margin: 0;
    padding: 0 10px 0 20px;
    font-weight: 400;
    transform: rotate(-5deg);
    color: #fff;
    text-align: left;
    width: 200px;
}

a {
    color: #fff;
    text-decoration: none;
}


</style>

### M324

# Code - Qualität

---

# Formatter und Linter

- Tools zur Hilfe bei der Entwicklung im Team
- Gemeinsame Standards mit möglichst wenig Aufwand
- Ziel: Einheitlicher Code innerhalb Team oder Projekt


---

# Formatter

- Ein Formatter ist ein Tool, das Quellcode automatisch formatiert.
- Es passt Einrückungen, Leerzeichen, Zeilenumbrüche und andere Formatierungen an.
- Das Ziel ist es, ein konsistentes Layout und einen einheitlichen Stil im Code zu gewährleisten.
- Formatter verbessern die Codelesbarkeit und -wartbarkeit.
- Sie helfen dabei, den Code gemäss den formatierungsspezifischen Konventionen anzupassen.
- Formattierungseinstellungen sind oft anpassbar, um den Anforderungen des Projekts oder Teams gerecht zu werden.


---

# Linter

- Ein Linter ist ein statisches Code-Analyse-Tool.
- Es prüft den Quellcode auf potenzielle Fehler, Stilprobleme und Codierungsstandards.
- Linter helfen dabei, Fehler frühzeitig zu erkennen.
- Sie verbessern den Codequalitätsstandard.
- Linter stellen sicher, dass der Code den definierten Richtlinien entspricht.
- Sie unterstützen die Einhaltung von Best Practices und Coding-Standards.

---

# Bekannteste Tools

- Prettier (https://prettier.io/)
- ESlint (https://eslint.org/), TSlint, SonarQube

---

# Spannende Neuentwicklung

Biome (https://biomejs.dev/)