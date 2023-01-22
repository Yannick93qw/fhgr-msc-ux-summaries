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
