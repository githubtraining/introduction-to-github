## Step 5: Commit a file

:tada: You created a branch!

Creating a branch allows you to make modifications to your project without changing the deployed `master` branch. Now that you have a branch, it’s time to create a file and make your first commit!

<details><summary>Commits 101</summary>

## Commits 101

When you’re finished creating or making changes to a file on GitHub, scroll to the bottom of the page. Then find the "Commit new file" section.

In the first field, type a commit message. The commit message should briefly tell contributors about the changes you are introducing to the file.

### Rules to live by for commit messages:

- Don’t end your commit message with a period.
- Keep your commit messages to 50 characters or less. Add extra detail in the extended description window if necessary. This is located just below the subject line.
- Use active voice. For example, "add" instead of "added" and "merge" instead of "merged".
- Think of your commit as expressing intent to introduce a change.

<hr>
</details>

### :keyboard: Activity: Your first commit

The following steps will guide you through the process of committing a change on GitHub.

{% if preferences.gitTool == 'cli' %}
1. Check out to your branch:
      ```shell
      git checkout {{ thePayload.ref }}
      ```
1. Create a new file named `_posts/0000-01-02-{{ user.username }}.md`.
1. Add the following content to your file:
      ```yaml 
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
1. Stage your new file:
      ```shell
      git add _posts/0000-01-02-{{ user.username }}.md
      ```
1. After adding the text, commit the change and a commit message, check out the **Commits 101** drop-down, just above these instructions:
      ```shell
      git commit -m "<YOUR-MESSAGE>"
      ```
1. Push your new commit to GitHub:
      ```shell
      git push
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. In the `_posts` folder, create a new file named `0000-01-02-{{ user.username }}.md`. The full path to your file will be: `_posts/0000-01-02-{{ user.username }}.md`.
1. Add the following content to your file and save it:
      ```yaml 
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
1. To stage your new file: go to the Source Control view and click the **+** button next to the file. You can also follow along with [VS Code's official documentation](https://code.visualstudio.com/docs/editor/versioncontrol#_commit).
      ![a screenshot of the staging button in the source control view](https://user-images.githubusercontent.com/16547949/53641057-d5b8d100-3bfb-11e9-9b69-53b0661cd5cd.png)
1. Commit the change by typing a commit message in the text field and pressing <kbd>Ctrl+Enter</kbd> on Windows or <kbd>Command ⌘+Enter</kbd> on macOS.
      ![a screenshot of the commit message on VS Code](https://user-images.githubusercontent.com/16547949/53641276-698a9d00-3bfc-11e9-9b3d-01680fd01d7c.png)
1. Click on the ellipsis (...) and select **Push**.

{% else %}
1. Create a new file on this branch, in a `_posts` folder called `0000-01-02-{{ user.username }}.md`. You can do so using [this shortcut]({{ thePayload.repository.html_url }}/new/{{ thePayload.ref }}?filename=_posts/0000-01-02-{{ user.username }}.md) or manually as follows:
      - Return to the "Code" tab
      - In the branch drop-down, select "{{ thePayload.ref }}"
      - Click **Create new file**
      - In the "file name" field, type `_posts/0000-01-02-{{ user.username }}.md`. Entering the `/` in the filename will automatically place your file in the `_posts` directory.
1. When you’re done naming the file, add the following content to your file:
      ```yaml
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
1. After adding the text, you can commit the change by entering a commit message in the text-entry field below the file edit view. For guidelines on commit messages, check out the **Commits 101** drop-down, just above these instructions
1. When you’ve entered a commit message, click **Commit new file**
{% endif %}
<hr>
<h3 align="center">I'll respond when I detect a new commit on this branch.</h3>
