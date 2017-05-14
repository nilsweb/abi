---
title: Engpassrechnung
date: 2017-04-23
ref: TKR
order: 10
excerpt: >
    Sollten wir aufgrund eines möglichen Engpasses nicht alle Produkte vollständig produzieren können, so gilt es, das optimale Produktionsprogramm zu ermitteln.
---

> **Aufgabe**  
> Über unsere aktuelle Produktion sind Ihnen folgende Angaben bekannt:
> <br><br>
>
> |                       | Golfbälle   | Tennisbälle | Fußbälle   |
> |                       | ----------- | ----------- | ---------- |
> | Nettoerlös/Stück      | 15,00 €     | 20,00 €     | 25,00 €    |
> | variable Kosten/Stück | 8,00 €      | 12,00 €     | 17,00 €    |
> | maximale Absatzmenge  | 5.000 St.   | 3.000 St.   | 2.000 St.  |
> | Produktionszeit M1    | 8 Minuten   | 10 Minuten  | 12 Minuten |
> | Produktionszeit M2    | 12 Minuten  | 4 Minuten   | 5 Minuten  |
> | Erzeugnisfixe Kosten  | 24.000,00 € | 9.600,00 €  | 2.400,00 € |
>
> <br>
> Zusätzlich fallen noch 12.000,00 € unternehmensfixe Kosten an.
> <br><br>
> Die Maschine M1 hat eine Kapazität von 100.000 Minuten, M2 eine Kapazität von 80.000 Minuten.
> Ermitteln Sie das optimale Produktionsprogramm.

# Ermittlung des Engpasses

Zuerst gilt es herauszufinden, ob und auf welcher Maschine ein möglicher Engpass[^1] vorliegt. Dazu rechnet man dies für jede Maschine einmal durch.
Sollte bereits angegeben sein, auf welcher Maschine ein Engpass besteht, so ist dieser Schritt hinfällig.

|             | Maschine M1       | Maschine M2        |
| ----------- | ----------------- | ------------------ |
| Kapazität   | 100.000 Minuten   | 80.000 Minuten     |
| Golfbälle   | 40.000 Minuten    | 60.000 Minuten     |
| Tennisbälle | 30.000 Minuten    | 12.000 Minuten     |
| Fußbälle    | 24.000 Minuten    | 10.000 Minuten     |
| **frei**    | **6.000 Minuten** | **-2.000 Minuten** |

Es liegt also ein Engpass auf Maschine M2 in Höhe von 2.000 Minuten vor. Für die folgenden Schritte müssen wir daher nur diese Maschine beachten.
Sollte kein Engpass vorliegen, so müsste kein optimales Produktionsprogramm ermittelt werden, da alles produziert werden kann.


# Ermittlung des relativen Deckungsbeitrags und der Rangfolge

Als nächstes ist es nötig zu bestimmen, welches Produkt den größten Deckungsbeitrag gesehen auf die verfügbare Zeit erwirtschaftet.
Dazu wird der relative Deckungsbeitrag[^2] $$ db_{rel} $$ herangezogen.

|       |                                                | Golfbälle       | Tennisbälle     | Fußbälle       |
| ----- | ---------------------------------------------- | --------------- | --------------- | -------------- |
|       | Nettoerlös/St. ($$ e $$)                       | 15,00 €         | 20,00 €         | 25,00 €        |
| $$-$$ | variable Kosten/St. ($$ k_v $$)                | 8,00 €          | 12,00 €         | 17,00 €        |
| $$=$$ | **Deckungsbeitrag ($$ db $$)**                 | **7,00 €**      | **8,00 €**      | **8,00 €**     |
| $$÷$$ | Fertigungszeit M2                              | 12 Minuten      | 4 Minuten       | 5 Minuten      |
| $$=$$ | **relativer Deckungsbeitrag ($$ db_{rel} $$)** | **0,58 €**      | **2,00 €**      | **1,60 €**     |
|       | Rang                                           | $$ III $$       | $$ I $$         | $$ II $$       |

Wirtschaftlich gesehen sollten wir somit zuerst die Tennisbälle, anschließend die Fußbälle und zuletzt die Golfbälle (von denen wir dann nicht alle 5.000 Stück produzieren können) herstellen.


# Ermittlung des optimalen Produktionsprogramms

Nun haben wir alle Kriterien zusammen, um das optimale Produktionsprogramm zu ermitteln. Dies geschieht wie folgt:

|             | Menge     | Zeit pro Stück | Zeit gesamt    | Restkapazität  |
| ----------- | --------- | -------------- | -------------- | -------------- |
| Kapazität   |           |                |                | 80.000 Minuten |
| Tennisbälle | 3.000 St. | 4 Minuten      | 12.000 Minuten | 68.000 Minuten |
| Fußbälle    | 2.000 St. | 5 Minuten      | 10.000 Minuten | 58.000 Minuten |
| Golfbälle   | 4.833 St. | 12 Minuten     | 57.996 Minuten | 4 Minuten      |

$$ m_{Golf} = \frac{58.000}{12} \approx 4.833,33 $$

> **Achtung!**  
> In diesem Fall muss die Menge immer *abgerundet* werden!

Es ist jetzt noch mal empfehlenswert, die jeweiligen Stückzahlen einmal sauber aufzulisten. Unser optimales Produktionsprogramm sieht also so aus:

| Produkt     | Menge     |
| ----------- | --------- |
| Tennisbälle | 3.000 St. |
| Fußbälle    | 2.000 St. |
| Golfbälle   | 4.833 St. |


# Ermittlung des Betriebsergebnisses

> Ermitteln Sie auch das Betriebsergebnis.

Sollte dieser Zusatz enthalten sein, so wird einfach eine Teilkostenrechnung für die jeweils ermittelten Stückzahlen durchgeführt.

|       |                                        | Golfbälle       | Tennisbälle     | Fußbälle        | Gesamt          |
| ----- | -------------------------------------- | --------------- | --------------- | --------------- | --------------- |
|       | Nettoerlös/St. ($$ e $$)               | 15,00 €         | 20,00 €         | 25,00 €         |                 |
| $$-$$ | variable Kosten/St. ($$ k_v $$)        | 8,00 €          | 12,00 €         | 17,00 €         |                 |
| $$=$$ | **Deckungsbeitrag ($$ db $$)**         | **7,00 €**      | **8,00 €**      | **8,00 €**      |                 |
| $$*$$ | Produktionsmenge ($$ m $$)             | 4.833 St.       | 3.000 St.       | 2.000 St.       |                 |
| $$=$$ | **Deckungsbeitrag I ($$ DB_I $$)**     | **33.831,00 €** | **24.000,00 €** | **16.000,00 €** |                 |
| $$-$$ | Erzeugnisfixe K. ($$ K_{fE} $$)        | 24.000,00 €     | 9.600,00 €      | 2.400,00 €      |                 |
| $$=$$ | **Deckungsbeitrag II ($$ DB_{II} $$)** | **9.831,00 €**  | **14.400,00 €** | **13.600,00 €** | **37.831,00 €** |
| $$-$$ | Unternehmensfixe K. ($$ K_{fU} $$)     |                 |                 |                 | 12.000,00 €     |
| $$=$$ | **Betriebsergebnis ($$ BE $$)**        |                 |                 |                 | **25.831,00 €** |


# Umrüstzeiten

> Maschine M1 besitzt eine Umrüstzeit von 5 Stunden. Maschine M2 fällt jeweils 3 Stunden zwischen den Produkten aus.

Es kann auch vorkommen, dass zwischen den Produkten die jeweiligen Maschinen umgebaut werden müssen.
Dies muss dann bei der Ermittlung des Engpasses berücksichtigt werden.

|             | Maschine M1       | Maschine M2        |
| ----------- | ----------------- | ------------------ |
| Kapazität   | 100.000 Minuten   | 80.000 Minuten     |
| Golfbälle   | 40.000 Minuten    | 60.000 Minuten     |
| Umrüstung   | 300 Minuten       | 180 Minuten        |
| Tennisbälle | 30.000 Minuten    | 12.000 Minuten     |
| Umrüstung   | 300 Minuten       | 180 Minuten        |
| Fußbälle    | 24.000 Minuten    | 10.000 Minuten     |
| **frei**    | **5.400 Minuten** | **-2.360 Minuten** |

Ebenso werden die Umrüstzeiten am Ende zur Ermittlung des optimalen Produktionsprogramms miteinbezogen.

|             | Menge     | Zeit pro Stück | Zeit gesamt    | Restkapazität  |
| ----------- | --------- | -------------- | -------------- | -------------- |
| Kapazität   |           |                |                | 80.000 Minuten |
| Tennisbälle | 3.000 St. | 4 Minuten      | 12.000 Minuten | 68.000 Minuten |
| Umrüstung   |           |                | 180 Minuten    | 67.820 Minuten |
| Fußbälle    | 2.000 St. | 5 Minuten      | 10.000 Minuten | 57.820 Minuten |
| Umrüstung   |           |                | 180 Minuten    | 57.640 Minuten |
| Golfbälle   | 4.803 St. | 12 Minuten     | 57.636 Minuten | 4 Minuten      |

$$ m_{Golf} = \frac{57.640}{12} \approx 4.803,33 $$

Das optimale Produktionsprogramm lautet also:

| Produkt     | Menge     |
| ----------- | --------- |
| Tennisbälle | 3.000 St. |
| Fußbälle    | 2.000 St. |
| Golfbälle   | 4.803 St. |


# Lieferverpflichtungen

Weiterhin ist es möglich, dass das Unternehmen Lieferverpflichtungen gegenüber bestimmten Kunden besitzt.
Kann es nicht die gewünschte Menge liefern, so muss eine Strafgebühr bezahlt werden. Dies wollen wir natürlich vermeiden.
Daher werden die jeweiligen Lieferverpflichtungen unabhängig der ermittelten Ränge zuerst behandelt.

> Folgende Lieferverpflichtungen sind uns bekannt:
> <br><br>
>
> |       | Golfbälle   | Tennisbälle | Fußbälle   |
> |       | ----------- | ----------- | ---------- |
> | Menge | 4.900 St.   | 200 St.     | 800 St.    |

Das optimale Produktionsprogramm wird dann wie folgt ermittelt:

|                    | Menge     | Zeit pro Stück | Zeit gesamt    | Restkapazität  |
| ------------------ | --------- | -------------- | -------------- | -------------- |
| Kapazität          |           |                |                | 80.000 Minuten |
| Tennisbälle (LV)   | 200 St.   | 4 Minuten      | 800 Minuten    | 79.200 Minuten |
| Umrüstung          |           |                | 180 Minuten    | 79.020 Minuten |
| Fußbälle (LV)      | 800 St.   | 5 Minuten      | 4.000 Minuten  | 75.020 Minuten |
| Umrüstung          |           |                | 180 Minuten    | 74.840 Minuten |
| Golfbälle (LV)     | 4.900 St. | 12 Minuten     | 58.800 Minuten | 16.040 Minuten |
| Tennisbälle (Rest) | 2.800 St. | 4 Minuten      | 11.200 Minuten | 4.840 Minuten  |
| Fußbälle (Rest)    | 968 St.   | 5 Minuten      | 4.840 Minuten  | 0 Minuten      |
| Golfbälle (Rest)   | 0 St.     | 12 Minuten     | 0 Minuten      | 0 Minuten      |

Somit kann es auch vorkommen, dass höherrangige Produkte nicht vollständig produziert werden können.
Zu beachten ist auch noch, dass die Umrüstzeiten jeweils nur einmal berücksichtigt werden müssen, da wir später in unserer Produktion erst alle Tennisbälle,
dann alle Fußbälle und zuletzt alle Golfbälle herstellen. Das optimale Produktionsprogramm sieht also so aus:

| Produkt     | Menge     |
| ----------- | --------- |
| Tennisbälle | 3.000 St. |
| Fußbälle    | 1.768 St. |
| Golfbälle   | 4.900 St. |

Besonders bei diesem Aufgabentyp ist es nötig, die zu produzierenden Stückzahlen nochmals separat aufzulisten.


<br>

---
[^1]: Sollten wir mehr Produkte absetzen als produzieren können, liegt ein Engpass vor.
[^2]: Der relative Deckungsbeitrag ist der Deckungsbeitrag pro Zeiteinheit, hier also pro Minute. Dazu teilt man den Deckungsbeitrag durch die benötigte Fertigungszeit.
