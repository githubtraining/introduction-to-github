## Step 7: Respond to a review

Your pull request is looking great!

Let’s add some content to your file. Replace line 5 of your file with a quotation or meme and witty caption. Remember: [Markdown](https://guides.github.com/features/mastering-markdown/) is supported.

### :keyboard: Activity: Change your file

{% if preferences.gitTool == 'cli' %}
1. Check out to your branch:
    ```shell
    git checkout {{ branch }}
    ```
1. Open the file `_posts/0000-01-02-{{ user.username }}.md`.
1. Replace line 5 of the file with something new. 
1. Stage your new changes:
    ```shell
    git add _posts/0000-01-02-{{ user.username }}.md
    ```
1. Commit your changes:
    ```shell
    git commit -m "<YOUR-MESSAGE>"
    ```
1. Push your edits to GitHub:
    ```shell
    git push
    ```

{% elsif preferences.gitTool == 'vscode' %}
1. Open the file `_posts/0000-01-02-{{ user.username }}.md`.
1. Replace line 5 of the file with something new. 
1. Stage your new changes. As a reminder, you can do this in the Source Control view, click the **+** symbol next to the file.
1. Commit your changes. You can do this in the Source Control view, enter a commit message in the text field and press <kbd>Ctrl+Enter</kbd> on Windows or <kbd>Command ⌘+Enter</kbd> on macOS.
1. Push your edits to GitHub. In the Source Control view, click on the ellipsis (...), and select **Push**.

{% else %}
1. Click the [Files Changed tab]({{ url }}) in this pull request
1. Click on the pencil icon found on the right side of the screen to edit your newly added file
1. Replace line 5 with something new
1. Scroll to the bottom and click **Commit Changes**
{% endif %}

<hr>
<h3 align="center">I'll respond when I detect a commit on this branch.</h3>
