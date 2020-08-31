## Paso 5: Confirma un archivo

:tada: ¡Haz creado una rama!

Crear una rama te permite hacer modificaciones a tu proyecto sin tener que cambiar la rama `master`. Ahora que tienes una rama, es hora de crear un archivo y ¡hacer tu primera confirmación de cambios!

<details><summary>Commits 101</summary>

## Commits 101

Cuando hayas terminado de crear o hacer cambios a tu archivo en GitHub, desplázate hasta la parte inferior de la página. Después, encuentra la sección titulada "Commit new file".

En el primer campo, escribe un mensaje de confirmación (o _commit message_). El mensaje debe informar a tus colaboradores de forma breve sobre los cambios que has introducido al archivo. 

### Recomendaciones para los mensajes de confirmación:

- No termines tu mensaje con un punto. 
- Mantén tu mensaje con 50 o menos caracteres. Si es necesario añade detalles extra en la ventana de descripción extendida. Esta se encuentra justo debajo de la línea de asunto. 
- Usa la voz activa. Por ejemplo, "añade" en vez de "añadí" y "une" en vez de "uní".
- Piensa en tu confirmación de cambios como una manera de expresar que quieres introducir una modificación. 

<hr>
</details>

### :keyboard: Actividad: Tu primera confirmación de cambios (o _commit_)

Los siguientes pasos te guiarán a través del proceso de hacer una confirmación de cambios (_commit_) para una modificación en GitHub. 

{% if preferences.gitTool == 'cli' %}
1. Selecciona tu rama:
      ```shell
      git checkout {{ thePayload.ref }}
      ```
1. Crea un nuevo archivo llamado `_posts/0000-01-02-{{ user.username }}.md`.
1. Añade el siguiente contenido a tu archivo:
      ```yaml 
      ---
      layout: slide
      title: "Bienvenidos a la segunda página!"
      ---
      Tu texto
      Utiliza la flecha hacia la izquierda para volver!
      ```
1. Añade tu nuevo archivo:
      ```shell
      git add _posts/0000-01-02-{{ user.username }}.md
      ```
1. Después de añadir tu texto, haz una confirmación de cambios y agrega un mensaje de confirmación, comprueba el desplegable **Commits 101**, justo arriba de estas instrucciones:
      ```shell
      git commit -m "<TU-MENSAJE>"
      ```
1. Manda tu nueva confirmación de cambios a GitHub:
      ```shell
      git push
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. En el directorio `_posts` , crea un nuevo archivo llamado `0000-01-02-{{ user.username }}.md`. La ruta completa a tu archivo será: `_posts/0000-01-02-{{ user.username }}.md`.
1. Añade el siguiente contenido a tu archivo y guárdalo:
      ```yaml 
      ---
      layout: slide
      title: "Bienvenidos a la segunda página!"
      ---
      Tu texto
      Utiliza la flecha hacia la izquierda para volver!
      ```
1. Para añadir tu nuevo archivo ve a la vista de Source Control y haz clic en el botón **+** a lado del archivo. También puedes seguir este paso con la [documentación oficial de VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_commit).
      ![una captura del botón de staging en la vista Source  Control](https://user-images.githubusercontent.com/16547949/53641057-d5b8d100-3bfb-11e9-9b69-53b0661cd5cd.png)
1. Haz una confirmación de cambios escribiendo un mensaje de confirmación en el campo de texto y después presionando<kbd>Ctrl+Enter</kbd> en Windows o <kbd>Comando ⌘+Enter</kbd> en macOS.
      ![una captura del mensaje de confirmación de cambios VS Code](https://user-images.githubusercontent.com/16547949/53641276-698a9d00-3bfc-11e9-9b3d-01680fd01d7c.png)
1. Haz clic en los puntos suspensivos (...) y selecciona **Push**.

{% else %}
1. Crea un nuevo archivo en esta rama, en un directorio llamado `_posts` y llámalo `0000-01-02-{{ user.username }}.md`. Lo puedes hacer usando [este atajo]({{ thePayload.repository.html_url }}/new/{{ thePayload.ref }}?filename=_posts/0000-01-02-{{ user.username }}.md) o manualmente de la siguiente manera:
      - Regresa a la pestaña "Code"
      - En la lista desplegable de ramas, selecciona "{{ thePayload.ref }}"
      - Haz clic en **Create new file**
      - En el campo "file name", escribe `_posts/0000-01-02-{{ user.username }}.md`. Escribir `/` en el nombre del archivo va a poner tu archivo automáticamente en el directorio `_posts`.
1. Cuando hayas acabado de nombrar tu archivo, añade el siguiente contenido a tu archivo:
      ```yaml 
      ---
      layout: slide
      title: "Bienvenidos a la segunda página!"
      ---
      Tu texto
      Utiliza la flecha hacia la izquierda para volver!
      ```
1. Después de añadir tu texto, puedes hacer una confirmación de cambios al agregar un mensaje de confirmación en el campo text-entry abajo de la vista de edición de archivo. Para más información sobre mensajes de confirmación, comprueba el desplegable **Commits 101** , justo arriba de estas instrucciones:
1. Cuando hayas escrito tu mensaje de confirmación , haz clic en **Commit new file**
{% endif %}
<hr>
<h3 align="center">Responderé cuando haya detectado una nueva confirmación de cambio en esta rama.</h3>
