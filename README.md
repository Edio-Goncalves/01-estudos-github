## Funcionalidades básicas do github

### COMANDOS BASICOS

- `git init` //inicializar um novo repositório
- `git add .` //adicionar os arquivos atuais ao próximo commit
- `git status` //verificar status atual do repositorio git
- `git commit -m "mensagem do commit"` //criar novo commit com uma mensagem
- `git push` //enviar arquivos na nuvem na branch atualmente ativa
- `git pull` //atualizar a branch atualmente ativa para pegar a última versão

##

### BRANCH & MERGE

- `git branch` //permite listar e ver branch ativa atualmente
- `git checkout <nomeDaBranchExistente>` //permite mudar para uma nova branch
- `git checkout -b <nomeDaNovaBranch> <nomeDaBranchExistente>` //para criar uma nova branch com base nos arquivos de uma branch existente
- `git merge <nomeBranchTEMPORARIA>` //permite fazer o merge da branch ativa atualmente com os arquivos da temporária
- `git push origin --delete <nomeDaBranch>` //para deletar uma branch remota (no github)
- `git branch -d <nomeDaBranch>` //para deletar uma branch local
- `git pull origin <nomeDaBranch>` //para buscar os arquivos de determinada branch
-  `git pull --rebase origin` //para forçar a busca de arquivos de determinada branch

##

### ALTERAR VERSÕES

- `git reflog` //para verificar as versões, sendo a versão mais atual vai ser a do topo
- `git reset --hard <numeroVersão>` //serve para ir a uma versão no passado ou futuro

##

### FONTES

- https://www.youtube.com/watch?v=kB5e-gTAl_s (comandos básicos)
- https://www.youtube.com/watch?v=NXJjNk7aHrI (mudança de repositório)

##

## EXEMPLO DE PASSOS CORRIQUEIROS

#### Iniciando um repositorio

1. Criar repositório no site do github para podermos vincular os arquivos ao servidor.
2. `git init` //iniciar um novo repositório
3. `git status` //verificar status atual dos arquivos
4. `git add .` //adicionar todos arquivos para a proxima commit
5. `git commit -m "mensagem git inicial"` //criar commit com mensagem
6. `git remote add <nome> <linkRepositorio>` //linkando o local com o remoto
7. `git push --set-upstream <nome> <nomeBranchPrincipal>` //Enviando os arquivos pela primeira vez

#### Adicionando modificações

Após ter criado novas funcionalidades e testado vamos seguir os passos:

1. `git status` //verificar status atual dos arquivos
2. `git add .` //adicionar todos arquivos para a próxima commit
3. `git commit -m "commitName"` //add nome do commit
4. `git push` //para enviar os arquivos

#### Mudar de repositório

1. `git remote -v` //para identificar as urls remotas do diretório
2. `git remote remove origin` //vai remover as urls no origin
3. `git remote remove add origin <url>` //vai vincular o diretório ao link do novo repositório
4. `git branch --set-upstream-to=origin/<branch> master` //caso precise dar um 'git pull' para pegar os arquivos do novo link
5. `git push --set-upstream origin master` //caso o repositório esteja vazio e precisamos criar a master para enviar os arquivos

#### Trabalhar com mais de uma branch e efetuar merge

1. de um "git pull" na branch principal para ter certeza que está na ultima versão. <br>
   `git pull`
2. gerar uma nova branch a partir da branch principal <br>
   `git branch <nomedabranch>`
3. verifique se as brench existentes para ver se ela foi criada <br>
   `git branch`
4. mude para a branch temporária para efetuar os trabalhos <br>
   `git checkout <nomedabranch>`
5. trabalhe e adicione novas funcionalidades na brench temporária e depois de testado jogue os arquivos na branch <br>
   `git add .` <br>
   `git commit -m "comentario do trabalho"` <br>
   `git push` <br>
6. vá para a git principal <br>
   `git checkout <nomedabranch>`
7. de um novo git pull para verificar se esta na ultima versão <br>
   `git pull`
8. combine os arquivos da branch temporária com a branch principal <br>
   `git merge <nomedabranchTEMPORARIA>`
9. jogue na nuvem <br>
   `git push`
