## Étape 5: Soumettre un fichier

:tada: Vous avez créé une branche!

Créer une branche vous permet d'apporter des modifications à votre projet sans changer `master`, la branche déployée. Maintenant que vous avez une branche, il est temps de créer un fichier et d'effectuer votre première contribution!

<details><summary>Bases de la contribution</summary>

## Bases de la contribution

Lorsque vous avez fini la création ou l'édition d'un fichier sur GitHub, faites défiler la page jusqu'en bas et répérez la section "Commit new file".

Saisissez un intitulé à la contribution. Ce message doit informer rapidement les contributeurs sur l'objet du changement introduit dans le fichier.

### Règles de bienséance pour l'écriture d'un intitulé de contribution:

- Ne pas terminer votre message par un point.
- Restreignez votre message à 50 caractères ou moins. Ajoutez si nécessaire les détails complémentaires dans la fenêtre de description étendue. Elle se situe juste sous la ligne d'intitulé.
- Utilisez la forme active. Par exemple, "Ajout" au lieu de "Ajouté" and "correction" au lieu de "corrigé".
- Considérez votre intitulé de contribution comme l'expression de votre intention lors de l'introduction du changement.

<hr>
</details>

### :keyboard: Activité: Votre première contribution

Les prochaines étapes vous guideront à travers le processus de soumission d'un changement sur GitHub.

{% if preferences.gitTool == 'cli' %}
1. Récupérez votre branche:
      ```shell
      git checkout {{ thePayload.ref }}
      ```
1. Créez un nouveau fichier nommé `_posts/0000-01-02-{{ user.username }}.md`.
1. Ajoutez le contenu suivant à votre fichier :
      ```yaml 
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
1. Ajoutez votre fichier à l'espace de travail:
      ```shell
      git add _posts/0000-01-02-{{ user.username }}.md
      ```
1. Soumettez le fichiez en fournissant un intitulé :
      ```shell
      git commit -m "<YOUR-MESSAGE>"
      ```
1. Envoyez votre contribution à GitHub:
      ```shell
      git push
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. Dans le dossier `_posts`, créez un nouveau fichier nommé `0000-01-02-{{ user.username }}.md`. Le nom complet de votre fichier doit être: `_posts/0000-01-02-{{ user.username }}.md`.
1. Ajoutez le contenu suivant à votre fichier et enregistrez-le :
      ```yaml 
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
1. Pour ajouter votre fichier à l'espace de travail : allez dans la vue Source Control et cliquez le bouton **+** à côté du fichier. Vous pouvez également vous référer à [la documentation officielle de VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_commit).
      ![a screenshot of the staging button in the source control view](https://user-images.githubusercontent.com/16547949/53641057-d5b8d100-3bfb-11e9-9b69-53b0661cd5cd.png)
1. Soumetez le changement en saisissant un intitulé dans le champ de texte puis en pressant <kbd>Ctrl+Enter</kbd> sur Windows ou <kbd>Command ⌘+Enter</kbd> sur macOS.
      ![a screenshot of the commit message on VS Code](https://user-images.githubusercontent.com/16547949/53641276-698a9d00-3bfc-11e9-9b3d-01680fd01d7c.png)
1. Cliquez sur les points de suspension (...) et sélectionnez **Push**.

{% else %}
1. Sur cette branche, créez un dossier `_posts` et ajoutez y un nouveau fichier nommé `0000-01-02-{{ user.username }}.md`. Vous pouvez le faire en utilisant [ce raccourci]({{ thePayload.repository.html_url }}/new/{{ thePayload.ref }}?filename=_posts/0000-01-02-{{ user.username }}.md) ou manuellement comme suit:
      - Retournez à l'onglet "Code"
      - Dans la liste déroulante des branches, sélectionnez "{{ thePayload.ref }}"
      - Cliquez **Create new file**
      - Dans le champ "file name", saisissez `_posts/0000-01-02-{{ user.username }}.md`. La saisie de `/` dans le nom de fichier placera automatiquement votre fichier dans le répertoire `_posts`.
1. Lorsque vous aurez nommé le fichier, ajoutez-y le contenu suivant:
      ```yaml
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
1. Après avoir ajouté le texte, vous pouvez soumettre le changement en fournissant un intitulé dans le champ de texte sous la fenêtre d'édition du fichier. Des recommendations relatives aux intitulés de soumission sont disponibles via le lien déroulant **Bases de la contribution**, juste au-dessus de ces instructions
1. Une fois saisis votre intitulé de contribution, cliquez **Commit new file**
{% endif %}
<hr>
<h3 align="center">Je vous répondrai lorsque j'aurai détecté une nouvelle contibution sur cette branche.</h3>
