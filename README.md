
Navar@DESKTOP-IPH2O36 MINGW64 ~ (master)
$ PWD
/c/Users/Navar

Navar@DESKTOP-IPH2O36 MINGW64 ~ (master)
$ mkdir seccion3

Navar@DESKTOP-IPH2O36 MINGW64 ~ (master)
$ cd seccion3/

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git init
Initialized empty Git repository in C:/Users/Navar/seccion3/.git/

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ touch index.html

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ ls
index.html

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ pwd
/c/Users/Navar/seccion3

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ code.
bash: code.: command not found

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ code .

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git add index.html

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git commit -m "Agregado archivo index.html"
[master (root-commit) 9890bc1] Agregado archivo index.html
 1 file changed, 13 insertions(+)
 create mode 100644 index.html

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git branch develop

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git checkout develop
Switched to branch 'develop'

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ touch .env

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ touch .gitignore

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git add .gitignore

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git add index.html

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git commit -m "Cambios en la rama develop"
[develop 1f983e0] Cambios en la rama develop
 2 files changed, 13 insertions(+), 1 deletion(-)
 create mode 100644 .gitignore

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git checkout main
error: pathspec 'main' did not match any file(s) known to git

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git status
On branch develop
nothing to commit, working tree clean

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git checkout main
error: pathspec 'main' did not match any file(s) known to git

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git branch
* develop
  master

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (develop)
$ git checkout master
Switched to branch 'master'

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ cat index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>seccio3</title>
</head>
<body>
    <h1>seccion3</h1>

</body>
</html>
Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git merge develop
Updating 9890bc1..1f983e0
Fast-forward
 .gitignore |  1 +
 index.html | 13 ++++++++++++-
 2 files changed, 13 insertions(+), 1 deletion(-)
 create mode 100644 .gitignore

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ cat index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>seccio3</title>
</head>

<body>
    <h1>seccion3</h1>
    <p>Esta es una página de ejemplo.</p>
    <p>Agregado un nuevo párrafo</p>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laboriosam, veritatis sequi asperiores placeat quasi
        quam, enim nostrum consequuntur animi, ipsum illo reiciendis. Eos nemo eligendi pariatur deserunt suscipit,
        eaque iste.</p>
    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Placeat, ex! Id ut non cupiditate illum doloribus?
        Porro praesentium optio dolorum quibusdam eos distinctio voluptas, amet incidunt mollitia quis labore veritatis!
    </p>

</body>

</html>
Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git ls-files --other --ignored --exclude-standard
.env

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ touch README.MD

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git remote add origin https://github.com/joker2207/aspirantes-mir-ejercicioi-3.git

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (master)
$ git branch -M main

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (main)
$ git push -u origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (7/7), 1017 bytes | 169.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/joker2207/aspirantes-mir-ejercicioi-3.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Navar@DESKTOP-IPH2O36 MINGW64 ~/seccion3 (main)
$