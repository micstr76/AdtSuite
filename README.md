# AdtSuite — Public Distribution

Public-Repo nur für **Releases** und **Update-Info**.

## Was ist hier drinnen
- `version.json` — Versions-Metadata für den App-internen Update-Check
- Releases-Tab: zukünftig MSI/EXE als Download-Assets

## Source-Code
Der Source-Code liegt in einem privaten Repo. Diese Distributions-Seite dient
nur zur Verteilung der fertigen Anwendung an Beta-Tester und Nutzer.

## Lizenz
AdtSuite ist in der **Free-Version unentgeltlich nutzbar**, auch in Unternehmen.
Erweiterte Funktionen erfordern einen Lizenzschlüssel, der direkt über die
Anwendung angefordert wird. Die vollständigen Bedingungen stehen in
[LICENSE](LICENSE).

Versionen bis einschließlich 1.7.0 wurden unter der MIT-Lizenz veröffentlicht;
für diese gelten weiterhin die damaligen Bedingungen.

## App-Update-Check
Die installierte App prüft beim Start (asynchron) und bei Klick im "Über"-Dialog
`https://raw.githubusercontent.com/micstr76/AdtSuite/main/version.json` und
zeigt einen Hinweis falls eine neuere Version online verfügbar ist.

