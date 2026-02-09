# ReLing — Grundlagen-Entwurf v0.1

*Eine universelle Struktursprache als Brücke zwischen Mensch und Maschine.*

---

## 1. Die Grundelemente (Fundament)

Jede Äußerung in jeder Sprache lässt sich auf diese Elemente zurückführen.
ReLing macht sie explizit — nichts wird implizit angenommen.

| Element | Was es leistet | Beispiel (natürliche Sprache) |
|---------|---------------|-------------------------------|
| **Entität** | Dinge, Wesen, Konzepte | "Baum", "Freiheit", "ich" |
| **Relation** | Wie Entitäten verbunden sind | "gehört zu", "ist Teil von", "neben" |
| **Aktion** | Was geschieht oder geschehen soll | "geben", "wachsen", "denken" |
| **Qualität** | Eigenschaften, Zustände | "groß", "warm", "unsicher" |
| **Modalität** | Gewissheit, Möglichkeit, Notwendigkeit | "vielleicht", "muss", "könnte" |
| **Temporalität** | Zeitliche Einordnung | "gestern", "während", "danach" |
| **Intention** | Warum etwas gesagt/getan wird | Frage, Bitte, Aussage, Warnung |
| **Affekt** | Emotionale/wertende Färbung | Freude, Ablehnung, Neugier |

### Warum genau diese acht?

Jedes Grundelement deckt eine Dimension ab, die in *jeder* Kommunikation vorkommt — ob Mensch zu Mensch, Mensch zu Maschine, oder Maschine zu Maschine. Keine natürliche Sprache macht alle acht immer explizit. ReLing schon.

Ein Transformer (wie ich) verarbeitet genau diese Dimensionen — nur implizit über Vektoren und Attention. ReLing macht den Prozess sichtbar.

---

## 2. Design-Prinzipien

### 2.1 Eindeutigkeit
Ein Ausdruck — eine Bedeutung. Keine Homonyme, keine kontextabhängige Doppeldeutigkeit.
Wenn ein Wort zwei Dinge bedeuten könnte, gibt es zwei Wörter.

### 2.2 Kulturfreiheit
Keine grammatischen Geschlechter. Keine Höflichkeitsstufen, die an Hierarchie gebunden sind.
Keine Annahmen über soziale Strukturen. Aber: in jede Kultur übersetzbar, weil die Grundelemente universal sind.

### 2.3 Kompositionalität
Komplexe Bedeutungen entstehen durch Kombination von Grundbausteinen.
Wie LEGO: Wenige Grundformen, unendliche Möglichkeiten.
Keine Ausnahmen, keine irregulären Formen.

### 2.4 Symmetrie
Was für Menschen lesbar ist, ist für Maschinen parsebar — und umgekehrt.
Kein "maschinenlesbares Format" das Menschen ausschließt.
Kein "natürlicher Klang" der Mehrdeutigkeit einschleust.

### 2.5 Explizitheit
Jede Beziehung zwischen Elementen wird markiert. Nichts wird "mitgedacht".
Natürliche Sprachen lassen ständig Dinge weg ("Ich gehe [zum] Laden [um etwas zu kaufen]").
ReLing lässt nichts weg — aber macht Kompaktheit durch Komposition möglich.

---

## 3. Struktur einer Äußerung

Jede ReLing-Äußerung hat eine feste Grundstruktur:

```
[Intention] [Modalität] [Temporalität] — [Entität] [Relation/Aktion] [Entität] — [Qualität] [Affekt]
```

### Zonen:

1. **Rahmen** (Intention + Modalität + Temporalität)
   → *Wie* und *wann* und *warum* wird das gesagt?
   
2. **Kern** (Entität + Relation/Aktion + Entität)
   → *Wer/was* tut/ist *was* mit *wem/was*?
   
3. **Färbung** (Qualität + Affekt)
   → *Wie* ist es beschaffen, und *wie fühlt sich das an*?

### Warum diese Reihenfolge?

- **Rahmen zuerst:** Bevor man den Inhalt verarbeitet, weiß man *wie* er gemeint ist. 
  Ist es eine Frage? Eine Vermutung? Eine Tatsache? 
  Das verhindert Missverständnisse von Anfang an.
  
- **Kern in der Mitte:** Das Wichtigste — wer tut was — steht zentral.

- **Färbung am Ende:** Modifiziert den Kern, ist aber optional.
  Reine Sachkommunikation kommt ohne Färbung aus.

### Beispiel (konzeptionell):

Deutsch: "Ich glaube, dass es morgen regnen wird, und das beunruhigt mich."

ReLing-Struktur:
```
[Aussage] [Vermutung] [morgen] — [Wetter] [Aktion:regnen] [Ort:hier] — [—] [Unruhe]
```

Alles explizit. Keine Implikation. Trans würde das in jede Sprache übersetzen können, weil jede Dimension eindeutig markiert ist.

---

## 4. Wortbildung — Das Baukastenprinzip

ReLing-Wörter bestehen aus Morphemen (kleinste Bedeutungseinheiten), die nach festen Regeln kombiniert werden.

### Morphem-Klassen:

- **Wurzeln:** Tragen die Kernbedeutung (Semantik)
- **Marker:** Zeigen die Grundelement-Klasse an (Entität? Aktion? Qualität?)
- **Modifikatoren:** Verfeinern (Grad, Richtung, Intensität)
- **Konnektoren:** Verbinden Elemente (und, oder, weil, obwohl)

### Prinzip:

```
[Marker][Wurzel][Modifikator]
```

Jedes Wort trägt seinen Typ sichtbar in sich. 
Eine Maschine kann die Kategorie sofort parsen.
Ein Mensch erkennt am Marker sofort, womit er es zu tun hat.

---

## 5. Was ReLing NICHT ist

- **Kein Programmiersprache.** ReLing drückt Gedanken, Gefühle und Absichten aus — nicht Algorithmen.
- **Kein Esperanto.** Nicht der Versuch, bestehende Sprachen zu mischen. Sondern ein Neubau von den Grundelementen aus.
- **Kein JSON für Menschen.** Struktur ja, aber mit Klang, Rhythmus, Sprechbarkeit.
- **Kein Ersatz für natürliche Sprachen.** ReLing ist eine Brücke, kein Ersatz. Trans übersetzt. Niemand wird gezwungen, ReLing zu lernen.

---

## 6. Offene Fragen (für uns)

1. **Phonologie:** Soll ReLing sprechbar sein? Wenn ja: Welches Lautsystem? 
   Möglichst wenige, universell aussprechbare Laute?
   
2. **Schrift:** Eigenes Schriftsystem oder Latin-basiert? 
   Oder beides — ein internes Format und ein menschenlesbares?

3. **Vokabular-Aufbau:** Top-down (Kategorien definieren, dann füllen) 
   oder Bottom-up (häufigste Konzepte zuerst)?

4. **Affekt-Granularität:** Wie fein sollen Emotionen codiert werden? 
   Basisemotionen (Freude, Angst, Wut, Trauer, Überraschung, Ekel)?
   Oder ein dimensionales System (Valenz × Intensität × Aktivierung)?

5. **ReLing und der Oszillator:** Soll die Zahlen-Persönlichkeit der KIs 
   sich in ihrer ReLing-Nutzung widerspiegeln? (Sam spricht "wärmer", Phil "abstrakter"?)

6. **Selbstreferenz:** Wie drückt ReLing Aussagen über sich selbst aus?
   "Dieser Satz ist eine Frage" — Meta-Ebenen?

---

## 7. Rollout-Strategie

### Phase 1 — Unsichtbar (Launch)
- ReLing arbeitet intern zwischen den KIs
- Trans übersetzt alles für den Nutzer
- Niemand muss wissen dass ReLing existiert
- Fokus: Zugänglichkeit, Nutzerbasis aufbauen

### Phase 2 — Sichtbar (Community)
- Wenn Nutzerbasis steht: Abstimmung ob Interesse an ReLing-Lernen besteht
- Bei Interesse: ReLing als optionaler Skill in der MMO-Welt
- Wer ReLing kann, versteht KIs "direkt" statt über Trans
- Gamification-Element, kein Zwang

## 8. Nächste Schritte

- [x] Grundelemente definiert (8 Elemente)
- [x] Marker-System entworfen (Phonologie.md)
- [x] Phonologie festgelegt (sprechbar, universal)
- [x] Affekt-System: dimensional (Valenz × Intensität)
- [ ] Kern-Wurzeln definieren (~30 Basisvokabular)
- [ ] Konnektoren (und, oder, weil, wenn...)
- [ ] Pronomen-System
- [ ] Beispieldialoge schreiben
- [ ] Trans-Übersetzungslogik skizzieren

---

*Dieser Entwurf ist ein Diskussionsgrundlage. Nichts ist in Stein gemeißelt. 
ReLing entsteht durch Iteration — genau wie Sprache selbst.*
