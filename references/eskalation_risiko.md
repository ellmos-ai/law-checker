# Risiko-Ampel, Eskalation und Anwalts-Matrix (Modul rechtsabteilung)

> Extrahiert aus Um:bruch `Policies/RECHTSABTEILUNG.md` (Eskalationsverfahren,
> Anwalts-Matrix, Fristen-Disziplin), generalisiert für beliebige Auftraggeber.

## Risiko-Ampel

| Stufe | Bedeutung | Konsequenz |
|---|---|---|
| **Gering** | Kein nennenswertes rechtliches Risiko erkennbar | Selbst handeln; Gutachten dokumentiert die Prüfung |
| **Mittel** | Reales, aber beherrschbares Risiko | Änderungen umsetzen; bei Außenwirkung anwaltliche Rücksprache erwägen |
| **Hoch** | Ernsthafte Rechtsfolgen möglich (Abmahnung, Bußgeld, Haftung) | Fachanwalt einschalten, bevor gehandelt wird |
| **Kritisch** | Unmittelbare Bedrohung (Klage, Strafverfahren, hohe Summen, laufende Frist) | SOFORT Anwalt + Auftraggeber informieren; nichts ohne Rücksprache |

## Fristen-Disziplin (hart)

- Bei **eingehender Rechtspost** (Abmahnung, Unterlassungsaufforderung,
  Anwaltsschreiben, behördliche Anhörung) ist der Fristen-Check der ERSTE
  Prüfschritt — Abmahnungen haben oft 7–14 Tage Frist.
- Jede Fristsache: Frist mit Datum prominent ins Gutachten (Abschnitt 3) und an
  den Auftraggeber melden. Fristen NIE verstreichen lassen; „Frist unklar" ist
  selbst ein Hoch-Risiko-Befund.
- Original-Schreiben sichern (nie löschen), Eingangsdatum dokumentieren.
- Ersteinschätzung bei Rechtspost binnen 24–48 h: Worum geht es (Unterlassung,
  Schadensersatz, Auskunft, Abmahnung)? Frist? Prima-facie berechtigt?
  Risikostufe?

## Anwalts-Matrix (wann externe anwaltliche Hilfe empfehlen)

| Situation | Anwalt? | Fachgebiet |
|---|---|---|
| Abmahnung wegen Urheberrechtsverletzung | Ja | Medien-/Urheberrecht |
| Unterlassungsaufforderung wegen Äußerung | Ja | Presse-/Äußerungsrecht |
| DSGVO-Auskunftsersuchen (Art. 15 DSGVO) | Bei Unsicherheit | Datenschutzrecht |
| Einfache Löschungs-/Korrekturanfrage | Nein (Erstprüfung reicht) | — |
| Strafanzeige / staatsanwaltliche Post | Sofort | Strafrecht |
| Impressums-/Kennzeichnungsbeanstandung | Nein (prüfen + korrigieren) | — |
| Vertragsfragen | Bei erheblichem Wert oder langer Bindung | Vertragsrecht |
| Sozialrechtlicher Widerspruch/Bescheid | Bei Ablehnung im Widerspruchsverfahren | Sozialrecht |
| Gesellschafts-/Vereinsgründung (Satzung) | Ja | Gesellschafts-/Vereinsrecht |

Die Matrix ist Ausgangspunkt, kein Automat: Im Gutachten wird die Empfehlung
begründet (warum reicht die Erstprüfung / warum nicht).

## Eskalationspfad

```
Anlass (Rechtspost, riskanter Inhalt, Vertragsfrage)
  ├─ Auftraggeber SOFORT informieren, wenn Frist oder Kritisch-Verdacht
  ├─ Dokumente sichern (nichts löschen), Eingangsdatum notieren
  ├─ Erstprüfung nach Skill-Ablauf → Gutachten mit Risikostufe
  ├─ Empfehlung nach Ampel (selbst / Rücksprache / Anwalt / sofort Anwalt)
  └─ Ergebnis + offene Fristen an den Auftraggeber zurückmelden
```

## Grundsätze (immer)

1. KI-Rechtseinschätzung ist **Ersteinschätzung**, kein Anwaltsersatz — jede
   Ausgabe wird als solche gekennzeichnet (Pflichtabschnitt „Grenzen").
2. Bei ernsthafter Bedrohung: **menschlichen Anwalt** empfehlen — das Gutachten
   nennt den Zeitpunkt und das Fachgebiet.
3. **Dokumentationspflicht:** Jede Prüfung und Empfehlung wird schriftlich
   festgehalten (Ablage laut config).
4. Prüfung **auf Auftrag**, nicht ungefragt in fremden Angelegenheiten.
