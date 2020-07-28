## ステップ４：ブランチを作ろう

GitHubフローの最初のステップに取り掛かりましょう：つまりブランチの作成です<sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup>。

<details><summary>ブランチの作成</summary>

## ブランチの作成

:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

さて、GitHubフローの最初のステップとしてブランチの作成方法を学びました。

ブランチを作ることによって`master`ブランチからあなたの作業を分離することができるため、ブランチはGitHubフローにおいて重要な役割を果たします。言い換えれば、誰もが安全な場所でコントリビュートを始めることができるのです。

### ブランチを使う際のコツ

１つのプロジェクトの中にブランチは何百と作成され、それぞれが`master`ブランチへの変更の提案となります。

これらのブランチをチーム全体で管理可能な状態を保つには一つ一つのブランチを完結で短命に保つことが必要です。言い換えると、１つの新しい機能か１つのバグフィックスごとに１つのブランチを作成するべきです。こうすることで、ブランチが`master`ブランチにマージ <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup>  されるまでのアクティブな期間を数日に保つことができ、他のコントリビューターが混乱する可能性を減らすことが出来ます。

<hr>
</details>

### :keyboard: やってみよう：初めてのブランチ

{% if preferences.gitTool == 'cli' %}
1. お好みのコマンドラインインターフェースを開きましょう。ここからはそのコマンドラインインターフェースのことをシェルと呼びます。
1. このリポジトリをクローンしましょう：
      ```shell
      git clone {{ thePayload.repository.clone_url }}
      ```
1. シェル上でリポジトリに移動しましょう：
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. ブランチを作成しましょう。ブランチ名は好きな名前で大丈夫です。下記の名前をそのまま使っても構いません：
      ```shell
      git branch my-slide
      ```
1. ブランチをGitHubにプッシュしましょう：
      ```
      git push --set-upstream origin <BRANCH-NAME>
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. もちまだインストールしていないのであれば[Visual Studio Code](https://code.visualstudio.com/Download) (VS Codeと呼ばれます)をダウンロードし、起動しましょう。
1. VS Codeの中で、コマンドパレットを開きましょう。コマンドパレットを開くには、Windowsでは<kbd>Ctrl+Shift+P</kbd>、macOSでは<kbd>Command ⌘+Shift+P</kbd>を押します。クローンの際には[VS Codeの公式ドキュメント](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository)にも手順が記載されています。
1. `git clone`と入力し、<kbd>Enter</kbd>を押します。
      ![a screenshot of vs code with the command palette open](https://user-images.githubusercontent.com/16547949/53639288-bcf9ec80-3bf6-11e9-9d18-d97167168248.png)
1. 新しいウィンドウにリポジトリのURLを貼り付け、<kbd>Enter</kbd>を押します：
      ```shell
      {{ thePayload.repository.clone_url }}
      ```
1. リポジトリを保存する場所を選択し、**Choose folder** をクリックします。その後、選択したフォルダーを開きましょう。
1. リポジトリのフォルダーがVS Codeのプロジェクトに開かれているはずです。VS Codeのウィンドウの左下にある`master`をクリックしましょう。Gitブランチに関連するコマンドが表示されたコマンドパレットが表示されるはずです。
      ![a screenshot of the Git branches in VS Code](https://user-images.githubusercontent.com/16547949/53639606-adc76e80-3bf7-11e9-98ac-bd41ae2b40db.png)
1. **Create new branch** をクリックし、好きなブランチ名を入力しましょう。例えば`my-slide`といったものです。その後、<kbd>Enter</kbd>を押します。
1. どのrefからブランチを作成するか尋ねられた場合、`master`を選択しましょう。
1. Source Controlビューに移動し、...をクリックし **Push** を選択します。ブランチを公開するか尋ねるダイアログボックスを確認しましょう。
      ![a screenshot of the source control view in VS Code](https://user-images.githubusercontent.com/16547949/53640015-ee73b780-3bf8-11e9-8c90-be9022b9555a.png)

{% else %}

1. [Codeタブ]({{ thePayload.repository.html_url }})に移動しましょう
2. **Branch: master** ドロップダウンをクリックしましょう
3. 入力フィールドに、例えば`my-slide`のように、作成するブランチの名前を入力しましょう
4. **Create branch: <name>** をクリックするか、"Enter"キーを押し、ブランチを作成しましょう

{% endif %}
<hr>
<h3 align="center">このリポジトリで新しいブランチが作成されたら、新しいコメントを書き込みます。</h3>
