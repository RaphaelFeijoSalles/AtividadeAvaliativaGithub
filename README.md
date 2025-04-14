# Atividade Avaliativa - Git Colaborativo com Portugol

## Integrantes do grupo
- Raphael Feijó Salles
- Eduardo Silva Rodrigues

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
Dei git add .
Dei git commit(Alterações no README2 - Raphael)
Dei git push

Eduardo Silva Rodrigues: 
- retirei o usuário, o email e a chave ssh que estavam na maquina 
- coloquei meu nome errado e tive de refazer apagando o nome e criando outro
- coloquei meu email
- gerei uma chave ssh com meu email
- iniciei o agent ssh
- adicionei a chave ssh ao agente 
- copiei a chave para registrar no github
- coloquei a chave ssh em meu github
- verifiquei a conexão com o github 
- Errei ao clonar o repositório git e tentei novamente 
- Ao usar o meu nome não consegui acessar o repositorio, por tanto usei o nome do Raphael para clonar o repositorio
- errei o comando do “git pull”
- acessei a pasta do repositório 
- Alterei o arquivo do portugol 
- Alterei o arquivo README
- dei git add .
- dei git commit -m ("Alterações README e Portugol - Eduardo")
- dei git push 
- alterei o arquivo README denovo, inseri meu terminal 
- dei git add .
- dei git commit -m ("Alterações README e Portugol2 - Eduardo") 



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

### Comandos de Eduardo

compuni@maker312 MINGW64 ~
$ git config --global --unset user.name

compuni@maker312 MINGW64 ~
$ git config --global --unset user.email

compuni@maker312 MINGW64 ~
$ rm -f ~/.ssh/id_rsa*

compuni@maker312 MINGW64 ~
$ git config --global user.name "Seu Nome"

compuni@maker312 MINGW64 ~
$ git config --global --unset user.name

compuni@maker312 MINGW64 ~
$ git config --global user.name Fleshax

compuni@maker312 MINGW64 ~
$ git config --global user.email eduardo.silva@edu.unifil.br

compuni@maker312 MINGW64 ~
$ ssh-keygen -t rsa -b 4096 -C eduardo.silva@edu.unifil.br
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/compuni/.ssh/id_rsa):
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/compuni/.ssh/id_rsa
Your public key has been saved in /c/Users/compuni/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:IHFTeipxONL6Ok4lLDfeY/Gr0dEv8WkNEB7lq8421IU eduardo.silva@edu.unifil.br
The key's randomart image is:
+---[RSA 4096]----+
|    . o.+..      |
|   . + + +       |
|  . * + + ..     |
| . o = = .E..    |
|. * + o S.o.     |
| + * = ..=.+     |
|  o * o.o = .    |
| ..o o +oo       |
| .o.....o.       |
+----[SHA256]-----+

compuni@maker312 MINGW64 ~
$ eval "$(ssh-agent -s)"
Agent pid 168

compuni@maker312 MINGW64 ~
$ ssh-add ~/.ssh/id_rsa
Identity added: /c/Users/compuni/.ssh/id_rsa (eduardo.silva@edu.unifil.br)

compuni@maker312 MINGW64 ~
$ clip < ~/.ssh/id_rsa.pub

compuni@maker312 MINGW64 ~
$ ssh -T git@github.com
The authenticity of host 'github.com (20.201.28.151)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? y
Please type 'yes', 'no' or the fingerprint: yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
Hi Fleshax! You've successfully authenticated, but GitHub does not provide shell access.

compuni@maker312 MINGW64 ~
$ git clone git@github.com:Fleshax/AtividadeAvaliativaGithub.git
Cloning into 'AtividadeAvaliativaGithub'...
ERROR: Repository not found.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

compuni@maker312 MINGW64 ~
$ git clone git@github.com:Fleshax/AtividadeAvaliativaGithub.git
Cloning into 'AtividadeAvaliativaGithub'...
ERROR: Repository not found.
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

compuni@maker312 MINGW64 ~
$ git clone git@github.com:RaphaelFeijoSalles/AtividadeAvaliativaGithub.git
Cloning into 'AtividadeAvaliativaGithub'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

compuni@maker312 MINGW64 ~
$ git pull
fatal: not a git repository (or any of the parent directories): .git

compuni@maker312 MINGW64 ~
$ cd AtividadeAvaliativaGithub

compuni@maker312 MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git pull
remote: Enumerating objects: 11, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 9 (delta 1), reused 9 (delta 1), pack-reused 0 (from 0)
Unpacking objects: 100% (9/9), 2.69 KiB | 43.00 KiB/s, done.
From github.com:RaphaelFeijoSalles/AtividadeAvaliativaGithub
   c95360e..1194d6a  main       -> origin/main
Updating c95360e..1194d6a
Fast-forward
 README.md                         | 167 +++++++++++++++++++++++++++++++++++++-
 "Subtra\303\247\303\243o.por.por" |  19 +++++
 2 files changed, 185 insertions(+), 1 deletion(-)
 create mode 100644 "Subtra\303\247\303\243o.por.por"

compuni@maker312 MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git add .
warning: LF will be replaced by CRLF in Subtração.por.por.
The file will have its original line endings in your working directory

compuni@maker312 MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git commit -m "Alterações README e Portugol - Eduardo"
[main e71c8c4] Alterações README e Portugol - Eduardo
 1 file changed, 3 insertions(+), 1 deletion(-)

compuni@maker312 MINGW64 ~/AtividadeAvaliativaGithub (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 404 bytes | 404.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:RaphaelFeijoSalles/AtividadeAvaliativaGithub.git
   1194d6a..e71c8c4  main -> main

compuni@maker312 MINGW64 ~/AtividadeAvaliativaGithub (main)
$



