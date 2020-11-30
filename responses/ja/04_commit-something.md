## ステップ５：ファイルをコミットしよう

:tada: ブランチを作成できました！

ブランチを作成することで、`master`ブランチに変更を加えることなくプロジェクトへの修正を行うことができるようになります。さて、ブランチの作成が完了したので、次はファイルを作成し、初めてのコミットを行いましょう！

<details><summary>コミットの基礎</summary>

## コミットの基礎

GitHub上で新しいファイルを作成したり、ファイルの修正をし終えたら、ページの下にスクロースしましょう。"Commit new file"セクションが見つかるはずです。

最初のフィールドにはコミットメッセージを入力します。コミットメッセージでは、このファイルに対して行った変更を他の人に完結に伝える必要があります。

### コミットメッセージを書く際の決まり：

- コミットメッセージの終わりにピリオドは付けない
- コミットメッセージは５０文字以内とする。必要であれば、詳細な情報は追加の詳細フィールドに記載する。これはタイトルのラインのすぐ下にあるフィールドです
- 現在形を使う。例えば、「追加した」の代わりに「追加する」を書いたり、「マージした」の代わりに「マージする」と書く
- ファイルを変更する上での意図を書く

<hr>
</details>

### :keyboard: やってみよう：初めてのコミット

下記の手順に従うことによって、GitHub上に変更をコミットすることが出来ます。

{% if preferences.gitTool == 'cli' %}
1. ブランチをチェックアウトしましょう：
      ```shell
      git checkout {{ thePayload.ref }}
      ```
1. `_posts/0000-01-02-{{ user.username }}.md`という名前の新しいファイルを作成しましょう。
1. ファイルに下記の内容を追記しましょう：
      ```yaml 
      ---
      layout: slide
      title: "２枚目のスライドにようこそ！"
      ---
      何かを書く。
      戻るには戻るボタンを使いましょう！
      ```
1. 新しいファイルをステージに追加しましょう：
      ```shell
      git add _posts/0000-01-02-{{ user.username }}.md
      ```
1. テキストを追加し、変更とコミットメッセージをコミットしたら、手順のすぐ上にある**コミットの基礎**ドロップダウンを開き内容を確認しましょう：
      ```shell
      git commit -m "<YOUR-MESSAGE>"
      ```
1. Push your new commit to GitHub:
      ```shell
      git push
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. `_posts`フォルダに`0000-01-02-{{ user.username }}.md`という名前の新しいファイルを作成しましょう。ファイルのパスは`_posts/0000-01-02-{{ user.username }}.md`となるはずです。
1. ファイルに以下の内容を追加し、保存しましょう：
      ```yaml 
      ---
      layout: slide
      title: "２枚目のスライドにようこそ！"
      ---
      何かを書く。
      戻るには戻るボタンを使いましょう！
      ```
1. 新しいファイルをステージに追加するには：Source Controlビューに移動し、ファイルの横にある**+**ボタンをクリックしましょう。[VS Codeの公式ドキュメント](https://code.visualstudio.com/docs/editor/versioncontrol#_commit)にも手順が記載されています。
      ![a screenshot of the staging button in the source control view](https://user-images.githubusercontent.com/16547949/53641057-d5b8d100-3bfb-11e9-9b69-53b0661cd5cd.png)
1. テキストフィールドにコミットメッセージを入力し、Windowsの場合は<kbd>Ctrl+Enter</kbd>、macOSの場合は<kbd>Command ⌘+Enter</kbd>を押すことで変更をコミットしましょう。
      ![a screenshot of the commit message on VS Code](https://user-images.githubusercontent.com/16547949/53641276-698a9d00-3bfc-11e9-9b3d-01680fd01d7c.png)
1. ...をクリックし、**Push**を選択しましょう。

{% else %}
1. このブランチに新しいファイルを作成しましょう。`_posts`フォルダーに`0000-01-02-{{ user.username }}.md`という名前のファイルを作成します。[このリンクをクリックする]({{ thePayload.repository.html_url }}/new/{{ thePayload.ref }}?filename=_posts/0000-01-02-{{ user.username }}.md)か、以下の手順でファイルを作成することが出来ます：
      - "Code"タブに戻る
      - ブランチドロップダウンにて、"{{ thePayload.ref }}"を選択
      - **Create new file**をクリック
      - "file name"フィールドに`_posts/0000-01-02-{{ user.username }}.md`と入力する。ファイル名の中に`/`を入れることで自動的にそのファイルを`_posts`ディレクトリに保存することが出来ます。
1. ファイルの名前を入力したら、以下の内容をファイルに追加する：
      ```yaml 
      ---
      layout: slide
      title: "２枚目のスライドにようこそ！"
      ---
      何かを書く。
      戻るには戻るボタンを使いましょう！
      ```
1. テキストを追加後、ファイル編集ビューのすぐ下にあるテキスト入力フィールドにコミットメッセージを入れることで、この変更をコミットすることが出来ます。コミットメッセージのガイドラインとしては、手順のすぐ上にある**コミットの基礎**を参照してください。
1. コミットメッセージを入力したら、**Commit new file**をクリック
{% endif %}
<hr>
<h3 align="center">このブランチに新しいコミットが行われたら、追加のコメントを書き込みます。</h3>
