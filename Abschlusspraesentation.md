---
theme: "Night"
transition: "convex"
backgroundTransition: "fade"
highlightTheme: 'dracula'
slideNumber: true
controlsLayout: "edges"
center: true
---

<!-- styling -->
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.0.13/css/all.css" integrity="sha384-DNOHZ68U8hZfKXOrtjWvjxusGo9WQnrNx2sqG0tfsghAvtVlRW3tvkXWZh58N9jp" crossorigin="anonymous">
<style>
html.back .slide-background.present {
	opacity: 0.7 !important;
    background-color: white;
}
html.img .reveal img {
    height: 500px;
    width: 500px;
}
</style>
<!-- /styling -->

### Entwicklung einer internetbasierten Liferantenplattform für Qualitätsdaten 

<small>Nils Nieuwenhuis</small>

<small>Flender GmbH</small>

note: Man was ein Scheiss.

---

### Agenda <i class="far fa-calendar-alt"></i>
- Unternehmen
- Projektumfeld
    - Management
    - Planung
- Schnittstellenanalyse
- Applikationsaufbau
- Umsetzung
- Demo
---

<!-- .slide: data-background="Produktionsstandorte_BigPic.jpg" data-state="back" -->
## Unternehmen
--
- Tochter der Siemens AG
- Getriebe und Kupplungen
- Hauptsitz Bocholt
- Produktionsstandorte: Frankreich, USA, Indien, China
--

### IT Abteilung <i class="fas fa-laptop"></i>
- berät internen Kunden
- SCM, PLM, CRM
- 80 Mitarbeiter
--

### Qualitätsabteilung <i class="fas fa-clipboard-check"></i>
- Sicherung Produkt- und Prozessqualität
- Wirtschaftlichkeit, Gesetzgebung, Umwelt, Forderungen
- Qualitätsplanung, Qualitätslenkung, Qualitätsprüfung, Qualitätsverbesserung
---

<!-- .slide: data-background="projekt.jpg" -->
---

<!-- .slide: data-background="management.jpg" data-state="back" -->

### Management
--

### Team <i class="fas fa-users"></i>
- 10 Mitarbeiter
- Projektleiter Qualitätsabteilung
- Scrum Master IT
- 3 Entwickler
- 5 Mitarbeiter aus Fachabteilungen
--

### Organisation <i class="fas fa-toolbox"></i>
- OpenProject
- Scrum (Umsetzung)
- Git
- E-Mail, Circuit
- **Servoy**
--

### Servoy
- Rapid Application Development
- Javabasiert
- Programmcode in Javascript
- Eigene IDE Servoy-Developper (Eclipse-Addon)
- Deployment auf Applikationsserver
--

### Zielsetzung <i class="fas fa-bullseye"></i>
- Neue Internetschnittstelle
- Qualitätsprüfungen (Maßprotokolle)
- Erfassungsmaske für externe Lieferanten
- Prüfung der Eingaben
- Speicherung Qualitätsdatenbank
- Qualitätszeugniss (PDF)
- **Prototyp** => manuelle Eingabe + Übertragung
---

<!-- .slide: data-background="planung.png" data-state="back" -->
### Planung
--

### Ablauf <i class="fas fa-clock"></i>
![Ablauf](ablauf.png)
--

### Vorgehensweise <i class="fas fa-list-ol"></i>
- Schnittstellenanalyse + Applikationsaufbau => vergleichbar Wasserfall
- Warum? => Scrum erwartet fertiges Produkt
- Umsetzung => Scrum
- UserStories > ProductBacklog > Storypoints > Sprint Planning > Sprint (14d) > Sprint Review Meeting > <i class="fas fa-redo"></i>
--

### Status vor Beginn <i class="fas fa-history"></i>
![Ablauf alt](status_alt.png)
---

<!-- .slide: data-background="analyse.jpg" data-state="back" -->
## Schnittstellenanalyse
--

### Ist
- Stammdatenübertragung Produktivsystem
- im Testsystem + PLM benötigt => Druck prüfen
- händische Übertragung
- Klassifizierung nötig SAP
- nicht komplett ausgerollt
- lange Antwortzeiten
- keine komplette Teilidentifikation
- gute Plausiprüfung
--

### Soll
- mehrsprachig
- Arbeitsvorrat anzeigen
- Vorgaben ersichtlich
- Plausiprüfung bei Eingabe
- Uploaddatei + Anzeige der Daten
- Anhänge
- Prüfprotokoll wenn gültig und geprüft
--

### Ergebnis
![Anwendungsfalldiagramm](Anwendungsfalldiagramm.png)
--

![Anwendungsfallbeispiel](Anwendungsfallbeispiel.png)
---

<!-- .slide: data-background="Applikationsaufbau.jpg" data-state="back" -->
## Applikationsaufbau 
--

### Systemübersicht <i class="fas fa-server"></i>
![Systemübersicht](Systemuebersicht.png) <!-- .element: style="Background-color:white" -->
--

### Forschungsarbeit <i class="fas fa-vial"></i>
- Plattformen für Webapplikationen der Flender GmbH
- Kriterien: Betreuung, Funktionen, Sicherheit, Performance
- Plattformen: Server-VM, Cloudplattform
- Empfehlung AWS
--

### Datenbankmodell <i class="fas fa-database"></i>
![Datenmodell1](Datenmodell1.png) <!-- .element: style="height:500px"-->
--

![Datenmodell2](Datenmodell2.png) <!-- .element: style="height:500px"-->
--

### Mockupbeispiel
![Prüfdatenerfassung](MockupPruefdatenerfassung.png)
---

<!-- .slide: data-background="Umsetzung.jpg" data-state="back" -->
## Umsetzung
--

### Business Logic <i class="fas fa-code"></i>
![Klassendiagramm](Klassendiagramm.png) <!-- .element: style="Background-color:white;height:500px" -->
---

<!-- .slide: data-background="Demo.jpg" data-state="back" -->
## Demo
---

#### Quellen
<small>
- Präsentationstool: [reveal.js](https://revealjs.com)
- Icons: [Font Awesome](www.fontawesome.com)

**Hintergrundbilder**
- Projektbild: https://www.youtube.com/watch?v=FzWU1A_N-a0
- Managementbild: https://www.saba.com/blog/is-your-people-management-strategy-people-focused
- Planungsbild: http://www.schwarzkopf-professional.de/skp/de/de/home/ausbildung/ask/business/0614/jeder-saloninhaber-benotigt-einen-geschaftsplan.html?desktop=true
- Analysebild: https://www.cms-webprojekte.de/beratung/ist-analyse/
-Applikationsaufbaubild: https://www.perm4.com/karriere-im-bereich-it-telekommunikation/
- Umsetzungsbild: https://www.perm4.com/brands-mandanten/personalberatung-ittk/
<small>- Demobild: http://blog.servoy.com/page/3/
</small>
