# FFNBSee-Website

Internetseiten des Fördervereins Freie Netze Bodensee e.V.

Wir verwenden [lektor](https://getlektor.com) zum Generieren der Seite.

## Installation

lektor ist ist ein Python Programm und kann mit pip installiert werden.
Dafür haben wir dir ein Makefile vorbereitet und du kannst das mit folgenden Befehl installieren: *(nachdem du das git repo geklont hast)*

```bash
# lektor mit abhängigkeiten installieren
make install
```

## Lektor Server

Um die Webseite zu bearbeiten empfiehlt es sich einen lokalen Webserver laufen zu lassen und darin die Webseite zu bearbeiten.
Dieser läuft standardmäßig auf `http://localhost:5000`.

Der Server lässt sich mit dem folgenden Befehl aus dem Makefile starten:

```bash
make server
```

## LFS

Wir speichern große Dateien auf einem LFS Server auf [gitea.see-base.de](https://gitea.see-base.de/FFBSee/ffnbsee-website.git):

```txt
https://gitea.see-base.de/FFBSee/ffnbsee-website.git
```

## SASS/CSS

Bei Problemen mit dem lokalen Generieren der SASS empfiehlt es sich folgenden Make Befehl auszuführen:

```bash
make build
```

## Veröffentlichen

Sofern du SSH Zugang zum Webserver hast, kannst du die Seite mit folgenden make Befehl deployen:

```bash
make deploy
```
