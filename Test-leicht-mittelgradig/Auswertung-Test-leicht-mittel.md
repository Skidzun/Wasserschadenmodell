# Auswertung mit generierten Verfremdungen
Beide Modelle wurden gegen drei Sets (à 3 Seiten) getestet:
1. unbearbeitete Digitalisate (leichte Wasserschäden, v.a. Bleeding-through)
2. Digitalisate bearbeitet mit smooth radius 15
3. Digitalisate bewarbeitet mit smooth radius 20

Weichzeichnungsradius: Angabe der Pixel, über die weichgezeichnet werden soll

Hier: Radius von 15 soll leichten Wasserschaden simulieren, 20 soll mittelgradigen Schaden simulieren.

## CER
Modell|CER clear|CER smooth 15|CER smooth 20
---|---|---|---
formulary|1.42/1.24|3.03/2.44|8.52/7.72
damaged|1.69/1.27|2.29/1.85|5.58/4.97

Umfang Test: 137 Zeilen, 6.809 Zeichen (6.596 ohne Interpunktion)

## Block Statistics 
### Damaged (20, no punctuation)
Block|Count|Correct|Incorrect|Correct Ratio|Incorrect Ratio
---|---|---|---|---|---
Lowercase Latin alphabet |5035 |4795 |240 |95.23 |4.77
Uppercase Latin alphabet |132 |119 |13 |90.15 |9.85

Häufige Verwechslungen (Ausgabe vs. korrekt):
- ſ für f (f gesamt: 72) = 10 (13,9 %)
- n für m (m gemsat: 157) = 6 (3,8 %)
- l für k (k gesamt: 54) = 10 (18,5 %)

### Formulary (20, no punctuation)
Block|Count|Correct|Incorrect|Correct Ratio|Incorrect Ratio
---|---|---|---|---|---
Lowercase Latin alphabet |5035 |4624 |411 |91.84 |8.16
Uppercase Latin alphabet |132 |118 |14 |89.39 |10.61

Häufige Verwechslungen (Ausgabe vs. korrekt):
- ſ für f (f gesamt: 72) = 22 (30,6 %)
- l für k (k gesamt: 54) = 22 (40,7 %)
- n für m (m gesamt: 157) = 12 (7,6 %)

### Damage (15, no punctuation)
Block|Count|Correct|Incorrect|Correct Ratio|Incorrect Ratio
---|---|---|---|---|---
Lowercase Latin alphabet |5035 |4958 |77 |98.47 |1.53
Uppercase Latin alphabet |132 |128 |4 |96.97 |3.03

Häufige Verwechslungen (Ausgabe vs. korrekt):
- ſ für f (f gesamt: 72) = 6 gesamt (8 %)

### Formulary (15, no punctuation)
Block|Count|Correct|Incorrect|Correct Ratio|Incorrect Ratio
---|---|---|---|---|---
Lowercase Latin alphabet |5035 |4920 |115 |97.72 |2.28
Uppercase Latin alphabet |132 |125 |7 |94.7 |5.3

- ſ für f (f gesamt: 72) = 8 (11,1 %)

### Damaged (GT, no punctuation)
Block|Count|Correct|Incorrect|Correct Ratio|Incorrect Ratio
---|---|---|---|---|---
Lowercase Latin alphabet |5035 |4988 |47 |99.07 |0.93
Uppercase Latin alphabet |132 |129 |3 |97.73 |2.27

### Formulary (GT, no punctuation)
Block|Count|Correct|Incorrect|Correct Ratio|Incorrect Ratio
---|---|---|---|---|---
Lowercase Latin alphabet |5035 |4984 |51 |98.99 |1.01
Uppercase Latin alphabet |132 |130 |2 |98.48 |1.52