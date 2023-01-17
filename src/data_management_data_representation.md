# Erhebungen und deren Datenrepräsentation

## RDM vs ODM
RDM steht für `Research Data Management` und zeichnet sich durch folgende Eigenschaften aus:
* Forschungsdatenmanagement
* Zielrichtung ist das `Testen und Wiederlegen von Thesen und Theorien`
* Verfolgung eines offenen Ansatzes (OpenData, OpenScience)

ODM steht für `Operational Data Management` und zeichnet sich durch folgende Eigenschaften aus:
* Betriebliches Datenmanagement
* Befasst sich mit Daten, welche `in einem Betrieb anfallen`
* Effektive Managen von Prozessen und das Erwirtschaften von Mehrwert, d.h. Daten werden oft unter Verschluss gehalten da diese Geschäftsgeheimnisse betreffen

## Nicht klar zugeordnete Daten
* Administrative Daten (Ämter und Verwaltung)
* Prozessdaten (Daten welche in einem Prozess entstehen und nicht das Ziel des Prozesses waren)
* Metadaten (Daten über Daten)

## Data Life Cycle
Wenn Daten richtig behandelt werden, haben diese `auch einen entsprechenden Wert`.
Wichtig hierbei ist, dass `nicht nur kurzfristige Verwertung` der Daten angestrebt wird, es sollte als Lebenszyklus
mit verschiedenen `Phasen` angesehen werden:
* Evaluate and Specify Needs
* Design and Redesign
* Build and Rebuild
* Collect
* Process and Analyse
* Archive, Preserve and Curate
* Data Disseminiation and Discovery
* Research Publish
* Retrospective Evaluation

## Erhebungsdesign
Im Erhebungsdesign können unterschiedliche `Typen von Erhebungsdaten` anfallen:
* Befragungsdaten - Daten werden gezielt für die Beantwortung von Forschungsfragen erhoben
* Administrativeaten - Daten, die in administrativen Prozesse entstehen
* Statistikdaten - Gezielt für die Erstellung von Statistiken (Bundesamt für Statistik) gesammelte Daten
* Prozessdaten - Daten die in Prozessen anfallen, beispielsweise Sensordaten

Grundsätzlich läuft das `Erhebungsdesign nach folgenden Schritten ab`

### Wahl des Forschungsproblems
Oftmals muss für eine komplexe Fragestellung im Vorfeld zuerst eine `Studie durchgeführt werden`.
Fragestellungen können sich jedoch auch auf einen `bestimmten Teilaspekt fokussieren und kleinteiliger sein`.

### Theoriebildung
Theorien bilden die  `Grundlage für die Ausformung von Erhebungen`. Mithilfe der Theorie können `Hypothesen gebildet` und `später getestet werden`.

### Erhebungsdesign
Es muss ein `grosser Aufwand in die Beantwortung der Frage, wie eine Umsetzung in Daten erfolgt` investiert werden.
Es müssen entsprechende Fragestellungen, Skalen und Umfragen vorbereitet und entsprechend durchgeführt werden.
Auch muss man sich Gedanken über die `Auswahl der Untersuchungsobjekte und Sampling machen`
Für die eigentliche `Erhebung können folgende Datenerhebungstechniken` eingesetzt werden:
* Befragungen (Interviews, Fragebogen)
* Tests (schriftlich, computergestützt)
* Beobachtungen

Hierbei muss auch eine Unterscheidung erfolgen, ob `quantitativ (hohe Fallzahl) oder qualitativ (geringe Fallzahl)` gearbeitet werden soll.

## Durchführung von Erhebungen

Für die eigentliche Erhebung der Daten können auch `Erhebungsinstitute eingesetzt werden`, diese übernehmen:
* Schulung von Interview-Personal
* Aufbereitung von Dokumenten (Studieninfo)
* Überprüfung der Übereinstimmung mit dem geplanten Sampling
* Sicherung der Daten

Eine weitere Möglichkeit ist das `Feldmonitoring`. Hierbei ist es wichtig, dass die Kontrolle und Dokumentation der Feldarbeit
sorgfälltig gemacht wird. Kam es bei der Erhebung zu Fehlern, können diese ausgeglichen werden. Das Feldmonitoring sollte
zudem durch `digitale Tools` unterstützt werden.

## Datenrepräsentation
Daten können in unterschiedlichen `Formen und Formaten` daherkommen:
* Binär (0 und 1)
* JSON
* Matrixfiles
* Häufigkeitsverteilungen

Für das Datenmanagement ist nebst den standardisierten Abläufen auch die `Frage nach der Darstellung der Daten wichtig`.
Für eine optimale Verarbeitung dieser Daten werden oft `verschiedene Systeme miteinander kombiniert`, hier spricht man dann von `Polyglot`.

## Datenschutz
Ein bekanntes Modell um den Datenschutz zu gewährleisten ist das `Five Safes Framework`. Hierbei ist es wichtig zu verstehen dass ein optimaler
Datenschutz `durch die Kombination` der einzelnen Frameworkbestandteile erreicht werden kann.

### Safe Data
Hier geht es um `Anonymisierung von Datenbeständen`, sodass `keine Individuen Re-Identifiziert` werden können.

### Safe Projects
Projekte müssen durch einen `Datenmanagementplan` beweisen, dass `keine Datenschutzgefahr besteht`. Vorallem bei Themen wie `Datenzugriff` kann es zu Konflikten in den Bereichen `Dateneigentum` und `Freiheit der Forschung` kommen.

### Safe People
Personen müssen entsprechend gegen `Datenschutzverstösse geschult werden`. Hierbei ist auch auf `unterschiedliche Personengruppen` zu achten.
In der Wissenschaft steht bei einem Datenschutzverstoss die Karriere auf dem Spiel.

### Safe Settings
Mit den Daten sollte nur in sicheren Umgebungen wie im `eigenen Büro oder Labor` handiert werden (standardisierter Datenschutzraum für die Arbeit mit Daten).

### Safe Outputs
Datensätze können datenschutzrelevante Informationen enthalten. Bei der `Veröffentlichung der Daten müssen diese entfernt werden`.

### Anonymisierung
Für die Anonymisierung wreden `meistens Kateogrien` gebildet. Es werden somit genaue Angaben wie Alter, Einkommen etc. in Gruppen zusammengefasst.
Dies zerstört jedoch unter Umständen kostbare Datenbestände. Daher sollte schon bereits vorher mit dem Five Safes Framework Hand angehoben werden.

Bei der Anonymisierung gibt es folgende Varianten:
* Formal anonym - direkte Identifizierung ist durch `Pseudonymisierung ausgeschlossen`
* Faktisch anonym -  De-Anonymisierung ist nicht ausgeschlossen, jedoch `nur mit sehr hohem Aufwand möglich`
* Absolut anonym - Daten wurden gelöscht oder zusammengefasst, d.h. ist keine Re-Identifizierung möglich

## Datenzugang
Eine Möglichkeit den Datenzugang zu sichern ist `Secure Remote Access`:
* Sicheres Remote Access Device (PC mit Bildschirm und Tastatur)
* Research Data Center, welches die Authentifizierung und den Datenzugriff regelt
* Remote Access Device schickt Maus und Tastatureingaben an das Data Center und sieht das Ergebnis auf dem Bildschirm

## FAIR Principles

### Findable
Die Daten sollten entsprechend auffindbar sein:
* DOI (Digital Object Identifier) welches den Namen, die URL sowie Metadaten beinhaltet
* Suchbar über eine Online Suchmaschine

### Accessible
Personen oder Maschinen sollten Zugriff auf die Daten haben. FAIR bedeutet `jedoch nicht dass die Daten offen zur Verfügung gestellt werden`.
Jedoch sollten zumindest die Metadaten vorhanden sein, selbst dann wenn kein freier Zugriff auf die Daten möglich ist.

### Interoperable
Sowohl die Daten als auch die Metadaten sollten sich an `standardisierte Datenformate` halten. Dies erlaubt eine einfache `Kombination und Weitergabe`.

### Reuseable
* Daten sollten genau beschrieben sein und die entsprechend relevanten Attribute auflisten
* Daten haben eine klar verständliche Nutzungslizenz hinterlegt
* Es ist verständlich wie und von welcher Person die Daten erstellt und verarbeitet worden sind 
