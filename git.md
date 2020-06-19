
#Comandos basicos git
git clone
git status
git add
git commit -m "comentário"
git push

#Primeiros Passos
git init
git add README.md
git commit -m "first commit"
git push -u origin master
git push https://github.com/wburlani/git master -f

#Editor Sublime no git:
git config --global core.editor subl
git config --global --edit

#Configurações de atalhos(alias) git:

[core]
	editor = subl --wait
[alias]
	c = !git add --all && git commit -m
	s = !git status -s
	l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s == %C(cyan)%cn, %C(green)%cr'
	amend = !git add --all && git commit --amend --no-edit
	count = !git shortlog -s --grep

#Alias:

git c
git s
git l
git amend
git count

#Tipos de tags para comentários git commit "":

feat: (novo recurso para o usuário, não um novo recurso para script de construção)
fix: (correção de bug para o usuário, não uma correção para um script de construção)
docs: (alterações na documentação)
style: (formatação, ponto e vírgula ausente, etc.; nenhuma alteração no código de produção)
refactor: (refatorando o código de produção, por exemplo, renomeando uma variável)
test: (adicionando testes ausentes, refatorando testes; nenhuma alteração no código de produção)
chore: (atualização de tarefas grunhidas, etc; nenhuma alteração no código de produção)
