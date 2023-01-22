# Quantiative Methods

## Begriffsdefinitionen

### Item
> Fragen, Meinungen und Aussagen in einem Test

### Skala
> Eine Zusammenfassung von mehreren Einzelitems zu einem Gesamtkonstrukt. Wird verwendet um mehrere Variablenwerte zu einem Skalenwert zusammenzufassen. Deshalb sind Skalen auch `wesentlich robuster gegen Fehler als Werte von Einzelitems`

### Manifeste Variablen
> Sind Variablen, welche direkt messbar und beobachtbar sind

### Latente Variablen
> Sind nicht direkt Messbar und werden über `manifeste Variablen erschlossen`

### Primäre Häufigkeitstabellen
> Stellt die `Verteilung eines Merkmals dar` und gibt Aufschluss darüber, wie `häufig eine Ausprägung vorkommt`

### Sekundäre Häufigkeitstabellen
> Es werden Merkmalsausprägungen `zu Intervallen zusammengefasst`, dies funktioniert `aber nur bei metrischen Variablen`

### Histogramme
> Stellt die Häufigkeiten oder die prozentualen Häufigkeiten graphisch anschaulich als Säulen dar. Hierbei muss die Y-Skala immer mit 0 beginnen und Säulen dürfen nicht unterbrochen oder verkürzt sein.

### Kreisdiagramme
> Stelt die Häufigkeiten graphisch als Kreisauschnitt dar, wie beim Histogramm kann es auch hier `einen Ausschnitt für fehlende Werte` geben. Achtung `das Kreisdiagramm sollte für Nominalskalen verwendet werden`
### Polygonzug
> Über Säulen wird eine Linie gezogen (jeweils vom Säulenmittelpunkt aus). Achtung `Polygonzüge dürfen nur bei metrischen Variablen verwendet werden`.

### Streuungsmasse
> Sind erst ab `ordinalem Skalenniveau sinnvoll`. Beispiele hierfür sind `Spannweiten, Quartilsabstände, Standardabweichung und Varianz (bei metrischem Skalenniveau)`

### Durchschnittliche Abweichung der Beträge vom Mittelwert
> Gibt Auskunft über die Dispersion, `sagt jedoch noch nichts über die Verschiedenheit der einzelnen Abweichungen aus`.

### Normalverteilung / Standardnormalverteilung
* Bei der Normalverteilung liegen zwischen -1 und +1 vom Mittelwert 68.27% der Gesamtlfäche
* Zwischen +2 und -2 vom Mittelwert liegen 95.45% der Gesamtläche
* Bei einer Normalverteilung sind `Modalwert, Median und arithmetischer Mittelwert identisch`
* Bei einer Standardnormalverteilung ist der arithemtische Mittelwert 0 und die Standardabweichung 1 
* Ermöglicht die Berechnung von `Konfidenzintervallen`

### Z-Wert
* Mithilfe des Z-Wertes kann bestummen werden, wo in der `Verteilung die Werte liegen`

### QQ-Plot
* Kann benutzt werden um eine `statistische Überprüfung der Normalverteilung` durchzuführen.
* Es werden `zwei Variablen` benötigt
* Bei einer Normalverteilung `liegen die Werte auf einer Linie`

### Klassische Testtheorie (KTT)
Die klassische Testtheorie (KTT) besagt, `dass jede Messung sich aus einem wahren Wert und einem zufälligen Messfehler zusammensetzt`. Wichtig hierbei ist, dass die `Messfehler einzelner Items und Personen nicht korrelieren`, d.h:
\\[
\rho(\epsilon_{vi},\epsilon_{vj}) = 0
\\]

Der eigentliche `Messwert setzt sich aus dem wahren Wert und dem Messfehler zusammen`, d.h. \\( Messwert = Wahrer Wert + Messfehler \\)

Hierbei gilt es aber folgendes zu beachten:
* Verteilung der Messwerte sollte schmal sein
* Einzelner Messwert zeigt zuverlässiger den wahren Testwert, wenn die  `Verteilung der Messwerte breit ist`, d.h. der `Standardmessfehler klein ist`

Kurz zusammengefasst bedeutet KTT dass:
* Eine Skala bildet die Summe von Messungen aus verschiedenen Items ab
* Jedes Item sollte das latente Konstrukt gleichermassen gut abbilden
* Für jedes Item `resultiert ein Messwert, der möglichst nah am wahren Wert liegen sollte`

### Itemschwierigkeit
Drückt aus, wie `schwer eine Aufgabe für Personen zu beantworten war`, d.h. wie viele die richtige Lösung erhalten haben.

### Schiefe (v)
* Bei symmetrischen Verteilungen ist die Schiefe = 0
* Linkssteil bedeutet `v > 0`
* Rechtssteil bedeutet `v < 0`
* Schiefe sollte bei Skalenitems nicht > 1 oder < - 1 sein

### Kurtosis
Sollte bei Skalenitems nicht über 8 liegen

### Reliabilität
* Beschreibt die  `Zuverlässigkeit eines Tests`
* Wertebreich von 0 bis 1 (1 = messfehlerfrei)

### Cronbachs alpha
* Test wird in so viele Teile zerlegt wie er Items hat, d.h. `jedes Item wird als Testteil behandelt`
* Anschliesend wird der `Durchschnittswert der Korrelationen aller möglichen Parre von Items berechnet`

### Trennschärfe
Ermöglicht eine Einschätzung, `wie gut ein Item zwischen Personen mit niedrieger und hoher Merkmalsausprägung trennt`
* Wert liegt zwischen -1 und 1
* Wenn die Trennschärfe = 0 ist, bedeutet das, dass `ein Item mit dem restlichen Test nichts gemeinsam hat`
* Eine `negative Trennschärfe` bedeutet, dass ein `Item genau falsch herum verstanden wurde`
* Wichtig: `Der Wert der Trennschärfe sollte den Wert des Cronbach alpha nicht übersteigen`
* Je `niedriger die Varianz ist, desto höher die Trennschärfe`

### Inferenzstatistik
Wird auch als `schliessende Statistik bezeichnet`, hierbei wird von der `Stichprobe auf die Grundgesamtheit` geschlossen:
* Mittelwert einer Stichprobe kann `berechnet werden`
* Mittelwert einer Grundgesamtheit `muss geschätzt werden`, hierbei sind Fehler (Stichprobenfehler) möglich

## Geschichtete Zufallsstichprobe
Die Population wird in `verschiedene Gruppen aufgeteilt, nach einem für die Untersuchung relevanten Merkmal (bpsw. Kantone)`. Aus diesem Grund sind diese Art von Stichproben auch `spezifisch repräsentativ`.

## Klumpenstichprobe
Grundgesamtheit wird in Klumpen (Cluster) eingeteilt (bspw. Schulklasse). Anschliessend wird zufällig von diesen Klumpen ausgewählt. Klumpenstichproben `sind nur eingeschränkt repräsentativ`.

## Stichprobenkennwerteverteilung
Die Streuung aus der Kennwerteverteilung gilt als Mass dafür, wie gut `ein einzelner Stichprobenmittelwert den Populationsmittelwert schätzen kann`.
* Mit dem Stichprobenmittelwert `kann direkt auf den Mittelwert der Grundgesamtheit geschlossen werden` aber ist dabei nicht 100% genau wegen der Streuung

## Standardstichprobenfehler
Ist die `Standardabweichung der Stichprobenkennwerteverteilung`.

## Standardfehler
* Je kleiner, desto kleiner die Varianz \\( s^2 \\) ist
* Je kleiner, desto `grösser die Stichprobe ist`

## Signifikanztests
Bei einem Signifikanztest muss `immer eine Hypothese überprüft werden`, d.h. `kann die Hypothese mit einer genügend hohen Sicherheit verworfen werden`.

## Unterschiedshypothese
* Behauptet Unterschiede zwischen Gruppen auf Mittelwerte oder Häufigkeiten
* Unterscheidung zwischen ungerichtet (behauptet nur dass ein Unterschied besteht) und zielgerichtet (behauptet dass eine Gruppe besser oder schlechter abschneidet als eine andere)

## Zusammenhangshypothese
* Behauptet, dass ein Zusammenhang zwischen Variablen besteht
* Beispiel: "Es besteht ein Zusammenhang zwischen den geleisteten Übungsstunden und dem Prüfungsergebnis"
* Ungerichtet behauptet dass es einen Zusammenhang gibt, gerichtet wiederum ob dieser positiv oder negativ ist

## Hypothesenprüfung
Es werden die Hypothesen `H0 und H1` aufgestellt:
* H1 (Alternativhypothese) behauptet `dass es einen Zusammenhang / Unterschied gibt`
* H0 (Nullhypothese) behauptet `dass es keinen Zusammenhang / Unterschied gibt`

Bei Hypothesenprüfungen ist `ein konservatives Vorgehgen zugunsten der H0 zu bevorzugen`.

## Alpha Fehler
> Bedeutet, dass fälschlicherweise die H0 verworfen wurde

## Beta Fehler
> Bedeutet, dass fälschlicherweise die H1 verworfen wurde
* Kann nur bei `spezifischen Hypothesen bestimmt werden, weil sonst die Verteilung der H1 nicht bestimmbar ist`

## Alpha Niveau
> Legt fest, welche Wahrscheinlichkeit für einen Alpha Fehler noch akzeptabel ist und muss im Vorfeld definiert werden (üblicherweise 0.05 und 0.01, d.h. 5% und 1%).
* Bei gerichteten Hypothesen schneidet das Alpha Niveau nur die `linke oder rechte Seite`
* Bei ungerichteten Hypothesen schneidet das Alpha Niveau `sowohl die link und die rechte Seite und muss deshalb halbiert werden auf jeder Seite`

## t-Test
Untersucht bei `unabhängigen Stichproben`die `Gültigkeit von Unterschiedshypothesen`.
Ein Beispiel hierzu ist die Einteilung in die Geschlechter männlich und weiblich. Hierbei ist das Geschlecht das Merkmal und die Ausprägungen davon wären männlich und weiblich

## Varianzanalyse
Man will herausfinden, `ob Gruppenmittelwerte hinsichtlich einer Kriteriumsvariable (abhängige Variable) signifikante Unterschiede aufweisen`:
* Vergleich zwischen der Varianz `zwischen den Gruppenmittelwerten und der Varianz innerhalb der Gruppen`

## F-Test
Überprüft `ob ein signifikanter Effekt der Gruppenzugehörigkeit besteht`, d.h. ob die Zwischengruppenvarianz im Vergleich zur Innergruppenvarianz signifikant gross ist:
* F-Wert von 1 beduetet dass es `keinen Effekt gibt` (F-Wert kann in F-Tabelle nachgeschlagen werden)
* Wenn F-Wert > 1 bedeutet dass, dass es `signifikante Gruppenutnerschiede` gibt

## Erklärte Varianz
\\(  \eta^2 \\) gibt an welcher `Anteil der Gesamtvarianz durch die Gruppenzugehörigkeit erklärt werden kann`.

## Tukey-Test
Wird verwendet um herauszufinden `welche Gruppen sich voneinander unterscheiden`.

## Signifikanzniveau
Ist die Irrtumswahrscheinlichkeit im Fall, dass man einen Unterschied zwischen den Kategorien hinsichtlich des Kriteriums annimmt
