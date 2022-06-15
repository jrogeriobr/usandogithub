# USANDO O GITHUB
Orientações para iniciantes no GitHub. Meio que uma receita de bolo.
Abra o Git Bash Here e use os comandos desejados;
1. **Git Init** - Digite na pasta onde será feito o projeto a ser enviado para seu GitHub. Esse arquivo é criado automaticamente e não deve ser alterado. No explorer é preciso marcar a opção arquivos ocultos;
2. **Git Status** - Informa todos os arquivos que foram incluídos no Controle de Versão e, os que ainda não foram. Informa as versões dos Commit enviados. É sempre usado para saber se existe algo a ser adicionado ao GithUB;
3. **Git Add "nome do arquivo"** - Utilizado para enviar de forma individual, um arquivo para a área de Stages. Somente depois realizamos um Commit;
4. **Git Add .** - Utilizado para enviar todos os arquivos criados e/ou modificados de uma só vez para a área de Stages. Somente depois realizamos um Commit;
5. **Git Commit -m "Breve descrição do arquivo, ou de sua alteração, enviado para o GitHub"** - Informa versões, edições e qualquer outro tipo de informação que identifica um arquivo enviado, quer ele seja novo ou apenas alterado;
6. **Git --global user-email "seu email", pressione Enter. Em seguida digite Git --global user-name "seu nick"** - Caso o comando do item 5 esteja sendo executado pela primeira vez, esses comando precisam ser executados, mas, não se preocupe porque o próprio **Git Bash Here** vai solicitar e mostrar a sintaxe destes comandos. Com ele teremos atrelados o usuário com as versões enviadas para seu GitHub;
7. **Git remote add origin "endereço do repositório para onde os arquivos serão enviados"** - Desta forma os arquivos serão direcionados para o repositório desejado. Lembrando que é na hora da criação do Repositório que definimos se ele é público ou privado. Esse endereço solicitado é obtido dentro do repositório criado;
8. **Git push --set --upstream origin master** - É possível que abra uma janela solicitando o login, pode fornecer. Depois que esse comando é executado, atualize o GitHub e veja que o Brunch e o repositório correspondentes, receberam estas alterações;
9. **Git push -u origin master** - Esse comando será utilizado, ao invés do anterior (9), sempre que o primeiro commit foi executado;
10. **Git branch -M "nome da nova branch"** - Comando utilizado para trocar de branch;
11. **Git checkout -b "Nome da nova Branch"** - Comando utilizado para criar uma Branch;
12. **Merge** - Acontece quando juntamos uma Branch com outra (em geral a principal);
13. **Git checkout "nome da Branch"** - Entre numa Branch desejada;
14. **Git merge "nome da Branch a ser incorporada"** - Esse comando incorpora essa Branch a Branch principal do projeto;
15. **Git push origin master** - Depois do comando anterior, execute esse comando para colocar as alterações, no caso, a fusão dessas branchs, no GitHub;
16. **Git Reflog** - Utilize este comando para ver o histórico das atualizações de um repositório;
17. **Git reset --hard "ID da versão que se deseja fazer o retorno"** - Comando utilizado para retornar seu projeto para uma versão específica. Para saber a identificação dessa versão de retorno, use o comando anterior (16);
18. **Staging** - É o nome dado a um Branch que está recebendo atualizações, mas, ainda não foi colocado em produção;

# GITHUB X VSCODE
1. Crie um Repositório no GitHub - Defina se ele será público ou privado e, de preferência crie um Readme.md, com o objetivo de orientar aos usuários, quanto a sua utilização;
2.Depois de criado o Repositório, copie em CODE seu link (endereço);
3. Abra a pasta que desejar no Explorer;
4. Abra o **Git Bash Here** nesta pasta e digite **Git clone "cole o link copiado (2)"** - Será criado uma pasta com o mesmo nome do Repositório criado no GitHub, veja opção (1);
5. Entre nesta pasta e, com o botão direito, clique na opção "Abrir com VS CODE";
6. **code .** - Digite esse código caso não apareça a opção citada anteriormente (5) - Em ambas será possível abrir o VS Code já nesta pasta;
7. **Git --global user-email "seu email", pressione Enter. Em seguida digite Git --global user-name "seu nick"** - Isso vai conferir se o config do email e username estão ok;
8. **Faça um Teste* - Crie um novo arquivo no VS Code. Feito isso você vai perceber uma **notificação no ícone do Source Control** e a letra **U** após o nome do arquivo criado;
9. Abra o **Source Control** - Desta forma será possível ver todas as alterações realizadas e enviar os arquivos para a área de Stages. Depois disso realizamos o **Commit**;
10. É possível possível enviar todos os arquivos alterados e/ou criados para a área de stages e já fazer o **Commit** de forma simultânea (Colocando inclusive o texto com o motivo do commit) clicando no **ícone do Commit**;
11. Depois do envio, somem tantos o número que indicava as notificações, quando a letra **U**, dos arquivos enviados;
12. Para fazer o envio definitivo destes arquivos **"commitados"** clique no botão PUSH/PULL, no canto esquerdo inferior (em geral ele informa quantos arquivos precisam ser atualizados no GitHub e no VS Code;
13. É só atualizar o GitHub para saber se as alterações foram realizadas;
14. **Se eu alterar um arquivos no GitHub, ele altera também no VS Code?** - De jeito nenhum. Volte para o VS Code, veja que essa atulização simultânea não aconteceu e, clique no ícone PUSH/PULL para que isso aconteça;
15. Para confirmar, atualize o VS Code;
16. Qualdo se altera um arquivo no VS Code, perceba que além da notificação, o arquivo alterado fica com a letra **M** logo após seu nome. Para atualizar no GitHub é só clicar no ícone PUSH/PULL;

# CRIANDO OUTRA BRANCH
1. A nova **Branch** será criada no VS code e, em seguida, será feito o upload para o GitHub;
2. No VS Code, clique em **main**, no canto inferior esquerdo e, em seguida, em **+ Create new Branch** (Digite o nome da nova Branch);
3. **Atenção** - Veja que além de criar, o VS Code já troca de **main** para a Branch nova (veja no canto inferior esquerdo);
4. **Testando** - Faça a atualização de um arquivo qualquer no VS Code. Em seguida faça o **Commit** desse arquivo;
5. **Atenção Atenção** - Veja que ao lado da nova Branch (canto inferior esquerdo do VS code) existe um sinal indicando que essa **Branch Criada**, ainda não foi adicionada ao Repositório no GitHub. Clique nele para atualizar o GitHub;
6. Vá para o GitHub e atualize.veja que agora existem duas Branch, a principal e a que foi criada. Clique em cada uma delas e veja seus arquivos, percebendo as alterações realizadas no arquivo da **Nova Branch**, que ainda não consta na principal;
7. ** fazendo o MERGE** - Volte para o VS Code para unificar as Branchs, atualizando a principal. No canto superior esquerdo, ao lado de onde se faz o Commit, clique nos três pontinhos **...**. Em seguida em **Branch** e, por fim em **Merge Branch** (selecione o Branch a ser mesclado);
8. Feito isso, ainda no VS Code, suba essas atualizações para o GitHub utilizando o ícone PUSH/PULL;
