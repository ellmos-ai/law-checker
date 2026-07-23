# TODO: law-checker / rechtsabteilung

**Audit Date:** 2026-07-16  
**Auditor:** Codex  
**Target Repo:** `ellmos-ai/law-checker` / `.AI/.MODULES/.DOMAINS/rechtsabteilung`

---

## STATUS

| Category | Status | Notes |
|---|---|---|
| Secrets | OK | Final Gate Check fand keine Secret-Muster in getrackten Dateien. |
| Private Data (PII) | OK | Final Gate Check fand keine PII-Muster in getrackten Dateien. |
| .gitignore | OK | Mindestmuster für `.env`, `*.db`, `.venv/`, `.idea/`, `.vscode/`, `__pycache__/` und `*.pyc` sind vorhanden. |
| Language (English) | OK with follow-up | README enthält englischen TL;DR; deutsche Modultexte sind bewusst Teil der Domäne. |
| BACH Internals | OK | Keine BACH-internen Release-Dokumente im Gate-Scope. |
| Database Files | OK | Keine `.db`-Dateien getrackt. |
| README.md | OK | README vorhanden. |
| LICENSE | OK | MIT-Lizenz vorhanden. |
| Overall | GATE-READY, PUBLIC-RELEASE PENDING | Automatischer Gate kann grün laufen; Public-Release braucht noch dokumentierte Release-Gate-Entscheidung und Security-Review. |

**Gate Check Exit Code:** `0` nach Hygiene-Fix erwartet; bei Release neu ausführen und in `RELEASE_GATE.md` dokumentieren.

---

## BLOCKER

- [x] `.gitignore` um Gate-Mindestmuster ergänzen.
- [x] Root-`TODO.md` mit STATUS-Tabelle anlegen.

## HIGH PRIORITY

- [ ] `RELEASE_GATE.md` mit aktuellem Final-Gate-Protokoll anlegen, bevor das Repo öffentlich geschaltet oder neu getaggt wird.
- [ ] `SECURITY.md` ergänzen: sensible Rechtssachverhalte, Cloud-LLM-Warnung, lokale `_gutachten/`, `_data/gesetze/`, `config.local.json` und Responsible-Disclosure-Weg beschreiben.
- [ ] Deutsche End-User-/Konfigurationstexte auf echte Umlaute normalisieren, ohne JSON-Schlüssel oder externe Dateinamen zu brechen.

## MEDIUM PRIORITY

- [ ] `CHANGELOG.md` ergänzen oder einen klaren Changelog-Abschnitt in der README pflegen; Registry-Versionen aus `config.json` dort nachziehen.
- [ ] `CONTRIBUTING.md` ergänzen, falls externe Beiträge erwartet werden.
- [ ] Offline-Smoke dokumentieren: `python _tools/gesetze_fetch.py --list` plus optionaler Fetch gegen einen temporären Datenordner.

## LOW PRIORITY

- [ ] Kleine Testabdeckung für `gesetze_fetch.py` ergänzen: Registry-Parsing, unbekannter Schlüssel, `--list`, XML-Extraktion aus Fixture-Zip.
- [ ] Installationshinweise für Windows PowerShell, macOS/Linux-Shell und Claude-Code-Skill-Kopie trennen.
