# 01-estudos-github
Funcionalidades básicas

## COMANDOS BASICOS
* `git init` //inicializar um novo repositório
* `git add .` //adicionar os arquivos atuais ao próximo commit
* `git status` //verificar status atual do repositorio git
* `git commit -m "mensagem do commit"` //criar novo commit com uma mensagem
* `git push` //enviar arquivos na nuvem na branch atualmente ativa
* `git pull` //atualizar a branch atualmente ativa para pegar a última versão

## COMANDOS BASICOS BRANCH & MERGE
* `git branch` //permite listar e ver branch ativa atualmente
* `git checkout <nomeDaBranchExistente>` //permite mudar para uma nova branch
* `git checkout -b <nomeDaNovaBranch> <nomeDaBranchExistente>` //para criar uma nova branch com base nos arquivos de uma branch existente
* `git merge <nomeBranchTEMPORARIA>` //permite fazer o merge da branch ativa atualmente com os arquivos da temporária
* `git push origin --delete <nomeDaBranch>` //para deletar uma branch remota (no github)
* `git branch -d <nomeDaBranch>` //para deletar uma branch local

## COMANDOS VERSÕES
* `git reflog` //para verificar as versões, sendo a versão mais atual vai ser a do topo
* `git reset --hard <numeroVersão>` //serve para ir a uma versão no passado ou futuro

## MUDAR DE REPOSITORIO
* `git remote -v` //para identificar as urls remotas do diretório
* `git remote remove origin` //vai remover as urls no origin
* `git remote remove add origin` //vai vincular o diretório ao link do novo repositório
* `git branch --set-upstream-to=origin/<branch> master` //caso precise dar um 'git pull' para pegar os arquivos do novo link
* `git push --set-upstream origin master` //caso o repositório esteja vazio e precisamos criar a master para enviar os arquivos


## FONTES
* https://www.youtube.com/watch?v=kB5e-gTAl_s (comandos básicos)
* https://www.youtube.com/watch?v=NXJjNk7aHrI (mudar de repositório)
