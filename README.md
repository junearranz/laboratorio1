# LABORATORIO DE GIT

Este laboratorio tiene como objetivo practicar los comandos básicos de Git.

## 1. Crear un repositorio en local

Entro a la carpeta donde voy a crear el repositorio:
```console
June@DESKTOP-4ABLAGV MINGW64 ~
$ cd repositorios
```
Creo la carpeta:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios
$ mkdir laboratorio1
```
Entro a la carpeta:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios
$ cd laboratorio1
```
Incializo el repositorio:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1
$ git init
Initialized empty Git repository in C:/Users/June/Repositorios/laboratorio1/.git/
```

## 2. Subir el repositorio a GitHub

Creo un nuevo repositorio en GitHub:

https://github.com/junearranz/laboratorio1.git
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git init
Reinitialized existing Git repository in C:/Users/June/Repositorios/laboratorio1/.git/
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git add .
warning: in the working copy of 'package-lock.json', LF will be replaced by CRLF the next time Git touches it
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git commit -m "Hellooo Git"
[master (root-commit) 57a9fc1] Hellooo Git
 1 file changed, 6 insertions(+)
 create mode 100644 package-lock.json
```
``` console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git remote add origin git@github.com:junearranz/laboratorio1.git
```
```console
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
```

## 3. Hacer un commit y un push: Añado varios archivos del repositorio de ejemplo (carpeta src, package.json), creo .gitignore y los sincronizo con GitHub:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git add .
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git commit -m "Añadimos archivo gitignore"
[master 4f7ce01] Añadimos archivo gitignore
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 .gitignore
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git remote add origin git@github.com:junearranz/laboratorio1.git
error: remote origin already exists.
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git push origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 297 bytes | 297.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:junearranz/laboratorio1.git
   7cc1344..4f7ce01  master -> master
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git add .
warning: in the working copy of 'package.json', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'src/index.html', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'src/index.js', LF will be replaced by CRLF the next time Git touches it
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git commit -m "Añadiendo archivos: Carpeta src y package.json"
[master 1acd773] Añadiendo archivos: Carpeta src y package.json
 4 files changed, 30 insertions(+)
 create mode 100644 package.json
 create mode 100644 src/index.html
 create mode 100644 src/index.js
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git push origin master
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 16 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (7/7), 845 bytes | 422.00 KiB/s, done.
Total 7 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:junearranz/laboratorio1.git
   4f7ce01..1acd773  master -> master
```

### 3.1: Cambiando el texto a mostrar por pantalla de los archivos de ejemplo:

```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git add .
warning: in the working copy of 'src/index.html', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'src/index.js', LF will be replaced by CRLF the next time Git touches it
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git commit -m "Cambiando el texto a mostrar por pantalla"
[master 16c4260] Cambiando el texto a mostrar por pantalla
 2 files changed, 2 insertions(+), 2 deletions(-)
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ git push origin master
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 451 bytes | 451.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:junearranz/laboratorio1.git
   1acd773..16c4260  master -> master
```

### 3.2. Instalo dependencias del proyecto y compruebo que funciona:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ npm install
npm warn deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a stable sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility

added 199 packages, and audited 200 packages in 2m

90 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/repositorios/laboratorio1 (master)
$ npm start

> 00-boilerplate@1.0.0 start
> rimraf dist && parcel ./src/index.html --open

Server running at http://localhost:1234
✨ Built in 411ms
```

## 4. Crear una rama

Reviso el estado del proyecto:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/Repositorios/laboratorio1 (master)
$ git status
On branch master
nothing to commit, working tree clean
```
Creo una nueva rama:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/Repositorios/laboratorio1 (master)
$ git branch development
```
Muestro por pantalla todas las ramas existentes:
```console
June@DESKTOP-4ABLAGV MINGW64 ~/Repositorios/laboratorio1 (master)
$ git log --oneline --decorate --graph --all
* 7642bdd (HEAD -> master, origin/master, development) cambios
* 16c4260 Cambiando el texto a mostrar por pantalla
* 1acd773 Añadiendo archivos: Carpeta src y package.json
* 4f7ce01 Añadimos archivo gitignore
* 7cc1344 Hellooo Git
```
Cambio a la rama development
```console
June@DESKTOP-4ABLAGV MINGW64 ~/Repositorios/laboratorio1 (master)
$ git checkout development
Switched to branch 'development'
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/Repositorios/laboratorio1 (development)        
$
```
```console
June@DESKTOP-4ABLAGV MINGW64 ~/Repositorios/laboratorio1 (development)        
$ git status
On branch development
nothing to commit, working tree clean
```

## 5. Hacer un merge

_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx_


## Autores ✒️

* **June Arranz** - [junearranz](https://github.com/junearranz)
