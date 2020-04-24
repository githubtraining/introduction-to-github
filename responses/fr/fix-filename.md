J'espérai que votre fichier soit nommé **{{ expected }}**. 

Editons cette Pull Request afin de corriger ce problème.

## :keyboard: Activité: Corriger votre Pull Request

{% if preferences.gitTool == 'cli' %}
1. Récupérez votre branche :
    ```shell
    git checkout {{ branch }}
    ```
1. Tapez `ls` afin d'obtenir le contenu votre répertoire racine.
1. Confirmez que vous possédez un répertoire nommé `_posts`.
1. Déplacez vous dans le répertoire à l'aide de la commande `cd _posts`.
1. Tapez `ls` afin d'obtenir le contenu votre répertoire `_posts`.
1. Vérifiez que vous possédez un fichier nommé `{{ expected }}`.
1. Si vous constatez que vous devez effectuer des changements, ajoutez les à l'espace de travail, soumettez puis publiez les :
    ```shell
    git add .
    git commit -m "<YOUR-MESSAGE>"
    git push
    ```
{% else %}
1. Cliquez [l'onglet Files Changed]({{ url }}) dans cette Pull Request
1. Vérifiez que le seul fichier édité se nomme `{{ expected }}`.
1. Si le fichier n'est pas correctement nommé, ou n'est pas au bon endroit, utilisez la fonctionalité d'édition afin de corriger cela.
1. Au dessus du contenu du fichier, sélectionnez tout le texte du champ contenant le nom du fichier et supprimez ce texte.
1. Continuez de presser la touche retour arrière (<kbd>Backspace</kbd>) afin de supprimer également d'éventuels noms de répertoire.
1. Saisissez le nom de fichier correct:
    ```shell
    {{ expected }}
    ```
1. Faites défiler la fenêtre jusqu'en bas puis, dans la section **Commit Changes**, saisissez un intitulé de contribution et soumettez le.
{% endif %}

**Note**: Vous ne trouvez pas le bouton d'édition du fichier ? Il peut ressemble à un crayon ou a des points de suspension.

ISi vous avez besoin d'assistance, créez une convesation sur le forum [GitHub Community]({{ communityBoard }}). Vous pouvez également y effectuer une recherche et vérifier si d'autres n'ont pas rencontré et résolu un problème similaire dans le passé. 

<hr>
<h3 align="center">Je vous répondrai lorsque j'aurai détecté une contribution sur cette branche.</h3>
