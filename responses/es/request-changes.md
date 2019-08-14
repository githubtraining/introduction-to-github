## Paso 7: Responde a una revisión

¡Tu solicitud de extracción se ve súper bien!

Agreguemos contenido a tu archivo. Reemplaza la línea 5 de tu archivo con una cita textual o con un meme y una leyenda chistosa. Recuerda: Usar el formato[Markdown](https://guides.github.com/features/mastering-markdown/) es aceptado.

### :keyboard: Actividad: Actualiza tu archivo

{% if preferences.gitTool == 'cli' %}
1. Usa el comando checkout para cambiar de rama:
    ```shell
    git checkout {{ branch }}
    ```
1. Abre el archivo `_posts/0000-01-02-{{ user.username }}.md`.
1. Reemplaza la línea 5 de tu archivo con algo nuevo.
1. Añade tus nuevos cambios:
    ```shell
    git add _posts/0000-01-02-{{ user.username }}.md
    ```
1. Haz una confirmación de cambios para las modificaciones que acabas de hacer:
    ```shell
    git commit -m "<YOUR-MESSAGE>"
    ```
1. Sube tus cambios a GitHub:
    ```shell
    git push
    ```

{% elsif preferences.gitTool == 'vscode' %}
1. Abre el archivo `_posts/0000-01-02-{{ user.username }}.md`.
1. Reemplaza la línea 5 de tu archivo con algo nuevo.
1. Añade tus nuevos cambios. Recuerda: puedes hacer esto desde la vista de Source Control, haz click en el símbolo **+** al lado del archivo.
1. Haz una confirmación de cambios. Puedes hacer esto desde la vista de Source Control, incluyendo un mensaje de confirmación en el recuadro de texto y después presionando <kbd>Ctrl+Enter</kbd> en Windows o <kbd>Command ⌘+Enter</kbd> en macOS.
1. Sube tus cambios a GitHub. En la vista de Source Control, haz click en los puntos suspensivos (...), y selecciona **Push**.

{% else %}
1. Haz click en [Files Changed tab]({{ url }}) en esta solicitud de extracción
1. Haz click en el ícono de lápiz que puedes encontrar al lado derecho de tu pantalla para editar el archivo que acabas de agregar.
1. Reemplaza la línea 5 con algo nuevo.
1. Navega hacia abajo y haz click en **Commit Changes**
{% endif %}

<hr>
<h3 align="center">Responderé cuando detecte una confirmación de cambios en esta rama</h3>
