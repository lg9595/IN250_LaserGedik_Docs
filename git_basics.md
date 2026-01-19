# Git Basics – IN250

## Ziel
In dieser Aufgabe habe ich ein GitHub Repository erstellt und meine Schritte mit Markdown dokumentiert.

---

## Repository erstellen
Ich habe auf GitHub ein neues Repository mit dem Namen  
**IN250_LaserGedik_Docs** erstellt.

Dabei habe ich:
- GitHub geöffnet
- Ein neues Repository erstellt
- Das Repository initialisiert mit einer README Datei

---

## Repository lokal klonen
Danach habe ich das Repository auf meinen Computer geklont.

Dazu habe ich:
1. Die Repository URL kopiert
2. In VS Code den Befehl **Git: Clone** verwendet
3. Das Repository lokal geöffnet

---

## Markdown Datei erstellen
Im Repository habe ich die Datei **git_basics.md** erstellt.  
Diese Datei dient zur Dokumentation der Arbeitsschritte.

---

## Änderungen speichern
Nachdem ich den Text geschrieben habe, habe ich die Änderungen gespeichert und in GitHub hochgeladen.

---

## Fazit
GitHub und Markdown sind nützliche Werkzeuge, um Projekte zu versionieren und sauber zu dokumentieren.


---

## Repository klonen

Für diese Aufgabe habe ich mein zuvor erstelltes GitHub Repository auf meinen Computer geklont.

Dazu bin ich wie folgt vorgegangen:
1. Ich habe mein Repository auf GitHub geöffnet
2. Die Repository URL über den „Code“ Button kopiert
3. In VS Code den Befehl **Git: Clone** verwendet
4. Die URL eingefügt und einen lokalen Ordner ausgewählt
5. Das Repository anschliessend in VS Code geöffnet

Nach dem Klonen war das Repository lokal verfügbar und ich konnte mit der Datei `git_basics.md` weiterarbeiten.

---

## Markdown Cheatsheet ins Repository kopieren

Für diese Aufgabe habe ich mein zuvor erstelltes Markdown Cheatsheet in den Ordner meines geklonten Git Repositories kopiert.

Dabei bin ich wie folgt vorgegangen:
1. Ich habe die Datei `markdown_basics.md` aus ihrem ursprünglichen Speicherort kopiert
2. Die Datei in den Ordner des geklonten Repositories eingefügt
3. In VS Code überprüft, dass die Datei als Änderung erkannt wird
4. Die Datei gestaged und einen Commit mit der Nachricht **Initial commit** erstellt
5. Die Änderungen anschliessend auf GitHub hochgeladen

---

## Gitignore Datei erstellen

Für diese Aufgabe habe ich eine `.gitignore` Datei in meinem Git Repository erstellt.

In der Datei habe ich festgelegt, dass:
- alle Dateien mit der Endung `.log` ignoriert werden
- die Datei `GeheimeBankInformationen.txt` nicht von Git versioniert wird

Anschliessend habe ich die `.gitignore` Datei gespeichert, einen Commit mit der Nachricht **Add gitignore** erstellt und die Änderungen auf GitHub hochgeladen.

---

## Zweites lokales Repository mit git init und Remote verbinden

Für diese Aufgabe habe ich einen zweiten lokalen Ordner erstellt und darin ein neues Git Repository initialisiert.

### Vorgehen
1. Neuen Ordner erstellt (zweites lokales Arbeitsverzeichnis)
2. In VS Code geöffnet und im Terminal `git init` ausgeführt
3. Das Remote Repository (GitHub) als `origin` gesetzt
4. Danach versucht, das lokale Repository mit dem Remote zu synchronisieren (`git fetch` / `git pull`)

### Beobachtung
Das neue lokale Repository hatte am Anfang eine andere bzw. leere Historie als das Repository auf GitHub. Beim Synchronisieren gab es deshalb eine Meldung, dass die Historien nicht direkt zusammenpassen bzw. dass ein Merge nicht automatisch möglich ist.

### Was passiert, wenn im alten Ordner vorher gepushed wurde
Wenn ich im alten Ordner die Änderungen bereits auf GitHub gepushed habe, enthält das Remote Repository den aktuellen Stand. Beim Synchronisieren im neuen Ordner werden diese Änderungen vom Remote geholt. Wenn im neuen Ordner bereits Dateien mit gleichem Namen existieren, können Merge Konflikte entstehen.

---

## Aufgabe 6: Warum Git in der Softwareentwicklung wichtig ist

Git wird in der Softwareentwicklung verwendet, um Änderungen am Code nachvollziehbar zu speichern. Jeder Stand eines Projekts kann mit einem Commit festgehalten werden. Dadurch ist es möglich, frühere Versionen wiederherzustellen, Fehler nachzuvollziehen und Änderungen von verschiedenen Personen sauber zusammenzuführen.

Ein weiterer Vorteil von Git ist die Zusammenarbeit im Team. Mehrere Entwickler können gleichzeitig am gleichen Projekt arbeiten, ohne sich gegenseitig zu überschreiben. Git hilft dabei, Änderungen zu vergleichen und Konflikte kontrolliert zu lösen.

Git sorgt ausserdem für Sicherheit, da der Code nicht nur lokal gespeichert ist, sondern auch auf einem Remote Repository wie GitHub. Dadurch geht Arbeit nicht verloren, wenn ein Computer ausfällt oder beschädigt wird.

---

## Warum bei einem Feuer zuerst Git Commit und Git Push erfolgen sollten

Das Beispiel mit dem Feuer soll zeigen, wie wichtig Versionskontrolle ist. Ein Commit speichert den aktuellen Stand des Projekts lokal. Ein Push lädt diesen Stand zusätzlich auf das Remote Repository hoch.

Wenn zuerst ein Commit und danach ein Push gemacht wird, ist der aktuelle Stand des Projekts sicher auf GitHub gespeichert. Selbst wenn der Computer danach zerstört wird, kann der Code jederzeit wiederhergestellt werden.

Ohne Commit und Push wären die letzten Änderungen nur lokal vorhanden und könnten verloren gehen. Das Beispiel verdeutlicht, dass Git nicht nur für Organisation, sondern auch für Datensicherheit wichtig ist.
