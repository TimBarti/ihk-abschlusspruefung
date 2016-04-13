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
##### 3.3 Nicht-monetäre Vorteile
##### 3.4 Anwendungsfälle
##### 3.5 Lastenheft / Fachkonzept

### 4 Entwurfsphase

##### 4.1 Zielplattform
##### 4.2 Architekturdesign
##### 4.3 Entwurf der Benutzeroberfläche
##### 4.4 Datenmodell
##### 4.5 Geschäftslogik
##### 4.6 Pflichtenheft

### 5 Implementierungsphase

##### 5.1 Iterationsplaung
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

