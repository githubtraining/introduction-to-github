## Étape 4: Création d'une branche

Réalisons la première étape d'une démarche typique sur GitHub : la création d'une branche <sup>[:book:](https://help.github.com/articles/github-glossary/#branch)</sup>.

<details><summary>Création d'une branche</summary>

## Création d'une branche

:tv: [Video: Branches](https://www.youtube.com/watch?v=xgQmu81G1yY)

Vous venez d'apprendre à créer une branche, la première étape du travail sur GitHub.

Les branches sont des éléments importants de la démarche sur GitHub car elles nous permettent d'isoler le travail en cours de la branche principale `master`. En d'autres termes, le travail des autres est protégé pendant que vous mettez au point votre contribution.

### Conseils pour l'utilisation de branches

Un projet seul peut avoir des centaines de branches, chacune comportant une nouvelle modification de la branche `master`.

La meilleure façon de gérer ces branches quand on travaille en équipe est de veiller à les maintenir concises et éphémères. Autrement dit, une branche doit comporter une seule nouvelle fonctionalité ou correction de bug. Les incompréhensions entre contributeurs sont réduites lorsque les branches ne sont actives que quelques jours avant d'être fusionnées <sup>[:book:](https://help.github.com/articles/github-glossary/#merge)</sup> avec la branche `master`.

<hr>
</details>

### :keyboard: Activité : Votre première branche

{% if preferences.gitTool == 'cli' %}
1. Ouvrez votre interface de ligne de commande préférée, que nous appelerons votre shell à partir de maintenant.
1. Clonez cd dépôt :
      ```shell
      git clone {{ thePayload.repository.clone_url }}
      ```
1. Naviguez vers ce dépôt dans votre shell :
      ```shell
      cd {{ thePayload.repository.name }}
      ```
1. Créez une branche avec le nom que vous désirez. Vous pouvez également utiliser le nom suggéré ci-dessous. 
      ```shell
      git branch my-slide
      ```
1. Poussez la branche vers GitHub:
      ```
      git push --set-upstream origin <BRANCH-NAME>
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. Téléchargez et installez [Visual Studio Code](https://code.visualstudio.com/Download) (aussi appelé VS Code) si vous ne l'avez pas déjà.
1. Dans VS Code, ouvrez la pallette de commandes (Command Palette) avec <kbd>Ctrl+Shift+P</kbd> sous Windows, ou <kbd>Command ⌘+Shift+P</kbd> sous macOS. Vous pourvez égalememnt consulter [la documentation officielle de VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_cloning-a-repository) sur la création de clones.
1. Tapez: `git clone` et pressez <kbd>Enter</kbd>
      ![a screenshot of vs code with the command palette open](https://user-images.githubusercontent.com/16547949/53639288-bcf9ec80-3bf6-11e9-9d18-d97167168248.png)
1. Collez l'adresse du dépôt dans la nouvelle fenêtre et pressez <kbd>Enter</kbd>:
      ```shell
      {{ thePayload.repository.clone_url }}
      ```
1. Sélectionnez l'emplacement où sauvegarder le dépôt et cliquez **Choose folder**. Ouvrez ensuite l'emplacement que vous avez sélectionné.
1. Le répertoire du dépôt doit maintenant être ouvert dans votre espace de travail VS Code. Cliquez sur `master` en bas et à gauche de la fenêtre VS Code. Ceci ouvrira la palette avec les commandes relatives aux branches Git.
      ![a screenshot of the Git branches in VS Code](https://user-images.githubusercontent.com/16547949/53639606-adc76e80-3bf7-11e9-98ac-bd41ae2b40db.png)
1. Cliquez sur **Create new branch** et saisissez le nom que vous désirez, par exemple `my-slide`. Pressez ensuite <kbd>Enter</kbd>.
1. Lorsqu'il vous est demandé de sélectioner la référence à partir de laquelle créer la branche, sélectioner `master`.
1. Allez dans la vue "Source Control", cliquez sur les points de suspension (...) et séléctionnez **Push**. Confirmez lorsque le boite de dialogue vous propose de publier la branche.
      ![a screenshot of the source control view in VS Code](https://user-images.githubusercontent.com/16547949/53640015-ee73b780-3bf8-11e9-8c90-be9022b9555a.png)

{% else %}

1. Naviguez vers [l'onglet Code]({{ thePayload.repository.html_url }})
2. Cliquez **Branch: master** dans la liste déroulante
3. Dans le champs de texte, saisissez un nom de branche, tel que `my-slide`
4. Cliquez **Create branch: <name>** ou pressez la touche <kbd>Enter</kbd> pour créer votre branche

{% endif %}
<hr>
<h3 align="center">Je vous répondrai ici lorsque j'aurai détecté qu'une nouvelle branche a été crée dans ce dépôt.</h3>
