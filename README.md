# PaperLabHQ – öffentliches NBA- und EuroLeague-Wettjournal

**Öffentliche Webseite:** https://paperlabhq.github.io/

Dieses Repository ist die **maßgebliche Datenquelle** für die öffentliche, schreibgeschützte Ansicht. Die GitHub-Pages-Seite lädt die Ergebnisse aus `journal-data.json`.

## Update-Workflow

1. Vor Änderungen die aktuelle `journal-data.json` vom `main`-Branch laden; keine alten lokalen Kopien überschreiben lassen.
2. Neue Tipps nur nach ausdrücklicher Bestätigung des Nutzers als gespielt eintragen. Spielergebnis und Start-/Einsatzwerte nicht erfinden.
3. Nach Spielende die tatsächlichen Spielerstatistiken anhand eines verlässlichen Boxscores verifizieren; Treffer/Verlust oder DNP/Void korrekt eintragen und die Nachanalyse dokumentieren.
4. Die bereits vorhandenen Datensätze, IDs, Quoten und Einsatzwerte unverändert lassen, soweit keine konkrete Korrektur beauftragt wurde.
5. `journal-data.json` per GitHub-Commit aktualisieren, danach den neuen Stand und GitHub-Pages-Deployment prüfen. Die Versionsnummer bleibt bei reinen Wett- und Ergebnisupdates gleich.

## Verbindlicher Analyse-Standard

Der **vollständige, aktuelle Master-Prompt** für NBA-/EuroLeague-Player-Prop-Analysen ist in [ANALYSE_STANDARD.md](ANALYSE_STANDARD.md) dokumentiert. **Diese Datei hat für neue Analysen Vorrang vor den verkürzten Hinweisen unten.** Insbesondere: keine Tipps ohne bestätigte Quote, exakte L5/L10/L20-Game-Logs, relevante historische On/Off-Vergleiche, vorsichtige EV-Schätzung, maximal zwei Picks pro Matchup, und keine Pflicht zu wetten.

## Verbindliche Regeln für künftige Picks (zuletzt aktualisiert 11.11.2026)

- **Pro NBA-/EuroLeague-Spiel maximal ZWEI platzierte Tipps insgesamt**. Das Limit gilt für alle Spieler und erlaubten Marktarten zusammen (Punkte, Assists, Rebounds, Dreier und Kombimärkte P+R, P+A, R+A, PRA). Nicht drei Tipps aus demselben Matchup empfehlen oder spielen lassen.
- Die Obergrenze ist keine Pflicht, zwei Wetten zu finden. Nur Picks mit fundierter Markt-/Quotenprüfung und einem plausiblen positiven Erwartungswert empfehlen; bei unklarem Vorteil auslassen.
- **Steals, Blocks und Steals + Blocks nicht analysieren oder empfehlen.** Dies ist eine ausdrückliche Nutzerpräferenz wegen der hohen Varianz dieser seltenen Ereignisse, nicht eine technische Einschränkung des Bots.
- Rotation, Ausfälle, tatsächlich vergleichbare On/Off-Game-Logs, Spielminuten, Spieltempo, Matchup sowie Korrelation mehrerer Props berücksichtigen. Historische Trefferquoten nicht als sichere Prognosen behandeln.
- Nur tatsächliche bestätigte Quoten und Buchmacher nennen, und ohne ausdrückliche Bestätigung keine Einsätze verändern.

## Lessons learned – 09.11.2026

- SAS @ PHX wurde mit drei Props überbelegt (Harper, Bridges, Castle); daraus folgten 1 Sieg und 2 Niederlagen. Die Partie endete 122:96. Gemeinsame Spielverlaufsrisiken künftig durch die 2-Picks-Grenze begrenzen.
- Stephon Castle erzielte 4 Punkte + 8 Rebounds bei einer Linie von 19,5 P+R trotz seiner zuvor starken kleinen 10-Spiele-Stichprobe; Trefferquoten aus kleinen Samples nicht übergewichten.
- Daniel Gafford erzielte 0 Blocks bei Over 1,5; historische Lehre: Die hohe Varianz seltener Defensivstatistiken kann kurze Treffer-Serien irreführend machen. Seit 11.11.2026 sind Steals-/Blocks-Märkte auf ausdrücklichen Nutzerwunsch ausgeschlossen.
- Austin Reaves spielte krankheitsbedingt nicht; als DNP/Void im simulierten Journal verbucht. Eine reale Buchmacherabrechnung muss separat geprüft werden.

## Dateien

- `index.html` – öffentliches Dashboard
- `journal-data.json` – maßgebliche Wett- und Ergebnisdaten

Die alte Seite unter `cl0ckh0us3.github.io/paperlab/` dient nicht mehr als primäre Veröffentlichungsquelle. Dieses Repository ist die aktuelle Produktionsversion.
