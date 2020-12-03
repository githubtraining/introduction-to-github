## Schritt 5: Commit eine Datei

:tada: Du hast eine Branche erstellt!

Beim Branche Erstellungen kann man Änderungen machen zum Projekt, ohne Änderung zur `main` Branche. Nachdem du eine Branch hast, ist es zeit eine neue Datei zu erstellen, und auch deine erste Commit durchzuführen.

<details><summary>Commits 101</summary>

## Commits 101

Wenn man fertig ist, mit Dateischaffungen oder Änderungen, scrolle bis zum Ende des Seite. Dann, finde die "Commit new file" teil.

In der erste Sektor, schreiben eine Commit-Mitteilung. Die Commit-Mitteilung ist ein kurzer, beschreibender Text zu einem Commit, in dem die Änderung kommuniziert wird, die der Commit nach sich zieht.

### Regeln für Commit-Mitteilungen:

- Ende Commit-Mitteilungen ohne punkt.
- Halten Commit-Mitteilungen weniger als 50 Charakter. Zusätzliche Details wird hinzugefügt in dem “extended description” schaufenster wenn es nötig ist. Dass findet man direkt unter die Subjekt-Linie. 
- Aktive schreiben. Zum Beispiel, “schreiben”, statt “geschrieben”, oder "merge" instead of "merged".
- Erwägen deinen Commit wie ein Ausdrück deine Absicht, eine Änderung vorzustellen.

<hr>
</details>

### :keyboard: Activität: Deine erste Commit

Die folgenden Schritte führen du durch die Prozess, eine Änderung an GitHub zu Commiten.

{% if preferences.gitTool == 'cli' %}
1. Auschecken zu dein Branch:
      ```shell
      git checkout {{ thePayload.ref }}
      ```
1. Erstelle eine neue Datei mit dem Namen `_posts/0000-01-02-{{ user.username }}.md`.
1. Füge deiner Datei den folgenden Inhalt hinzu:
      ```yaml 
      ---
      layout: slide
      title: "Willkommen zu unserer zweiten Folie!"
      ---
      Dein text
      Verwenden Sie den Pfeil nach links, um zurückzukehren!
      ```
1. Stelle deine neue Datei bereit:
      ```shell
      git add _posts/0000-01-02-{{ user.username }}.md
      ```
1. Nachdem du deine Text hinzugefügt hat, Commit die Änderung und gebe eine Commit-Mitteilung ein. Richtlinien zum Commit-Mitteilungen finde auf der **Commits 101** Menu, direkt über diesen Anweisungen:
      ```shell
      git commit -m "<YOUR-MESSAGE>"
      ```
1. Pushe deine neue Commit zu GitHub:
      ```shell
      git push
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. In dem `_posts` Folie, erstelle eine neue Datei mit dem Namen `0000-01-02-{{ user.username }}.md`. Der vollständige Pfad zu Ihrer Datei lautet: `_posts/0000-01-02-{{ user.username }}.md`.
1. Stelle und speichere deine neue Datei bereit:
      ```yaml 
      ---
      layout: slide
      title: "Willkommen zu unserer zweiten Folie!"
      ---
      Dein text
      Verwenden Sie den Pfeil nach links, um zurückzukehren!
      ```
1. Um deine neue Folie zu vorbereiten: gehe zur Quellcodeverwaltungsansicht und klicke auf die Schaltfläche **+** neben der Datei. Du kannst auch mit [VS Code's offizielle Dokumentation (auf Englisch)](https://code.visualstudio.com/docs/editor/versioncontrol#_commit) folgen.
      ![a screenshot of the staging button in the source control view](https://user-images.githubusercontent.com/16547949/53641057-d5b8d100-3bfb-11e9-9b69-53b0661cd5cd.png)
1. Commit die Änderung, indem du eine Commit-Mitteilung in das Textfeld eingeben und drücken <kbd>Ctrl+Enter</kbd> auf Windows or <kbd>Command ⌘+Enter</kbd> auf macOS.
      ![a screenshot of the commit message on VS Code](https://user-images.githubusercontent.com/16547949/53641276-698a9d00-3bfc-11e9-9b3d-01680fd01d7c.png)
1. Klicke auf die Auslassungspunkte (...) and wähle **Push** aus.

{% else %}
1. Erstelle eine neue Datei in dem `_posts` Folie, mit dem Namen `0000-01-02-{{ user.username }}.md`. Du kannst das mit [diese Abkürzung]({{ thePayload.repository.html_url }}/new/{{ thePayload.ref }}?filename=_posts/0000-01-02-{{ user.username }}.md) oder manuell wie folgt:
      - Kehre zur Registerkarte “Code” zurück
      - In der Dropdown-Liste, wähle "{{ thePayload.ref }}" aus
      - Klicke **Create new file**
      - In dem "file name" Sektor, schreibe `_posts/0000-01-02-{{ user.username }}.md`. Wenn man das `/` in den Dateinamen eingebe, wird die Datei automatisch im Verzeichnis `_posts` abgelegt.
1. When you’re done naming the file, add the following content to your file:
      ```yaml
      ---
      layout: slide
      title: "Willkommen zu unserer zweiten Folie!"
      ---
      Dein text
      Verwenden Sie den Pfeil nach links, um zurückzukehren!
      ```
1. Nach dem Hinzufügen des Textes kann man die Änderung festschreiben, indem man eine Commit-Mitteilung in das Texteingabefeld unterhalb der Datei Bearbeitungsansicht eingeben. Richtlinien zum Commit-Mitteilungen finde auf der **Commits 101** Menu, direkt über diesen Anweisungen.
1. Wenn du ein Commit-Mitteilung eingegeben habe, klicke **Commit new file**.
{% endif %}
<hr>
<h3 align="center">Ich antworte, wenn ich erkenne, dass ein neuer Commit in diesem Branch erstellt wurde.</h3>


