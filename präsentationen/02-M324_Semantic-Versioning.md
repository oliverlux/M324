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

# Semantic Versioning

---

# Was ist Semantic Versioning

- Sie haben sicher bereits Versionsnummern von Software gesehen, welche drei Komponenten haben im Schema n.m.k, also beispielsweise 4.0.2
- Diese nennt man semantische Versionierung, und in diesem Schema haben die einzelnen Ziffern n, m und k eine spezielle Bedeutung.
- Um dieser Bedeutung auf den Grund zu gehen, müssen wir ganz wenig ausholen…


---

# Warum Semantic Versioning

- Sie stellen eine API öffentlich zur Verfügung und implementieren eine neue Funktionalität. Diese Änderung hat aber einen Einfluss auf bestehende Nutzer, d.h. diejenigen müssen eine Änderung vornehmen.
- Wie können Sie Code markieren, dass alle wissen, ob sie ihren Code ändern müssen oder nicht, wenn eine neue Version herauskommt?
- Semantic Versioning!

---

# Funktionsweise Semantic Versioning

Versionsnummer hat folgendes Format: `MAJOR.MINOR.PATCH`

- `MAJOR:` Mit vorherigen Versionen inkompatible API-Änderungen (Signaturen ändern) - 0.y.z ist für die erste Entwicklung, wo sich noch alles, auch die API ändern kann.
- `MINOR:` Weitere, rückwärtskompatible API-Funktionen hinzugefügt (Signaturen ändern nicht)
- `PATCH:` Rückwärtskompatible bug-Behebungen (= eine Änderung im Code, welche falsches Verhalten behebt)

