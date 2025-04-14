# Atividade Avaliativa - Git Colaborativo com Portugol

## Integrantes do grupo
- Raphael Feijó Salles

## Objetivo
Desenvolver colaborativamente um algoritmo em Portugol de subtração

## Etapas realizadas por cada membro
Raphael Feijó Salles:
Criei o repositório;
Criei o docs;
Baixei o arquivo portugol vazio;
Como era a minha máquina aproveitei o e-mail e o usuário da atividade passada;
Gerar uma nova chave SSH;
Iniciei o agente SSH;
Adicionei a chave SSH ao agente;
Copiei a chave pública para registrar no GitHub;
Copiei a chave pública para registrar no GitHub;
Testei a conexão com o GitHub(Apareceu uma mensagem de sucesso);
Clonei um repositório do GitHub;
Entrei na pasta do repositório clonado;
Adicionei as alterações no github;
Utilizei a pasta errada para inserir o arquivo.por, fiz 3 git add . até perceber o erro;
Clonei o repositório no local correto;
Inseri o arquivo no local correto;
Fiz modificações no arquivo;
Mudei o README descrevendo o que fiz;
Dei git add .
Dei git commit(Alterações no README - Raphael)

## Comandos utilizados
Todos os comandos foram executados via terminal utilizando chave SSH:
### Comandos de Raphael
laerc@DesktopInova▒▒o MINGW64 ~
$ git config --global user.name
Raphael

laerc@DesktopInova▒▒o MINGW64 ~
$ git config --global user.email
raphael.feijo@edu.unifil.br

laerc@DesktopInova▒▒o MINGW64 ~
$ ssh-keygen -t rsa -b 4096 -C "raphael.feijo@edu.unifil.br"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/laerc/.ssh/id_rsa):
/c/Users/laerc/.ssh/id_rsa already exists.
Overwrite (y/n)?

laerc@DesktopInova▒▒o MINGW64 ~
$ eval "$(ssh-agent -s)"
Agent pid 1949

laerc@DesktopInova▒▒o MINGW64 ~
$ ssh-add ~/.ssh/id_rsa
Identity added: /c/Users/laerc/.ssh/id_rsa (raphael.feijo@edu.unifil.br)

laerc@DesktopInova▒▒o MINGW64 ~
$ clip < ~/.ssh/id_rsa.pub

laerc@DesktopInova▒▒o MINGW64 ~
$ clip < ~/.ssh/id_rsa.pub

laerc@DesktopInova▒▒o MINGW64 ~
$ ssh -T git@github.com
Hi RaphaelFeijoSalles! You've successfully authenticated, but GitHub does not provide shell access.

laerc@DesktopInova▒▒o MINGW64 ~
$ git clone git@github.com:RaphaelFeijoSalles/AtividadeAvaliativaGithub
Cloning into 'AtividadeAvaliativaGithub'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

laerc@DesktopInova▒▒o MINGW64 ~
$ cd AtividadeAvaliativaGithub

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git add .

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git commit -m "Adicao de arquivo.por"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git push
Everything up-to-date

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git add .

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git clone git@github.com:RaphaelFeijoSalles/AtividadeAvaliativaGithub.git
Cloning into 'AtividadeAvaliativaGithub'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub (main)
$ cd AtividadeAvaliativaGithub

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub/AtividadeAvaliativaGithub (main)
$ git add .

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub/AtividadeAvaliativaGithub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub/AtividadeAvaliativaGithub (main)
$ git add .
warning: in the working copy of 'Subtração.por.por', LF will be replaced by CRLF the next time Git touches it

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub/AtividadeAvaliativaGithub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   "Subtra\303\247\303\243o.por.por"


laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub/AtividadeAvaliativaGithub (main)
$ git commit -m "Adicao de Subtração.por"
[main b39a365] Adicao de Subtração.por
 1 file changed, 19 insertions(+)
 create mode 100644 "Subtra\303\247\303\243o.por.por"

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub/AtividadeAvaliativaGithub (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 655 bytes | 327.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:RaphaelFeijoSalles/AtividadeAvaliativaGithub.git
   c95360e..b39a365  main -> main

laerc@DesktopInova▒▒o MINGW64 ~/AtividadeAvaliativaGithub/AtividadeAvaliativaGithub (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean


