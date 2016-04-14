# IHK Projektdokumentation

### Inhaltsverzeichnis

### 1 Einleitung

#####1.1. Projektbeschreibung
#####1.2. Projektumfeld
#####1.3. Projektziel
#####1.4. Projektbegründung

### 2 Projektplanung

##### 2.1 Projektphasen
##### 2.2 Ressourcenplanung
##### 2.3 Entwicklungsprozess

### 3 Analysephase

##### 3.1 Ist-Analyse
##### 3.2 Wirtschaftlichkeitsanalyse
##### 3.2.1 "Make or Buy"-Entscheidung
##### 3.2.2 Projektkosten
##### 3.2.3 Amortisationsdauer
##### 3.3 Anwendungsfälle
##### 3.4 Lastenheft / Fachkonzept

### 4 Entwurfsphase

##### 4.1 Zielplattform
##### 4.2 Architekturdesign
##### 4.3 Entwurf der Benutzeroberfläche
##### 4.4 Datenmodell
##### 4.5 Geschäftslogik
##### 4.6 Pflichtenheft

### 5 Implementierungsphase

##### 5.1 Iterationsplanung
##### 5.2 Implementierung der Datenstrukturen
##### 5.3 Implementierung der Geschäftslogik
##### 5.4 Implementierung der Benutzeroberfläche

### 6 Abnahme- und Einführungsphase

##### 6.1 Abnahme durch den Fachbereich
##### 6.2 Deployment und Einführung

### 7 Dokumentation

### 8 Fazit

##### 8.1 Soll-/Ist-Vergleich
##### 8.2 Lessons Learned
##### 8.3 Ausblick

## 1 Einleitung

Diese Projektdokumentation beschreibt den Ablauf des IHK-Abschlussprojektes, die der Autor
während seiner Ausbildung zum Fachinformatiker - Anwendungsentwicklung abgeschlossen hat.

Durchgeführt wurde die Ausbildung bei der Firma eKomi Limited in Berlin. Das Internet-Startup wurde
2008 gegründet und beschäftigt im Moment ca. 300 Mitarbeiter.

Das Produkt ist es für Unternehmen unabhängige transaktionsbasierte Bewertungen zu sammeln.
Zu unsere Kunden zählen größtenteils Onlineshop, allerdings auch Banken und Versicherungen.
Durch die unabhängig gesammelten Bewertungen, soll bei Neukunden Vertrauen für den Onlineshop geweckt werden.

####1.1 Projektbeschreibung

Bei eKomi haben die einzelnen Abteilungen in der Regel zwischen 10 und 25 Mitarbeiter.
Die meisten Mitarbeiter haben eine feste Arbeitszeit um unseren Kunden den Support zu garantieren.
Aus diesem Grund wird jedem Mitarbeiter von dem zuständigen Teamlead eine feste Schicht zugeordnet.
Innerhalb einer Abteilung gibt es Mitarbeiter mit vielen unterschiedlichen Sprachen, die basierend auf der Sprache bestimmte Schichten belegen müssen.
Desweiteren muss der Schichtplaner anzeigen, wenn ein Mitarbeiter im Urlaub oder Krank ist.

####1.2 Projektumfeld

Grundsätzlich wird der Schichtplanner natürlich nur von Leuten aktiv genutzt, die auch in Schichten arbeiten.
Zum Beispiel unsere Entwicklungsabteilung hat keine festen Arbeitszeiten und kann zwischen 8 - 20 Uhr arbeiten.

Die Leute die feste Schichten haben, lassen sich in 2 Gruppen unterteilen.
Erstens normale Mitarbeiter die nur bestehende Schichten betrachten und Teamleads die bestehende Schichten
bearbeiten und neue Schichten und Personen anlegen.

####1.3 Projektziel

Ziel des Projektes ist es einen übersichtlichen und einfach zu benutzenden Online-Schichtplanner zu erstellen.

Der Fokus liegt dabei zum einen auf das betrachten der bereits bestehenden Schichten.
Welches bei großen Teams vorallem durch Filteroptionen vereinfacht werden soll.
Zum anderen soll den Teamleads ein intuitives Interface zum erstellen, bearbeiten und löschen von Daten zur Verfügung gestellt werden.

Aufgrund der Tatsache das in einem Team viele Mitarbeiter mit unterschiedlichen Sprachen sind und diese Sprachen
ausschlaggebend für die Schichtplannung sind, muss der Schichtplanner neben der Person und den zugehörigen Schichten auch die Sprachen in welcher die Person Kunden betreut, dargestellt werden.
Neben der Sprache soll jeder Person auch eine oder mehrere Rollen zugeordnet werden können, z.B. Teamlead, Support-Agent, Trainer etc.
Desweiteren soll jedem Mitarbeiter auch ein Skill bzw. Aufgabenfeld zugeordnet werden können, z.B. 1st Level, 2nd Level oder bestimmte Programmiersprachen.

Nach all diesen Kriterien soll gefiltert können. Hinzukommt das es möglich sein soll eine Person über den Namen zu finden.
Ein Dropdownmenu soll es ermöglichen zwischen Abteilungen zu wechseln.

Um eine übersichtliche Ansicht zu gewährleisten soll pro Abteilung nur 1 Woche werden, entsprechende Buttons sollen es ermöglichen die nächste bzw. vorherige Woche einzusehen.



####1.4 Projektbegründung

Es gibt im Moment einen Schichtplaner, der auch intern entwickelt wurde. Allerdings weist dieser erhebliche Schwächen in der Benutzbarkeit und in der Übersichtlichkeit auf.

Zum einen wird immer der gesamte Monat abgebildet, allerdings werden auf dem Bildschirm aus Platzgründen nur 2 Wochen angezeigt. Um die restlichen 2 Wochen zu sehen muss man nach rechts scrollen, wobei die Anzeige der Namen verschwindet. Das macht es sehr umständlich die Schichten für einen speziellen Mitarbeiter in den letzten 2 Wochen eines Monats herauszufinden.

Ein weiteres Problem ist das immer 3 Monate untereinander angezeigt werden, man muss sowohl horizontal als auch vertikal scrollen um alle Informationen zu erfassen und es gibt keine Möglichkeit die Ansicht auf einen bestimmten Zeitrahmen festzulegen.

Desweiteren gibt es auch sonst keine Möglichkeit die Dargestellten Informationen zu filter, sollte man z.B. nur die Mitarbeiter mit einer bestimmten Sprache betrachten wollen, gäbe es keine Möglichkeit nur diese anzuzeigen.

##2 Projektplanung

####2.1 Projektphasen

Zur Abschießung des Projektes stehen dem Autor 70 Stunden zur Verfügung. Zum Anfang des Projektes wurden verschiedene Projektphasen und deren geschätzte Dauer festgelegt.
Dabei wurden 2 Unterteilungen vorgenommen, zum einen eine grobe Unterteilung, welche die Hauptphasen enthält.
Diese wird in _Tabelle 1: Grobe Zeitplanung_ dargestellt. Diese können allerdings noch weiter detaillierter aufgelistet werden, indem man die Hauptphasen noch in Unterpunkte zerlegt. Diese detaillierte Tabelle ist im Anhang unter _A.1 Detaillierte Zeitplanung_ zu finden.

Projektphase | geplante Zeit (in Stunden)
-------------|--------------
Analyse | 5
Entwurf | 10
Implementierung | 35
Deployment | 10
Dokumentation | 10

_Tabelle 1: Grobe Zeitplanung_

####2.2 Ressourcenplanung

In _Anhang 2: Verwendete Ressourcen_ sind alle verwendeten Ressourcen ausführlich aufgelistet. Darunter zählen sowohl Hard-, Software als auch Personal.
Aufgrund der Leidenschaft des Autors zu Open Source wurde größtenteils auf Open Source Software gesetzt.
Das hatte auch den Vorteil das keine Lizenzkosten angefallen sind.

####2.3 Entwicklungsprozess

Um möglichst häufig und frühzeitig Feedback zu erhalten, hat sich Autor für einen agilen Ansatz entschieden.
Dabei soll am Ende jedes Tages ein kurzes Gespräch mit den Auftraggebern geführt werden, dadürch soll gewährleistet werden das etwaige Missverständnisse frühzeitig aufgedeckt und dementsprechend behoben werden können. Durch das rechtzeitige entdecken von falschen Entwicklungen, ist deren Wiedergutmachung günstiger als bei einer späteren Entdeckung.

Desweiteren soll die Anwendung testgetrieben entwickelt werden. Test Driven Development führt in der Regel zu besserer Codequalität und einfacherer Erweiterbarkeit. Wenn der Code verbessert (refactoring) werden soll, kann deren Funktionalität durch die bestehenden Tests überprüft werden.

Das ist vorallem wichtig das es sich bei diesem Projekt um eine minimal Lösung (minimum valuable product).
Es ist geplant das das Produkt nach Abschluss der initialen Entwicklungsphase weiter entwickelt wird.

##3 Analysephase

####3.1 Ist-Analyse

Wie bereits unter Punkt 1.4 beschrieben gibt es bereits ein bestehendes Produkt, welches jedoch __erhebliche__
Schwächen in Punkto Benutzbarkeit und Bedienbarkeit hat. Das führt dazu das viele Mitarbeiter unnötig viel Zeit dafür aufwenden Ihre eigenen oder die Schichten von Kollegen herrauszufinden.
Desweiteren ist das erstellen neuer Schichten und Personen umständlich, was auch zu ineffizienter Arbeit der Teamleads führt.

####3.2 Wirtschaftlichkeitsanalyse

Durch die Probleme der bestehenden Lösung die in 1.4 und 3.1 ausführlich beschrieben wurden, würde eine Umsetzung die Arbeit aller Mitarbeiter die in Schichten arbeiten effizienter gestaltet werden.
Ob die Umsetzung auch aus finanzieller Sicht zu rechtfertigen ist, soll in den folgenden Punkten untersucht werden.

####3.2.1 "Make or Buy"-Entscheidung

Aufgrund der unternehmensspezifischen Anforderung an den Schichtplanner, bezüglich Sprachen und Rollen jeweiliger Personen, befriedigt keine kostenlose Lösung auf dem Markt alle Bedürfnisse.
Aus diesem Grund soll das Projekt intern entwickelt werden.

####3.2.2 Projektkosten

Die Kosten die während der Umsetzung des Projektes anfallen würden, sollen berechnet werden.
Da bei der Software auf Open Source gesetzt wurde fallen keine Kosten für Lizenzen an.
Die anstehenden Ausgaben entstehen nur in Form von Arbeitszeit von internen Mitarbeitern.
Dabei wird für den Auszubildenen ein Stundensatz von 5€ festgelegt und für einen fest angestellten
Teamlead 25€.

Die gesamten Projektkosten und deren Zusammensetzung können der _Tabelle 2: Kostenaufstellung entnommen werden.

Vorgang | Mitarbeiter | Zeit (in Stunden) | Kosten (in €)
--------|-------------|------------------|-------
Entwicklungskosten | 1 Auszubildender | 70 | 350
Erstellung des Lastenheftes | 1 Teamlead | 2 | 50
tägliches Feedback | 1 Teamlead | 3 | 75
__Projektkosten gesamt:__ | | | __475__

####3.2.3 Amortisationsdauer

Folgend soll berechnet werden, wie lange es dauern wird bis sich die Ausgaben amortisieren und ab wann das Produkt Gewinn für das Unternehmen erwirtschaftet.

Der primäre Vorteil des Produktes liegt in der verbesserten Bedienbarkeit, welche dazu führt das weniger Zeit notwendig ist um bestimmte Aktionen durchzuführen.

Eine kleine Umfrage hat ergeben das ungefähr 70% der Mitarbeiter in festen Schichten arbeiten und dementsprechend den Schichtplaner jeden Tag nutzen. Desweiteren hat die Umfrage ergeben das der alte Schichtplanner im Schnitt jeden Tag für 2 Minuten benutzt wird.
Durch die massiv verbesserte Übersichtlichkeit wird davon ausgegangen, das das betrachten von Schichten einer bestimmten Person um 50% schneller ist.
Das administieren der Schichten durch den Teamlead soll 20% schneller gehen.

Vorgang | Anzahl _pro Monat_ | Zeit (alt) _pro Vorgang_ | Zeit (neu) _pro Vorgang_ | Einsparung
--------|--------|------------|------------|-----------
herrausfinden einer Schicht | 4200 | 2 min | 1 min | 35 h
Administration des Schichtplanners | 200 | 5 min | 4 min | 3 h 20 min
__Zeiteinsparung gesamt pro Monat:__ | | | | __38 h 20 min__

__Berechnung der Amortisationsdauer:__

_Anzahl der Aufrufe pro Monat:_

Von 300 Mitarbeitern benutzen 70% den Schichtplanner täglich. Das sind __210__ Mitarbeiter. Bei 20 Arbeitstagen pro Monat resultiert das in
__4200__ Aufrufen pro Monat.

_Ersparnis durch schnelleren Zugriff auf bestehende Schichten:_

Wie bereits in der Tabelle ersichtlich ergibt sich dadurch im Monat eine Zeitersparnis von __35 Stunden!__
Wenn wir von einem durchschnittlichen Stundenlohn von 15€ ausgehen ergibt das bereits im ersten Monat eine Einsparung von __525 €!__

_Ersparnis durch vereinfachte Administartion des Schichtplanners:_

Wir gehen davon aus das ein Teamlead im Schnitt 5 Minuten am Tag für die Administration des Schichtplanners aufbringen muss.
Bei 10 verschiedenen Abteilungen beläuft sich das auf 200 (10 Zugriffe pro Tag x 20 Tage) Vorgänge im Monat.
Bei der Administation gab es weniger potenzial den Workflow zu verbessern, aus diesem Grund ist der Vorgang nur 20% schneller.
Was trotzdem jeden Tag 1 Minute Zeit einspart. Bei Teamleads gehen wir von einem durchschnittlichen Stundenlohn von 25 € aus.
Das würde bedeuten das weitere __83,33 €__ (3 1/3 h x 25 € / h) pro Monat gespart werden können.

Das bedeutet das wir pro Monat __608,33 €__ sparen! Das sind 30,42 € pro Tag.
Bei Projektkosten von lediglich 475 € bedeutet das, das sich das Projekt bereits nach __16 Arbeitstagen__ amortisiert hat!

Aus diesem Grund kann das Projekt aus wirtschaftlichen Gesichtspunten als sehr lukrativ eingestuft werden.

####3.3 Anwendungsfälle

kommt später

####3.4 Lastenheft / Fachkonzept

Am Ende der Analysephase wurde zusammen mit dem Teamlead vom Customer Care ein Lastenheft erstellt, welches alle
Anforderungen des Auftraggebers an die ANwendung zusammenfasst.
Einen Auschschnitt aus dem Lastenheft ist im _Anhang 3: Auszug des Lastenheftes_ zu finden.

##4 Entwurfsphase

####4.1 Zielplattform

Vom Auftraggeber gab es keine Beschränkung welche Programmiersprache verwendet werden soll.
Es sollte lediglich ein webbasierter Schichtplanner sein.

Aus diesem Grund hat sich der Autor für Software entschieden die seinen persönlichen Vorlieben entspricht.
Als Programmiersprache wurde Ruby gewählt, was zur Wahl von Ruby on Rails als Webframework führte.
Da ein Schichtplanner sehr dynamisch ist und viel Javascript erfordert, hat sich der Autor für ein dediziertes Javascript-Frontend-Framework entschieden. Im speziellen wurde AngularJS ausgewählt.
Da die Darstellung der Daten AngularJS obliegt, wird Ruby on Rails als JSON-API betrieben.
Um die Daten permanent zu speichern wurde PostgreSQL als ORDBMS gewählt.

####4.2 Architekturdesign



####4.3 Entwurf der Benutzeroberfläche
####4.4 Datenmodell
####4.5 Geschäftslogik
####4.6 Pflichtenheft

##Anhang:

####Anhang 1: Detaillierte Zeitplanung

Projektphase | geplante Zeit (in Stunden)
-------------|--------------
__Analyse__ | __5__
Ist-Analyse | 1
Durchführung einer Wirtschaftlichkeitsanalyse und Amortisationsrechnung | 1
Ermittlung von Use-Cases | 1
Unterstützung bei der Erstellung des Lastenhefts | 2
__Entwurf__ | __10__
Erstellung eines ER-Model | 1
Entwurf der API | 2
Markup für das Frontend | 3
Erstellung eines Pflichtenheftes | 4
__Implementierung__ | __35__
Implementierung der API | 10
Implementierung des Frontends | 25
__Deployment__ | __10__
Aufsetzen des Server | 2
Einrichtung des Coninuous Integration-Prozesses | 8
__Dokumentation__ | __10__
Erstellen der Projektdokumentation | 10

####Anhang 2: Verwendete Ressourcen

__Hardware:__

- 1 PC, 2 Bildschirme, Maus, Tastatur

__Software:__

- Xubuntu 14.04
- Sublime Text 3
- Firefox
- Rails 5.0
- Angular 1
- Git
- Nginx
- Passenger
- PostgreSQL 9.5
- Docker
- Bootstrap 3
- Ansible
- Jenkins

__Personal:__

- Entwickler - Umsetzung des Projektes
- Teamlead von Customer Care - UI and UX Feedback

####Anhang 3: Auszug des Lastenheftes

auszug lastenheft

Anforderungen:
- a
- b
- c
- d