Esperaba que tu archivo se llamara **{{ expected }}**.

Editemos esta solicitud de extracción para arreglar ambos problemas.

## :keyboard: Actividad: Arregla tu solicitud de extracción

{% if preferences.gitTool == 'cli' %}
1. Revisa tu rama:
    ```shell
    git checkout {{ branch }}
    ```
1. Escribe `ls` para ver un listado del contenido de tu directorio de raíz.
1. Confirma que tienes un directorio llamado `_posts`.
1. Entra al directorio usando `cd _posts`.
1. Escribe `ls` para ver un listado de el contenido de tu directorio `_posts`.
1. Asegúrate que tienes un archivo llamado `{{ expected }}`
1. Si encuentras que tienes que hacer cambios, entonces añade, confirma tus cambios, y sube esos cambios:
    ```shell
    git add .
    git commit -m "<TU-MENSAJE>"
    git push
    ```
{% else %}
1. Haz clic en la pestaña [Files Changed]({{ url }}) en esta solicitud de extracción
1. Verifica que sólo el archivo que editaste se llame `{{ expected }}`.
1. Si el archivo tiene el nombre incorrecto, o no esta en el lugar correcto, haz clic en el icono de lápiz que se encuentra al lado derecho de la pantalla para editar.
1. Arriba del contenido del archivo, selecciona "all text" en el campo que contiene el nombre del archivo y bórralo.
1. Continúa presionando la tecla backspace para también borrar cualquier directorio que exista.
1. Escribe el nombre de archivo apropiado:
    ```shell
    {{ expected }}
    ```
1. Desplázate hasta el final de la página y escribe un mensaje de confirmación y haz una confirmación de cambios en la sección **Commit Changes** .
{% endif %}

Si necesitas ayuda buscando solución a tu problema, crea una publicación en [GitHub Community]({{ communityBoard }}). También puedes buscar otras publicaciones acerca de tu issue si otras personas lo han resuelto previamente.

<hr>
<h3 align="center">Responderé abajo cuando detecte una confirmación de cambios en esta rama.</h3>
