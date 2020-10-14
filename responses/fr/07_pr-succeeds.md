## Étape 8: Fusionnez votre Pull Request

Bien joué @{{ user.username }} ! :sparkles:

Vous avez créé avec succès une Pull Request et elle a passé tous les tests avec succès. Vous pouvez maintenant fusionner votre Pull Request.

### :keyboard: Activité: Fusionnez votre Pull Request

{% if preferences.gitTool == 'cli' %}
1. Récupérez votre branche `main` :
    ```shell
    git checkout main
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
1. Cliquez sur **Merge pull request**
1. Cliquez sur  **Confirm merge**
{% endif %}
1. Une fois votre branche fusionnée, vous n'en avez plus besoin. Cliquez **Delete branch**.

<hr>
<h3 align="center">Je vous répondrai lorsque cette Pull Request sera fusionnée.</h3>
