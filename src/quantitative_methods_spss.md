# SPPS Cheatsheet

## Numerische Variable berechnen
```
numeric alter(f2).
var lab alter "Alter".
exe.
compute alter=2021-H007.
```

## Häufigkeitstabelle ausgeben
```
fre W001R.
```

## T-Test
Independent Samples t-Test unter "compare means"

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
