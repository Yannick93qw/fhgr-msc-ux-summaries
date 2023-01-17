# Dokumentenamangement
Ein erster Schritt in Richtung Dokumentenmanagementsystem wurde mit der Einführung `von Hypertext gemacht`.

## Hypertext
Einzelne Texte wurden in kleinere Textknoten unterteilt, welche untereinander verlinkt werden konnten.

## CERN - World Wide Web
Die Grundindee hinter CERN war eine "elektronische Zeitschrift" für Hochenergiephysik.
Tim Berners Lee Entwickelte daraus das WWW (World Wide Web), dieses bringte aber gewisse `Limitationen` mit sich:
* Prinzip dass Links in Dokumenten eingebettet sind funktionierte nicht, Links sind `eigenständige Objekte (siehe Hypertext)`
* Keine Trennung von Design und Inhalt
* WWW kennt nur Point and Klick, Sessions müssen separat über Cookies gelöst werden
* Information Retrieval wurde völlig vergessen

## Information Retrieval
Ist ein Entscheidungsprozess, welcher die `Ähnlichkeit zwischen der Repräsentation der Suchanfragen und der Repräsentation der Informationseinheit bestimmt`
Information Retrieval ist `zwischen der Suchanfrage und den Daten` und versucht die Suchanfrage zu verstehen und die gewünschten Daten zurückzuliefern.

### Indexierung
Information Retrieval funktioniert mithilfe einer Indexierungssprache, Beispiele für Indexierungssprachen sind:
* Abstracts
* Freige Schlagworte
* Dokument-Attribute
* Relevanzurteile eines Endnutzers

Basiernd auf Indexierung gibt es einige `kommerzielle Online-Produkte`:
* Bibliografische Datenbanken (Referenzdatenbank)
* Faktendatenbank
* Volltextdatenbanken

In diesen Datenbanken kann mithilfe von `Satzattributen` gesucht werden:
* AU: Author
* TI: Titel

### Invertierter Index
Eine Möglichkeit um Information Retrieval umzusetzen ist der `invertierte Index`. Hierbei wird pro Sachgebiet gespeichert, in welchen Dokumenten dieses vorkommt.

### Automatische Indexierung
Eine weitere Möglichkeit besteht darin eine automatische Indexierung zu implementieren:
* Entgegennehmen der kompletten Suchanfrage
* Wortgrenzen ermitteln (Satzzeichen und Umbrüche wegmachen)
* Stoppworte ermitteln
* Reduktion

Was am Ende übrig bleibt ist ein entsprechender Begriff, welcher wieder in die Datenbank geschrieben werden kann.

### Modi der Reduktion
Grundsätzlich gibt es drei verschiedene Modi wie Texte reduziert werden können:
* Lemmatisierung / Lexikografische Grundform - Form, in welcher das Wort `im Wörterbuch zu finden ist`
* formale Grundform - Wortfragemente bei denen normale englische und fremdsprache `Flexionsendungen abgetrennt sind`
* Stammform nach linguistischen Prinzipien - Zeichenketten sollen durch `Rekodierung vereinheitlicht werden`

Jedoch behebt die `Reduktion nicht alle Probleme`, so bleiben Probleme bezüglich `Termeigenschaften und ihre Auswirkungen auf die Indexierung bestehen`

### Nutzen für das Information Retrieval
* Wörter werden mithilfe der Reduktionsmodi heruntergebrochen und als `Indexterme` verwendet
* Wörter einer Anfrage werden ebenfalls mit den Reduktionsmodi heruntergebrochen, bevor sie mit den Wörtern in der Datenbank verglichen werden

### Named-Entity Recognition
Python-Pakete wie SpaCy erlauben es Entitäten aus einem Text zu erkennen, unter Entitäten sind Dinge wie Personen, Orte, Organisationen, Datumsangaben etc. gemeint

### Boole'sche Retrievalmodell
Der Benutzer drückt die Suchoperation in einer `exakten Retrievalsprache` aus mithilfe von `Termen und Boolescher Logik`.
Schlussendlich wird nur entschieden, ob ein `Dokument ein Match war oder nicht`. Hierbei gibt es folgende Boolesche Operatoren:
* AND (Beide Begriffe müssen passen)
* OR (Nur ein Begriff muss passen)
* NOT (Ein Begriff welcher in einem Dokument vorkommt aber nicht im Anderen)

`Ranking via Boole'schem Retrieval` ist ebenfalls möglich. Voraussetzung hierbei ist jedoch dass die Terme bei der Anfrage oder der Indexierung gewichtet werden.
Schlussendlich erlaubt dieses Verfahren ein Ranking, bei welchem die relevantesten Dokumente `am Anfang stehen`.

### Retrievaleffektivität
Die Ergebnisse einer Suchanfrage können in `vier unterschiedliche Kategorien` eingeteilt werden:
* tp (True positives) - Treffer / relevante Dokumente
* tn (True negatives) - Umgangene oder als "nicht relevant" empfundene Dokumente
* fp (False positives) - "Ballast" bzw. als fälschlicherweise relevant gefundenen Dokumente
* fn (False negatives) - Vermissten und stillen relevanten Dokumente

Hieraus lassen sich wiederum `Precision, Recall und Fallout Ratio berechnen`.

`Precision / Relevanzquote = tp / (tp + fp)`
`Recall / Nachweisquote = tp / (tp + fn)`
`Fallout Ratio / Ausfallquote = fp / (fp + tn)`

### Verbesserung der Indexierung
Eine Möglichkeit die Indexierung zu verbessern, ist die Verwendung eines `Thesauri, bei welchem alle terminologien und Begriffe festgeschrieben sind`.
Eine weitere Möglichkeit ist die Verwendung von `Klassifikationsverfahren`:
* Facettenklassifikation - Wörter werden in der Chemie Notation geschrieben wobei die Chemischen Substanzen entsprechende Bedeutungen haben

Klassifikationen haben `im Retrieval eine hohe Precision` wobei `Thesauri beim Retrieval einen hohen Recall ermöglichen`.

### Termgewichtungsverfahren
* TF (Termfrequenz) - Anzahl wie oft ein Wort im Verhältnis zu allen Wörtern in einem Dokument vorkommt
* DF (Dokumentfrequenz) - Anzahl der Dokumente welche einen bestimmten Term beinhalten im Verhältnis zu allen Dokumenten
* IDF Inverse Dokumentfrequenz - Alle Dokumente im Verhätlnis zu den Dokumenten welche einen bestimmten Term beinhalten

Hieraus kann dann die Termgewichtung innerhalb eines Dokumentes berechnet werden TFIDF = TF * IDF

### Beispiele für Information Retrieval Systeme
* SpaCy (Python Framework)
* Apache Lucene + Solr
* Elastic Search
* Kibana
* Logstash