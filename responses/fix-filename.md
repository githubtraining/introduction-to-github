I was expecting your file to be named **{{ expected }}**. 

Let's edit this pull request to fix both of these issues.

## :keyboard: Activity: Fixing your pull request

{% if preferences.gitTool == 'cli' %}
1. Check out to your branch:
    ```shell
    git checkout {{ branch }}
    ```
1. Type `ls` to see a listing of your root directory.
1. Confirm that you've got a folder titled `_posts`.
1. Step into the folder with `cd _posts`.
1. Type `ls` to see a listing of your `_posts` folder.
1. Ensure you've got a file named `{{ expected }}`
1. If you find you have to any changes, then stage, commit, and push those changes:
    ```shell
    git add .
    git commit -m "<YOUR-MESSAGE>"
    git push
    ```
{% else %}
1. Click the [Files Changed tab]({{ url }}) in this pull request
1. Verify that the only file edited is named `{{ expected }}`.
1. If the file is improperly named, or not in an improper location, click on the pencil icon found on the right side of the screen to edit it.
1. Above the contents of the file, select all text in the field that contains the filename and delete it.
1. Continue pressing your backspace key to also delete any directory names that exist.
1. Type the proper filename:
    ```shell
    {{ expected }}
    ```
1. Scroll to the bottom and enter a commit message and commit in the **Commit Changes** section.
{% endif %}

If you would like assistance troubleshooting the issue you are encountering, create a post on the [GitHub Community]({{ communityBoard }}) board. You might also want to search for your issue to see if other people have resolved it in the past.

<hr>
<h3 align="center">I'll respond below when I detect a commit on this branch.</h3>
