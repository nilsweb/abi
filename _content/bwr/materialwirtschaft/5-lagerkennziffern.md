---
title: Lagerkennziffern
date: 2017-05-15
ref: MAT
order: 5
---

Um die Lagerhaltung zu optimieren werden verschiedene Lagerkennziffern zur Beurteilung herangezogen.
Bei allen Rechnungen werden die Prozentsätze der Einfachheit halber als Dezimalzahl verwendet (5% = 0,05).

# Durchschnittlicher Lagerbestand

Dieser gibt an, wie viele Vorräte wir durchschnittlich Lagern.

$$ ∅ Lagerbestand = \frac{Bestellmenge}{2} + Mindesbestand $$

Sofern keine Informationen über die Bestellmenge bekannt sind, ließe sich diese auch so berechnen:

$$ Bestellmenge = \frac{Bedarf}{Bestellhäufigkeit} $$

Bei einem gleichmäßigen Verbrauch oder einer sehr kurzen Periode kann auch diese Formel eingesetzt werden:

$$ ∅ Lagerbestand = \frac{Anfangsbestand + Endbestand}{2} $$

Sind die Zu- und Abgänge allerdings ungleichmäßig, so muss mit dieser Formel gearbeitet werden:

$$ ∅ Lagerbestand = \frac{Anfangsbestand + Monatsendbestände}{13} $$

Berechnet man den durchschnittlichen Lagerbestand in Euro, so erhält man das durchschnittlich gebundene Kapital, welches später gebraucht wird.
Dazu multipliziert man den Bestand mit dem Bezugspreis/Stück.

$$ ∅ Lagerbestand_€ = ∅ Lagerbestand_{St.} * Bezugspreis_{pro \ Stück} $$

**Bewertung**  
Je geringer der Lagerbestand, desto weniger Kosten fallen für das Lager an.
Ein kleiner Lagerbestand ist somit erstrebenswert.
Erreichbar ist dies durch Just-in-Time-Belieferung, kleine Bestellmengen oder einen geringen Mindesbestand.


# Umschlagshäufigkeit

Die Lagerumschlagshäufigkeit gibt an, wie oft der durchschnittliche Bestand pro Jahr umgeschlagen - also wie oft Material verbraucht und durch Neueinlagerung ersetzt - wurde.

$$ Umschlagshäufigkeit = \frac{Jahresverbrauch}{∅ Lagerbestand} $$

Eine Umschlagshäufigkeit von 5 würde bedeuten, dass der betrachtete Stoff dreimal pro Jahr erneuert wurde.

**Bewertung**  
Eine höhere Umschlagshäufigkeit ist vorteilhaft.
Ebenfalls lässt sich das durch einen geringeren Mindesbestand sowie kürzere Beschaffungsintervalle erreichen.
Eine weitere Möglichkeit wäre es, durch Sonderverkaufsaktionen und Marketing-Maßnahmen die Produktion und somit den Verbrauch anzukurbeln.


# Durchschnittliche Lagerdauer

Diese gibt an, wie lange Vorräte durchschnittlich auf Lager sind.

$$ ∅ Lagerdauer = \frac{360}{Umschlagshäufigkeit} $$

**Bewertung**  
Hier treffen die gleichen Aussagen wie beim durchschnittlichen Lagerbestand zu.
Erreichen lässt sich das ebenfalls durch die Maßnahmen zur Erhöhung der Umschlagshäufigkeit.


# Lagerzinssatz

Der Lagerzinssatz beschreibt den Zinssatz den das - durch den durchschnittlichen Lagerbestand gebundene - Kapital, kostet.
Beispielsweise entgehen uns nach dem Kauf der Ware Guthabenzinsen von der Bank.
Analog dazu müssen wir Zinsen aufgrund einer Überziehung des Kontos zahlen.

$$ Lagerzinssatz = \frac{Jahreszinssatz + ∅ Lagerdauer}{360} $$

Der Zinssatz bezieht sich dabei auf das durchschnittlich gebundene Kapital bzw. den durchschnittlichen Lagerbestand in Euro.
Daher gilt für die Berechnung der Lagerzinsen bzw. Kapitalbindungskosten:

$$ Lagerzinsen = ∅ Lagerbestand_€ * Lagerzinssatz $$

**Bewertung**  
Je geringer der Lagerzinssatz, desto weniger Kosten entstehen durch die Lagerhaltung.
Ein kleiner Lagerzinssatz kann z. B. durch eine hohe Umschlagshäufigkeit erreicht werden.


# Lagerkostensatz

Der Lagerkostensatz ist der Prozentsatz der Lagerkosten am durchschnittlich gebundenen Kapital.
Lagerkosten sind z. B. Miete, Versicherungen sowie Personalkosten.

$$ Lagerkostensatz = \frac{∅ Lagerkosten}{∅ Lagerbestand_€} $$

Für die Lagerkosten ergibt sich also folgende Rechnung:

$$ Lagerkosten = ∅ Lagerbestand_€ * Lagerkostensatz $$


# Lagerhaltungskostensatz

Die Lagerhaltungskosten ist die Summe aus Lagerkosten und Zinskosten.
Die Prozentsätze können ebenfalls addiert werden, da sie sich auf den selben Grundwert beziehen.

$$ Lagerhaltungskostensatz = Lagerkostensatz + Lagersinssatz $$

Gleiches gilt auch für die Euro-Beträge:

$$ Lagerhaltungskosten = Lagerkosten + Zinskosten $$
