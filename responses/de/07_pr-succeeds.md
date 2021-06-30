## Schritt 8: Merge deine Pull Request

Gut gemacht @{{ user.username }}! :sparkles:

Du hast erfolgreich eine Pull Request erstellt und alle Tests bestanden. Du kannst jetzt deine Pull Request mergen.

### :keyboard: Activität: Merge die Pull Request

{% if preferences.gitTool == 'cli' %}
1. Auschecken zu dem `main` branch:
    ```shell
    git checkout main
    ```
2. Merge deine Branch:
    ```shell
    git merge {{ branch }}
    ```
3. Übertrage den merged Verlauf an GitHub:
    ```shell
    git push
    ```
4. Lösche den Branch lokal:
    ```shell
    git branch -d {{ branch }}
    ```
{% else %}
1. Klike **Merge pull request**
1. Klike **Confirm merge**
{% endif %}
1. Sobald der Branch merged wurde, brauche man ihn nicht mehr. Klicke auf **Delete branch**.

<hr>
<h3 align="center">Ich antworte wenn diese Branch merged ist.</h3>
