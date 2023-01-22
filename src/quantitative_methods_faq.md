# FAQ

## Woran kann man nicht brauchbare Items erkennen?
Nicht brauchbare Items erkennt man häufig daran dass:
* Antwortkategorien werden nicht ausgeschöpft
* Extrem schiefe Verteilungen, wo Normalverteilung angenommen wurde
* Hohe Anzahl von fehlenden Werten
* Items lassen sich nicht zu einer Skala zusammenfassen

## Warum sind metrische Skalen sinnvoll?
Eine ganze Reihe von statistischen Vrefahren verlangt, dass `Variablen metrisch sind` und `erhöht somit die Aussagemöglichkeiten`

## Was muss bei sekundären Häufigkeitstabellen beachtet werden?
* Je grösser das Kollektiv, `desto kleiner die Intervallbreite`
* Maximale Anzahl von Kategorien ist 20
* Alle geschlossenen `Intervalle müssen gleich gross sein`
* Bei `Extremwerten im unteren oder oberen Bereich` muss man `offene Intervalle Bilden`

## Welche statistischen Kennwerte gibt es?
Bei den statistischen Kennwerten unterscheidet man zwischen `zentralen Tendenzen und Streuungsmasse`.

## Welches sind beispiele für Masse der zentralen Tendenz?
* Median
* Arithmetische Mittle (Mittelwert)

## Sind Perzentile ein Mass für zentrale Tendenzen?
Nein

## Welche Nachteile haben Quantile, Perzentile etc sowie Variationsbreiten?
Ihre Berechnung beruht nur auf zwei Werten der Verteilung. Für `Ordinaldaten sind sie gut geeignet`, für `intervall- oder verhältnisskalierte Daten sind Streuungsmasse vorzuziehen`.

## Welche Gründe gibt es bei der Quadrierung der Varianz?
* Es interessiert der `relative Abstand zum Mittelwert`
* Vorzeichen sind unwichtig `stärkere Abweichungen werden mehr gewichtet` und werden daher verstärkt, d.h bessere Repräsentation von Streuung

## Welche Methoden zur Reliabilitätsbestimmung gibt es?
* Retest-Reliabilität
* Paralleltest-Reliabilität
* Interne Konsistenz
  * Halbtest-Reliabilität (Test wird in zwei gleich lange Hälften geteilt)
  * Alpha-Koeffizient (Cronbachs alpha)

  Es ist nur dann `sinnvoll, wenn das erfasste Merkmal zeitlich stabil ist`.

## Ab wann können Tests als parallel betrachtet werden?
* Wenn beiden Messungen der `gleiche wahre Wert zugrunde liegt`
* Gleiche Streuungen und gleiche Anteile von wahrer Varianz und Fehlervarianz vorhanden sind

## Welche Vorteile hat die interne Konsistenz bei der Schätzung der Reliabilität?
* Es muss nur eine Messung durchgeführt werden
* Es müssen `keine Parallelformen eines Tests konstruiert werden`
* Erfasstes Mekmal `muss nicht zeitlich stabil sein`

## Was ist das Problem mit Stichproben?
Stichproben sind `nicht repräsentativ für die Gesamtbevölkerung`. Sie sind immer mit gewissen Auswahlkriterien etc. verbunden.

## Wann ist eine Stichprobe repräsentativ?
Sie ist dann repräsentativ, wenn das `Auswahlverfahren keine Elemente der Population in Bezug auf ihre Merkmale bevorzugt hat, d.h. jedes Element hat die gleiche Chancen`.

## Was ist der Designeffekt?
Die Verzerrung in der Repräsentatitivität `gegenüber einer einfachen Zufallsstichprobe`.
* Bei Schulklassen sind Designeffekte bis zu 10 möglich, d.h. es braucht eine 10x grössere Stichprobengrösse für eine vergleichbare Repräsentativität

## Wann kann eine Hypothese verworfen oder beibehalten werden?
Wenn die Irrtumswahrscheinlichkeit \\( \rho < \alpha \\) ist, kann die H0 verworfen werde, ansonsten muss sie beibehalten werden.

## Welche Voraussetzungen braucht es für einen t-Test?
* dichotome Prädikatorvariable (Variable welche eine andere beeinflusst)
* Metrische Variable

## Welche Voraussetzungen braucht es für eine Varianzanalyse?
* Nominalskalierter Prädiktor
* Metrische Variable

## Wie kann festgestellt werden, ob die Zugehörigkeit zu einer Gruppe einen Effekt hat?
Wenn die Varianz zwischen den Gruppen im Vergleich mit der `Innergruppenvarianz` gross ist

## Was ist der Unterschied zwischen der Varianzanalyse und dem t-Test?
* t-Test kann `jeweils nur zwei Gruppenmittelwerte einbeziehen`
* Wendet man den t-Test für `nominalskalierte, nicht-dichotome Variablen an, müssen einzelne Gruppenvergleiche durchgeführt werden`
* Abgesehen von den vielen Tests `summiert sich auch der Alpha fehler`

## Wann können parametrische Tests überhaupt durchgeführt werden?
Es muss eine `normalverteilte Kriteriumsvariable` vorliegen, sonst müssen nicht parametrische Tests durchgeführt werden
