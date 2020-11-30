## Paso 4: Crea una rama

Completemos el primer paso del flujo de GitHub: crear una rama (o _branch_) <sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup>.

<details><summary>Creando una rama</summary>

## Creando una rama

:tv: [Video: Ramas](https://www.youtube.com/watch?v=xgQmu81G1yY)

Acabas de aprender cómo crear una rama—el primer paso del flujo de GitHub. 

Las ramas son una parte importante del flujo de GitHub porque nos permite separar nuestro trabajo de la rama principal o `master`. En otras palabras, el trabajo de todos está a salvo mientras aportas contribuciones. 

### Tips para usar ramas
Un solo proyecto puede tener cientos de ramas, cada una sugiriendo un nuevo cambio a la rama principal o `master`.

La mejor manera de mantener tus ramas organizadas en un equipo es mantenerlas concisas y efímeras. En otras palabras, una sola rama debería representar solamente una nueva característica o una corrección de errores. Esto permite que haya menos confusión entre colaboradores cuando las ramas solamente están activas por unos días antes de que sean fusionadas <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup> con la rama principal o `master`.  

<hr>
</details>

### :keyboard: Actividad: Tu primera rama

{% if preferences.gitTool == 'cli' %}
1. Abre tu interfaz de línea de comandos (CLI) preferida, a la cual llamaremos shell de aquí en adelante. 
1. Clona este repositorio:
      ```shell
      git clone {{ thePayload.repository.clone_url }}
      ```
1. Navega a este repositorio en tu shell:
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. Crea una rama, usa el nombre que quieras. Siéntete libre de usar el nombre sugerido a continuación.  
      ```shell
      git branch my-slide
      ```
1. Sube la rama a GitHub:
      ```
      git push --set-upstream origin <NOMBRE-DE-LA-RAMA>
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. Descarga y abre [Visual Studio Code](https://code.visualstudio.com/Download) (referido como VS Code) si aún no lo tienes.
1. En VS Code, abre la Paleta de Comandos (o _Command Palette_) usando <kbd>Ctrl+Mayús+P</kbd> en Windows, o <kbd>Command ⌘+Mayús+P</kbd> en macOS. También puedes seguir [la documentación oficial de VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository) sobre clonar repositorios.
1. Escribe `git clone`y presiona <kbd>Enter</kbd>
      ![una captura de pantalla de VS Code con la Paleta de Comandos abierta](https://user-images.githubusercontent.com/16547949/53639288-bcf9ec80-3bf6-11e9-9d18-d97167168248.png)
1. Pega la URL del repositorio en la nueva ventana y presiona <kbd>Enter</kbd>:
      ```shell
      {{ thePayload.repository.clone_url }}
      ```
1. Selecciona la ubicación en el que quieres guardar el repositorio y haz clic en **Choose folder**. Después, abre la ubicación que seleccionaste.  
1. El directorio del repositiorio debería estar ahora abierto en tu proyecto de VS Code. Haz clic en `master` en la parte inferior de la ventana de VS Code. Esto abrirá la Paleta de Comandos con todos los comandos relacionados a ramas de Git. 
      ![una captura de pantalla de las ramas de Git en VS Code](https://user-images.githubusercontent.com/16547949/53639606-adc76e80-3bf7-11e9-98ac-bd41ae2b40db.png)
1. Haz clic en **Create new branch** e ingresa cualquier nombre que le quieras dar a tu rama, como `mi-rama`. A continuación, presiona <kbd>Enter</kbd>.
1. Cuando te hagan seleccionar la rama que servirá de referencia para tu nueva rama, selecciona `master`.
1. Ve a la vista de Source Control, haz clic en los punto suspensivos (...) y selecciona **Push**. En la caja de diálogo preguntándote si quieres publicar tu rama, confirma que sí.
      ![una captura de pantalla de la vista de Source Control en VS Code](https://user-images.githubusercontent.com/16547949/53640015-ee73b780-3bf8-11e9-8c90-be9022b9555a.png)

{% else %}

1. Navega a la  [pestaña titulada Code]({{ thePayload.repository.html_url }})
2. Haz clic en **Branch: master** en el desplegable
3. En el campo, ingresa un nombre para tu rama, como `mi-rama`
4. Haz clic en **Create branch: <nombre>** o presiona la tecla "Enter" para crear tu rama

{% endif %}
<hr>
<h3 align="center">Responderé cuando haya detectado que una nueva rama ha sido creada en este repositorio.</h3>