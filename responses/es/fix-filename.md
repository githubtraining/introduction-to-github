Esperaba que tu archivo se llamara **{{ expected }}**.

Editemos este pull request para arreglar ambos issues.

## :keyboard: Actividad: Arregla tu pull request

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
1. Si encuentras que tienes que hacer cambios, entonces añade, commit, y empuja esos cambios:
    ```shell
    git add .
    git commit -m "<YOUR-MESSAGE>"
    git push
    ```
{% else %}
1. Haz click en la pestaña [Files Changed]({{ url }}) en este pull request
1. Verifica que sólo el archivo que editaste se llame `{{ expected }}`.
1. Si el archivo tiene el nombre incorrecto, o no esta en el lugar incorrecto, haz click en el ícono de lápiz que se encuentra al lado derecho de la pantalla para editar.
1. Arriba del contenido del archivo, selecciona "all text" en el campo que contiene el nombre del archivo y bórralo.
1. Continúa presionando la tecla backspace para también borrar cualquier directorio que exista.
1. Escribe el nombre de archivo apropiado:
    ```shell
    {{ expected }}
    ```
1. Desplázate hasta el fondo de la página y escribe un mensaje de commit y commit en la sección **Commit Changes** .
{% endif %}

Si necesitas ayuda buscando solución a tu problema, crea un post en [GitHub Community]({{ communityBoard }}) . También puedes buscar otros posts acerca de tu issue si otras personas lo han resuelto previamente.

<hr>
<h3 align="center">Responderé abajo cuando detecte un commit en esta rama.</h3>
