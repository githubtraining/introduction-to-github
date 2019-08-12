## Paso 8: Une tus pull request

Bien hecho @{{ user.username }}! :sparkles:

Has creado un pull request satisfactoriamente, y ha pasado todas las pruebas. Ahora puedes unir tu pull request.

### :keyboard: Actividad: Une tu pull request

{% if preferences.gitTool == 'cli' %}
1. Haz checkout de la rama `master`:
    ```shell
    git checkout master
    ```
2. Une tu rama:
    ```shell
    git merge {{ branch }}
    ```
3. Empuja tu historial unido a GitHub:
    ```shell
    git push
    ```
4. Borra tu rama localmente:
    ```shell
    git branch -d {{ branch }}
    ```
{% else %}
1. Haz click en **Merge pull request**
1. Haz click en **Confirm merge**
{% endif %}
1. Cuando tu rama se haya unido, no la necesitarás nuevamente. Haz click en **Delete branch**.

<hr>
<h3 align="center">Responderé cuando este pull request se haya unido.</h3>
