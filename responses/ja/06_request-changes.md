## ステップ７：レビュー対応をしよう

正しくプルリクエストが作成できました！

ファイルになにか追加してみましょう。ファイルの５行目をなにか新しい内容で置き換えてみましょう。忘れないでください：[Markdown](https://guides.github.com/features/mastering-markdown/)が使えます。

### :keyboard: やってみよう：ファイルの変更

{% if preferences.gitTool == 'cli' %}
1. ブランチをチェックアウトします：
    ```shell
    git checkout {{ branch }}
    ```
1. `_posts/0000-01-02-{{ user.username }}.md` を開きます。
1. ファイルの５行目をなにか新しい内容で置き換えます。
1. 新しい変更をステージします：
    ```shell
    git add _posts/0000-01-02-{{ user.username }}.md
    ```
1. 変更をコミットします：
    ```shell
    git commit -m "<YOUR-MESSAGE>"
    ```
1. 変更をGitHubにプッシュします：
    ```shell
    git push
    ```

{% elsif preferences.gitTool == 'vscode' %}
1. `_posts/0000-01-02-{{ user.username }}.md`を開きます。
1. ファイルの５行目をなにか新しい内容で置き換えます。
1. 新しい変更をステージします。もう一度言いますが、Source Controlビューでファイルの横の **+** をクリックすることでステージすることができます。
1. 変更をコミットします。Source Controlビューでテキストフィールドにコミットメッセージを入力し、Windowsの場合は<kbd>Ctrl+Enter</kbd>、macOSの場合は<kbd>Command ⌘+Enter</kbd>と入力することでコミットすることができます。
1. 変更をGitHubにプッシュします。Source Controlビューで、...をクリックし、 **Push** を選択しましょう。

{% else %}
1. このプルリクエストの[Files Changedタブ]({{ url }})をクリックします。
1. 画面右側の ... アイコンの中の "Edit file" をクリックし、新しく追加されたファイルを編集します。
1. ファイルの５行目をなにか新しい内容で置き換えます。
1. 画面の下にスクロールし、**Commit Changes** をクリックします。
{% endif %}

<hr>
<h3 align="center">このブランチへのコミットが行われたら、新しいコメントを書き込みます。</h3>
