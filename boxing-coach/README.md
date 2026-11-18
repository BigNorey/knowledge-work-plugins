# Boxing Coach 🥊

Ein Plugin für Boxer: Du beschreibst, wie dein Sparringspartner (oder nächster Gegner) boxt – Claude erkennt den Stil, findet seine Gewohnheiten und Schwächen und sagt dir, **wie du ihn auskonterst** und **was du trainieren solltest**.

## Skills

| Skill | Was er macht |
|---|---|
| **sparring-analyse** | Stil-Einschätzung (Druckboxer, Konterboxer, Distanzboxer …), Konter für jede beschriebene Gewohnheit, Gameplan fürs nächste Sparring, passende Drills |
| **trainingsplan** | Wochenplan, der gezielt auf diesen Gegner vorbereitet – angepasst an deine Trainingstage und was du zur Verfügung hast (Partner, Pratzen, Sandsack) |

## Beispiel

> Mein Sparringspartner ist Orthodox, etwas größer als ich. Er jabt viel, aber lässt nach dem Jab immer die linke Hand fallen. Wenn ich Druck mache, geht er gerade zurück. In Runde 3 wird er müde. Ich bin auch Orthodox, boxe seit 2 Jahren.

Claude antwortet mit:
- **Stil:** Distanzboxer mit Konditionsschwäche
- **Konter:** Slip außen + Cross über den Jab; Doppel-Jab und 2, wenn er gerade zurückgeht; ab Runde 3 Druck
- **Gameplan** mit 3–5 merkbaren Punkten
- **Drills** wie Slip-Counter und Ring abschneiden

Danach: „Mach mir einen Trainingsplan bis Samstag" → Wochenplan.

## Web-App (Testversion)

`app/sparring-analyse.html` ist eine eigenständige Web-App:

- **Mehrere Sparringspartner**: für jeden ein eigenes Profil
- **Analyse**: Stil, Konter für jede Gewohnheit (passend zur Auslage), Gameplan, Drills, plus Details wie Lieblingskombi, Reaktion auf Treffer und Verhalten an den Seilen
- **Tagebuch**: nach dem Sparring eintragen, welche Konter geklappt haben. Konter, die mehrfach nicht klappen, werden durch eine Alternative ersetzt, und was klappt, wird zur Konter-Falle im Gameplan
- **Trainingsplan**: Wochenplan nach Trainingstagen, Dauer und Ausrüstung, mit leichtem Tag vor dem Sparring
- **Rundentimer**: mit Gong und 10-Sekunden-Warnung. In der Pause zeigt er die drei wichtigsten Gameplan-Punkte an
- **Claude-Analyse** (optional): ausführliche Analyse und Wochenplan, mit Nachfragen

## Tipp

Gib nach dem Sparring Feedback („der Cross-Konter hat geklappt, aber er hat dann angefangen zu doppeln") – dann wird die Analyse immer genauer.

## Hinweis

Sparring ist Training. Sprecht die Intensität ab, tragt Schutzausrüstung, und besprecht den Plan mit eurem Trainer. Bei Kopfschmerzen, Schwindel o. Ä. nach dem Sparring: Pause und Arzt.

## Installation (Claude Code)

```bash
claude plugin marketplace add BigNorey/knowledge-work-plugins
claude plugin install boxing-coach@knowledge-work-plugins
```
