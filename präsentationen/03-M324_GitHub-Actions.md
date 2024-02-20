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

# GitHub Actions

---

# Komponenten von GitHub Actions

1. Workflows
1. Events
1. Jobs
1. Steps
1. Actions
1. Runners

![bg right](https://res.cloudinary.com/luggs/image/upload/v1708436541/Informatik/Modul%20324/GitHub-Actions.png)

---

# 1. Workflows

Ein Workflow: 

- ... ist eine automatische Prozedur, die einem Repository hinzugefügt werden kann
- ... besteht aus einem oder mehreren Jobs, die entweder zeit- oder ereignisgesteuert gestartet werden
- ... kann verwendet werden um Software zu bauen (BUILD), zu testen (TEST), zu realisieren (RELEASE) und produktiv zu setzen (DEPLOY)
- ... wird in .github/workflows als .yml Datei gespeichert

---

# 2. Events

- Ein Event löst einen Workflow aus, durch Commits, einem Issue oder einem Pull Request
- Ein Event kann auch durch ein externes Ereignis ausgelöst werden

---

# 3. Jobs

- Einzelne Schritte innerhalb desselben Runners
- Jobs können parallel oder sequenziell durchlaufen werden. Sequenziell macht Sinn, wenn zuerst getestet wird und er danach released

---

# 4. Steps

- Ein Step ist eine individuelle Aufgabe innerhalb eines Jobs
- Ein Step kann eine Action oder ein Shell Kommando sein
- Steps laufen unter dem selben Runner, d.h. es können Daten ausgetauscht werden

---

# 5. Actions

- Actions sind die kleinste Einheit in einem Workflow
- Actions können selber erstellt werden oder es können bereits vorhandene Actions ausgewählt werden

---

# 6. Runner

- Ein Runner ist ein Server, wo die GitHub Action ausgeführt wird
- Ein Runner kann selber oder bei GitHub gehostet werden