# eCrampus

**Desktop-Client für einen übersichtlicheren Lernalltag während meiner FIAE-Umschulung.**

eCrampus bündelt Kursunterlagen, Berichtsheft, Prüfungsergebnisse und Posteingang der Lernplattform in einer Windows-Anwendung und meldet Neuigkeiten von selbst. Das Projekt entstand aus wiederkehrenden Schwierigkeiten in meinem eigenen Unterricht. Es ist mein eigenständiges Projekt und kein offizielles Angebot der WBS.

[Live-Demo mit fiktiven Daten](https://nullframe-sh.github.io/ecrampus-showcase/) · [Showcase-Repository](https://github.com/nullframe-sh/ecrampus-showcase) · [Portfolio](https://nullframe.sh) · [Kontakt](mailto:phsc@nullframe.sh)

## Ausgangspunkt

Im Lernalltag wechselte ich ständig zwischen Kursordnern, Lerninhalten, Prüfungsergebnissen und Posteingang und erledigte jede Woche dieselben Schritte für das Berichtsheft. Daraus entstand die Idee, diese Abläufe in einem Desktop-Client zusammenzuführen.

Mein Produktziel: Wer morgens die Anwendung öffnet, soll sofort sehen, was heute ansteht, ohne sich erst durch eine Anleitung arbeiten zu müssen.

## Funktionen

| Bereich | Was er im Alltag leistet |
| --- | --- |
| Heute | Tagesüberblick aus bereits geladenen Daten: Unterricht, Termine, neue Unterlagen und Nachrichten |
| Kursmaterial | Ordnerbaum, Dateitabelle und Vorschau statt vieler Browser-Tabs |
| Berichtsheft | Wochenansicht mit Stunden und Vorbefüllung; eigene Einträge bleiben unangetastet |
| Prüfungen und Posteingang | Ergebnisse und Nachrichten an einem Ort, Benachrichtigung bei Neuem |
| Hilfe | F1-Hilfe je Bereich und ein geführter Rundgang für neue Nutzer |

## Nutzung

Laut integriertem Online-Zähler nutzen 10–12 der 22 Teilnehmenden meines Kurses eCrampus aktiv (Stand Oktober 2026). Der Zähler lässt sich in der Anwendung abschalten und überträgt nur eine zufällige Kennung pro App-Start.

## Meine Arbeit daran

- Funktionen und Bedienabläufe festlegen und Rückmeldungen aus dem Kurs einarbeiten.
- Fehler über Konsole, Logdateien und Entwicklerwerkzeuge verfolgen und im Code eingrenzen.
- Den Code mit KI-Unterstützung erstellen und dort lesen, wo es auf Logik und Daten ankommt.
- Fehlschlagende Tests lesen und festlegen, welches Verhalten ein Regressionstest absichern soll.
- Releases betreuen: Installer bauen, Installations- und Upgrade-Test, Verteilung über meinen eigenen Update-Server.

## Qualitätssicherung

Vor jeder Veröffentlichung laufen Typprüfung, Linting und die automatisierten Tests; danach prüfe ich Installation und Upgrade auf Testinstallationen. Dabei achte ich besonders darauf, dass

- nach einem Kontowechsel keine Daten des vorherigen Kontos erscheinen,
- eigene Berichtsheft-Einträge bei der Vorbefüllung erhalten bleiben,
- Inhalte und Fensterlayouts vollständig sichtbar sind.

## Technologien

| Technologie | Einsatz |
| --- | --- |
| Electron | Desktop-Anwendung mit getrennten Main-, Preload- und Renderer-Prozessen |
| React, TypeScript | Benutzeroberfläche und Anwendungslogik |
| Jest | Automatisierte Tests |
| electron-builder, electron-updater | Windows-Installer und Auto-Update |

## Quellcode

Der Quellcode der Desktop-Anwendung ist nicht öffentlich. Die Oberfläche lässt sich in der [Live-Demo](https://nullframe-sh.github.io/ecrampus-showcase/) mit fiktiven Daten ausprobieren.

## Kontakt

**Philipp Schott** · Kaiserslautern  
[phsc@nullframe.sh](mailto:phsc@nullframe.sh) · [nullframe.sh](https://nullframe.sh)
