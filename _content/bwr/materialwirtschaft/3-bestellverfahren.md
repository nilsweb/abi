---
title: Bestellverfahren
date: 2017-05-14
ref: MAT
order: 3
---

Bei der Bestellplanung gibt es zwei relativ ähnliche Verfahren, die angewandt werden können.
Diese sind das Bestellpunktverfahren sowie das Bestellrhythmusverfahren.


# Bestellpunktverfahren

Bei diesem Bestellverfahren wird eine neue Bestellung ausgelöst, sobald der aktuelle Lagerbestand einen vorher festgelegten Bestand - den Meldebestand - erreicht. Dabei ist der Bestellrhythmus[^1] variabel und die Bestellmenge konstant.

> **Beispiel**  
> Der konstante Tagesverbrauch an Kunststoffgranulat beträgt 50kg.
> Sobald wir eine neue Bestellung aufgeben, braucht der Lieferant im Schnitt drei Tage, um diese zuzustellen.
> Wir halten keinen Sicherheitsbestand[^2] in unserem Lager.
> Eine Bestellung umfasst immer 800kg.  
> Berechnen Sie den Meldebestand.

Eine Bestellung á 800kg ist somit für 16 Tage ausreichend. Allerdings können wir unsere Bestellung nicht erst nach 16 Tagen aufgeben, da der Lieferant eine Beschaffungszeit von drei Tagen benötigt. Es ist also nötig, bereits nach 13 Tagen zu bestellen.

Der Meldebestand lässt sich nun wie folgt berechnen:

$$ Meldebestand = Tagesverbrauch * Beschaffungszeit $$

Für unser Beispiel lautet dieser also:

$$ Meldebestand = 50 * 3 = 150kg $$

Es ist also nötig, bei einem Lagerbestand von 150kg eine neue Bestellung abzusetzen.
Grafisch gesehen sieht der Verlauf des Lagerbestands folgendermaßen aus:

{% include vectors/bwr/materialwirtschaft/bestellpunkt_ohne_sicherheit.svg %}

Das Problem hierbei ist allerdings, dass unsere Produktion bei Lieferausfällen stillsteht, da wir keinen Sicherheitsbestand in unserem Lager führen, den wir in einem solchen Notfall anzapfen könnten.

> Wir entschließen uns dazu, einen Sicherheitsbestand von 200kg zu führen.  
> Berechnen Sie den Meldebestand.

Der Meldebestand erhöht sich nun um den angegebenen Sicherheitsbestand. Die Formel lautet nun:

$$ Meldebestand = Tagesverbrauch * Beschaffungszeit + Sicherheitsbestand $$

Auf das Beispiel bezogen bedeutet das:

$$ Meldebestand = 50 * 3 + 200 = 350kg $$

Die Bestellung muss also bereits bei 350kg aufgegeben werden.
Die grafische Repräsentation dazu wäre lediglich eine Verschiebung der sog. *Sägezahnkurve* nach oben:

{% include vectors/bwr/materialwirtschaft/bestellpunkt_mit_sicherheit.svg %}

Weiterhin sind diese Formeln für ein schnelleres Vorgehen bei der Aufgabenbearbeitung wissenswert.

$$ Jahresverbrauch = Anfangsbestand + Zugänge - Endbestand $$

$$ Jahresverbrauch = Tagesverbrauch * Arbeitstage \ pro \ Jahr $$

Ist der Verbrauch konstant, so kann diese Formel auch umgestellt werden, um den Tagesverbrauch zu ermitteln:

$$ Tagesverbrauch = \frac{Jahresbedarf}{Arbeitstage \ pro \ Jahr} $$

Ist dies nicht der Fall, lässt sich der durchschnittliche Tagesverbrauch in einer Preiode auch so berechnen:

$$ ∅ Tagesverbrauch =  \frac{Anfangebestand + Lagerzugänge \ der \ Periode - Endbestand}{Arbeitstage \ der \ Periode} $$

$$ ∅ Tagesverbrauch =  \frac{Lagerabgänge \ der \ Periode}{Arbeitstage \ der \ Periode} $$

Die vollständig beschriftete Zeichnung zu diesem Szenario sieht so aus:

{% include vectors/bwr/materialwirtschaft/bestellpunkt_all.svg %}

1. Beschaffungszeit
2. Bestellrhythmus/-intervall
3. Bestellzeitpunkt
4. Lieferzeitpunkt
5. Sicherheitsbestand/Mindesbestand/eiserner Bestand
6. Meldebestand
7. Höchstbestand
8. Verbrauch zwischen Bestellung und Lieferung
9. Bestellmenge

Auch diese Angaben können jeweils berechnet werden:

$$ Bestellmenge = Höchstbestand - Sicherheitsbestand $$

$$ Bestellrhythmus = \frac{Bestellmenge}{Tagesverbrauch} $$

$$ Höchstbestand = Mindesbestand + Bestellmenge $$

**Vorteile**
- Lagerzugänge und Lagerabgänge erfolgen in gleichmäßig
- die Liefertermine sind flexibel wählbar
- geringe Bindung an Lieferanten, da keine Lieferungen im Voraus vereinbart sind

**Nachteile**
- Bestand muss ständig überwacht werden, damit rechtzeitig eine Bestellung aufgegeben werden kann (EDV-Unterstützung notwendig)
- die Bestellzeitpunkte sind oft unregelmäßig, was zu höheren Bestellkosten führen kann


# Bestellrhythmusverfahren

Beim Bestellrhythmusverfahren hingegen ist die Bestellmenge variabel und der Bestellrhythmus fix.
Der Verlauf des Lagerbestands kann dabei so aussehen:

{% include vectors/bwr/materialwirtschaft/bestellrhythmus.svg %}

Hier wird der Lagerbestand periodisch überprüft und anschließend eine Bestellung initiiert.
Dabei ist der Tagesverbrauch nicht konstant, weshalb sich die Bestellmenge von Bestellung zu Bestellung unterscheidet.

Der Höchstbestand lässt sich hier so berechnen:

$$ Höchstbestand = Sicherheitsbestand + (ÜZ + BZ) * ∅ Verbrauch $$

**Vorteile**
- keine EDV-Unterstützung notwendig
- Planung der Bestellzeitpunkte entfällt, da diese fix sind

**Nachteile**
- Lager wird unterschiedlich ausgelastet
- bei schwankender Produktion ergeben sich hohe Lagerkosten, da hier Kapital gebunden ist
- Abhängigkeit von Lieferanten


<br>

---
[^1]: Zeitraum zwischen zwei Bestellungen
[^2]: Dieser Bestand *muss* immer im Lager vorhanden sein und darf nur in absoluten Notfällen unterschritten werden. Er wird ebenfalls als eiserner Bestand oder Mindesbestand bezeichnet.
