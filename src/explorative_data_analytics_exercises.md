# Mögliche Aufgaben

## Python Aufgaben
>Schreiben sie einen Generator (Funktion mit "yield"), der aufsteigend ungerade Zahlen ab 20 ausgibt. Rufen sie diesen Generator in einer Schleife auf und speichern sie die ersten 10 Werte in einer Liste. Geben sie davon die Werte 4-7 aus.
```python
def odd_numbers_from_20():
    x = 20
    while True:
        if x % 2 != 0:
            yield x
        x += 1


generator = odd_numbers_from_20()
result = [next(generator) for x in range(10)]
print(result[4:7])
```

>Denken sie sich ihre Lottozahlen für "6 aus 45" aus und speichern sie diese als Liste. Versuchen sie nun mittels eines Zufallsprozesses auch Lottozahlen zu ermitteln und zählen sie die Versuche, bis ihre Zahlen erreicht werden.

```python
import random

lottery_numbers = range(45)
winning_numbers = sorted(random.sample(lottery_numbers, 6))

tries = 0
while True:
    guess = range(45)
    guessed_numbers = random.sample(guess, 6)

    if sorted(guessed_numbers) == winning_numbers:
        print(f"You won the lottery")
        break

    tries += 1    
print(f"You needed {tries} number of tries")
```

> Schreiben sie eine List Comprehension welche Zahlenpaare ausgibt

```python
pairs = [(x, y)
         for x in range(5)
         for y in range(5)]
print(pairs)
```

> Schreiben sie eine List Comprehension welche inkrementelle Zahlenpaare ausgibt

```python
increasing_pairs = [(x, y)                       # only pairs with x < y,
                    for x in range(5)
                    for y in range(x + 1, 5)]
print(increasing_pairs)
```

> Wörter zählen mit Dictionary

```python
document = ["explorative", "datenanalyse", "macht", "spass"]

word_counts = {}
for word in document:
    if word in word_counts:
        word_counts[word] += 1
    else:
        word_counts[word] = 1
```

> Wörter zählen mit Standard Dictionary

```python
from collections import defaultdict

document = ["explorative", "datenanalyse", "macht", "spass"]
word_counts = defaultdict(int)          # int() produces 0
for word in document:
    word_counts[word] += 1
```

> Wörter zählen mit Counter

```python
from collections import Counter

document = ["explorative", "datenanalyse", "macht", "spass"]
word_counts = Counter(document)
```

 
> Erzeugung von Data Frames mit benannten Spalten

```python
import pandas as pd

daten_2_listen = [["CHN", "China", 1398.72],
                  ["IND", "India", 1351.16],
                  ["USA", "US", 329.74]]
daten_2_frame = pd.DataFrame(daten_2_listen, columns=["Kuerzel", "Name", "Einwohner"])
```

> Zugriff auf Data Frame mit Spaltenname

```python
import pandas as pd
daten_2_frame["Name"]
```

> Zugriff auf Data Frame anhand einer bestimmten Zeile

```python
daten_3_frame.loc[3]
```

> Zugriff auf alle Werte innerhalb eines Data Frames anhand von bestimmten Spalten

```python
daten_3_frame.loc[:, ["Kuerzel", "Name"]]
```

> Bedingter Zugriff

```python
daten_3_frame.loc[:, ["Name"]][daten_3_frame["Einwohner"] > 1000]
```

> Data Frames mit numpy erzeugen

```python
import numpy as np
df1 = pd.DataFrame(np.arange(12.).reshape((3, 4)), columns=list('abcd'))
df1
```

> Funktionen auf ganze Spalten anwenden
```python
f = lambda x: x.max() - x.min()

df1.apply(f)
```

> Index auf eine bestimmte Spalte setzen

```python
#gewünscht wäre "years" als Index
df1.set_index("years", inplace=True)
df1
```

> Missing Values in einem Datensatz als Heatmap darstellen
```python
import seaborn as sns
import matplotlib.pyplot as plt


plt.figure(figsize=(10,8))
cols = boston_housing.columns

colors = ["yellow", "blue"]
sns.heatmap(boston_housing[cols].isna(), cmap=sns.color_palette(colors))
```

