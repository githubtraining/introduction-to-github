Ich hatte erwartet, das die Datei bennant wird **{{ expected }}**. 

Lasse uns diese Pull Request bearbeiten, um diese beiden Probleme zu beheben.

## :keyboard: Activität: Fixieren der Pull Request

{% if preferences.gitTool == 'cli' %}
1. Auschecken zu dein Branch:
    ```shell
    git checkout {{ branch }}
    ```
1. Gebe `ls` ein, um eine Liste des Stammverzeichnisses anzuzeigen.
1. Bestätige, dass du einen Ordner mit dem Titel `_posts` habe.
1. Betrete den Ordner mit `cd _posts`.
1. Gebe `ls` ein, um eine Liste des Ordners `_posts` anzuzeigen.
1. Stelle sicher, dass es eine Datei mit dem Namen `{{ expected }}` gibt.
1. Wenn du feststellst, dass du Änderungen vornehmen müsst, müsst du diese Änderungen bereitstellen, festschreiben und vorantreiben:
    ```shell
    git add .
    git commit -m "<YOUR-MESSAGE>"
    git push
    ```
{% else %}
1. Klicke die [Files Changed Tab]({{ url }}) in diesem Pull Request.
1. Stelle sicher, dass die einzige bearbeitete Datei den Namen `{{ expected }}` hat.
1. Wenn die Datei falsch benannt ist oder sich nicht an einem geeigneten Ort befindet, korrigiere sie mit der Bearbeitungsfunktion.
1. Wähle über dem Inhalt der Datei den gesamten Text in dem Feld aus, das den Dateinamen enthält, und lösche ihn.
1. Drücke weiterhin die Rücktaste, um auch vorhandene Verzeichnisnamen zu löschen.
1. Gebe den richtigen Dateinamen ein:
    ```shell
    {{ expected }}
    ```
1. Scrolle nach unten und gebe eine Commit-Mitteilung und ein Commit in Abschnitt **Commit Changes** ein.
{% endif %}

**Hinweis**: Du kannst die Schaltfläche zum Bearbeiten der Datei nicht finden? Es kann wie ein Bleistift aussehen, oder es kann wie erei Punkte aussehen.

Wenn man Hilfe bei der Fehlerbehebung für das Problem benötige, erstelle einen Beitrag auf der [GitHub Community]({{ communityBoard }}) Forum. Möglicherweise möchte man auch nach dem Problem suchen, um festzustellen, ob andere Personen es in der Vergangenheit erhalten haben.

<hr>
<h3 align="center">Ich antworte, wenn ich erkenne, dass ein neuer Commit in diesem Branch erstellt wurde.</h3>

