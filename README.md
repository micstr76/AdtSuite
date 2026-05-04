# AdtSuite — Public Distribution

Public-Repo nur für **Releases** und **Update-Info**.

## Was ist hier drinnen
- `version.json` — Versions-Metadata für den App-internen Update-Check
- Releases-Tab: zukünftig MSI/EXE als Download-Assets

## Source-Code
Der Source-Code liegt in einem privaten Repo. Diese Distributions-Seite dient
nur zur Verteilung der fertigen Anwendung an Beta-Tester und Nutzer.

## App-Update-Check
Die installierte App prüft beim Start (asynchron) und bei Klick im "Über"-Dialog
`https://raw.githubusercontent.com/micstr76/AdtSuite/main/version.json` und
zeigt einen Hinweis falls eine neuere Version online verfügbar ist.

