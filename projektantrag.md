#Antrag für die betriebliche Projektarbeit

##1. Projektbezeichnung

Entwicklung eines unternehmensinternen Schichtplaners.

##2. Kurzform der Aufgabenerstellung

Für die eKomi Limited soll ein webbasierter Schichtplaner programmiert werden, 
welcher den Mitarbeitern einen schnellen und übersichtlichen Zugriff
auf ihre Schichten ermöglichen soll. Desweiteren soll es für die Teamleiter ein
intuitives Interface zum erstellen neuer Schichten geben.

##3. Zielsetzung entwickeln - Was soll am Ende des Projektes erreicht werden?

###3.1. Ist-Analyse

Es gibt im Moment einen Schichtplaner, der auch intern entwickelt wurde.
Allerdings weist dieser erhebliche Schwächen in der Benutzbarkeit und in der 
Übersichtlichkeit auf. 

Zum einen wird immer der gesamte Monat abgebildet, allerdings werden auf dem 
Bildschirm aus Platzgründen nur 2 Wochen angezeigt. Um die restlichen 2 Wochen zu 
sehen muss man nach rechts scrollen, wobei die Anzeige der Namen verschwindet.
Das macht es sehr umständlich die Schichten für einen speziellen Mitarbeiter in 
den letzten 2 Wochen eines Monats herauszufinden.

Ein weiteres Problem ist das immer 3 Monate untereinander angezeigt werden, man 
muss sowohl horizontal als auch vertikal scrollen um alle Informationen 
zu erfassen und es gibt keine Möglichkeit die Ansicht auf einen bestimmten 
Zeitrahmen festzulegen.

Desweiteren gibt es auch sonst keine Möglichkeit die Dargestellten Informationen
zu filter, sollte man z.B. nur die Mitarbeiter mit einer bestimmten Sprache betrachten
wollen, gäbe es keine Möglichkeit nur diese anzuzeigen.

###3.2. Was soll am Ende des Projektes erreicht sein?

Durch den neuen Schichtplaner soll mit AngularJS und Bootstrap ein übersichtliches und 
schneller Zugriff auf die Schichten erfolgen, dabei dient Rails im Backend als JSON-API.

###3.3 Welche Anforderungen müssen erfüllt sein

Folgende Anforderungen sollen von dem Schichtplaner erfüllt sein:

- übersichtliche Darstellung
- Einfache Erstellung und Aktualisierung neuer Schichten
- Anzeige der Schichten der kommenden und vergangen Wochen
- Filterung der Angezeigten Schichten

##4. Projektstrukturplan entwickeln

###4.1. Aufgaben auflisten

- Analyse
  * Durchführung einer Ist-Analyse
  * Durchführung einer Wirtschaftlichkeitsanalyse und Amortisationsrechnung Analyse
  * Ermittlung von Use-Cases
  * Erstellung eines Lastenheftes

- Entwürfe
  * Erstellung eines ER-Model
  * Entwurf der API
  * Markup für das Frontend
  * Erstellung eines Pflichtenheftes

- Implementierung
  * Implementierung der API
  * Erstellung des Designs
  * Integrierung der API in das Frontend

- Deployment
  * Aufsetzen des Servers
  * Einrichtung des Continuous Integration-Prozesses

- Dokumentation
  * Erstellung der Projektdokumentation

###4.2. Projektphasen mit Zeitplanung in Stunden

Zeitplanung |
--------|---------
**Analyse | 5h**
Ist-Analyse | 1h
Durchführung einer Wirtschaftlichkeitsanalyse und Amortisationsrechnung Analyse | 1h
Ermittlung von Use-Cases | 1h
Unterstützung des Fachbereichs bei der Erstellung des Lastenheftes | 2h
**Entwurf** | **10h**
Erstellung eines ER-Model | 2h
Entwurf der API | 2h
Markup für das Frontend | 2h
Erstellung eines Pflichtenheftes | 4h
**Implementierung** | **35h**
Implementierung der API | 7h
Erstellung des Designs | 5h
Integrierung der API in das Frontend | 22h
**Deployment** | **10h**
Aufsetzen des Server | 2h
Einrichtung des Coninuous Integration-Prozesses | 8h
**Erstellen der Dokumentation** | **10h**
Erstellen der Projektdokumentation | 10h


##5. Name der Ausbildungsstätte in dem das Projekt durchgeführt wird

eKomi Limited

###5.1 Name des Ausbilders

Achim Galeski