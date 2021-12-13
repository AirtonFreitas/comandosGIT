# Comandos GIT
### Abaixo alguns comandos básicos de GIT

### CURSO 1
git clone linkdoGithub (faz um clone local do repositório)

git init - Iniciar Repositório na pasta local. (cria os arquivos .git iniciando assim o controle do repositório local)

echo "texto dentro do arquivo" > readme.md (usado para criar o arquivo readme.md)

git remote add origin linkdoGithub (vincula seu repositório local em um repositório do github)

git status - exibe o status do repositório local (exibe se os arquivos que estão no repositórios já foram commitados ou se estão desatualizados. Exibe o status Unmodified, Modified ou Staged)

git add . - Adiciona os arquivos dentro do commit. (Antes do commit os arquivos ficam no estado de Staged)

git commit -m "mensagem do commit" (Cria o commit com a anotação antes de enviar para o repositório do github)

git push origin master(master escolhida para enviar) - Envia o Commit para o github





### CURSO 2

git remote -v (Exibe os repositórios remotos vinculados.)

git commit --amend - renomeia um commit anterior antes que ele seja enviado para o github

git checkout -b nomedaBranch (o -b cria a nova branch com o nome informado. O checkout faz somente a movimentação para a branch)

git merge nomedaBranch (informar a branch que você deseja unir a branch que está selecionado)

git branch - Exibe todas as branches locais

git branch -m "novo nome" (renomeia a branche em que está)

git branch -m "nome antigo" "novo nome" (renomeia a branch antiga informada, independente da branch que estiver)

git branch -d "nome da branch" (deleta a branch escolhida)

### Manipulando arquivos para Stash

git stash save "comentario" (salva tudo que está no staging area ou index )

git stash pop "número do array" ("extrai" os arquivos do index ou stash para sua branch para ser commitado)

git stash clear (limpa os arquivos em stash, "index")



### Logs do GIT
git log (mostra o histórico completo do repositório)

git log "pasta" (mostra o histórico da pasta específica)

git log --oneline (mostra o histórico resumida, em apenas uma linha por evento)

git log --graph (mostra o histórico semelhante a uma interface gráfica, onde ficamais intuitivo para visualizar)


### Reversão de commits
#### Reset
git reset hash sha1

git reset HEAD~2(volta nas últimas 2 HEAD)

git reset --soft HEAD~2(tira todos os arquivos do commit e volta para o index, para staged)

git reset --mixed (volta os arquivos para o estado anterior)

git reset --hard HEAD~2 (apaga os arquivos do commit escolhido)



#### Revert (faz um novo commit revertendo o commit selecionado)
git revert hash sha1
git revert HEAD~2(volta nas últimas 2 HEAD)





### Semantic Versioning 3.2.7

3 - Major
2 - Minor
7 - Patch

https://www.conventionalcommits.org/en/v1.0.0/
