## Étape 7: Répondre à une relecture

Votre Pull Request à l'air sensationelle!

Continuons en ajoutant du contenu à votre fichier. Remplacez la ligne 5 de votre fichier par une citation ou un meme et une légende pleine d'esprit. N'oubliez pas: le [Markdown](https://guides.github.com/features/mastering-markdown/) est supporté.

### :keyboard: Activité : Modifier un fichier

{% if preferences.gitTool == 'cli' %}
1. Récupérez votre branche:
    ```shell
    git checkout {{ branch }}
    ```
1. Ouvrez le fichier `_posts/0000-01-02-{{ user.username }}.md`.
1. Remplacez la ligne 5 du fichier par quelque chose de nouveau. 
1. Ajoutez vos changements à l'espace de travail :
    ```shell
    git add _posts/0000-01-02-{{ user.username }}.md
    ```
1. Soumettez vos changements :
    ```shell
    git commit -m "<YOUR-MESSAGE>"
    ```
1. Publiez vers GitHub :
    ```shell
    git push
    ```

{% elsif preferences.gitTool == 'vscode' %}
1. Ouvrez le fichier `_posts/0000-01-02-{{ user.username }}.md`.
1. Remplacez la ligne 5 du fichier par quelque chose de nouveau. 
1. Ajoutez vos changements à l'espace de travail. Pour rappel, vous pouvez effectuer cela dans la vue Source Control, cliquez le symbole **+** à côté du fichier.
1. Soumettez vos changements. Ceci peut se faire depuis la vue Source Control : saisissez un message de commit dans le champ de texte et pressez <kbd>Ctrl+Enter</kbd> sous Windows ou <kbd>Command ⌘+Enter</kbd> sous macOS.
1. Publiez vers GitHub. Dans la vue Source Control, cliquez sur les points de suspension (...) et sélectionnez **Push**.

{% else %}
1. Cliquez [l'onglet Files Changed]({{ url }}) de cette Pull Request
1. Editez votre fichier nouvellement ajouté
1. Remplacez la ligne 5 du fichier par quelque chose de nouveau
1. Défilez vers le bas et cliquez **Commit Changes**
{% endif %}

**Note**: Vous ne trouvez pas le bouton d'édition du fichier ? Il peut ressemble à un crayon ou a des points de suspension.

<hr>
<h3 align="center">Je vous répondrai lorsque j'aurai détecté une nouvelle contibution sur cette branche.</h3>