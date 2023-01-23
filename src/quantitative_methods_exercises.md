# Mögliche Aufgaben

## Z-Wert
> Angenommen, Sie haben mit einem Intelligenztest herausbekommen, dass Ihr IQ 125 beträgt. Wie hoch ist der Anteil derjenigen in der Bevölkerung, die einen höheren IQ haben? Der arithmetische Mittelwert der Bevölkerung liegt bei 100 Punkten und die Standardabweichung bei 15 Punkten.
* Ist nur möglich, wenn der IQ `normalverteilt ist`

## Itemschwierigkeit
> In einer Klausuraufgabe erhält man für das Lösen einer Aufgabe einen Punkt(max(xi) = 1), für eine falsche Antwort null Punkte (min(xi) = 0).

* Der Mittelwert für dieses Item beträgt 0.75

\\[
Pi = \frac{\bar{x_i}}{max(x_i)} * 100 = \frac{0.75}{1} * 100 = 75
\\]

Konkret bedeutet dass, dass diese `Aufgabe zu 75% richtig gelöst wurde`.

## Ermittlung optimale Stichprobengrösse
In einem ersten Schritt wird das Effektniveau bestimmt, nehmen wir an wir `wollen kleine Effekte Zuverlässig erkennen`:

\\[
\epsilon = \frac{\bar{x}_A - \bar{x}_B}{s} = 0.2
\\]

Der Mittelwertunterschied entspricht dann

\\[
\bar{x}_A - \bar{x}_B = 0.2s
\\]

Das Konfidenzintervall kann folgendermassen angegeben werden

\\[
0.2s + z_1 - \frac{\alpha}{2}SE > 0 > 0.2s - z_1 - \frac{\alpha}{2}SE
\\]

Anschliessend kann die `Grenze des Intervalls auf einer Seite bestimmt werden`

\\[
0.2s - z_1 - \frac{\alpha}{2}SE = 0
\\]

Wenn wir nun ein `eine Irrtumswahrscheinlichkeit von 5% annehmen erhalten wir für den Standardfehler den Wert 1.96`:

\\[
0.2s - 1.96SE = 0
\\]

Anschliessend setzen wir die Formel für SE ein und erhalten

\\[
0.2s = 1.96 \frac{s}{\sqrt{n}}
\\]

Nach n aufgelöst ergibt sich

\\[
n = (\frac{1.96}{0.2})^2 = 96
\\]

Achtung `dies gilt nur für reine Zufallsstichproben, für Klumpen müssen Designeffekte berücksichtig werden und die Stichprobe ist daher 5-10 mal grösser`.
