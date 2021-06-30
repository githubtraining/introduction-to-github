Translation
## Schritt 4: Erstellung eines Branches

Schließen wir den ersten Schritt des GitHub-Flow ab: die Erstellung eines Branches.<sup>[:book:](https://docs.github.com/de/free-pro-team@latest/github/getting-started-with-github/github-glossary#branch)</sup>.

<details><summary>Die Erstellung eines Branches</summary>

## Die Erstellung eines Branches

:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

Du hast gerade gelernt, wie man einen Branch erstellt -- der erste Schritt in dem GitHub-Flow.

Branches sind ein wichtiger Aspekt des GitHub-Flow, weil sie uns die Möglichkeit geben, unsere Arbeit von dem Basis-Branch zu trennen. Quasi bleiben die Arbeitsergebnisse von allen sicher während du einen Beitrag leistest.

### Hinweise für die Branch-Benutzung

Jedes Projekt könnte hunderte von Branches haben, von denen jeder eine neue Änderung zum Basis-Branch vorschlägt.

Die beste Art und Weise um die Ordnung der Branches mit einem Team zu wahren, ist die Branches prägnant und kurzlebig zu halten. Quasi sollte jeder Branch ein einzelnes neues Feature oder Bug-Fix repräsentieren. Branches, die nur für ein paar Tage aktiv sind, bevor sie mit dem Basis-Branch verbunden werden, reduzieren Verwirrung zwischen anderen Mitwirkenden. <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup>.

<hr>
</details>

### :keyboard: Aufgabe: Dein erster Branch

{% if preferences.gitTool == 'cli' %}
1. Öffne deine bevorzugte Befehlszeile, die wir ab sofort deinen Shell nennen.
1. Klone dieses Repository:
      ```shell
      git clone {{ thePayload.repository.clone_url }}
      ```
1. Steure zum Repository in deinem Shell:
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. Erstelle einen Branch mit einem beliebigen Namen. Du könntest die unten vorgeschlagenen Namen verwenden. 
      ```shell
      git branch my-slide
      ```
1. Pushe den Branch zu GitHub:
      ```
      git push --set-upstream origin <BRANCH-NAME>
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. Wenn du Visual Studio Code (VS Code) noch nicht hast, [lade es herunter](https://code.visualstudio.com/Download) und öffne es.
1. Öffne die Command Palette in VS Code mit <kbd>Ctrl+Shift+P</kbd> für Windows, oder <kbd>Command ⌘+Shift+P</kbd> für macOS. Du kannst auch [VS Codes offizieller Dokumentation](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository) über das Klonen folgen.
1. Tippe: `git clone` und drücke <kbd>Enter</kbd> 
      ![a screenshot of vs code with the command palette open](https://user-images.githubusercontent.com/16547949/53639288-bcf9ec80-3bf6-11e9-9d18-d97167168248.png)
1. Füge die Repository-URL in das neue Fenster ein und drücke <kbd>Enter</kbd>:
      ```shell
      {{ thePayload.repository.clone_url }}
      ```
1. Wähle den Ort, in dem das Repository gespeichert werden soll, und klicke **Choose folder**. Dann öffne den ausgewählten Ort. 
2. Der Repository-Ordner sollte jetzt in deinem VS Code Projekt geöffnet sein. Klicke auf `main` unten im VS Code Fenster. Das wird die Command Palette mit den relevanten Befehlen für Git-Branches laden.
      ![a screenshot of the Git branches in VS Code](https://user-images.githubusercontent.com/16547949/53639606-adc76e80-3bf7-11e9-98ac-bd41ae2b40db.png)
3. Klicke **Create new branch** und gebe einen beliebigen Branch-Namen ein, zum Beispiel `meine-folie`. Dann drücke <kbd>Enter</kbd>.
4. Wenn du dann aufgefordert wirst, einen Ref auszuwählen von dem der Branch erstellt wird, wähle `main`.
5. Gehe zu der “Source Control” Ansicht, klicke auf die Ellipsis (...) und wähle **Push**. Bestätige die Dialog-Box, die nachfragt, ob du den Branch veröffentlichen möchtest. 
      ![a screenshot of the source control view in VS Code](https://user-images.githubusercontent.com/16547949/53640015-ee73b780-3bf8-11e9-8c90-be9022b9555a.png)

{% else %}

1. Steure zum [Code seite]({{ thePayload.repository.html_url }})
2. Klicke auf **Branch: main** in dem Menü
3. Fülle in der Lücke einen Namen für deinen Branch aus, wie z.B. `meine-folie`.
4. Klicke auf **Create branch: <name>** oder drücke die <kbd>Enter</kbd> Taste, um deinen Branch zu erstellen.

{% endif %}
<hr>
<h3 align="center">Ich antworte, wenn ich erkenne, dass ein neuer Branch in diesem Repository erstellt wurde.</h3>

