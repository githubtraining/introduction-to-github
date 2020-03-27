## Étape 8: Fusionnez votre demande d'extraction

Bien joué @{{ user.username }} ! :sparkles:

Vous avez créé avec succès une demande d'extraction et elle a réussi tous les tests. Vous pouvez maintenant fusionner votre demande d'extraction.

### :keyboard: Activité: Fusionnez votre demande d'extraction

{% if preferences.gitTool == 'cli' %}
1. Récupérez votre branche `master` :
    ```shell
    git checkout master
    ```
2. Fusionnez votre branche :
    ```shell
    git merge {{ branch }}
    ```
3. Publiez l'historique combiné vers GitHub :
    ```shell
    git push
    ```
4. Supprimez la branche locale :
    ```shell
    git branch -d {{ branch }}
    ```
{% else %}
1. Cliquez **Merge pull request**
1. Cliquez **Confirm merge**
{% endif %}
1. Une fois votre branche fusionnée, vous n'en avez plus besoin. Cliquez **Delete branch**.

<hr>
<h3 align="center">Je vous répondrai lorsque cette demande d'extraction sera fusionnée.</h3>
