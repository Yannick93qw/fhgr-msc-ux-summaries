# Datenanalyse
Die Datenanalse ist das `primäre Ziel des Datenamangements`. Die Datenanalyse ist `stark abhängig von der entsprechenden Domäne`.
Grundvoraussetzungen für eine Datenanalyse sind `Datenharmonisierung, Datenverbindungen sowie Datendokumentation`.

## Die vier Eckpfeiler des Datenmanagements

### Datenarchitektur
Hier soll die Architektur fomuliert und entsprechend gepflegt werden. Hierunter fällt auch die `Unterstützung der Anwendungsentwicklung bei der Datenmodellierung`.

### Datenadministration
Verwalten von Daten und Funktionen anhand von standardisierten Richtlinien, Normen etc. Hierunter zählt auch die `Beratung von Entwicklern und Ennutzern`.

### Datentechnik
Installieren, Reorganisieren und Sicherstellen von Datenbanken sowie anfälligen Restaurierungen im Fehlerfall.

### Datennutzung
Bereitstellung von Auswertungs- und Reportfunktionen unter Berücksichtigung des Datenschutzes

## Formen der Datenanalyse
* Befragungen
* Statistiken
* Interview
* Social Media
* Sensoren

## Datenharmonisierung und Manipulation

### Datenaufbereitung
In einem ersten Schritt müssen die Daten entsprechend aufbereitet werden, hierzu sind folgende Schritte notwendig:
* Integrate Data
* Classify and Code
* Explore, validate and clean Data
* Input missing Data
* Construct new variables and units
* Calculate weights
* Calculate aggregates
* Anonymize data
* Finalize Data outputs

Die Datenaufbereitung ist einer der `aufwendigsten Phasen im Data Life Cycle`:
* Müssen für den entsprechenden Analysebedarf entsprechend aufbereitet werden
* Umfängliche und zielführende Dokumentation muss erstellt werden
* Langzeitarchivierung von Ahbängigkeiten muss entsprechend eingeplant werden

## Data Linkage
Es gibt drei verschiedene Methoden des Data Linkage:
* Deterministic (Exact) Matching Method - Identifikation `per ID`
* Probalistic Data Linkage - Aufgrund von verschiedenen Faktoren wird ein `potenzieller Match ermittelt`
* Privacy-preserving Record Linkage - Variablen sind `mit Verschlüsselungsverfahren entsprechend geschützt`

### Restriktionen
* Datensätze sind `nicht harmonisiert und können nicht zusammengespielt werden`
* Statistische Methoden zum Linkage sind `zeitaufwendig`
* Datenschutzregeln `können das Verbinden von Daten untersagen`

## Dateninfrastruktur
Infrastrukturen werden von einer Vielzahl von Anbietern angeboten, darunter Google und Amazon. Infrastrukturen
bestehen dabei  `aus verschiedenen Komponenten wie Speicherung und Netzwerke`.

### Grad der Anonymität
Je "näher" an der Quelle sich die Daten befinden, desto weniger sind sie anonymisiert. Hierbei wird noch zwischen `Off-Site-Nutzung` und `On-Site-Nutzung` unterschieden.
Off-Site Nutzung bedeutet, man holt sich die Daten zum Beispiel aus dem Internet, wohingegen On-Site-Nutzung heisst, dass man sich pyhsisch bei den Daten befindet.

### Infrastrukturvarianten
* Secure Remote Access
* European Remote Access Network
* Virtual Research Environment
* European Open Science Cloud

## Metadaten, Paradaten und Zugangsdaten (Social Science)
Bei Metadaten hanelt es sich um `Forschungsdaten`, Paradaten sind `Daten über Erhebungsprozesse` und Zugangsdaten sind `Daten welche den Datenzugang betreffen`.
Forschungsdaten benötigen `zusätzliche Daten um sinnvoll genutzt werden zu können`. Ein Standard ist schwer umsetzbar aber dringend notwendig.

### Metadaten
Ein entspechendes Metadatenkonzept kann anhand der `DDI (Data Document Initiative)` aufgestellt werden.
Daten im Sinne von Metadaten bedeuten `Mikrodaten` wobei der Fokus auf `Sozial und Geisteswissenschaften` liegt.

### Document
Beschreibt die `Quelle der Daten`, die `inolvierten Personen` wie die Daten `erhoben wurden` und `wo auf die Daten zugegriffen` werden kann.

### Discover
Befasst sich mit dem `elektronischen Zugriff auf die Daten` und beinhaltet auch `Detailinformationen über Grösse, Format und Verfügbarkeit`

### Interoperate
Stellt eine `saubere Terminologie und Vokabular` sicher.

### Paradaten
Paradaten sind wie bereits erwähnt `Daten über Erhebungsprozesse`:
* Screen Interatkionen mittels Maus und Tastatur
* Anzahl an Unterbrechungen während eines Interviews
* Anzahl Logeinträge von einer bestimmten Aktivität

### Zugangsdaten
Zugangsbeschreibungen zu schützenswerten Daten über eine `Kombination von festgelegten Werten (siehe 5 Safes)`

## Datenstrukturen
Dateiformate wie `Word oder PDF sind für Menschen gedacht` aber nicht um damit Datenverarbeitung zu betreiben.
Wie Daten richtig strukturiert werden können, ist mithilfe von DDI beschrieben.

### Data Documentation Initiative (DDI)
DDI ist eine `Struktur` um `konsistent Daten und Metadaten zu definieren`. Das Ziel von DDI ist es `eine intelligente Nutzung der Daten über die Zeit zu ermöglichen`.
DDI besteht aus folgenden Komponenten:
* Variable
* Logical Redord - Zeigt auf die relevanten Variablen
* Record Layout - Zeigt auf die entsprechen Logical Records
* Data File - Zeigt auf das Record Layout

DDI wird meist `als XML dargestellt`. Es nutzt die Grundstruktur von XML und `setzt eigene Definitionen ein`.
