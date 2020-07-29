## ステップ８：プルリクエストをマージしよう

よく出来ました、@{{ user.username }}！ :sparkles:

無事にプルリクエストを作成し、全部のテストが成功しました。プルリクエストをマージする準備が出来ました。

### :keyboard: やってみよう：プルリクエストのマージ

{% if preferences.gitTool == 'cli' %}
1. `master`ブランチをチェックアウトする：
    ```shell
    git checkout master
    ```
2. ブランチをマージする：
    ```shell
    git merge {{ branch }}
    ```
3. マージされた履歴をGitHubにプッシュする：
    ```shell
    git push
    ```
4. ローカルブランチを削除する：
    ```shell
    git branch -d {{ branch }}
    ```
{% else %}
1. **Merge pull request**をクリックする
1. **Confirm merge**をクリックする
{% endif %}
1. 一度ブランチがマージされたら、もはやそのブランチは必要ありません。**Delete branch**をクリックしましょう。

<hr>
<h3 align="center">このプルリクエストがマージされたら、新しいコメントを書き込みます。</h3>
