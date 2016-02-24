#Antrag für die betriebliche Projektarbeit

##1. Projektbezeichnung

Entwicklung eines unternehmensinternen Schichtplaners.

###1.1. Kurzform der Aufgabenerstellung

Für die eKomi Limited soll ein webbasierter Schichtplaner programmiert werden, 
welcher den Mitarbeitern einen schnellen und übersichtlichen Zugriff
auf ihre Schichten ermöglichen soll. Desweiteren soll es für die Teamleiter ein
intuitives Interface zum erstellen neuer Schichten geben.

###1.2. Ist-Analyse

Es gibt im Moment einen Schichtplaner, der auch intern entwickelt wurde.
Allerdings weist dieser erhebliche Schwächen in der Benutzbarkeit und in der 
Übersichtlichkeit auf. 

Zum einen wird immer der gesamte Monat abgebildet, allerdings werden auf dem 
Bildschirm aus Platzgründen nur 2 Wochen angezeigt. Um die restlichen 2 Wochen zu 
sehen muss man nach rechts scrollen, wobei die Anzeige der Namen verschwindet.
Das macht es sehr umständlich die Schichten für einen speziellen Mitarbeiter in 
den letzten 2 Wochen eines Monats herauszufinden.

Ein weiteres Problem ist das immer 3 Monate untereinander angezeigt werden, man 
muss also sowohl horizontal als auch vertikal scrollen um alle Informationen 
zu erfassen und es gibt keine Möglichkeit die Ansicht auf einen bestimmten 
Zeitrahmen festzulegen.

Desweiteren gibt es auch sonst keine Möglichkeit die Dargestellten Informationen
zu filter, sollte man z.B. nur die Mitarbeiter mit einer bestimmten Sprache betrachten
wollen, gäbe es keine Möglichkeit nur diese anzuzeigen.

##2. Zielsetzung entwickeln / Soll-Konzept

###2.1. Was soll am Ende des Projektes erreicht sein?

Durch den neuen Schichtplaner soll mit AngularJS und Bootstrap ein übersichtliches und 
schneller Zugriff auf die Schichten erfolgen, dabei dient Rails im Backend als JSON-API.

###2.2 Welche Anforderungen müssen erfüllt sein

Folgende Anforderungen sollen von dem Schichtplaner erfüllt sein:

- übersichtliche Darstellung
- Einfache Erstellung und Aktualisierung neuer Schichten
- Anzeige der Schichten der kommenden und vergangen Wochen
- Filterung der Angezeigten Schichten

##3. Projektstrukturplan entwickeln

###3.1. Was ist zur Erfüllung der Zielsetzung erforderlich?

Das Projekt soll agil Entwickelt werden. Kurze Iterationszyklen erlauben häufige Rücksprache mit den Auftraggegebern, was wiederum erlaubt früh auf Änderungswünsche einzugehen. Das gesamte Projekt wird mithilfe von Git versioniert und die einzelnen Aufgaben werden in einem Ticketsystem dokumentiert.

###3.2. Aufgaben auflisten

- Analyse
  * Durchführung einer Ist-Analyse
  * Durchführung einer Wirtschaftlichkeitsanalyse und Amortisationsrechnung Analyse
  * Ermittlung von Use-Cases
  * Erstellung eines Lastenheftes

- Entwurfe
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

-Dokumentation
  * Erstellung der Projektdokumentation

##4. Projektphasen mit Zeitplanung in Stunden

Analyse | 4h
--------|---------
Ist-Analyse | 1h
Durchführung einer Wirtschaftlichkeitsanalyse und Amortisationsrechnung Analyse | 1h
Ermittlung von Use-Cases | 0,5h
Unterstützung des Fachbereichs bei der Erstellung des Lastenheftes | 1,5h
**Entwurf** | **6h**
Erstellung eines ER-Model | 1h
Entwurf der API | 1h
Markup für das Frontend | 1h
Erstellung eines Pflichtenheftes | 3h
**Implementierung** | **52h**
Implementierung der API | 7h
Erstellung des Designs | 5h
Integrierung der API in das Frontend | 30h
**Deployment** | **8h**
Aufsetzen des Server | 1h
Einrichtung des Coninuous Integration-Prozesses | 7h
**Erstellen der Dokumentation** | **10h**
Erstellen der Projektdokumentation | 10h


##5. Name der Ausbildungsstätte in dem das Projekt durchgeführt wird

eKomi Limited

###5.1 Name des Ausbilders

Achim Galeski