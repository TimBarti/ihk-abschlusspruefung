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
##### 4.3 Entwurf der API
##### 4.4 Entwurf der Benutzeroberfläche
##### 4.5 Datenmodell
##### 4.6 Geschäftslogik
##### 4.7 Pflichtenheft

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

Das Produkt ist es für Unternehmen unabhängige und transaktionsbasierte Bewertungen zu sammeln.
Zu unseren Kunden zählen größtenteils Onlineshop, allerdings auch Banken und Versicherungen.
Durch die unabhängig gesammelten Bewertungen, soll bei Neukunden Vertrauen für den Onlineshop geweckt werden.
Desweiteren erhöhen die gesammelten Bewertungen in signifikantem Maße das SEO-Ranking.

####1.1 Projektbeschreibung

Bei eKomi haben die einzelnen Abteilungen in der Regel zwischen 10 und 25 Mitarbeiter.
Die meisten Mitarbeiter haben eine feste Arbeitszeit, um den Kunden zuverlässigen Support zu garantieren.
Aus diesem Grund wird jedem Mitarbeiter von dem zuständigen Teamleiter eine feste Schicht zugeordnet.
Innerhalb einer Abteilung gibt es Mitarbeiter mit vielen unterschiedlichen Sprachen, die basierend auf der Sprache bestimmte Schichten belegen müssen.
Um diese Schichten zu planen wird ein Schichtplaner benötigt.
Dieser muss anzeigen, wenn ein Mitarbeiter im Urlaub oder Krank ist.

####1.2 Projektumfeld

Grundsätzlich wird der Schichtplanner natürlich nur von Mitarbeitern aktiv genutzt, die auch in Schichten arbeiten.
Zum Beispiel hat unsere Entwicklungsabteilung keine festen Arbeitszeiten und kann in der Zeit zwischen 8 - 20 Uhr arbeiten.

Die Leute die feste Schichten haben, lassen sich in reguläre Mitarbeiter und Teamleiter einteilen.

Reguläre Mitarbeiter betrachten bestehende Schichten und Teamleiter die Schichten
zuweiesn, neue Schichttypen anlegen und neue Mitarbeiter hinzufügen können.

####1.3 Projektziel

Ziel des Projektes ist es einen übersichtlichen und einfach zu benutzenden Online-Schichtplanner zu erstellen.

Der Fokus liegt dabei zum einen auf das betrachten der bereits bestehenden Schichten,
welches bei großen Teams vorallem durch Filteroptionen vereinfacht werden soll.
Zum anderen soll den Teamleitern ein intuitives Interface zum erstellen, bearbeiten und löschen von Daten zur Verfügung gestellt werden.

In jedem Team sind mehrere Sprachen vertreten. Diese verschiedenen Sprachen müssen im Schichtplanner berücktsichtigt werden. Mit dem Schichtplaner soll sichergestellt werden, dass Kunden in allen Sprachen betreut werden können.

Neben der Sprache soll jeder Person auch eine oder mehrere Rollen zugeordnet werden können. Bei den Rollen kann es sich beispielweise um Teamleiter, Support-Agent oder Trainer handeln. 
Desweiteren soll jedem Mitarbeiter auch eine Fähigkeit oder ein Aufgabenfeld zugeordnet werden können. Diese könnten, 1st Level, 2nd Level oder eine bestimmte Programmiersprachen ,sein.

Nach all diesen Kriterien soll gefiltert werden können. Hinzu kommt, dass es möglich sein soll eine Person über den Namen zu finden.
Ein Dropdownmenue soll es ermöglichen zwischen Abteilungen zu wechseln.

Um eine übersichtliche Ansicht zu gewährleisten soll pro Abteilung nur eine Woche angezeigt werden. Entsprechende Buttons sollen es ermöglichen die nächste oder vorherige Woche einzusehen.

####1.4 Projektbegründung

Der alte Schichtplaner wurde auch intern entwickelt. Dieser weist erhebliche Schwächen in der Benutzbarkeit und in der Übersichtlichkeit auf (siehe _Anhang 10: Screenshot vom alten Schichtplanner_).

Zum einen wird immer der gesamte Monat abgebildet, jedoch sind auf dem Bildschirm aus Platzgründen nur 2 Wochen sichtbar. Um die restlichen 2 Wochen sehen zu können, muss man nach rechts scrollen. Die Spalte mit den Mitarbeiternamen ist nicht am Bildschirmrand fixiert, wodurch sie aus dem Blickfeld verschwindet. Das macht es sehr umständlich die Schichten für einen bestimmten Mitarbeiter für die letzten 2 Wochen eines Monats herauszufinden.

Ein weiteres Problem ist das immer 3 Monate untereinander angezeigt werden. Dies hat zur Folge, dass sowohl horizontal als auch vertikal gescrollt werden muss, um alle Informationen zu erfassen. Eine Möglichkeit die Ansicht auf einen bestimmten Zeitraum festzulegen gibt es nicht.

Desweiteren gibt es auch keine Möglichkeit die dargestellten Informationen zu filtern. Sollte man beispielsweise nur die Mitarbeiter mit einer bestimmten Sprache betrachten wollen, gäbe es keine Option um nur diese anzuzeigen.

##2 Projektplanung

####2.1 Projektphasen

Zum Abschluss des Projektes stehen dem Autor 70 Stunden zur Verfügung. Zum Anfang des Projektes wurden verschiedene Projektphasen und deren geschätzte Dauer festgelegt.
Dabei wurden zwei Unterteilungen vorgenommen, zum einen eine grobe Unterteilung, welche die Hauptphasen enthält.
Diese wird in _Tabelle 1: Grobe Zeitplanung_ dargestellt. Diese können allerdings noch weiter aufgeteilt werden, indem man die Hauptphasen noch in Unterpunkte zerlegt. Diese ausführliche Tabelle ist im Anhang unter _A.1 Detaillierte Zeitplanung_ zu finden.

Projektphase | geplante Zeit (in Stunden)
-------------|--------------
Analyse | 5
Entwurf | 8
Implementierung | 37
Deployment | 10
Dokumentation | 10

_Tabelle 1: Grobe Zeitplanung_

####2.2 Ressourcenplanung

In _Anhang 2: Verwendete Ressourcen_ sind alle verwendeten Ressourcen aufgelistet. Darunter zählen sowohl Hard- und Software als auch Personal.
Aufgrund der Leidenschaft des Autors zu Open Source, wurde größtenteils auf Open Source Software gesetzt.
Das hatte auch den Vorteil das keine Lizenzkosten angefallen sind.

####2.3 Entwicklungsprozess

Um möglichst häufig und frühzeitig Feedback zu erhalten, hat sich der Autor für den Ansatz der agilen Softwareentwicklung entschieden.
Dabei soll am Ende jeder Iteration ein kurzes Gespräch mit dem Ausbilder geführt werden. Dadurch soll gewährleistet werden, dass etwaige Missverständnisse frühzeitig aufgedeckt und dementsprechend behoben werden können. Durch das rechtzeitige Entdecken von falschen Entwicklungen, ist deren Korrektur günstiger.

Darüber hinaus soll die Anwendung testgetrieben entwickelt werden. Test Driven Development führt in der Regel zu besserer Codequalität und erhöhter Modularität. Wenn der Code verbessert (refactoring) werden soll, kann deren Funktionalität durch die bestehenden Tests überprüft werden.

Das ist vorallem wichtig, da es sich bei diesem Projekt um eine minimal Lösung handelt.
Es ist geplant das das Produkt nach Abschluss der initialen Entwicklungsphase weiter entwickelt wird.

##3 Analysephase

####3.1 Ist-Analyse

Wie unter Punkt 1.4 beschrieben gibt es eine bestehende Lösung, welches jedoch __erhebliche__
Schwächen in Punkto Benutzbarkeit und Bedienbarkeit hat. Das führt dazu, dass viele Mitarbeiter unnötig viel Zeit dafür aufwenden, ihre eigenen oder die Schichten von Kollegen herrauszufinden.
Des Weiteren ist das erstellen neuer Schichten und Personen umständlich, welches einen unnötigen Aufwand für die Teamleiter darstellt.

####3.2 Wirtschaftlichkeitsanalyse

Im Vergleich mit der bestehenden Lösung, die in 1.4 und 3.1 ausführlich beschrieben wurden, würde ein besserer Schichtplaner die Arbeit aller Mitarbeiter, die in Schichten arbeiten, effizienter gestaltet.
Ob die Umsetzung auch aus finanzieller Sicht zu rechtfertigen ist, soll in den folgenden Punkten untersucht werden.

####3.2.1 "Make or Buy"-Entscheidung

Aufgrund der unternehmensspezifischen Anforderung an den Schichtplanner, bezüglich Sprachen und Rollen der jeweiliger Personen, befriedigt keine kostenlose Lösung auf dem Markt alle Bedürfnisse.
Aus diesem Grund soll das Projekt intern entwickelt werden.
>>>kommentar von Tim: mach ne entscheidungsmatrix man<<<

####3.2.2 Projektkosten

Folgend sollen die Kosten für die Umsetzung des Projektes berechnet werden.
Da bei der Entwicklung auf kostenlose Open Source Software gesetzt wurde, fallen keine Kosten für Lizenzen an.
Die anstehenden Ausgaben entstehen nur in Form von Arbeitszeit von internen Mitarbeitern.
Dabei wird für den Auszubildenen ein Stundensatz von 5€ und für einen fest angestellten
Teamleiter 25€ angenommen.

Die gesamten Projektkosten und deren Zusammensetzung können der _Tabelle 2: Kostenaufstellung_ entnommen werden.

Vorgang | Mitarbeiter | Zeit (in Stunden) | Kosten (in €)
--------|-------------|------------------|-------
Entwicklungskosten | 1 Auszubildender | 70 | 350
Erstellung des Lastenheftes | 1 Teamleiter | 2 | 50
Feedback nach einer Iteration | 1 Teamleiter | 3 | 75
__Projektkosten gesamt:__ | | | __475__

_Tabelle 2: Kostenaufstellung_

####3.2.3 Amortisationsdauer

Als nächstes soll berechnet werden, wie lange es dauern wird bis sich die Ausgaben amortisiert haben und ab wann das Produkt Gewinn für das Unternehmen erwirtschaftet.

Der primäre Vorteil des Produktes liegt in der verbesserten Bedienbarkeit, welche dazu führt das weniger Zeit notwendig ist um den Schichtplaner zu bedienen.

Eine kleine Umfrage hat ergeben das ungefähr 70% der Mitarbeiter in festen Schichten arbeiten und dementsprechend den Schichtplaner jeden Tag nutzen. Weiter hat die Umfrage ergeben, dass der alte Schichtplanner im Durchschnitt jeden Tag für 2 Minuten benutzt wird.
Durch die massiv verbesserte Übersichtlichkeit wird davon ausgegangen, dass das Betrachten von Schichten einer bestimmten Person um 50% schneller bewerkstelligt werden kann.
Das Administieren der Schichten durch den Teamleiter soll 20% schneller gehen.

Vorgang | Anzahl _pro Monat_ | Zeit (alt) _pro Vorgang_ | Zeit (neu) _pro Vorgang_ | Einsparung
--------|--------|------------|------------|-----------
herrausfinden einer Schicht | 4200 | 2 min | 1 min | 35 h
Administration des Schichtplanners | 200 | 5 min | 4 min | 3 h 20 min
__Zeiteinsparung gesamt pro Monat:__ | | | | __38 h 20 min__

_Tabelle 4: Name suchen_

__Berechnung der Amortisationsdauer:__

_Anzahl der Aufrufe pro Monat:_

Von 300 Mitarbeitern benutzen 70% den Schichtplanner täglich. Das sind __210__ Mitarbeiter. Bei 20 Arbeitstagen pro Monat resultiert das in
__4200__ Aufrufen pro Monat.

_Ersparnis durch schnelleren Zugriff auf bestehende Schichten:_

Wie in _Tabelle 4_ ersichtlich ergibt sich dadurch im Monat eine Zeitersparnis von __35 Stunden!__
Wenn wir von einem durchschnittlichen Stundenlohn von 15€ ausgehen ergibt das bereits im ersten Monat eine Einsparung von __525 €!__

_Ersparnis durch vereinfachte Administration des Schichtplanners:_

Wir gehen davon aus, dass ein Teamleiter im Schnitt 5 Minuten am Tag für die Administration des Schichtplanners aufbringen muss.
Bei 10 verschiedenen Abteilungen beläuft sich das auf 200 (10 Zugriffe pro Tag x 20 Tage) Vorgänge im Monat.
Bei der Administration gab es weniger Potenzial den Arbeitsablauf zu verbessern. Aus diesem Grund ist der Vorgang nur 20% schneller.
Was trotzdem jeden Tag eine Minute pro Aufruf einspart. 
Das bedeutet das weitere __83,33 €__ (3 1/3 h x 25 € / h) pro Monat gespart werden können.
```
nochmal rechnung von 200 minuten zu 3 1/3 stunden
```

Das bedeutet, dass der Betrieb pro Monat __608,33 €__ spart! Das sind 30,42 € pro Tag.
Bei Projektkosten von lediglich 475 € bedeutet das, dass sich das Projekt bereits nach __16 Arbeitstagen__ amortisiert hat.

Aus diesem Grund kann das Projekt aus ökonomischer Perspektive als sehr lukrativ eingestuft werden.

####3.3 Anwendungsfälle

Es gibt Mitarbeiter und die Teamleiter. Beide benutzen den Schichtplaner um Schichten zu betrachten und eventuell die Vorteile einer fortgeschrittenen Filterfunktion für sich nutzbar zu machen.
Lediglich die Teamleiter haben die Möglichkeit Schichten zuzuweisen. Desweiteren können sie neue Datensätze erstellen oder bestehende bearbeiten. Bei diesen Vorgängen wird jeweils die Validität der Daten überprüft.
Teamleiter können auch Datensätze löschen. Vor dem Löschen soll der Nutzer durch einen interaktiven Dialog seine Anweisung bestätigen. 

####3.4 Lastenheft / Fachkonzept

Am Ende der Analysephase wurde zusammen mit dem Teamleiter der Supportabteilung ein Lastenheft erstellt, welches alle Anforderungen des Auftraggebers an die Anwendung zusammenfasst.
Einen Auschschnitt aus dem Lastenheft ist im _Anhang 3: Auszug des Lastenheftes_ zu finden.

##4 Entwurfsphase

####4.1 Zielplattform

Vom Auftraggeber gab es keine Beschränkung welche Programmiersprache verwendet werden soll.
Es sollte lediglich ein webbasierter Schichtplanner entstehen.

Aus diesem Grund hat sich der Autor für Software entschieden, die seinen persönlichen Vorlieben entspricht.
Als Programmiersprache wurde Ruby gewählt, was zur Wahl von Ruby on Rails als Webframework führte.
Da ein Schichtplanner sehr dynamisch ist und viel Javascript erfordert, hat sich der Autor für ein dediziertes Javascript-Frontend-Framework entschieden. Im speziellen wurde AngularJS ausgewählt. 

Um ein konsequentes Aussehen und eine einfache Umsetzung zu gewährleisten wurde dabei auf Bootstrap als CSS-Framework gesetzt.

Da die Darstellung der Daten AngularJS und Bootstrap obliegt, wird Ruby on Rails als JSON-API betrieben.
Um die Daten permanent zu speichern wurde PostgreSQL als ORDBMS gewählt.

####4.2 Architekturdesign

Rail Version 5 wurde gewählt, weil hier der API Gem bereits integriert ist.
Der API-Modus führt dazu das viele unnötige Komponenten schon bei erstellen der App weggelassen werden, was zu einer wesentlich schlankeren Anwendung führt.

Ruby on Rails folgt dem Model-View-Controller Pattern. In diesem Fall ist ein Teil der Funktionalität in das Frontend (AngularJS) ausgelagert worden. Rails ist hier lediglich für das Auslesen und Ausliefern der Daten, Datenempfang mit JSON, die Authentifizierung und Authorisierung verantwortlich.

AngularJS folgt nach eigener Aussage dem Model-View-Whatever Pattern. Es ist im groben an MVC angelehnt.
Zusätzlich wird das two-way-databinding Pattern implementiert, welches dazu führt, dass Daten ,die im Frontend geändert werden, automatisch an das Backend kommuniziert werden. Zusammen mit einer high-level-abstraction für AJAX-Calls ,führt dies zu einer wesentlich einfacheren Entwicklung von dynamischen Anwendungen.
Die Hauptaufgabe von Angular ist es die Informationen, die als JSON übermittelt wurden, ansprechend darzustellen und zu filtern.

Da genau bekannt ist, in welcher Form die Daten gespeichert werden sollen, hat sich der Autor für eine relationelle Datenbank entschieden.
Da wir die Informationen als JSON verschicken, wurde ein Datenbankmanagementsystem gesucht, welches den Datentyp JSON nativ unterstützt.
Aufgrund dieser Kriterien ist die Wahl ist auf PostgreSQL gefallen.

Da für die Hauptansicht 6 verschiedene Tabellen abgefragt werden, wird dafür auf das ORM (Active Record) von Rails verzichtet und auf Postgres spezifisches SQL gesetzt, siehe _Anhang 4: Main Query_.

####4.3 Entwurf der API

Grundsätzlich gibt es für jede Datenbanktabelle 5 API-Aufrufe. Eine Übersicht über alle API-Aufrufe finden Sie im _Anhang 12: API-Aufruf_. 

Der Index-Call gibt alle Daten, wie eine Auflistung aller Abteilungen, wieder. Die Index-Aufrufe für die Schichten und die Personen wurden weggelassen, da diese aufgrund der großen Anzahl an Daten zu lange dauern würden (377500 Schichten) und es keine Anwendungsszenario für diese Aufrufe gibt. 

Der Show-Call gibt immer exakt einen Datensatz zurück, um diesen zu identifizieren wird immer eine ID als Parameter übergeben. Eine Ausnahme bildet hier wieder der Call für eine spezifische Abteilung. Wir möchten nicht nur alle Personen in einer Abteilung abrufen, sondern auch die Schichten einer spezifischen Woche. Aus diesem Grund wird auch immer eine Woche als Integer übergeben. Die Woche 0 ist immer die aktuelle Woche und negative Wochen sind die vergangenen.

Die Update-, Create- und Delete-Aufruf sind selbsterklärend und bei allen Attributen vorhanden.

Für die Filter müssen alle Abteilungen, Rollen, Sprachen, Fähigkeiten und Schichttypen abgefragt werden. Um zu verhindern, dass jedes mal 5 API-Aufrufe getätigt werden müssen, wurde ein extra API-Aufruf eingeführt `/api/people_filter_criteria/:dept_id/week/:week`, dieser gibt alle nötigen Informationen mit einem mal zurück.
Um die Filterkriterien übersichtlich zu halten sollten nur die Schichttypen berücksichtigt werden, die auch tatsächlich innerhalb der Woche auftreten.
```
darauf hinweisen das nur atrribute angezeigt werden die in der woche / abteilung vertreten sind
```
Das zuständige SQL-query ist im _Anhang 13: SQL-query für alle Filterkriterien_ zu finden.

####4.4 Entwurf der Benutzeroberfläche

Der wichtigste Teil, der Benutzeroberfläche, ist die Ansicht die alle Personen einer Abteilung und ihre zugehörigen Schichten in einer spezifischen Woche darstellt. Um eine bestimmte Person oder Personengruppe schnell zu finden, sollen detaillierte Filteroptionen zur Verfügung gestellt werden. Damit die Filteroptionen mit wachsender Anzahl von Kriterien nicht unübersichtlich werden, sollen die möglichen Kriterien nach Kategorie in einem Dropdownmenu gruppiert werden. Das heißt, es wird die Möglichkeit geben, eine andere Abteilung anzuzeigen, nach Role, Skill, Sprache und Schicht per Checkbox zu filtern und eine bestimmte Person über ihren Namen zu suchen.
Alle Personen, ihre Attribute und Schichten werden in einer Tabelle dargestellt. Des Weiteren gibt es natürlich die Option die nächste oder vorherige Woche anzuzeigen. Innerhalb dieser Ansicht können lediglich die bestehenden Schichten geändert und neue zugewiesen werden.

Alle weiteren Aktionen, wie zum Beispiel das erstellen, bearbeiten und löschen von Rollen, Personen etc. sind in extra Seiten ausgelagert, um die Tabelle nicht mit Funktionen zu überladen.

Die Entwürfe wurden dabei mit Stift und Papier angefertigt (siehe _Anhang 5: GUI Mockup_) und mit dem Auftraggeber abgesprochen.

####4.5 Datenmodell

Um die notwendigen Datentypen zu erabeiten wurde der bestehende Schichtplanner analysiert. Dadurch wurden folgende Einheiten herausgearbeitet:

- Abteilung
- Person
- Schicht
- Schichttype
- Rolle
- Sprache
- Fähigkeit

Die Beziehungen zwischen den einzelnen Einheiten ist im _Anhang 6: ER-Model_ dargestellt.

####4.6 Geschäftslogik

In Ruby on Rails entspricht jede Datenbanktabelle einem Model. Das heißt, es gibt 7 Models.
Auf ein Model kommt mindestens ein Controller, welcher standardmäßig alle REST Aktionen abdeckt.

 Ruby on Rails ist neben dem aus- und einlesen von Daten auch für die Autorisierung und Authentifizierung zuständig. Diese Aufgaben werden mithilfe der Gems CanCanCan und Devise gelöst.

Im Frontend wird basierend auf dem JSON dynamisch die Tabelle erstellt (siehe _Anhang 7: JSON-response_).
Des Weiteren werden die dargestellten Informationen gefiltert. Um das zu realisieren werden die bestehenden Informationen mit den aktiven Filterkriterien verglichen und entsprechend angezeigt oder nicht.
Um den Nutzer zu helfen valide Daten (z.B. neue Personen) zu erstellen, werden die eingegeben Daten mit Hilfe von Stringoperationen auf ihre Vailidität überprüft. Dadurch können Daten überprüft werden bevor Sie zum Server gesendet werden.

Da diese Form von Validierung durch deaktiveren von Javascript umgangen werden kann, ist es essenziell das es eine serverseitige Validierung gibt.
Um das zu gewährleisten werden Constraints direkt in PostgreSQL angelegt. Diese Lösung bietet einen Kompromiss aus valider Daten in der Datenbank und einfache Benutzbarkeit. Der Nachteil ist das die Validierungen in zwei Stellen stattfindet. Das bedeutet, wenn sich die Validierung ändert, muss der Quellcode an zwei Stellen angepasst werden.

####4.7 Pflichtenheft

Am Ende der Entwurfsphase wurde, basierend auf dem Lastenheft, das Pflichtenheft erstellt.
Dieses legt die Umsetzung des Projektes fest. Einen Auszug davon befindet sich im _Anhang 8: Pflichtenheft_.

##5 Implementierungsphase

####5.1 Iterationsplanung

Am Anfang der Implementierungsphase wurde ein Iterationsplan erstellt. Dieser legt die einzelnen Iterationen fest. Am Ende jeder Iteration wird der aktuelle Stand dem Auftraggeber vorgestellt. Der Interationsplan befindet sich im _Anhang 9: Interationsplan_.

####5.2 Implementierung der Datenstrukturen

Basierend auf dem bereits erstelltem ER-Model wurde mit Hilfe des `rails generators` die Tabellenstruktur erstellt. Das könnte für die People Tabelle so aussehen:
`rails g model person name:string department:references`.

Dieser Kommandozeilenbefehl erstellt Dateien für das Model, die Tests und die Migration.
Migrations sind in Rails der Weg um die Struktur der Datenbank zu ändern. Sie erlauben es Änderungen an der Datenbank sehr einfach rückgängig zu machen. Die erstellte Migration sieht so aus:

```ruby
class CreatePerson < ActiveRecord::Migration[5.0]
  def change
    create_table :Person do |t|
      t.string :name
      t.references :department, foreign_key: true

      t.timestamps
    end
  end
end
```

Nach dem ausführen von `rails db:migrate` wird dieser Code von Active Record in das SQL für die jeweilige Datenbank, in unserem Fall PostgreSQL, übersetzt und ausgeführt. Diese Form der Datenbankverwaltung hat den Vorteil, dass wir immer einen Primärschlüssel haben der `id` heißt und sich automatisch erhöht. Zusätzlich haben wir immer die Felder created_at und updated_at die autmatisch von Rails verwaltet werden.
```
tbartilla 22.04.2016
Nach bestem wissen und gewissen bis zu diesen Punkt überprüft und Änderungen vorgeschlagen.
```
####5.3 Implementierung der Geschäftslogik

Im folgenden soll der Prozess der Implementierung erläutert werden. Als erstes wird jedoch das allgemeine Setup vorgestellt. Da es sich bei Ruby und Javascript und Skriptsprachen handelt wurde auf eine IDE verzichtet und stattdessen der gesamte Code mit einem Texteditor erstellt und bearbeitet. Aufgrund seiner zahlreichen Features und Erweiterbarkeit durch Packages ist die Wahl auf Sublime Text 3 gefallen.
Der Code wurde mithilfe von Git versioniert, das bietet den Vorteil nach einem Fehler einfach auf einer frühere, funktionierende Version zurück gewechselt werden kann. Desweiteren gibt es die Möglichkeit neue Features in einem extra Branch zu entwickeln, dadurch hat man immer einen stabile Version.

Um die Weiterentwicklung und Fehlersuche zu vereinfachen wurde großer Wert auf sinnvolle commit messages gelegt.
Der Header ist maximal 50 Zeichen lang und fängt immer mit einem Großbuchstaben an.
Der Body der Commit-Message ist durch eine Leerzeile getrennt und erklärt was und warum etwas gemacht wurde, statt zu erklären wie es gemacht wurde. Generell sollte Code selbsterklärend sein, falls nicht sollte er durch Kommentare im Quelltext erklärt werden und nicht in der commit message.

Aufgrund seiner Popularität und des kostenlosen Angebots wurde Github als Host für das Repository gewählt. Desweiteren erhält man dadurch die Möglichkeit ohne Probleme das Projekt auf einem anderen PC zu clonen bzw. bei einem neuen Release es von Github zu pullen. 

Gemäß dem Iterationsplan wurde als erstes die die Railsapp erstellt.

__Erstellen der Railsapp mit Datenbankstruktur & aller API-Calls:__

 Der erste Schritt war die Erstellung der Datenbankstruktur. Um schon während der Entwicklungsphase Performanceprobleme zu entdecken wurden 377500 Schichten, 500 Mitarbeiter und 10 Abteilungen erstellt. Der nächste Schritt war alle grundlegenden API-Calls (Ausgabe aller Rollen usw.) zu implementieren und unnötige API-Calls (z.B. alle Schichten) zu entfernen. Der letzte Schritt in der ersten Iteration war es ein SQL-query zu schreiben, welches alle nötigen Informationen, für die Hauptansicht des Schichtplanners, aus der Datenbank ausliest, siehe _Anhang 4: Main Query_.

__Implementierung Authentifizierung und Autorisierung:__

Um Authentifizierung zu implementieren wurde der Gem _Devise_ gewählt. Dieser ist in der Rubycommunity sehr weit verbreitet und bietet eine große Anzahl an Features. Um dafür zu sorgen das nicht jede Nutzer auch Daten erstellen, bearbeiten und löschen wurde die Autorisierung mithilfe von _CanCanCan_ integriert.

__Implementierung von erstellen und aktualisieren von Schichten:__

Das aktualisieren und zuweisen von Schichten soll auf die selbe Weise geschehen. Die zu bearbeitenden Schichten werden durch das gedrückt halten der linken Maustaste ausgewählt. Ausgewählte Schichten sind durch eine andere Hintergrundfarbe hervorgehoben. Durch einen weiteren Klick auf die bereits ausgewählten Schichten öffnet sich ein Modal, _siehe Anhang 16: Screenshot von der Auswahl einer Schicht_, innerhalb dessen werden alle zur Auswahl stehenden Schichten angezeigt. Mit einem Klick auf die neue Schicht werden alle zuvor markierten Schichten aktualisiert und die Hintergrundfarbe wird auf die Standardfarbe zurückgesetzt.

__Implementierung der Filter für die Schichttabelle:__

AngularJS kommt von Haus aus schon mit dem Prinzip der Filter. Diese werden über eine Pipe an die darzustellenden Informationen angefügt.

```html
 <tr ng-repeat="(i, person) in dept.people | peopleFilter:filter.criteria">
```

Mit `dept.people` enthält die Informationen aller dazustellenden Personen. Mit Hilfe von `ng-repeat` wird über das Array iteriert und jeweils ein Zeile pro Person erstellt.
Nach der Pipe kommt der Name des Filters der angewendet werden soll und nach dem Doppelpunkt kommen die Daten die an den Filter übergeben werden. `filter.criteria` verändert sich durch das setzen der Filteroptionen, wodurch dann der Inhalt der Tabelle beeinflusst wird.

__Implementierung von erstellen, bearbeiten und löschen von Personen, Rollen usw.:__

Für jede Operation aller Datensätze soll eine extra Seite zur Verfügung stehen. Erreichbar sind diese Operationen über das Einstellungsmenu.
Es werden mithilfe von Bootstrap simple html-Formulare erstellt. Die eingebenen Daten werden dann in AngularJS validiert und dann über die API an die Datenbank übermittelt.

####5.4 Implementierung der Benutzeroberfläche

Die GUI wurde auf Basis der angefertigten Mockups implementiert. Um einen konsequentes Aussehen und eine einfache Umsetzung zu gewährleisten wurde dabei auf Bootstrap als CSS-Framework gesetzt. Dieses bietet uns dank dem Grid-System eine einfach Möglichkeit unsere Objekte zu organisieren. Desweiteren gibt es fertige Lösungen für Dropdownmenus, Modals und Akkordions. 
Komponenten die Javascript benötigen, setzen allerdings alle jQuery voraus. Da AngularJS mit einer abgespeckten Version von jQuery, namens jqLite, daherkommt, möchten wir auf jQuery verzichten. Aus diesem Grund greifen wir auf angular-bootstrap zurück.
In dieser, vom Angular Team gepflegten Bibliothek, wurden alle Bootstrapkomponenten die Javascript benötigen in Angular neu geschrieben.

##6 Abnahme- und Einführungsphase

####6.1 Abnahme durch den Ausbilder

Nach Abschluss der Implementierungsphase wurde die Anwendung vom Ausbilder abgenommen und geprüft ob alle im Pflichtenheft festgelegten Anforderungen erfüllt wurden.
Durch den agilen Entwicklungsprozess war der Ausbilder bereits mit der Anwendung vertraut, was die Abnahme deutlich beschleunigte.

####6.2 Deployment und Einführung

kommt später
-ansible
-kubernetes
-jenkins etc

##7 Dokumentation

Zum erstellen der Projektdokumentation wurde _Markdown_ als markup language verwendet.
Es bietet die Möglichkeit sehr einfach grundlegende Textformatierung durchzuführen und lässt sich ohne Probleme in html übersetzen.

Desweiteren wurde auch die Projektdokumentation mit Git versioniert und auf Github gehostet. Das führte auch dazu das die Dokumentation online mit dem Githubtexteditor bearbeitet werden konnte.

Um eine ansprechende PDF zu erstellen wurde das Dokument am Ende noch einmal in Google Docs übertragen.

Bei der Erstellung des Schichtplanners wurde großen Wert auf eine einfache und selbsterklärende Benutzung gelegt, trotzdem sollte die Anwendung für die Mitarbeiter dokumentiert werden. Aus diesem Grund wurde ein Artikel im internen Wiki erstellt. Dieser erklärt kurz alle Features und wie sie benutzt werden können.

##8 Fazit

####8.1 Soll-/Ist-Vergleich

Zum Ende hin kann gesagt werden das alle im Pflichtenheft festgelegten Vorgaben erfüllt wurden und der vorgegebene Zeitrahmen von 70 Stunden lediglich um 1 Stunde überschritten wurde. Grundsätzlich wurde für die Analyse, Entwurf etwas zu viel eingeplant. Die Integration des Frontends und die Einrichtung des CI Workflows nahmen hingegegen mehr Zeit in Anspruch als geplant. Diese Diskrepanz ist darauf zurückzuführen das der Autor mit den verwendeten Tools noch nicht sehr vertraut war.

Projektphase | geplante Zeit (in Stunden) | genutzte Zeit (in Stunden) | Differenz (in Stunden)
-------------|--------------------------- | -------------------------- | ---------------------
__Analyse__ | __5__ | __3,5__ | __-1,5__
Ist-Analyse | 1  | 1 | 0
Durchführung einer Wirtschaftlichkeitsanalyse und Amortisationsrechnung | 1 | 0,5 | -0,5
Ermittlung von Use-Cases | 1 | 1 | 0
Unterstützung bei der Erstellung des Lastenhefts | 2 | 1 | -1
__Entwurf__ | __8__ | __5,5__ | __-2,5__
Erstellung eines ER-Model | 1 | 1 | 0
Entwurf der API | 1 | 0,5 | -0,5
Mockups für das Frontend | 2 | 1 | -1
Erstellung eines Pflichtenheftes | 4 | 3 | -1
__Implementierung__ | __37__ | __38__ | __+1__
Implementierung der API | 12 | 10 | -2
Implementierung des Frontends | 25 | 28 | +3
__Deployment__ | __10__ | __12__ | __+2__
Aufsetzen des Server | 2 | 1 | -1
Einrichtung des Coninuous Integration-Prozesses | 8 | 11 | +3
__Dokumentation__ | __10__ |  __12__ | __+2__
Erstellen der Projektdokumentation | 10 | 12  | +2
__gesamt:__ | __70__ | __71__ | __+1__

_Tabelle 3: Soll- /Ist-Vergleich_

####8.2 Lessons Learned

Grundsätzlich konnte der Autor sein Wissen und seine Erfahrung im Projektmanagement deutlich verbessern.
Hinzukommt das verbesserte Verständis von Test Driven Development in Rails, besseres allgemeines Verständnis von AngularJS, vertieftes Wissen von PostgreSQL und komplexen SQL-queries und mehr praktische Erfahrung beim Erstellen eines Continious-Integration-Workflows.

####8.3 Ausblick

Da es sich bei der Anwendung um ein MVP (minimum valuable product) handelt, ist noch viel Raum für weitere Funktionen. Die Umsetzung von TDD und CI kommen der kontinuierlichen Weiterentwicklung der Anwendung entgegen.

Denkbare Features wären eine Art Dashboard, wo man z.B. sehen kann wer wie oft welche Schicht hatte.
Eine Idee ist auch das die Schichten automatisch erstellt werden, indem für jede Person Regeln festgelegt werden. Zum Beispiel könnte eine Regel so aussehen das eine Person 20% Spätschicht, 50% Mittelschicht und 30% Frühschicht hat. Ein Algorithmus würde dann allen Personen automatisch ihre Schichten zuordnen. Dadurch würde sich der Administrationsaufwand für die Teamleiter erheblich verringern.
Wenn man das ganze noch einen Schritt weiter nehmen würde, könnten die Mitarbeiter die geänderten Schichten beantragen und der Teamleiter würde es nur noch genehmigen oder es würde sogar automatisch übernommen werden, wenn die Änderung den Regeln entspricht.


##Anhang:

####Anhang 1: Detaillierte Zeitplanung

Projektphase | geplante Zeit (in Stunden)
-------------|--------------
__Analyse__ | __5__
Ist-Analyse | 1
Durchführung einer Wirtschaftlichkeitsanalyse und Amortisationsrechnung | 1
Ermittlung von Use-Cases | 1
Unterstützung bei der Erstellung des Lastenhefts | 2
__Entwurf__ | __8__
Erstellung eines ER-Model | 1
Entwurf der API | 1
Mockups für das Frontend | 2
Erstellung eines Pflichtenheftes | 4
__Implementierung__ | __37__
Implementierung der API | 12
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
- Violet UML Creator
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
- Kubernetes

__Personal:__

- Entwickler - Umsetzung des Projektes
- Teamleiter von Customer Care - UI and UX Feedback

####Anhang 3: Auszug des Lastenheftes

Die Anwendung soll folgende Kriterien erfüllen:

- übersichtliche Darstellung aller Personen und ihrer Schichten in einer Abteilung in einer Woche
- der Tabellenkopf soll fixiert sein
- die Tabelle soll eine maximale Länge haben, so das die Seite selbst nie gescrollt wird, sondern nur die Tabelle
- Möglichkeit die Personen einer anderen Abteilung zu betrachten
- Möglichkeit die letzte bzw. nächste Woche zu betrachten
- Möglichkeit über Auswahl von Checkboxen nach Rolle, Sprache, Fähigkeit und/ oder Schicht zu filtern
- Möglichkeit über die Eingabe von Text nach dem Namen zu filtern
- Möglichkeit innerhalb der Schichtansicht neue Schichten zu erstellen und bestehende zu bearbeiten
- Möglichkeit in einer extra Ansicht Personen, Rollen, Sprachen, Fähigkeiten, Schichten, Schichttypen und Abteilungen zu erstellen, bearbeiten oder löschen.

####Anhang 4: Main Query

__improve variable names__

```sql
SELECT array_to_json(array_agg(row_to_json(persons))) as people_in_dept
      FROM (SELECT p.id,
                   p.name,
                   json_agg(DISTINCT(pr)) as roles,
                   json_agg(DISTINCT(ps)) as skills,
                   json_agg(DISTINCT(lp)) as languages,
                   json_agg(DISTINCT(x)) as shifts
                   FROM people p
     CROSS JOIN LATERAL (SELECT d.date_of_shift,
                                sh.id,
                                sh.name,
                                sh.shift_type_id
                           FROM generate_series('2016-03-07'::date, '2016-03-11', interval '1 day') AS d(date_of_shift)
              LEFT JOIN LATERAL (SELECT shifts.id, shifts.person_id, shifts.date_of_shift, shifts.shift_type_id, shift_types.name
                                   FROM shifts
                                   JOIN shift_types
                                     ON shift_types.id = shifts.shift_type_id
                                ) as sh
                             ON sh.date_of_shift = d.date_of_shift AND
                                sh.person_id = p.id
                   ) as x
 LEFT JOIN LATERAL (     SELECT sk.id,
                                s.person_id,
                                sk.name
                           FROM people_skills as s
                      LEFT JOIN skills as sk
                          ON sk.id = s.skill_id
                    ) as ps
                ON ps.person_id = p.id
 LEFT JOIN LATERAL (     SELECT r.name,
                                r.id,
                                pero.person_id
                           FROM roles as r
                      LEFT JOIN people_roles as pero
                             ON pero.role_id = r.id
                   ) as pr
                ON pr.person_id = p.id
 LEFT JOIN LATERAL (     SELECT l.name,
                                l.id,
                                lape.person_id
                           FROM languages as l
                      LEFT JOIN languages_people as lape
                             ON lape.language_id = l.id
                   ) as lp
                ON lp.person_id = p.id
             WHERE p.department_id = 43
             GROUP BY p.id)
   AS persons
```

####Anhang 5: GUI Mockup

todo

####Anhang 6: ER-Model

todo

####Anhang 7: JSON-response

Die Antwort der API für die Schichtansicht sieht z.B. so aus:

```json
[
  {
    "id": 2,
    "name": "person1",
    "shifts": [
      {
        "date_of_shift": "2016-04-18T00:00:00+00:00",
        "id": 1016,
        "name": "shift_type6",
        "shift_type_id": 7
      },
      {
        "date_of_shift": "2016-04-19T00:00:00+00:00",
        "id": 1017,
        "name": "shift_type4",
        "shift_type_id": 5
      },
      {
        "date_of_shift": "2016-04-20T00:00:00+00:00",
        "id": 1018,
        "name": "shift_type7",
        "shift_type_id": 8
      },
      {
        "date_of_shift": "2016-04-21T00:00:00+00:00",
        "id": 1019,
        "name": "shift_type2",
        "shift_type_id": 3
      },
      {
        "date_of_shift": "2016-04-22T00:00:00+00:00",
        "id": 1020,
        "name": "shift_type2",
        "shift_type_id": 3
      }
    ],
    "skills": [
      {
        "id": 10,
        "person_id": 2,
        "name": "skill9"
      }
    ],
    "roles": [
      {
        "name": "role5",
        "id": 6,
        "person_id": 2
      }
    ],
    "languages": [
      null
    ]
  },
  { }
]
```

####Anhang 8: Pflichtenheft

Der Auszug des Pflichtenhefts gibt wieder, wie die Anforderungen umgesetzt werden soll.

__Umsetzung der Anforderungen__

__A1:__

Die Schichtansicht soll alle Personen einer Abteilung und deren Rollen, Fähigkeiten, Sprachen und Schichten in der dieser Reihenfolgen darstellen. Die Tabelle soll mithilfe von Bootstrap angelegt werden um einen einheitliches Aussehen sicherzustellen, um das zu erreichen wird dem table tag die Bootstrapklasse `table` hinzugefügt.
Der gesamte Schichtplanner soll desweiteren komplett in AngularJS umgesetzt werden.

__A2:__

Der Tabellenkopf soll fixiert sein, um das umzusetzen wird dem table tag die Bootstrapklasse `fixed_headers` zugewiesen.

__A3:__

Die Tabelle soll maximal 60% der Höhe des Bildschirms einnehmen. Dadurch wird sichergestellt das immer alle  Komponenten erreichbar sind. Wenn die Tabelle mehr Zeilen hat, soll die Tabelle scrollbar werden. Das ganze soll in CSS umgesetzt werden.

__A4:__

Über der Tabelle soll ein Dropdownmenu zur Verfügung gestellt werden das es dem Nutzer erlaubt die Personen in einer anderen Abteilung zu betrachten.

__A5:__

Unter der Tabelle sollen Buttons sein die einen per Klick die Schichten der nächsten bzw. vorherigen Woche anzeigen.

__A6:__

Für jede Rolle, Fähigkeit, Sprache und Schicht soll es eine Checkbox geben. Ein Klick auf die Checkbox filtert den Inhalt der Tabelle nach Personen die dieses Kriterium erfüllen.
Wenn man mehrere Kriterien innerhalb einer Kategorie anwählt, sollen diese ODER verknüpft sein. Das bedeuted in dem Fall das die Checkboxen für deutsch und englisch gesetzt sind, werden Personen angezeigt die deutsch _oder_ englisch sprechen.
Falls Kriterien aus unterschiedlichen Kategorien ausgewählt werden, sollen diese UND verknüpft werden. Ein Beispiel wäre, wenn jemand die Checkboxen für Support-Agent und englisch auswählt werden alle Personen angezeigt die diese Kriterien besitzen, allerdings müssen sie nicht nur diese Kriterien haben. Es würden in diesem Beispiel auch Personen angezeigt werden die Support-Agents sind und deutsch und englisch sprechen.

Desweiteren sollen die Kriterien nach Kategorie in Dropdownmenus gruppiert werden, siehe _Anhang 17: Screenshot von den Filteroptionen_.

Kriterien die in der aktuellen Woche nicht auftreten sollen nicht als Filteroption zur Verfügung stehen, z.B. hat in einer Woche niemand Urlaub, dann soll Checkbox für die Urlaubsschicht nicht im Dropdownmenu für die Schichten erscheinen.

__A7:__

Als letzte Filteroption soll es eine Textfeld geben. Die Eingabe wird mit den Namen verglichen, dabei kann sich der gesuchte String irgendwo im Namen befinden. Wenn nach dem Buchstaben 'm' gesucht wird, würden sowohl Namen wie Timon als auch Max angezeigt werden. Die Groß- und Kleinschreibung spielt keine Rolle.

Der gesuchte Name wird auch mit den bereits aktiven Filtern UND vernüpft.

__A8:__



__A9:__



####Anhang 9: Iterationsplan

- Erstellen der Railsapp mit Datenbankstruktur & aller API-Calls
- Erstellen der Angularapp mit Schichttabelle
- Implementierung Authentifizierung und Autorisierung
- Implementierung von erstellen und aktualisieren von Schichten
- Implementierung der Filter für die Schichttabelle
- Implementierung von erstellen, bearbeiten und löschen Personen, Rollen etc.

####Anhang 10: Screenshot vom alten Schichtplanner

####Anhang 11: Screenshot vom neuen Schichtplanner

####Anhang 12: alle API-Calls

 Verb   | URI Pattern                                     | Controller#Action
--------|-------------------------------------------------|---------------------
 GET    | /api/departments                                | departments#index
 GET    | /api/departments/:id/week/:week                 | departments#show
 POST   | /api/departments                                | departments#create
 PATCH  | /api/departments/:id                            | departments#update
 PUT    | /api/departments/:id                            | departments#update
 DELETE | /api/departments/:id                            | departments#destroy
 POST   | /api/people                                     | people#create
 GET    | /api/people/:id                                 | people#show
 PATCH  | /api/people/:id                                 | people#update
 PUT    | /api/people/:id                                 | people#update
 DELETE | /api/people/:id                                 | people#destroy
 POST   | /api/shifts                                     | shifts#create
 GET    | /api/shifts/:id                                 | shifts#show
 PATCH  | /api/shifts/:id                                 | shifts#update
 PUT    | /api/shifts/:id                                 | shifts#update
 DELETE | /api/shifts/:id                                 | shifts#destroy
 GET    | /api/shift_types                                | shift_types#index
 POST   | /api/shift_types                                | shift_types#create
 GET    | /api/shift_types/:id                            | shift_types#show
 PATCH  | /api/shift_types/:id                            | shift_types#update
 PUT    | /api/shift_types/:id                            | shift_types#update
 DELETE | /api/shift_types/:id                            | shift_types#destroy
 GET    | /api/roles                                      | roles#index
 POST   | /api/roles                                      | roles#create
 GET    | /api/roles/:id                                  | roles#show
 PATCH  | /api/roles/:id                                  | roles#update
 PUT    | /api/roles/:id                                  | roles#update
 DELETE | /api/roles/:id                                  | roles#destroy
 GET    | /api/people_filter_criteria/:dept_id/week/:week | filters#people

####Anhang 13: SQL-query für alle Filterkriterien

```sql
SELECT row_to_json(result) as filter_criterias
FROM (SELECT (SELECT json_agg(roles) AS roles
        FROM (SELECT r.name, r.id
              FROM roles AS r
              WHERE r.id IN (SELECT pr.role_id
                              FROM people_roles AS pr
                              JOIN (SELECT p.id
                                      FROM people AS p
                                     WHERE p.department_id = ?
                                   ) AS  p
                                ON p.id = pr.person_id))
              AS roles),
       (SELECT json_agg(skills) AS skills
        FROM (SELECT s.id, s.name
              FROM skills AS s
             WHERE s.id IN (SELECT ps.skill_id
                              FROM people_skills AS ps
                              JOIN (SELECT p.id
                                      FROM people AS p
                                     WHERE p.department_id = ?
                                   ) AS  p
                                ON p.id = ps.person_id
                          GROUP BY ps.skill_id
                          ORDER BY ps.skill_id)
                      )
        AS skills),
       (SELECT json_agg(languages) as languages
        FROM (SELECT l.id, l.name
              FROM languages AS l
             WHERE l.id IN (SELECT lp.language_id
                              FROM languages_people AS lp
                              JOIN (SELECT p.id
                                      FROM people AS p
                                     WHERE p.department_id = ?
                                   ) AS  p
                                ON p.id = lp.person_id
                          GROUP BY lp.language_id
                          ORDER BY lp.language_id)
                      )
        AS languages),
       (SELECT json_agg(shifts) as shifts
        FROM (SELECT st.id, st.name
              FROM shift_types as st
             WHERE st.id IN (SELECT sh.shift_type_id
                               FROM shifts as sh
                              WHERE person_id IN (SELECT p.id
                                                    FROM people as p
                                                   WHERE p.department_id = ?)
                                    AND
                                    sh.date_of_shift BETWEEN ? AND ?
                           GROUP BY sh.shift_type_id)
                     ) as shifts)) as result
```

####Anhang 14: Use-Case Description

__Akteur__

- normaler Mitarbeiter
- Teamleiter

__Vorraussetzungen__

- internetfähiges Gerät
- Webbrowser installiert
- Zugang zum Internet

__Ziele__

- betrachten einer bestimmten Schicht
- zuweisen einer Schicht
- aktualisieren oder erstellen einer Person, Schicht, Abteilung, Sprache, Rolle, Fähigkeit oder eines Schichttypen
- löschen einer Person, Schicht, Abteilung, Sprache, Rolle, Fähigkeit oder eines Schichttypen

__führt zum Fehlschlag__

- eingegebene Daten entschprechen nicht den Regeln

__Erweiterungen__

- Fehlermeldung

####Anhang 15: Use-Case Diagram

atm in extra file

####Anhang 16: Screenshot von der Auswahl einer Schicht

####Anhang 17: Screenshot von den Filteroptionen
