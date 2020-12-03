## Schritt 7: Antwortung eine Bewertung

Deine Pull Request sieht toll aus!

Fügen wir der Datei Inhalte hinzu. Ersetze Zeile 5 der Datei durch ein Zitat oder ein Mem und eine witzige Beschriftung. Denke daran: [Markdown](https://guides.github.com/features/mastering-markdown/) wird unterstützt.

### :keyboard: Activität: Ändere die Datei

{% if preferences.gitTool == 'cli' %}
1. Auschecken zu dein Branch:
    ```shell
    git checkout {{ branch }}
    ```
1. Öffne die Datei `_posts/0000-01-02-{{ user.username }}.md`.
1. Ersetze Zeile 5 der Datei durch etwas Neues.
1. Stelle die neuen Änderungen bereit:
    ```shell
    git add _posts/0000-01-02-{{ user.username }}.md
    ```
1. Commit deine Änderungen:
    ```shell
    git commit -m "<YOUR-MESSAGE>"
    ```
1. Übertrage die Änderungen auf GitHub:
    ```shell
    git push
    ```

{% elsif preferences.gitTool == 'vscode' %}
1. Öffne die Datei `_posts/0000-01-02-{{ user.username }}.md`.
1. Ersetze Zeile 5 der Datei durch etwas Neues.
1. Stelle die neuen Änderungen bereit. Zur Erinnerung, du könntest dies in der Quellcodeverwaltung Ansicht tun, indem du auf das Symbol **+** neben der Datei klicken.
1. Commit deine Änderungen. Man kann dies in der Ansicht Quellcodeverwaltung tun, eine Commit-Mitteilung richt in das Textfeld eingeben und <kbd>Ctrl+Enter</kbd> auf Windows oder <kbd>Command ⌘+Enter</kbd> auf macOS drücken.
1. Klicke auf die Auslassungspunkte (...) and wähle **Push** aus.

{% else %}
1. Klicke die [Files Changed Tab]({{ url }}) in dieser Pull Request
1. Bearbeite die neu hinzugefügte Datei
1. Ersetze Zeile 5 durch etwas Neues
1. Scrolle nach unten und klicke auf **Commit Changes**
{% endif %}

**Hinweis**: Du kannst die Schaltfläche zum Bearbeiten der Datei nicht finden? Es kann wie ein Bleistift aussehen, oder es kann wie erei Punkte aussehen.

<hr>
<h3 align="center">Ich antworte, wenn ich erkenne, dass ein neuer Commit in diesem Branch erstellt wurde.</h3>
