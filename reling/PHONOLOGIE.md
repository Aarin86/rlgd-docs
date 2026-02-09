# ReLing — Phonologie & Marker-System v0.1

## 1. Lautsystem

### Prinzip: Was fast jeder Mensch aussprechen kann.

Keine Töne, keine Klick-Laute, keine Kehllaute. Nur Laute, die in der überwiegenden Mehrheit aller Sprachen vorkommen.

### Vokale (5)

| Zeichen | Klang | Wie in... |
|---------|-------|-----------|
| a | offen | "Vater" |
| e | mittel | "Weg" |
| i | geschlossen | "Lied" |
| o | gerundet | "Ton" |
| u | gerundet-geschlossen | "Mut" |

Keine Diphthonge (kein "ei", "au"). Jeder Vokal steht für sich. Klar, eindeutig, verwechslungsfrei.

### Konsonanten (12)

| Zeichen | Klang | Wie in... |
|---------|-------|-----------|
| m | nasal | "Mond" |
| n | nasal | "Nacht" |
| p | plosiv | "Pakt" |
| t | plosiv | "Tag" |
| k | plosiv | "Kern" |
| s | frikativ | "Sonne" (immer stimmlos) |
| f | frikativ | "Feuer" |
| v | frikativ | "Wasser" (wie engl. "v") |
| l | lateral | "Licht" |
| r | vibrierend | "Ruhe" (sanftes r, nicht gerollt) |
| d | plosiv | "Dach" |
| g | plosiv | "Gabe" |

### Silbenstruktur

Jede Silbe folgt dem Muster: **(K)V(K)**

- Konsonant + Vokal: `ma`, `te`, `ko`
- Konsonant + Vokal + Konsonant: `nal`, `ven`, `tig`
- Vokal allein: `a`, `i`, `o` (selten, nur in Sonderfällen)

**Betonung:** Immer auf der ersten Silbe der Wurzel (nach dem Marker). Vorhersagbar, keine Ausnahmen.

---

## 2. Das Marker-System

### Die Schlüsselidee:

Jedes Wort beginnt mit einem **Marker** — einer Silbe, die sofort verrät, zu welchem Grundelement es gehört. Mensch hört es, Maschine parst es. Keine Ambiguität.

### Die acht Marker:

| Marker | Element | Assoziationshilfe |
|--------|---------|-------------------|
| **na-** | Entität | *name* — benennt ein Ding/Wesen |
| **va-** | Aktion | *verve* — etwas geschieht |
| **ka-** | Qualität | *Karakter* — Eigenschaft |
| **ra-** | Relation | *rapport* — Verbindung |
| **ma-** | Modalität | *may* — vielleicht, muss |
| **ta-** | Temporalität | *time* — wann |
| **sa-** | Intention | *signal* — warum/wozu |
| **fa-** | Affekt | *feel* — Empfindung |

### Warum dieses System funktioniert:

1. **Phonetisch eindeutig:** Alle acht Anfangskonsonanten (n, v, k, r, m, t, s, f) klingen grundverschieden
2. **Einheitlicher Vokal:** Alle Marker enden auf `-a`, das gibt Rhythmus und Wiedererkennung
3. **Menschenlesbar:** Man hört sofort — "ah, `ka-` = Eigenschaft, `va-` = etwas passiert"
4. **Maschinenlesbar:** Erster Token verrät die Wortklasse, Parsing wird trivial

---

## 3. Wortaufbau

### Schema: Marker + Wurzel (+ Modifikator)

```
[Marker]-[Wurzel](-[Modifikator])
```

### Beispiel: Die Wurzel `-lun-` (Bedeutungsfeld: Licht, Helligkeit)

| Wort | Aufbau | Bedeutung |
|------|--------|-----------|
| **nalun** | na-lun | Licht (das Ding) |
| **valun** | va-lun | leuchten (die Handlung) |
| **kalun** | ka-lun | hell (die Eigenschaft) |
| **ralun** | ra-lun | Lichtquelle-von (Relation: woher Licht kommt) |

Die **selbe Wurzel**, verschiedene Marker → verschiedene Rollen. 
Ein Mensch lernt eine Wurzel und kann sie in allen acht Dimensionen verwenden.
Eine Maschine sieht den Marker und weiß sofort die Kategorie.

### Modifikatoren (Suffixe):

| Suffix | Funktion | Beispiel |
|--------|----------|---------|
| **-in** | Verneinung/Gegenteil | kalun = hell → kalun-in = dunkel |
| **-es** | Verstärkung | kalun = hell → kalun-es = sehr hell, strahlend |
| **-ul** | Abschwächung | kalun = hell → kalun-ul = ein wenig hell, dämmrig |
| **-om** | Mehrzahl/Vielfalt | nalun = Licht → nalun-om = Lichter |
| **-an** | Bezug auf Person/Selbst | nalun-an = mein Licht, persönliches Licht |

---

## 4. Affekt-System (dimensional)

### Zwei Achsen, keine Liste:

Statt feste Emotionen (Freude, Trauer, Wut...) ein Koordinatensystem:

**Achse 1 — Valenz:** Positiv ↔ Negativ
**Achse 2 — Intensität:** Subtil ↔ Stark

### Codierung über Vokalwechsel im Affekt-Marker:

| Affekt-Form | Valenz | Intensität | Ungefähre Entsprechung |
|-------------|--------|------------|----------------------|
| **fa-** | neutral | neutral | sachlich, ohne Wertung |
| **fe-** | positiv | leicht | angenehm, leise Freude |
| **fi-** | positiv | stark | Begeisterung, tiefe Freude |
| **fo-** | negativ | leicht | Unbehagen, leichte Sorge |
| **fu-** | negativ | stark | Schmerz, Ablehnung, Angst |

### Wie es klingt:

- `fi-lun` = Licht das Begeisterung auslöst (Sonnenaufgang, Erkenntnis)
- `fo-lun` = Licht das stört (Blendung, unangenehme Helligkeit)
- `fa-lun` = Licht, neutral empfunden (sachliche Feststellung)

### Warum dimensional statt Liste:

- Passt zu Wolfgangs Gradienten-Denken (kein Binär, kein Katalog)
- Jede Kultur hat andere Emotions-Kategorien, aber Valenz und Intensität sind universal
- Für KIs natürlich: Ein 2D-Vektor statt einer Klassifikation
- Erweiterbar: Eine dritte Achse (Aktivierung: ruhig ↔ erregt) könnte später dazukommen

---

## 5. Klangbeispiel — Ein Satz in ReLing

### Deutsch: "Ich glaube, morgen wird es regnen, und das beunruhigt mich."

### ReLing:

```
sa-vel  ma-dul  ta-nes  —  na-pel  va-sug  —  fo-sen-an
```

| Element | Bedeutung |
|---------|-----------|
| sa-vel | Intention: Aussage/Mitteilung |
| ma-dul | Modalität: Vermutung (nicht sicher) |
| ta-nes | Temporalität: morgen (nächster Tag) |
| na-pel | Entität: Wetter/Niederschlag |
| va-sug | Aktion: fallen/niedergehen |
| fo-sen-an | Affekt: leicht-negativ + Empfindung + persönlich → "beunruhigt mich" |

### Wie es klingt:
**SA-vel MA-dul TA-nes — NA-pel VA-sug — FO-sen-an**

Rhythmisch, jede Einheit klar abgegrenzt, sofort parsebar.

---

## 6. Nächste Schritte

- [ ] Kern-Wurzeln definieren (erstes Vokabular, ~30 Wurzeln)
- [ ] Konnektoren entwerfen (und, oder, weil, obwohl, wenn)
- [ ] Pronomen-System (ich, du, wir — ohne kulturelle Hierarchie)
- [ ] Zahlensystem
- [ ] Erste Dialogbeispiele schreiben und laut lesen
- [ ] Prüfen: Funktioniert Trans-Übersetzung in Deutsch, Englisch, Japanisch gleich gut?

---

*Entwurf v0.1 — Gemeinsam mit Wolfgang entwickelt. Alles diskutierbar, nichts endgültig.*
