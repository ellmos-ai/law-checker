# Berichtsformat — Rechtsgutachten (Modul rechtsabteilung)

> Extrahiert aus Um:bruch `Policies/RECHTSABTEILUNG.md` (5-Abschnitt-Template) und
> dessen Referenz-Ausführung `_editorial/recht_2026-04-05_redaktionspflichten.md`,
> erweitert um die Fundstellen-Disziplin des Skills lebende-verfassung.

## Ablage

`_gutachten/JJJJ-MM-TT_<slug>.md` — jedes Gutachten ist ein dokumentierter,
datierter Prüfvorgang. Korrekturen als neue Version mit Vermerk, nicht still
überschreiben.

## Gerüst (immer dieses)

```markdown
# Rechtliche Prüfung — {DATUM}
Prüfer: {Modell/Agent} | Skill rechtsabteilung v{N}, config v{M}
Typ: Inhaltsprüfung / Anlassprüfung / Vertragsfrage / Eingehende Rechtspost / Routinecheck
Auftrag: {Wer hat beauftragt, wann, worauf bezogen}
Gesetzbücher (aktiv): {Kurznamen aus der Registry + Abrufdatum der Normtexte}

## 1. Gegenstand und Prüfungsrahmen
- Was wird geprüft? (Sachverhalt neutral; geprüfte Dokumente auflisten)
- Prüfungsrahmen: die konkret in Betracht gezogenen Normen VORAB benennen

## 2. Rechtliche Einschätzung
- Gegliedert nach Rechtsgebieten bzw. Prüffragen
- JEDER Normbeleg im Pflichtformat (siehe unten)
- JEDER Rechtsprechungsbeleg im Pflichtformat (siehe unten)
- Tabellarische Subsumtion, wo Kriterienkataloge geprüft werden
  (Kriterium | erfüllt? | Begründung)
- Wo einschlägig: Bußgeld-/Haftungsrahmen und zuständige Aufsicht mit Norm benennen
- Vergleichsansatz, wo er trägt: Welche Pflichten entstehen HIER, die im
  Vergleichsfall (z. B. Privatperson, anderes Rechtsregime) NICHT bestünden?
- Kategorien-Label an jeder Kernaussage: Verdikt | Prüfauftrag | Hypothese

## 3. Risikoeinschätzung
- Ampel: Gering / Mittel / Hoch / Kritisch — mit Begründung je Risiko
- Fristen GESONDERT ausweisen (jede Fristsache mit Datum)

## 4. Empfehlung
- Handlungsempfehlung (umsetzen / ändern / zurückziehen / Anwalt einschalten)
- Bei Anwalts-Empfehlung: Fachgebiet nennen (references/eskalation_risiko.md)
- Begründung; die stärkste Gegenposition fair mitführen (Steelman)

## 5. Grenzen dieser Einschätzung
- Pflichttext: "KI-gestützte Erstorientierung, kein Ersatz für die individuelle
  Prüfung durch eine zugelassene Rechtsanwältin oder einen zugelassenen
  Rechtsanwalt. Ob ein konkreter Einsatz eine Rechtsdienstleistung darstellt
  und zulässig ist, hängt von Einsatzform, Betreiberrolle und Einzelfall ab.
  Keine Fristüberwachung, keine Vollständigkeits- oder Aktualitätsgarantie —
  bei Rechtspost und laufenden Fristen sofort professionelle Beratung. Bei
  Risikoeinschätzung 'Hoch' oder 'Kritisch' wird die Einschaltung eines
  Fachanwalts empfohlen." (Formulierung nach Review-Befund 8, 2026-07-11: ein
  Disclaimer darf kein rechtliches Ergebnis für jeden Einsatz behaupten.)
- Plus ehrlich: Was konnte NICHT geprüft werden (fehlende Normtexte,
  nicht ermittelte Rechtsprechung, offene Tatsachenfragen)? Insbesondere:
  Die Prüfung deckt nur die aktivierten Gesetzbücher der Registry ab —
  IMMER die vollständige Konfiguration ausweisen (auch aktive, aber nicht
  herangezogene Gesetze mit kurzer Begründung der Nichtheranziehung).

## 6. Recherchequellen
- Gegliedert: (a) Normtexte (lokale Quelle + Abrufdatum aus dem Dateikopf),
  (b) Rechtsprechung (verifizierte Fundstellen/URLs), (c) Behörden/amtliche
  Quellen, (d) Sekundärquellen — Provenienz amtlich/Verband/Presse trennen.
```

## Beleg-Pflichtformate

**Normbeleg** — so tief, wie die tragende Aussage reicht (Absatz-, wo nötig
Satz-genau), plus wörtliches Kurzzitat:

> § 19 Abs. 1 MStV: „…gelten die anerkannten journalistischen Grundsätze."
> (Quelle: MSTV.txt, Abschnitt `===== § 19 … =====`, abgerufen 2026-07-11)

**Rechtsprechungsbeleg** — nur web-verifiziert, nie aus dem Gedächtnis:

> BVerfG, Beschluss vom 24.03.2021 — 1 BvR 2656/18 u. a. (Klimabeschluss),
> ECLI:DE:BVerfG:2021:rs20210324.1bvr265618, Kernaussage in einem Satz,
> Fundstelle: bundesverfassungsgericht.de/… (abgerufen JJJJ-MM-TT)

Nichts gefunden → ausdrücklich „nicht ermittelt" schreiben. Ein fehlender Beleg
ist ein Befund, keine Lücke, die man mit Erinnerung füllt.

## Qualitätsregeln (aus den Erstlauf-Lektionen der Herkunftssysteme)

- **Endfassungs-Disziplin:** Bei Gesetzen/Beschlüssen die tatsächlich beschlossene
  Fassung prüfen (Ausschussfassung/Verkündung), nicht Entwürfe oder
  Pressemitteilungen.
- **Keine Scheinkonvergenz:** Prüfaufträge und Hypothesen nicht als unabhängige
  Bestätigungen eines Verdikts addieren.
- **Reichweiten-Disziplin:** Normen nicht über ihren Wortlaut-Anwendungsbereich
  hinaus verallgemeinern (Lektion: BGB § 42 gilt dem Vereinsvorstand, nicht
  „allen Trägern").
- **Unsicherheit ist Teil des Ergebnisses:** „nicht entscheidbar" ist zulässig
  und wertvoll.
