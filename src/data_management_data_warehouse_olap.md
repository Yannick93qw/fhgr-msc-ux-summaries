# Data Warehouse und OLAP

## Datenmanagementplan
Der Datenmanagementplan ist die `Grundlage für den Umgang mit Daten` sowie `dokumentierte Anpassungen im Projektverlauf`.
Er `zwingt Personen` zudem sich mid den `Daten` und dem `Life-Cycle` zu beschäftigen und ist ein `Dokument zur Sicherstellung und Einhaltung des Datenschutzes`

Der Datenmanagementplan `ist bei Forschungsförderungen oft Vorraussetzung` und ist zudem wichtig für die `Einschätzung von Ressourcen, Datenschutz und Nachhaltigkeit`.
Der Datenmanagementplan sollte zudem `mit dem Data-Life-Cylce und den FAIR Principles zusammenspielen`.

### Inhalte
* Planning
* Data collection and creation
* Appraisal and selection
* Documentation and metadata
* File formats
* Storage
* Ethics
* Copyright and intellectual property
* Sharing
* Long term management

## Data Warehouse
Eines der Hauptprobleme sind `verteilte Datenbestände`, Abfragen über `über mehrere Datenbanken sind kompliziert` und `Redundanzen werden nicht vermieden`.
Bei `zentralen Datenbanken` besteht ein `hoher Harmonisierungsbedarf` sowie `hoher Aufwand bei der Abfrage`.
Datenbanken `sind gut zur Speicherung strukturierter Daten, nicht für Analyseabfragen geeignet`, hier setzen Data Warehouses an.

Ein Data Warehouse ist eine `themenorientierte, dauerhafte Sammlung von Informationen zur Entscheidungsunterstützung`.

### Data Warehousing
Prozess von der Datenbeschaffung über die Speicherung bis hin zur Analyse.

### OLTP (Online Transactional Processing)
OLTP basiert auf dem `Datenbank Ansatz` und hat folgende Eigenschaften:
* Einfache Abfragestruktur
* Kurze Lese/Schreibtransaktionen
* Meist eine Datenquelle
* Einzeltupelzugriff

### Datenwürfel
Dimensionen und Kennzahlen, Data Mart als "Sicht" aus dem Datenwürfel. Die `Kanten des Würfels stellen hierbei eine bestimmte Dimension (Produkt, Zeit, Verkaufsort) dar.`
2 Dimensionen können in einer Tabelle dargestellt werden, `ab 3 Dimensionen braucht es einen Datenwürfel`.

### Data Mart
Sichten (extra gespeicherte Ausschnitte) aus dem Data Warehouse.

### OLAP (Online Analytical Processing)
OLAP basiert auf dem `Data Warehouse Ansatz` und ist die `erforschende und interaktive Analyse auf Basis des Datenwürfels`.
* Analyse von Daten, Reporting
* Komplexe Abfragestrukturen
* Lange Lesetransaktionen
* Meist mehrere Datenquellen

OLAP sollten `Anforderungen gemäss dem FASMI (Fast Analysis on Shared Multidimension Information) unterstützen`:
* Fast - Kurze Antwortzeiten
* Analysis - Adäquate Schnittstellen
* Shared - mehrere Nutzer
* Multidimensional - multidimensionale Modelle
* Information - vollständige Informationsbereitstellung inkl. Metadaten

### Data Mart
Sichten (extra gespeicherte Ausschnitte) aus dem Data Warehouse für einen `bestimmten Zweck`.
Für einen Data Mart sprechen viele `Gründe`:
* Eigenständigkeit - Daten spezifisch für einen bestimmten Geschäftsbereich
* Datenschutz - Nur bestimmte Gruppen dürfen die Daten sehen
* Lastverteilung - Weniger Belastung des Gesamtsystems, da viele dedizierte Data Marts
* Datenvolumen - Data Marts können aufgrund von spezifischen Informationen schneller und effizienter die Daten verarbeiten
* Mobiler Zugang - Kleinere Strukturen können auch auf mobilen Endgeräten genutzt werden

### Anforderungen an das Data Warehouse
* Unabhängigkeit zwischen Datenquellen und Analsesystem
* Dauerhafte Bereitstellung integrierter und abgeleiteter Daten
* Automatisierung von Abläufen
* Erweiterabrkeit (neue Datenquellen)
* Eindeutigkeit über Datenstruktur, Zugriffsberechtigungen und Prozesse

### Schemas
Für ein Data Warehouse können unterschiedliche Schemas verwendet werden:
* Snowflake Schema - `Eine Dimension wird in mehreren Tabellen dargestellt`, welche über Schlüssel miteinander verbunden werden; Vermeidung von Redundanzen bei aufwendiger Abfragestruktur
* Star-Schema - `Eine Dimension wird genau in einer Tabelle dargestellt`, die Tabellen befinden sich lediglich `in der 1. Normalform`, d.h. `keine Vermeidung von Redundanzen aber schnellere Abfragestruktur`

## Datensicherheit

### Bedrohungen
Bedrohungen können in Unterschiedliche `Kategorien eingeteilt werden`:
* Schwachstelle - Schwäche eines Systems, bzw. `verwundbarer Punkt`
* Verwundbarkeit - Schwachstelle über welche `die Sicherheitsdienste des Systems umgangen werden können`
* Bedrohung - Gezielte Ausnutzung `einer oder mehrerer Schachstellen oder Verwundbarkeiten um Datenverlust etc. zu erreichen`
* Risiko - `Wahrscheinlichkeit` mit welcher ein `Schadensereigniss eintreten kann`

### Gefährdungsfaktoren
* Höhere Gewalt - Blitzschlag, Feuer, Erdbeben
* Fahrlässigkeit - Irrtum, Fehlbedienung
* Vorsatz - Manipulation, Einbruch
* technisches Versagen - Stromausfall, Fehlfunktionen
* organisatorische Mängel - unberechtigter Zugriff, Raubkopie

## Sicherheit
Der Begriff Sicherheit lässt sich auf verschiedene Arten anwenden:
* Funktionssicherheit - `Ist-Funktionalität stimmt mit Soll-Funktionalität überein`, d.h. das System tut immer was es soll
* Informationssicherheit - Dient dem `Schutz vor Gefahren bzw. Bedrohungen`
* Datensicherheit - System soll nur Zustände annehmen, welche nicht eine `unauthorisierten Zugriff auf Systemressourcen und Daten beinhalten`
* Datenschutz - Datenschutz `ist nicht der Schutz der Daten` sondern das `Recht auf informationelle Selbstbestimmung`
* Zuverlässigkeit - System stellt sicher dass die spezifizierten Funktionen `zuverlässig erbracht werden`

## Schutzziele
Schutzziele sind die `zentralen Anforderungen beim Betrieb von sicheren Rechensystemen`.

### Authentizität
Personen müssen `eindeutig einer Identität zuzuordnen sein`. Dies kann durch Eigenschaften wie einem `Fingerabdruck` sichergestellt werden.

### Authorisation
Authorisation = Authentifizierung + Berechtigung

### Datenintegrität
Verhinderung der unauthorisierten und `unbemerkten Veränderung von Daten und Ressourcen`. Dies wird sichergestellt indem `unauthorisierte Schreibzugriffe sowie Integritätsverletzungen erkannt werden (bspw. via Checksumme)`.

Eine Verletzung ist möglich durch:
* unautorisierte Personen (Angriff von aussen)
* autorisierte Personen (Angriff von innen)

### Vertraulichkeit
`Verbergen von Daten`, d.h. nur die berechtigten Personen haben Zugriff. Wird durch `Ver- und Entschlüsselung sowie Zugriffskontrollen sichergestellt`

### Verfügbarkeit
Ist gewährleistet, wenn `authorisierte Personen in der Wahrnehmung nicht unautorisiert beeinträchtig werden`.
Beispiele hierfür sind Stromausfälle, Malware etc.

### Verbindlichkeit
`Kein unzulässiges Abstreiten druchgeführter Handlungen im Nachhinein`, d.h. Handlungen können eindeutig an Personen zugewiesen werden (Protokollierung von Benutzeraktionen).

### Anonymität
`Durchführen von Handlungen ohne Preisgabe der Identität`, dies kann mit folgenden Mitteln erreicht werden:
* Anonymisierung - Veränderung der Daten sodass ein Rekonstruieren nur mit übermässig hohem Aufwand möglich ist
* Pseudonimisierung - Einzelangaben können nicht mehr natürlichen Personen zugeordnet werden

### Vertrauen
Ist `kein klassisches Schutzziel` man ist jedoch von der `Verlässlichkeit und der Zuverlässigkeit einer Person überzeugt`, d.h. sehr subjektiv.


