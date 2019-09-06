 FFNBSee-Webseite
======================
Internetseiten des Fördervereins Freie Netze Bodensee e.V.

Wir verwenden [lektro](https://getlektor.com) zum generieren der Seite.

 Installation
--------------
lektor ist ist ein Python Programm und kann mit pip installiert werden.
Dafür haben wir dir ein Makefile vorbereitet und kannst das mit folgenden Befehl installieren *(nachdem du das git repo geklont hast)*
```bash
# lektor mit abhängigkeiten installieren
make install
```

 Lektor Server
--------------
Um die Webseite zu bearbeiten empfiehlt es sich einen lokalen Webserver laufen zu lassen und darin die Webseite zu bearbeiten.
Dieses läuft Standardmäßig auf ``http://localhost:5000``.

Das lässt sich starten mit dem folgenden Befehl aus der Makefile:
```
make server
```

 LFS:
---
Wir speichern LFS Dateien in einem Repo auf [gitea.see-base.de](https://gitea.see-base.de/FFBSee/ffnbsee-website.git):
```txt
https://gitea.see-base.de/FFBSee/ffnbsee-website.git
```

 SASS/CSS
--------
Bei Problemen mit dem lokal generieren der SASS empfiehlt es sich folgenden Make Befehl auszuführen:
```bash
make build
```

 Veröffentlichen
----------------
Sofern du SSH Zugang zum Webserver hast, kannst du das mit folgenden make Befehl deployen:
```bash
make deploy
```
