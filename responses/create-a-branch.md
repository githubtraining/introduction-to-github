## Step 4: Create a branch

Let’s complete the first step of the GitHub flow: creating a branch <sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup>.

<details><summary>Creating a branch</summary>

## Creating a branch

:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

You just learned how to create a branch—the first step in the GitHub flow.

Branches are an important part of the GitHub flow because they allow us to separate our work from the `master` branch. In other words, everyone's work is safe while you contribute.

### Tips for using branches

A single project can have hundreds of branches, each suggesting a new change to the `master` branch.

The best way to keep branches organized with a team is to keep them concise and short-lived. In other words, a single branch should represent a single new feature or bug fix. This reduces confusion among contributors when branches are only active for a few days before they’re merged <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup> into the `master` branch.

<hr>
</details>

### :keyboard: Activity: Your first branch

{% if preferences.gitTool == 'cli' %}
1. Open your preferred command line interface, which we'll call your shell from now on.
1. Clone this repository:
      ```shell
      git clone {{ thePayload.repository.clone_url }}
      ```
1. Navigate to the repository in your shell:
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. Create a branch, use whatever name you like. Feel free to use the suggested name below. 
      ```shell
      git branch my-slide
      ```
1. Push the branch to GitHub:
      ```
      git push --set-upstream origin <BRANCH-NAME>
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. Download and open [Visual Studio Code](https://code.visualstudio.com/Download) (referred to as VS Code) if you don't already have it.
1. In VS Code, open the Command Palette using <kbd>Ctrl+Shift+P</kbd> on Windows, or <kbd>Command ⌘+Shift+P</kbd> on macOS. You can also follow [VS Code's official documentation](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository) on cloning.
1. Type: `git clone` and press <kbd>Enter</kbd>
      ![a screenshot of vs code with the command palette open](https://user-images.githubusercontent.com/16547949/53639288-bcf9ec80-3bf6-11e9-9d18-d97167168248.png)
1. Paste in the URL of the repository in the new window and press <kbd>Enter</kbd>:
      ```shell
      {{ thePayload.repository.clone_url }}
      ```
1. Select the location in which to save the repository and click **Choose folder**. Then, open the location you selected.
1. The repository folder should now be open in your VS Code project. Click on `master` at the bottom left of the VS Code window. This will bring up the Command Palette with the commands related to Git branches.
      ![a screenshot of the Git branches in VS Code](https://user-images.githubusercontent.com/16547949/53639606-adc76e80-3bf7-11e9-98ac-bd41ae2b40db.png)
1. Click **Create new branch** and enter any branch name you'd like, such as `my-slide`. Then press <kbd>Enter</kbd>.
1. When asked to select the ref to create the branch from, select `master`.
1. Go to the Source Control view, click on the ellipsis (...) and select **Push**. Confirm the dialog box asking you to publish the branch.
      ![a screenshot of the source control view in VS Code](https://user-images.githubusercontent.com/16547949/53640015-ee73b780-3bf8-11e9-8c90-be9022b9555a.png)

{% else %}

1. Navigate to the [Code tab]({{ thePayload.repository.html_url }})
2. Click **Branch: master** in the drop-down
3. In the field, enter a name for your branch, like `my-slide`
4. Click **Create branch: <name>** or press the “Enter” key to create your branch

{% endif %}
<hr>
<h3 align="center">I'll respond when I detect a new branch has been created in this repository.</h3>
