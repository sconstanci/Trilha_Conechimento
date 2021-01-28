# Trilha_Conechimento

Curso GIT

GIT = Sistema de controle de versões distribuido

Aula 01: 
git config --global user.name "Sidney Constanci Salgueiro" **configura o user name do usuário da maquina 

git config --global user.email "sidney.salgueiro@neon.com.br" **configura o user email do usuario da maquina 

Aula 02:
git init **cria a estrutura de um repositório na pasta atual

git status **mostra em qual estado está seu repositório

git add <nome_do_arquvo> **adiciona o arquivo para ser commitado
git add *.<extencao> **adiciona todos os arquivos com aquela extenção
git add . **adiciona todos os arquivos novos para serem comitados

git commit -m "<texro_commit>" **comita para branch os arquivos que vão subir
git commit -a -, "<testo_commit>" **pula o passo de add os arquivos que vão subir

Aula 03: 
git diff **mostra todas as mudanças que foram feitas no arquivo
git diff --staged **mostra os arquivos que foram modificados e estão na stagedArea

git log **mostra um log de todas as alterações feitas no projeto
git log -p **alem de trazer o log dos commits mostra também as diff's que foram feitas em cada commit

git log -p -<numero_de_entradas_que_vc_quer_trazer> **traz na tela os commits a partir do commit foi passado pelo parâmetro

gitk **abre a interface gráfica para a visualização das alterações feitas no projeto

Aula 04:

git log --pretty=oneline **parâmetro que serve para mostrar somente o código e a mensagem do commit

git commit --amend -m "<Mensagem do commit>" **adiciona os dados em um commit novo a o ultimo commit existente(ele não gera um novo commit, ele adiciona ao ultimo commit)

git reset HEAD <Nome_do_arquivo> **remove um arquivo da stageArea

git checkout -- <file> **reverte um arquivo editado ao ultimo commit realizado

git rm <nome_do_arquivo> **remove arquivos deletados do repositório(quando o arquivo é deletado do projeto podemos usar esse comando para remover os mesmo do repositório)

Aula 05: 

git tag **lista as tag's criadas do sistema
git tag -a <nome_tag> -m "<mensagem **cria uma tag no sistema no commit atual
git tag -a <nome_tag> <codigo_commit> -m "<mensagem>" **cria uma tag no sistema em um commit existente
git show <nome_tag> **mostra as informações da tag
git checkout <nome_tag> **troca para a versão que a tag está apontando(restaurando o projeto com arquivos que estavam naquela versão)
git tag -d <nome_tag> **deleta a tag

git branch <nome_branch> **cria uma nova branch 
git checkout <nome_branch> **entra na branch selecionada
git checkout -b <nome_branch> **cria e entra dentro da branch
git branch ** lista as branch's existente

git merge <nome_branch> **junta os arquivos da branch (vc sempre tem que estar na branch que ira receber os arquivos para usar esse comando)

git branch -d <nome_branch> **deleta a branch

Aula 06:

git init --bare **iniciar um repositório para trabalho em rede local
git clone file:////<caminho_pasta> <nome_pasta >**clona o projeto da branch master para o work

git remote **mostra o nome do servidor remoto(por padrão quando você faz um clone ele vem como origin)
git push origin <branch_trabalho> **envia as mudanças da branch de trabalho para a branch origin

git pull origin <nome_branch> **traz as alterações da branch origin para a branch de trabalho
git fetch origin <nome_branc> **usado para não realizar o merge automatico do pull porem tem que criar um branch para usá-lo

Aula 07: 

ssh-keygen **cria uma chave de acesso ao github

