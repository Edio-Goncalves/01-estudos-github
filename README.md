# 01-estudos-github
Funlionalidades básicas

## COMANDOS BASICOS
* `git init` //inicializar um novo repositorio
* `git add .` //adicionar os arquivos atuais ao proximo commit
* `git status` //verificar status atual do repositorio git
* `git commit -m "mensagem do commit"` //criar novo commit com uma mensagem
* `git push` //enviar arquivos na nuvem na branch atualmente ativa
* `git pull` //atualizar a branch atualmente ativa para pegar a ultima versão

## COMANDOS BASICOS BRANCH & MERGE
* `git branch` //permite listar e ver branch ativa atualmente
* `git checkout <nomeDaBranchExistente>` //permite mudar para uma nova branch
* `git checkout -b <nomeDaNovaBranch> <nomeDaBranchExistente>` //para criar uma nova branch com base nos arquivos de uma branch existente
* `git merge <nomeBranchTEMPORARIA>` //permite fazer o merge da branch ativa atualmente com os arquivos da temporaria
* `git push origin --delete <nomeDaBranch>` //para deletar uma branch remota (no github)
* `git branch -d <nomeDaBranch>` //para deletar uma branch local

## COMANDOS VERSÕES
* `git reflog` //para verificar as versões, sendo a versão mais atual vai ser a do topo
* `git reset --hard <numeroVersão>` //serve para ir a uma versão no passado ou futuro

## VIDEO BASE DO ESTUDO
https://www.youtube.com/watch?v=kB5e-gTAl_s