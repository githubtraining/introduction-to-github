## Paso 8: Fusiona tu solicitud de extracción

Bien hecho @{{ user.username }}! :sparkles:

Has creado una solicitud de extracción satisfactoriamente, y ha pasado todas las pruebas. Ahora puedes fusionar tu solicitud de extracción.

### :keyboard: Actividad: Fusiona tu solicitud de extracción

{% if preferences.gitTool == 'cli' %}
1. Usa el checkout para cambiarte a la rama `master`:
    ```shell
    git checkout master
    ```
2. Fusiona tu rama:
    ```shell
    git merge {{ branch }}
    ```
3. Sube tu historial de fusión a GitHub:
    ```shell
    git push
    ```
4. Elimina tu rama localmente:
    ```shell
    git branch -d {{ branch }}
    ```
{% else %}
1. Haz clic en **Merge pull request**
1. Haz clic en **Confirm merge**
{% endif %}
1. Cuando tu rama se haya fusionado, ya no la vas a necesitar. Haz clic en **Delete branch**.

<hr>
<h3 align="center">Responderé cuando esta solicitud de extracción se haya fusionado.</h3>
