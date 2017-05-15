---
title: Lieferantenmatrix
date: 2017-05-14
ref: MAT
order: 2
---

Sollen mehrere Faktoren bei der Entscheidung der Bezugsquelle einbezogen werden, so ist die Lieferantenmatrix zur Bewertung zu verwenden.
Dazu werden die Lieferanten anhand verschiedener Kriterien wie z. B. Preis, Qualität, Nachhaltigkeit, Zuverlässigkeit, etc. beurteilt, welche unterschiedliche Gewichtung erhalten.

> **Aufgabe**  
> Wir erhalten für Kunstoffgranulat folgende Angebote:
> <br><br>
>
> |                 | Angebot A | Angebot B |
> |                 | --------- | --------- |
> | Listenpreis/kg  | 3,00 €    | 3,20 €    |
> | Rabatt          | ./.       | 10%       |
> | Skonto          | 2%        | ./.       |
> | Transportkosten | frei Haus | 100,00 €  |
>
> <br>
> Zur Beurteilung spielen neben dem Bezugspreis auch die Kriterien Termintreue, Qualität und Nachhaltigkeit eine Rolle.
> Dabei wird der Bezugspreis vierfach gewichtet, die Termintreue nur halb so viel, die Qualität sowie die Nachhaltigkeit einfach.
> <br><br>
> Die Bewertung der Anbieter erfolgt folgendermaßen:  
> Der günstigere Anbieter erhält beim Bezugspreis fünf Punkte, der teurere vier Punkte.
> Bei Anbieter A ist uns bekannt, dass dieser bereits in der Vergangenheit Lieferschwierigkeiten hatte.
> Er erhält daher nur drei Punkte. Anbieter B bekommt doppelt so viele.
> Die Qualität des Anbieters B ist allerdings geringfügig schlechter. Hier werden nur zwei Punkte vergeben, während A drei bekommt.
> Da sich beide Anbieter als nachhaltig bekannt sind, wird dies gleich gewertet.
> <br><br>
> Ermitteln Sie, welches Angebot bevorzugt werden soll.

Aus dem vorher durchgeführten [Angebotsvergleich]({{ baseurl }}/bwr/materialwirtschaft/1-angebotsvergleich/) ist uns bekannt, dass Angebot A (882,00 €) günstiger als Angebot B (964,00 €) ist.

Die Lieferantenmatrix sähe für dieses Beispiel so aus:

|                | Gewichtung | Punkte A | Gesamt A | Punkte B | Gesamt B |
| -------------- | :--------: | :------: | :------: | :------: | :------: |
| Bezugspreis    | 4          | 5        | 20       | 4        | 16       |
| Termintreue    | 2          | 3        | 6        | 6        | 12       |
| Qualität       | 1          | 3        | 3        | 2        | 2        |
| Nachhaltigkeit | 1          | 1        | 1        | 1        | 1        |
| **Gesamt**     |            |          | **30**   |          | **31**   |

Zuerst wird die Gewichtung eingetragen. Diese kann der Aufgabenstellung entnommen werden.
Als nächstes werden nach Anweisung die Punkte vergeben und in die jeweilige Spalte geschrieben.
Die Nachhaltigkeit wurde hier gleich gewertet. Daher erhalten beide Anbieter die gleiche Punktzahl oder kann weggelassen werden.
Um nun die Gesamtpunktzahl zu ermitteln, wird folgendermaßen gerechnet:

$$ Punkte_{gesamt} = Gewichtung * Punkte_{einfach} $$

Diese werden nun aufsummiert und miteinander verglichen.
Der Anbieter mit der höheren Punktzahl (hier Angebot B) erhält den Auftrag.

Es stellt sich nun nur noch die Frage, wie wir unsere Bestellung bei diesem Anbieter optimieren können.
Dafür wird die [optimale Bestellmenge]({{ baseur }}/bwr/materialwirtschaft/3-optimale-bestellmenge/) herangezogen.
