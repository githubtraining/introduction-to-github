## Step 8: Merge your pull request

Nicely done @{{ user.username }}! :sparkles:

You successfully created a pull request, and it has passed all of the tests. You can now merge your pull request.

### :keyboard: Activity: Merge the pull request

{% if preferences.gitTool == 'cli' %}
1. Check out to the `master` branch:
    ```shell
    git checkout master
    ```
2. Merge your branch:
    ```shell
    git merge {{ branch }}
    ```
3. Push the merged history to GitHub:
    ```shell
    git push
    ```
4. Delete your the branch locally:
    ```shell
    git branch -d {{ branch }}
    ```
{% else %}
1. Click **Merge pull request**
1. Click **Confirm merge**
{% endif %}
1. Once your branch has been merged, you don't need it anymore. Click **Delete branch**.

<hr>
<h3 align="center">I'll respond when this pull request is merged.</h3>
