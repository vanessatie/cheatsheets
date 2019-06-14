# Shell Commands

## Ebenen wechseln

- cd + Directory name = command - open directory
- cd - zurück zum höchsten Verzeichnis (User-Ordner)
- cd .. eine Ebene hoch gehen
- pwd - anzeigen, wo man sich zur Zeit befindet
- open = öffnen - Datei öffnen

## Anzeigen

- ls = list - Liste von Inhalten in aktueller Directory anzeigen
- ls -a - alles in aktueller Directory anzeigen, inkl. versteckter Dateien
- ls -l - Inhalt im Langformat anzeigen
- ls -t - Inhalt mit Details anzeigen
- ls -alt - Inhalt inkl. Details, im Langformat, nach Datum und Zeit geordnet

## Erstellen, Bewegen, kopieren etc.

- mv = move - verschieben (Dateiname und Ziel-Directory)/ umbenennen (zwei Dateinamen)
- mkdir = make directory - neue Directory/ Ordner anlegen
- touch - neue Datei anlegen
- rm = remove/ delete - löschen
- rm -r - Directory mit gesamtem Inhalt löschen
- cp = copy - kopieren (z.B. cp Ort des Files/File name neuer Ort/)
- cp _ - Gruppe kopieren, z.B. cp _ satire/

## Zusätzliches

- echo -
- cat - Inhalt einer Datei anzeigen
- less - ?
- open . - öffnet Dateien
- code . - öffnet die aktuelle Datei in VS Code

## Git

- git status (Abkürzung: gst) - Git-Status abrufen
- git add [Dateiname] - Datei stagen
- git add . (Abkürzung gaa - git add all) - alle Dateien stagen
- git pull - Dateien runterziehen
- git commit -m "[Message]" (Abkürzung: gcmsg - Git Commit Message) - Commit inkl. Message, was/ warum commited wurde
- gcmsg - Git Commit Message
- git log - Infos zum Commit (z.B. zum Branch) --> mit Q wieder raus
- git remote add origin - Befehl, um neues Projekt aus GitLab mit lokal erstelltem PRojekt zu verbinden
- git remote -v - prüfen, ob obenstehender Befehl geklapppt hat
- git push - Repository zu Git pushen
- git push --set-upstream origin master - Festlegen des Streams, wo das lokale Projekt hingepusht werden soll --> ab sofort kann immer git push gemacht werden (erscheint nach git push in der Nachricht/ Vorschlag, wenn das vorher noch nicht gemacht wurde; muss für jedes gemacht werden)
- git branch [Name des Branchs] - Branch erstellen
- git checkout [Name des Branchs] (Kurzform gco)- zum Branch in iterm wechseln
- git merge [Name des Branchs, der gemerged werden soll] - erstellten Branch mergen; dafür im Branch sein, in den hineingemerged werden soll, Name des Branchs eingeben, der darein gemerged werden soll
- git checkout -b [Name des gewünschten neuen Branchs] - Branch erzeugen und gleichzeitig reingehen
- git branch -d [Name des Branches] - Löschen eines Branches
- git branch - Anzeigen aller Branches

- npm - notepack manager
  aus WIM wieder raus mit ZZ

## Allgmeine Befehle in iterm

- Command + d - Neuen Tab in iterm öffnen
- Control + c - Beenden
