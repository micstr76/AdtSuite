# Security Policy

## 🛡️ Sicherheitslücken melden

Falls du eine **Sicherheitslücke** in AdtSuite entdeckst, melde sie bitte **nicht** über den öffentlichen Issue-Tracker, sondern privat — damit andere Nutzer nicht gefährdet werden, bevor ein Fix verfügbar ist.

### Meldung per GitHub Security Advisory (bevorzugt)

GitHub bietet einen privaten Kanal direkt im Repo:

➡️ **[Neues Security Advisory melden](https://github.com/micstr76/AdtSuite/security/advisories/new)**

Vorteile:
- Nur du und der Maintainer sehen die Meldung
- Strukturierte Eingabe (CVE-Vorlage, betroffene Versionen, CVSS)
- Nach dem Fix kann das Advisory gemeinsam veröffentlicht werden

### Meldung per Mail

Alternativ direkt an den Maintainer **(Bug-Report-Dialog der App nutzen ist auch OK — der nutzt eine Mail-Vorlage mit Verschlüsselungs-Hinweis)**.

## 🔍 Was zählt als Sicherheitslücke?

Für AdtSuite relevant:
- **Code-Injection** in generierten PowerShell-Scripts (z.B. via Snippet-Import oder Profil-Daten)
- **Path-Traversal** beim Lesen / Schreiben von Snippets / Profilen / ZIP-Exports
- **Credential-Leakage** (Logs, Crash-Dumps, oder unbeabsichtigte Klartextspeicherung)
- **Update-Check-Vergiftung** (Manipulation der `version.json`-Quelle)
- **Lizenz-Bypass / Signaturfälschung** im Strasser.Licensing-Modul
- Schwachstellen in einer der genutzten Dependencies (siehe `AdtSuite.csproj`)

## ⏱️ Was passiert nach der Meldung?

| Phase | Erwartete Zeit |
|---|---|
| **Empfangsbestätigung** | Innerhalb von 48 Stunden |
| **Bewertung & Reproduktion** | 3–7 Tage |
| **Fix-Entwicklung** | abhängig von der Komplexität |
| **Release & Disclosure** | nach Abstimmung mit dem Reporter |

Während der Beta-Phase kann es etwas länger dauern als bei einer stabilen Release-Linie.

## 🤝 Verantwortliche Veröffentlichung

Wir bitten darum, die Lücke **nicht öffentlich** zu beschreiben, bis ein Fix verfügbar ist. Im Gegenzug nennen wir dich gerne in den Release-Notes des Patches (auf Wunsch auch anonym).

## 📦 Unterstützte Versionen

| Version | Status |
|---|---|
| **1.0.x-beta** (aktuell) | ✅ Wird mit Sicherheits-Patches versorgt |
| Ältere Pre-Beta-Builds | ❌ Keine Unterstützung — bitte auf aktuelle Version updaten |

Danke, dass du AdtSuite sicherer machst! 🙏
