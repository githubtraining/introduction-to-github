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
{% else %}
1. Click the "Files Changed" tab in this pull request
1. Click on the pencil icon found on the right side of the screen
1. Replace line 5 with something new
1. Scroll to the bottom and click **Commit Changes**
{% endif %}

<hr>
<h3 align="center">Watch below for my response</h3>
