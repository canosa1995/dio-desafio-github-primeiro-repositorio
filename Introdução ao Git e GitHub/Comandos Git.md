```sh
# Inicializa um novo repositório Git.
$ git init

# Lista arquivos ocultos, neste caso temos o .git/
$ ls -a
./  ../  .git/

# Acessa o arquivo oculto, neste caso o .git/
$ cd .git/

# Lista todos os diretórios que estão dentro de .git/
$ ls -lhtr
total 15K
-rw-r--r-- 1 EAD+aleite7 4096  73 Dec 24 20:38 description
-rw-r--r-- 1 EAD+aleite7 4096 130 Dec 24 20:38 config
-rw-r--r-- 1 EAD+aleite7 4096  23 Dec 24 20:38 HEAD
drwxr-xr-x 1 EAD+aleite7 4096   0 Dec 24 20:38 hooks/
drwxr-xr-x 1 EAD+aleite7 4096   0 Dec 24 20:38 info/
drwxr-xr-x 1 EAD+aleite7 4096   0 Dec 24 20:38 objects/
drwxr-xr-x 1 EAD+aleite7 4096   0 Dec 24 20:38 refs/

# Comando que define o endereço de e-mail que o Git usará para identificar o autor dos commits.
# Configura o email em modo global para todos os repositórios Git no determinado sistema. 
$ git config --global user.email "teste@gmail.com"

# Comando que define o username que o Git usará para identificar o autor dos commits.
# Configura o usuário em modo global para todos os repositórios Git no determinado sistema.
$ git config --global user.name Teste

# Adiciona todos os arquivos no diretório atual à área de preparação.
# A área de preparação é onde você coloca as mudanças que deseja incluir no próximo commit.
$ git add *

# Salva as inclusões ou alterações no determinado código, arquivo, etc...
$ git commit -m "commit inicial"
[master (root-commit) 8c72207] commit inicial
 1 file changed, 27 insertions(+)
 create mode 100644 arquivo.md

# Inclue um apelido no repositório neste caso foi incluido o apelido ComandosGit para o repositório abaixo
$ git remote add ComandosGit https://github.com/canosa1995/dio-desafio-github-primeiro-repositorio.git

# Mostra o status
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

# Inclui de fato a pasta Introdução ao Git e GitHub/Comandos Git.md no repositório
$ git push ComandosGit
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 1.01 KiB | 257.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/canosa1995/dio-desafio-github-primeiro-repositorio.git
   832328c..a6f42a2  main -> main

```