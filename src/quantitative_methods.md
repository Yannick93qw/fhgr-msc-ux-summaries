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

### Trennschärfte
Ermöglicht eine Einschätzung, `wie gut ein Item zwischen Personen mit niedrieger und hoher Merkmalsausprägung trennt`
* Wert liegt zwischen -1 und 1
* Wenn die Trennschärfe = 0 ist, bedeutet das, dass `ein Item mit dem restlichen Test nichts gemeinsam hat`
* Eine `negative Trennschärfe` bedeutet, dass ein `Item genau falsch herum verstanden wurde`
* Wichtig: `Der Wert der Trennschärfe sollte den Wert des Cronbach alpha nicht übersteigen`
* Je `niedriger die Varianz ist, desto höher die Trennschärfe`
