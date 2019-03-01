## Step 6: Open a pull request

Nice work making that commit :sparkles:

Now that you’ve created a commit, it’s time to share your proposed change through a pull request! Where issues encourage discussion with other contributors and collaborators on a project, pull requests help you share your changes, receive feedback on them, and iterate on them until they’re perfect!

<details><summary>What is a pull request?</summary>

## Pull requests

Let’s think back to the GitHub flow again. You have created a branch, added a file, and committed the file to your branch. Now it’s time to collaborate on your file with other students taking this class. This collaboration happens in a pull request. Check out this video to learn more:

:tv: [Video: Introduction to pull requests](https://youtu.be/kJr-PIfLDl4)
<hr>
</details>

This pull request is going to keep the changes you just made on your branch and propose applying them to the `master` branch.

### :keyboard: Activity: Create a pull request

1. Open a pull request using [this shortcut]({{ url }}) or manually as follows:
    - From the "Pull requests" tab, click **New pull request**
    - In the "base:" drop-down menu, make sure the "master" branch is selected
    - In the "compare:" drop-down menu, select "{{ branch | remove: 'refs/heads/' }}"
1. When you’ve selected your branch, enter a title for your pull request. For example `Add {{ user.username }}'s file`
1. The next field helps you provide a description of the changes you made. Feel free to add a description of what you’ve accomplished so far. As a reminder, you have: created a branch, created a file and made a commit, and opened a pull request
1. Click **Create pull request**

<hr>
<h3 align="center">I'll respond in your new pull request.</h3>
