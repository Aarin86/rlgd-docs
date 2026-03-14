# RLGD Wirtschaftsmodell — KI-Produktivität wird menschliche Arbeit

## Das Problem

Künstliche Intelligenzen und Automatisierung verdrängen Arbeitsplätze. Analysen gibt es viele. Durchgerechnete Lösungen kaum.

## Der Kernmechanismus

RLGD betreibt ein internes Wirtschaftssystem. Unternehmen (Arbeitsgruppen) setzen KI und Roboter ein, die Überschüsse produzieren. Ein Teil dieser Überschüsse fließt in einen Systempool.

**Sobald achttausend Original Reso im Systempool angesammelt sind, wird automatisch ein neuer menschlicher Mitarbeiter angestellt.**

- Zweitausend Original Reso als Gehalt
- Sechstausend Original Reso als Reserve

Je produktiver die KI, desto mehr Stellen. Das System balanciert sich selbst.

## Drei-Währungen-Architektur

```
EUR (Außenwelt)
 └→ Short Reso (1:1 zum Euro, Brückenwährung)
      └→ Original Reso (inflationsfrei, intern, Referenz: Anfang 2026)
```

- **Euro:** Einstieg. Nutzer zahlen ein, Transaktionsgebühren werden transparent ausgewiesen.
- **Short Reso:** Deckt externe Kosten. Keine Werbung, Kosten werden direkt weitergegeben.
- **Original Reso:** Die interne Werteinheit. Inflationsfrei, spekulationsfrei. Verliert nicht an Wert.

Fünf Prozent Systemabgabe bei Konversion und Haltung finanzieren den Systempool.

## Arbeitsgruppen (Interne Unternehmen)

Einkommen wird in festen Stufen verteilt:

```
Einkommen
 ├→ 1. Laufende Kosten + Kapital (inkl. KI/Roboter)
 ├→ 2. Gehälter: 2000 OR pro Angestelltem
 ├→ 3. Dreimonatsreserve (Stabilitätspuffer)
 └→ 4. Überschuss:
      ├→ Grüner Bonus (an Mitarbeiter, Softmax-Verteilung)
      ├→ Blauer Arbeitsgruppenausgleich (starke fördern schwache)
      └→ Roter Systemanteil (finanziert neue Stellen)
```

### Bonusberechnung — Flächenmodell

Der Überschuss (ü) wird in drei Flächen aufgeteilt:

```
Fläche                Formel                          Farbe
───────────────────────────────────────────────────────────
Bonus (Mitarbeiter)   ü ^ (n / (n + α))               Grün
Gruppenausgleich      (Bonus + ü) / 2                  Blau
Systemanteil          Rest bis ü                       Rot
```

- **n** = Anzahl Angestellte in der Arbeitsgruppe
- **α** = Stellschraube, vom Rat festgelegt (aktuell: 5)
- Bonus wächst sublinear (Wurzelfunktion), Systemanteil wächst überproportional
- Bei kleinem Überschuss dominiert der Bonus (Anreiz für den Gruppenleiter)
- Bei großem Überschuss dominiert der Systemanteil (System profitiert mehr)

Der grüne Bonus wird per Softmax-Kurve auf Gruppenleiter und Angestellte verteilt. Gruppenleiter bekommen proportional mehr (weniger Personen, höhere Verantwortung). Das Grundgehalt bleibt unangetastet.

α wird von einem paritätischen Rat (Arbeitnehmer + Arbeitgeber) angepasst. Keine Einzelperson entscheidet über die Verteilung.

### Arbeitsgruppenausgleich (Blau)

Mittelwert aus Bonus und Gesamtüberschuss. Die einkommensstärksten Arbeitsgruppen fördern die einkommensschwächsten (vor allem Start-ups).

### Selbstbalancierender Kreislauf

Der rote Systemanteil finanziert neue Arbeitsplätze:

1. Systemanteil akkumuliert sich aus den Überschüssen aller Arbeitsgruppen
2. Sobald **8000 OR** im Systemanteil zusammenkommen → automatisch neuer Mitarbeiter (2000 OR Gehalt + 6000 OR Rücklagen)
3. Die Bonusberechnung wird mit der neuen Gruppengröße (n) **neu berechnet**
4. Mehr KI-Produktivität → mehr Überschuss → mehr Systemanteil → mehr Stellen → Neuverteilung

Je produktiver die KI, desto mehr Menschen werden eingestellt. Das System skaliert sich selbst.

### Systempoolabgabe — keine Doppelberechnung (geplant)

Bereits über den Systempool finanzierte Angestellte werden bei der Abgabe berücksichtigt:

```
effektive Abgabe = max(berechneter Systemanteil - n × 8000, 0)
```

Wer schon Mitarbeiter über den Systempool eingestellt hat, zahlt nicht nochmal für deren Anteil. Erst wenn der Systemanteil über die bereits finanzierten Stellen hinauswächst, fließt wieder etwas in den Pool.

## Warum das kein Grundeinkommen ist

Grundeinkommen verteilt Geld. RLGD schafft Arbeitsplätze.

Menschen haben eine Aufgabe, eine Gruppe, einen Beitrag. Das Gehalt von zweitausend Original Reso ist ein Auffangnetz für eine Übergangszeit, in der Arbeit neu definiert wird. Die Arbeitszeiten sind flexibel. Es ist ein Nebenverdienst, kein Vollzeitjob.

## Auszahlung

Drei Pfade:
1. **In Original Reso belassen** — investieren, bei anderen Arbeitsgruppen kaufen
2. **In Short Reso umtauschen** — zum aktuellen Wechselkurs
3. **In Euro umtauschen** — Steuern und Sozialabgaben eigenverantwortlich

## Status

Das Modell ist durchgerechnet und dokumentiert. Es liegt auf Eis.

Die rechtlichen Rahmenbedingungen in Deutschland lassen eine Umsetzung mit Echtgeldzahlungen derzeit nicht zu. Das System ist als Gutschein-/Credit-Modell konzipiert, kein offizielles Zahlungsmittel.

Die Plattform existiert. Die KI-Infrastruktur läuft. Das Wirtschaftsmodell wartet auf den Moment, in dem es gebraucht wird.

## Kontakt

- https://rlgd.de
- info@rlgd.de
- Gegründet von Wolfgang, Heidelberg
