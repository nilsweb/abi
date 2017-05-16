---
title: Optimale Bestellmenge
date: 2017-05-15
ref: MAT
order: 6
---

Um das Lager weiter zu optimieren, wird versucht, die bestmögliche Bestellmenge zu bestellen.
Dabei ist es in der Praxis meist schwierig, dies umzusetzen, da Lieferanten oft nur in bestimmten Mengen liefern können.

> **Aufgabe**  
> Folgende Angaben sind bekannt:
> <br><br>
>
> | Jahresbedarf            | 1000kg
> | Bezugspreis/Stück       | 20,00 €
> | Lagerhaltungskostensatz | 25%
> | Mindestbestellmenge     | 100kg
> | Mengenerhöhung          | 50kg
> | Höchstbestellmenge      | 300kg
> | Kosten pro Bestellung   | 100,00 €
>
> <br>
> Ermitteln Sie die optimale Bestellmenge.

Hierfür macht man sich eine Tabelle und rechnet für jede Menge einmal durch.
Zur Berechnung der optimalen Bestellmenge wird der Mindestbestand *nicht* berücksichtigt.
Aufgrund der besseren Übersicht werden folgende Abkürzungen verwendet:

| ∅ Lagerbestand          | = | ∅ LB |
| ∅ Lagerwert             | = | ∅ LW |
| Lagerkosten             | = | LK   |
| Bestellhäufigkeit       | = | BH   |
| Bestellkosten           | = | BK   |
| Gesamtkosten            | = | GK   |
| Einstandspreis          | = | EP   |
| Jahresbedarf            | = | JB   |
| Lagerhaltungskostensatz | = | LHKS |
| Kosten pro Bestellung   | = | KPB  |

| Menge | ∅ LB                         | ∅ LW            | LK                | BH                  | BK             | GK            |
| :---: | :--------------------------: | :-------------: | :---------------: | :------------------: | :-----------: | :-----------: |
|       | $$ \frac{Bestellmenge}{2} $$ | $$ ∅ LB * EP $$ | $$ ∅ LW * LHKS $$ | $$ \frac{JB}{BM} $$ | $$ BH * KPB $$ | $$ LK + BK $$ |
| 100kg | 50kg                         | 1.000,00 €      | 250,00            | 10                   | 1.000,00 €    | 1.250,00 €    |
| 150kg | 75kg                         | 1.500,00 €      | 375,00            | $$ 6\frac{2}{3} $$   | 666,67 €      | 1.041,67 €    |
| 200kg | 100kg                        | 2.000,00 €      | 500,00            | 5                    | 500,00 €      | 1.000,00 €    |
| 250kg | 125kg                        | 2.500,00 €      | 625,00            | 4                    | 400,00 €      | 1.025,00 €    |
| 300kg | 150kg                        | 3.000,00 €      | 750,00            | $$ 3\frac{1}{3} $$   | 333,33 €      | 1.083,33 €    |

Die optimale Bestellmenge liegt also bei 200kg, da die Kosten (1.000,00 €) hier am geringsten sind.

Da diese Berechnung relativ aufwendig ist, kann stattdessen auch folgende Formel verwendet werden:

$$ optimale \ Bestellmenge = \sqrt{ \frac{2 * Jahresbedarf * fixe \ Bestellkosten}{Einstandspreis * Lagerhaltungskostensatz} } $$

Für das obige Beispiel ergibt sich somit:

$$ optimale \ Bestellmenge = \sqrt{ \frac{2 * 1000 * 100,00}{20,00 * 25%} } = 200kg $$
