# 0001 – Hauptbildschirm: Kalender-Archiv mit direkter Korrektur

**Status:** entschieden (18.10.2026)

## Frage

Wie soll der Hauptbildschirm der Android-App aussehen, und wie wird ein Eintrag korrigiert?

## Entscheidung

Variante **C** aus dem UI-Prototyp (`prototype/sprach-tagebuch-ui/index.html`, Commit `e17fb2a`):

- **Startseite ist das Archiv:** Monatskalender mit geschriebenen Tagen und Serie, Hinweis auf fällige Karten, „Deine häufigsten Fehler“ (Fehlerprofil nach Typ) und Liste der Einträge.
- **Neuer Eintrag** über einen schwebenden Button („Heute schreiben“), Editor im Vollbild mit Schreibimpuls nach GER-Niveau.
- **Direkte Korrektur:** Nach „Korrigieren“ sieht man sofort die Lösung, umschaltbar zwischen Original, Korrigiert und Unterschied, darunter eine Liste mit Fehlertyp, Erklärung und „+ Karte“ pro Fehler.
- **Wiederholen** startet vom Hinweis auf der Startseite aus.

Verworfen: A (Selbstkorrektur zuerst, Tagesablauf mit unterer Navigationsleiste) und B (Chat mit Tandempartner, Inhalt vor Korrektur).

## Folgen

- Die Forschung stützt Selbstkorrektur vor der Lösung (siehe `docs/research/sprachtagebuch.md`, Abschnitt 3.1, Punkt 4). C verzichtet darauf. Ein optionaler Schritt „erst selbst versuchen“ im Editor bleibt als spätere Ergänzung offen.
- Fehlerprofil und Kalender brauchen von Anfang an gespeicherte Einträge mit typisierten Fehlern (Original-Span, Korrektur, Fehlertyp, Erklärung).
- Der Prototyp ist Wegwerf-Code und wird für die App neu geschrieben, nicht übernommen.
