# LABORATORIO DE GIT

Este laboratorio tiene como objetivo practicar los comandos básicos de Git.

## 1. Crear un repositorio en local
```
June@DESKTOP-4ABLAGV MINGW64 ~
$ cd repositorios
```
```
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios
$ mkdir laboratorio1
```
```
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios
$ cd laboratorio1
```
```
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1
$ git init
Initialized empty Git repository in C:/Users/June/Repositorios/laboratorio1/.git/
```

## 2. Subir el repositorio a GitHub

Creo un nuevo repositorio en GitHub:

https://github.com/junearranz/laboratorio1.git

June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git init
Reinitialized existing Git repository in C:/Users/June/Repositorios/laboratorio1/.git/

June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git add .
warning: in the working copy of 'package-lock.json', LF will be replaced by CRLF the next time Git touches it

June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git commit -m "Hellooo Git"
[master (root-commit) 57a9fc1] Hellooo Git
 1 file changed, 6 insertions(+)
 create mode 100644 package-lock.json
 
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git remote add origin git@github.com:junearranz/laboratorio1.git

June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 297 bytes | 297.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/junearranz/laboratorio1/pull/new/master       
remote:
To https://github.com/junearranz/laboratorio1.git
 * [new branch]      master -> master

## Hacer un commit y un push

_xxxxxxxxxxxxx_


## Crear una rama

_xxxxxxxxxxxxxx_

## Hacer un merge

_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx_


## Autores ✒️

* **June Arranz** - [junearranz](https://github.com/junearranz)
