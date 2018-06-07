Comando GIT.

git config --global user.name "nome_do_usuario"
->  (Faz a configuração do nome de usuário.)

git config --global user.email "email_do_usuario"
-> (Faz a configuração do e-mail do usuário.)

git config --global --list
-> (Faz a listagem dos valores atribuídos na configuração.)

git init
-> (Inicializa repositório git.)

git add --all
-> (Adiciona todos os arquivos para commit.)

git add <nome_do_arquivo.extensao>
-> (Adiciona único arquivo para commit.)

git commit -m "mensagem_commit"
-> (Salva mudanças no repositório local e adiciona mensagem de commit.)

git status
-> (Verifica estados dos arquivos do repositório.)

git log
-> (Mostra histórico de alterações em ordem cronológica.)

git log --stat
-> (Mostra histórico de alterações em ordem cronológica e quais arquivos foram alterados.)

git diff <commit_1> <commit_2>
-> (Mostra a diferença entre dois commits.)

git checkout <branch_name>
-> (Muda para outra branch.)

git checkout -b <branch_name>
-> (Cria uma nova branch e já muda para ela.)

git checkout index.html
-> (As alterações no arquivo "index.html" que estão no Working Directory serão descartadas.)

git reset --hard
-> (Desfaz todas as alterações que aconteceram em arquivos rastreados.)

git reset HEAD~1
-> (Desfaz o último commit, porém mantém as alterações feitas.)

git reset --hard HEAD~1
-> (Desfaz o último commit feito e também desfaz todas as alterações feitas.)

git clean -n
-> (Mostra uma lista de arquivos que serão apagados.)

git clean -f
-> (Apaga todos os novos arquivos não rastreados na alteração.)

git clean -n
-> (Mostra uma lista de opções para apagar somente alguns arquivos.)

git clone <origem>
-> (Faz a clonagem do repositório para a pasta corrente.)

git pull
-> (Repositório local é atualizado com os dados do repositorio remoto.)

git branch
-> (Faz a listagem de todas as branchs locais.)

git branch -r
-> (Faz a listagem de todas as branchs remotas.)

git branch -a
-> (Faz a listagem de todas as branchs locais e remotas.)

git branch -d <branch_name>
-> (Faz a remoção de um branch local.)

git branch -D <branch_name>
-> (Força a remoção de um branch local.)

git branch -m <nome_antigo> <nome_novo>
-> (Renomeia uma branch localmente.)

git push
-> (Faz o envio das mudanças comitadas localmente para a origem da branch rastreada.)

git push -u origin <nome_da_branch>
->  (o envio da branch para o servidor e rastreia com a branch local.)

git push origin <nome_da_branch>
-> (Faz o envio da branch para o servidor mas não rastreia com a branch local.)

git merge <nome_da_branch>
-> (Mescla as mudanças presentes na <nome_da_branch> na branch corrente.)

git tag
-> (Faz a listagem de tags.)

git tag <nome_da_tag>
-> (Faz a criação de uma tag no último commit da branch corrente.)

git tag <nome_da_tag> <hash_do_commit>
-> (Faz a criação de uma tag no commit específico.)

git push --tags
-> (Faz o envio das tags locais para o servidor.)

git tag -d <nome_da_tag>
-> (Faz a remoção da tag localmente.)

git push origin --delete <nome_da_tag>
-> (Faz a remoção de tag no servidor.)

git checkout -b <nome_da_branch> <nome_da_tag>
-> (Faz a criação de um branch a partir de uma tag.)

git stash
-> (Salva as mudanças ainda não comitadas em uma pilha temporária para uso posterior.)

git stash list
-> (Faz a listagem das mudanças salvas na pilha temporária.)

git stash apply
-> (Traz a alteração mais recente que foi salva para a branch atual.)

git stash apply stash@{x}
-> (Traz a alteração de posição X que foi salva para a branch atual.)

git stash drop
-> (Faz a remoção mais recente da pilha temporária.)

git stash pop
-> (Traz a alteração mais recente que foi salva para a branch atual e logo em seguida já faz a remoção dessa alteração da pilha.)

git config --global alias.<abreviacao> <comando_git>
-> (Cria uma abreviação para o comando do git.)

git config --global --unset alias.<abreviacao>
-> (Faz a remoção do alias cadastrado.)

git config --global alias.<abreviacao>
-> (Verifica o comando que foi cadastrado.)

git config --get-regexp
-> (Faz a listagem de todos os alias configurados.)
