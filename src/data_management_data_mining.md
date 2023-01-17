# Data-Mining Grundprinzipien
Data Mining ist die `Anwendung von systematischen Methoden zum Durchsuchen von Datenbeständen`.
Dabei geht es um das `Entdecken nicht offensichtlicher Zusammenhänge oder Muster in den Daten`.

Das Data Mining ist entstanden aus:
* Klassischer Statistik (Regressionsanalyse, Standardverteilung)
* Künstlichen Intelligenz-Forschung
* Maschinellen Lernen (Neuronale Netze)
* Datenbanksysteme
* Information-Retrieval

## Methoden und Aufgaben
Zu Beginn braucht es einen `ETL-Prozess welcher die Daten entsprechend vorbereitet`, anschiessend sind folgende Dinge möglich:
* Exploration - Keine Vorstellung von der Suchaufgabe, man sucht nach potentiell Interessantem
* Bestätigende Analyse - Hierzu braucht es eine zu beweisende Vermutung
* Prognose - Frühwarnsysteme, Risikoanalyse
* Präsentation - Fakten verdeutlichen und visuell aufbereiten

## Informationsvisualisierungen
Die Ursprünge der Informationsvisualisierung gehen bis ins Jahr 1854 zurück. John Snow konnte mit Stift, Papier und einer
selbst gezeichneten Karte von London den Cholera Ausbruch auf eine Wasserpumpe eingrenzen, indem er die infizierten Wohnorte
auf der Karte markierte.

### Koordinatensysteme
Koordinatensysteme eignen sich gut für `Vergleichsdarstellungen`. Jedoch muss Vorsicht bei der `Wahl des Stichzeitpunkts` geboten werden, da dieser den Eindruck beeinflussen kann.
Koordinatensysteme können auch einen `gleitenden Durchschnitt` haben, dies ist vorallem bei Alarmfunktionen sinnvoll.

### Interaktive 3D-Darstellungen
Tools wie RapidMiner erlauben auch die 3D Darstellung von Daten als Punktewolke

### Heatmap
Bei der Heatmap werden Häufigkeiten oder hohe Werte mit den Farben rot (heiss) und grün (kalt) codiert.
Im Data-Mining ist dies eine Methode `zur Cluster-Darstellung`.

### Gazeplot
Ist eine spezielle Darstellung für `Eyetracking-Ergebnisse`. Hierbei bekommt `jedes Einzelexperiemnt eine eigene Farbe`.
Anschliessend werden Kreise dargestellt, wobei der Radius von der `Aufenthaltsdauer` abhängig ist. Diese Kreise sind auch nummeriert.

### Streumatrix/Scatterplotmatrix
Jedes Objekt ist ein Punkt, welcher einer `Objektklasse zugeordnet wird`. Jede Objektklasse hat dabei eine eindeutige Farbe.

### Parallel Koordinaten
Wird eingesetzt um `Ansätze für Detailbetrachtung zu finden und Ausreisser zu identifizieren`. Kann gut eingesetzt werden, wenn `viele Objekte viele Attribute haben`.
Die `Vorteile dieser Darstellung` sind:
* Zusammenhänge erkennen
* Durchschnitte erkennen
* Übersicht über Streuungseigenschaften

Die `Nachteile` sind:
* kein direkter Vergleich zwischen Objekten möglich
* kein einzelnes Objekt erkennbar

### Ikonografische Darstellung
Die Idee hinter dieser Darstellung ist es `Icons in ein Koordinatensystem zu zeichnen` und `weitere Daten in das Icon zu kodieren (Candlesticks als Icons)`.
Eine weit verbreitete Darstellung in der beschreibenden Statistik ist hierbei die `Quartil-Darstellung`.

### Semantic-Faces nach Chernoff
Objekte im Koordinatensystem sind `Gesichter`. Die Attribute dieser Objekte `spiegeln sich in den Gesichtszügen wieder`.

### Kreisdiagramme
Kreisdiagramme werden oft eingesetzt um `Windverhältnisse zu erfassen`.

### Dashboards
Dashboards sollen `die wichtigsten Informationen auf einen Blick ersichtlich machen`.

## Anwendungsfelder

### Customer Relationship Management (CRM)
Per Data Mining können beispielsweise `vielversprechende Kunden` evaluiert werden. Zudem kann auch der `Abwanderungsrate` mithilfe von neuronalen Netzen entgegengewirkt werden.

### Betrugsanalse (Fraud Detection)
Logische Regression zur `Identifikation der Charaketristiken von Betrugsfällen` einsetzen.

### Finanzwirtschaft
Preisbewertung von festverzinslichen Wertpapieren

### Neue Anwendungsfelder
* Spam-Erkennung
* Forensik
* Personalisierung von Diensten im E-Commerce

## Durchführung des Data Mining Prozesses
* Entwicklung eines `Problemverständnis`
* Erschliessung von Datenquellen (Extract)
* Data-Cleaning und Vorverarbeitung (Transform)
* Auswahl der Data-Mining-Aufgabe
* Auswahl der Data-Mining-Algorithmen
* Anwendung der Algorithmen auf die Aufgabe (Load)
* Wiederholung der oberen Schritte falls notwendig
* Ergebnisse verwenden

## Machine Learning
Im Machine Learning werden folgende Verfahren angewendet:
* Regression
* Klassifizierung
* Clustering
* Natural Language Processing

### Regression
Die Regression versucht eine `Kurve zu ermitteln, welche durch möglichst viele Punkte hindurchgeht`.
Die einfachste Form dieser Kurve ist `f(x) = a * x + b`, es gibt aber auch nicht-lineare Modelle.

Bei der Regression können zwei Effekte auftreten. `Underfitting` tritt auf, wenn das `Modell zu grob ist und zu wenig Eigenschaften abbildet`.
`Overfitting` tritt auf, wenn `das Modell zu fein ist und zu starkt versucht ein korrektes Ergebnis zu erreichen`.

### Klassifizierung
Die Klassifizierung versucht `Punkte aufgrund von Eigenschaften an bestimmte Klassen zuzuordnen`. Bei der Klassifizierung stellt sich die Frage, `welche Eigenschaften herangezogen werden können`.
Beispiele für Klassifikationen sind:
* Kauf eines Produktes
* Brustkrebs
* Spam-Email Erkennung

### Clustering
Beim Clustering geht es darum `Clusterzentren in einer Menge von Datenpunkten zu finden`.

### Natural Language Processing
Die Hauptfunktion von NLP ist es `Informationen aus einem Text zu extrahieren`, typische Aufgaben hierbei sind:
* E-Mail Adressen aus einem Text extrahieren
* Sentimentanalyse auf einem Textkorpus (Stimmung bewerten)
* Named-Entity Recognition
* Automatisches Erzeugen von Abstracts
* Automatisches Übersetzen

## Modellbildung
Bei der Modellbildung wird zwischen zwei Arten unterschieden.

### Unsupervised Learning
Ist eine Modellbildung `ohne Ziel oder Vorhersage`. Hierunter zählen Aspekte wie:
* Clusteranalyse (K-Means, K-Nearest Neighbour)
* Topic Detection (Text-Mining)

#### K-Nearest Neighbour
Ein Element wird einem Cluster zugewiesen, wenn sich `die Mehrheit bereits in der Nähe befindet`.
Hierbei können jedoch Probleme auftreten, wenn zwei Cluster ineinander verlaufen. Dieses Verfahren funktioniert daher
nur, wenn `gute und repräsentative Cluster vorhanden sind`.

#### K-Means
Cluster `müssen bereits vorhanden sein und einen Mittelpunkt aufweisen`. Das Element wird demjenigen Cluster zugewisen, dessen `Mittelpunkt näher ist`.
Auch hier gibt es `Probleme, wenn Cluster unterschiedlich streuen`.

### Supervised Learning
Ist eine Modellbildung `mit einem bestimmten Ziel oder einer bestimmten Vorgabe`. Hierunter zählen:
* Regressionsanalyse
* Entscheidungsbäume
* Neuronale Netze
* Topic Classification (Text-Mining)

Grundvoraussetzung für ein Supervised Learning ist ein `entsprechend gelabelter Datensatz, bei welchem ein Experte Vorgaben gemacht hat`.
Das Modell soll die vorgegen Daten (auch Learning-Target genannt) möglichst genau reproduzieren.

Ein bekanntes Beispiel ist die Frage `Können wir heute Golf spielen?` Diese Frage kann mithilfe eines `Entscheidungsbaumes` beantwortet werden.

#### Naive-Bayes-Classifier
Der Satz von Bayes `definiert den Umgang mit bedingten Wahrscheinlichkeiten`. Dabei ist er weniger anschaulich als ein Decision Tree aber dafür genauer.

## Neuronale Netze
Das Vorbild für das neuronale Netz `ist das menschliche Gehirn`. Die Idee hierbei ist, dass `Nervenzellen im Computer simuliert werden`.

### Perceptron
Ist ein mathematisches Modell eines `Neurons` und benötigt eine `Aktivierungsfuntkion`. Eine typische Aktivierungsfunktion ist die `Sigmoid Funktion`.
Bei der Sigmoid Funktion werden negative Werte 0 und grosse Werte 1.

Logische Operatoren wie `AND, OR und NOT` können mit einem Perceptron abgebildet werden, `jedoch nicht das  XOR`.
Die Lösung für dieses Problem sind die `Multiliayer-Perceptrons (MLP) auch Hidden Layers genannt`.

### Grundprinzip
Jede `Eingabe X` beeinflusst `jede Ausgabe Y` mit einem bestimmten `Faktor W`. Diese Gewichte müssen entsprechend trainiert werden und viele `tausend male rotieren`.

## Deep Learning
Deep Learning ist das `Schalten von mehreren Neuronalen Netzen hintereinander` Hierbei sind noch zwei neue Komponenten im Spiel:
* ReLU - Gibt Werte nur ab einer Schwelle weiter
* Softmax - Ähnlich wie Sigmoid, normiert auf den Bereich 0 und 1 hebt grosse Werte hervor und verkleinert kleine Werte

Eine typische Ebenenstruktur im Deeplearning umfasst folgende Komponenten:
* Convolutional-Ebene 1
* ReLU
* Pooling-Ebene
* Convolutional-Ebene 2
* ReLU
* Pooling Ebene
* Dense-Ebene
* Dropout
* Softmax

### Dense Layers
Stellen den Normalfall dar, wo alle Neuronen mit allen Neuronen `der vorherigen Ebene verbunden sind`

### Dropout
Regularisierungsmethode zur Vermeidung von Overfitting, d.h. eine `bestimmte Anzahl von Neuronen wird ausgeschaltet`.

### Probleme
Probleme für das Deep Learning als auch Neuronale Netzte bereiten immer noch `Zeichen und Bilderkennung`.