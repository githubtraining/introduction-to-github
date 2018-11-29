## Step 4: Create a branch

Let’s complete the first step of the GitHub flow: creating a branch <sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup>.

<details><summary>Creating a branch</summary>

## Creating a branch

:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

You just learned how to create a branch—the first step in the GitHub flow.

Branches are an important part of the GitHub flow because they allow us to separate our work from the `master` branch. In other words, everyone's work is safe while you contribute.

### Tips for using branches

A single project can have hundreds of branches, each suggesting a new change to the `master` branch.

The best way to keep branches organized with a team is to keep them concise and short-lived. In other words, a single branch should represent a single new feature or bug fix. This reduces confusion among contributors when branches are only active for a few days before they’re merged <sup>[definition](https://help.github.com/articles/github-glossary/#merge)</sup> into the `master` branch.

<hr>
</details>

### :keyboard: Activity: Your first branch

{% if preferences.gitTool === 'cli' %}
       1. Open your preferred command line interface, which we'll call your shell from now on.
       1. Clone this repository:
              ```shell
              git clone {{ thePayload.repository.clone_url }}
              ```
       1. Navigate to the repository in your shell:
              ```shell
              cd {{ thePayload.repository.name }}
              ```
       1. Create a branch, use whatever name you like:
              ```shell
              git branch <BRANCH-NAME>
              ```
       1. Push the branch to GitHub:
              ```
              git push --set-upstream origin <BRANCH-NAME>
              ```
{% else %}

       1. Navigate to the “Code” tab
       2. Click **Branch: master** in the drop-down
       3. In the field, enter a name for your branch
       4. Click **Create branch: <name>** or press the “Enter” key to create your branch

{% endif %}
<hr>
<h3 align="center">Return to this issue for my response</h3>
