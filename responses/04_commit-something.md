## Step 5: Criando um commit de um arquivo

:tada: Você criou uma branch!

Quando criamos uma branch, a mesma permite a gente de fazer modificações no projeto, sem alterar a branch `master`. Agora que você já tem uma branch, é hora de criarmos um arquivo e fazer o seu primeiro commit!


<details><summary>Commits 101</summary>

## Commits 101

Quando você terminar de criar ou fazer mudanças em um arquivo no Github, vá até o final da página e encontre a seção "Commit new file".

No primeiro campo, digite uma mensagem para o seu commit. Essa mensagem deve descrever resumidamente para os colaboradores sobre as mudanças que você fez no arquivo.

### Rules to live by for commit messages:

- Não termine o seu commit com um ponto final.
- Mantenha o seu commit com 50 caracteres ou menos. Se necessário adicionar um conteúdo extra, você pode usar a janela de "extend description". A mesma está localizada abaixo da linha do título.
- Use voz ativa. Por exemplo, "add" ao invés de "adicionado" e "merge" ao invés de "merged".
- Pense no seu commit como uma intenção de apresentar uma mudança.

<hr>
</details>

### :keyboard: Atividade: Seu primeiro commit

Os passos a seguir irão te guiar no processo para fazer um commit de uma alteração de um arquivo, no Github.

{% if preferences.gitTool == 'cli' %}
1. Verifique em qual branch você está:
      ```shell
      git checkout {{ thePayload.ref }}
      ```
2. Crie um arquivo chamado `_posts/0000-01-02-{{ user.username }}.md`.
3. Adicione o conteúdo abaixo no arquivo criado:
      ```yaml 
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
4. Adicione o arquivo para ser rastreado pelo Github:
      ```shell
      git add _posts/0000-01-02-{{ user.username }}.md
      ```
5. Depois de adicionar o arquivo, faça o commit do mesmo, lembrando de resumir em uma mensagem as alterações feitas no arquivo. Se tiver dúvidas de como proceder com a mensagem, dê uma olhada no título **Commits 101**, localizado acima destas instruções:
      ```shell
      git commit -m "<SUA-MENSAGEM-AQUI>"
      ```
6. Envie o seu commit para o GitHub:
      ```shell
      git push
      ```

{% elsif preferences.gitTool == 'vscode' %}
1. Na pasta `_posts`, crie um novo arquivo chamado `0000-01-02-{{ user.username }}.md`. O caminho completo para o seu arquivo será: `_posts/0000-01-02-{{ user.username }}.md`.
2. Adicione o conteúdo abaixo no arquivo criado e salve-o:
      ```yaml 
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
3. Adicione o novo arquivo para rastreio: vá até o Source Control e clique no botão **+** próximo ao arquivo. Caso queira você pode seguir a [documentação oficial do VS Code](https://code.visualstudio.com/docs/editor/versioncontrol#_commit).
      ![a screenshot of the staging button in the source control view](https://user-images.githubusercontent.com/16547949/53641057-d5b8d100-3bfb-11e9-9b69-53b0661cd5cd.png)
4. Faça o commit da mudança e adicione a mensagem no campo de texto, e pressione <kbd>Ctrl+Enter</kbd> no Windows ou <kbd>Command ⌘+Enter</kbd> no macOS.
      ![a screenshot of the commit message on VS Code](https://user-images.githubusercontent.com/16547949/53641276-698a9d00-3bfc-11e9-9b3d-01680fd01d7c.png)
5. Clique nos três pontos (...) e selecione **Push**.

{% else %}
1. Crie um novo arquivo nesta branch, dentro da pasta `_posts` chamado `0000-01-02-{{ user.username }}.md`. Você pode usar este [atalho]({{ thePayload.repository.html_url }}/new/{{ thePayload.ref }}?filename=_posts/0000-01-02-{{ user.username }}.md) ou seguir os passos abaixo:
      - Volte para a aba "Code"
      - No menu drop-down branch, selecione "{{ thePayload.ref }}"
      - Clique em **Create new file**
      - No campo "file name", digite `_posts/0000-01-02-{{ user.username }}.md`. Inserindo `/` no nome do arquivo, irá automaticamente colocar o arquivo dentro do seu diretório `_posts`.
2. Quando você terminar de nomear o arquivo, adicione o conteúdo dentro do mesmo:
      ```yaml
      ---
      layout: slide
      title: "Welcome to our second slide!"
      ---
      Your text
      Use the left arrow to go back!
      ```
3. Depois de adicionar o texto, você pode fazer o commit da mudança, escrevendo a mensagem no campo de texto, localizado abaixo do campo de editar arquivo. Se tiver dúvidas de como proceder com a mensagem, dê uma olhada no título **Commits 101**, localizado acima destas instruções:

4. Quando terminar de escrever a mensagem no commit, clique em **Commit new file**
{% endif %}
<hr>
<h3 align="center">Eu irei responder quando eu detectar um novo commit nesta branch.</h3>
