# SPPS Cheatsheet

## CSV Datei einlesen
File > Import Data > CSV Data

## Numerische Variable berechnen
```
numeric alter(f2).
var lab alter "Alter".
exe.
compute alter=2021-H007.
```

## Modalwert berechnen
Häufigkeitstabelle ausgeben und dann den Wert nehmen, `der am häufigsten vorkommt`

```
fre <variable>
```

## Median, arithmetischer Mittelwert, Spannweite, Varianz, Standardabweichung, Quartile, Schräge und Kurtosis
Analyze > Descriptive Statistics > Frequencies:
* Variable auswählen
* Statistics... > 
  * Percentile Values > Quartiles
  * Central Tendency > Mean, Median
  * Dispersion > Std. deviation, Variance, Range
  * Distribution > Skewness, Kurtosis

Der Quartilsabstand ist die Differenz vom `25 und 75igsten Percentil`

## Häufigkeitstabelle ausgeben
```
fre W001R.
```

Um eine Häufigkeitstabelle für mehrere Werte zu generieren kann folgender Befehl verwendet werden

```
FREQUENCIES VARIABLES=TK001_01R TK002_01R TK003_01R TK004_01R TK005_01R TK006_01R.
```

## Neue Variable als Skala berechnen
Berechnung wenn nicht mehr `als 2 fehlende Werte auftauchen`

```
numeric TKAllg(f4.2).
var lab TKAllg "Nutzen DK für Allgemeinheit".
var lab Nutzen Allgemeinheit
 1 "Stimme überhaupt nicht zu"
 5 "Stimme voll zu".
 exec.

 compute TKAllg=MEAN.2(<variable_1>,<variable_2>,...).
```

## Q-Q-Plot erstellen
Analyze > Descriptive Statistics > Q-Q-Plot:
* Variable auswählen

## Histogramm erstellen
Analyze > Descriptive Statistics > Frequencies:
* Variable auswählen
* Charts... anklicken
* Histogramms auswählen


## Reliabilitätsanalyse durchführen
Analyze > Scale > Reliability Analysis:
* Statistics...
  * Descriptives for
    * Item
    * Scale
    * Scale if item deleted
  * Inter Item
    * Correlations
  * Summaries
    * Correlations

## T-Test
Independent Samples t-Test unter "compare means"

## Pearson Korrelation
Analyze > Correlate > Bivariate Correlations 

## Tukey-Test / Post-hoc-Test
Analyse > Mittelwerte vergleichen > Einfaktorielle ANOVA:
* `Abhängige metrische Variable` für Analyse (Dependent List) auswählen
* `Unabhängige nominalskalierte Variable` für Analyse (Faktor) auswählen
* Post-Hoc > Tukey auswählen
* Alpha Niveau eintragen (0.05)

## Korrelation
* Analysieren > Korrelation > Bivariat
* Zwei oder mehr Variablen auswählen > ok

## Regression
Analyse > Regression > Linear:
* Abhängige und unabhängige metrische Variablen eingeben
* Bei `stepwise erfolgt die Aufnahme der nächsten Variable nur, wenn diese relevante zusätzliche Varianz erklärt`

## Chi-Quadrat
Der Chi-Quadrat Test kann bei den `Kreuztabellen gefunden werden`.
