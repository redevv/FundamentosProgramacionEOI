# CLASE PROGRAMACIÓN 11/04/22
## Para cambiar de rama y traer archivos de una rama a otra:
````
git status
On branch master
Your branch is up to date with 'main/master'.

nothing to commit, working tree clean
MBPdeMacbook3:00-EOI davidrey$ git remote -v
main	https://github.com/redevv/FundamentosProgramacionEOI.git (fetch)
main	https://github.com/redevv/FundamentosProgramacionEOI.git (push)
MBPdeMacbook3:00-EOI davidrey$ git status
On branch master
Your branch is up to date with 'main/master'.

nothing to commit, working tree clean
MBPdeMacbook3:00-EOI davidrey$ git remote -v
main	https://github.com/redevv/FundamentosProgramacionEOI.git (fetch)
main	https://github.com/redevv/FundamentosProgramacionEOI.git (push)
MBPdeMacbook3:00-EOI davidrey$ git remote rm main
MBPdeMacbook3:00-EOI davidrey$ git remote add origin https://github.com/redevv/FundamentosProgramacionEOI
MBPdeMacbook3:00-EOI davidrey$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

MBPdeMacbook3:00-EOI davidrey$ git push --set-upstream origin master
Branch 'master' set up to track remote branch 'master' from 'origin'.
Everything up-to-date
MBPdeMacbook3:00-EOI davidrey$ git branch
* master
MBPdeMacbook3:00-EOI davidrey$ git branch main
MBPdeMacbook3:00-EOI davidrey$ git branch
  main
* master
MBPdeMacbook3:00-EOI davidrey$ git switch main
Switched to branch 'main'
MBPdeMacbook3:00-EOI davidrey$ git branch
* main
  master
MBPdeMacbook3:00-EOI davidrey$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

MBPdeMacbook3:00-EOI davidrey$     git push --set-upstream origin main
To https://github.com/redevv/FundamentosProgramacionEOI
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/redevv/FundamentosProgramacionEOI'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
MBPdeMacbook3:00-EOI davidrey$     git push --set-upstream origin main
To https://github.com/redevv/FundamentosProgramacionEOI
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/redevv/FundamentosProgramacionEOI'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
MBPdeMacbook3:00-EOI davidrey$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), 1.25 KiB | 116.00 KiB/s, done.
From https://github.com/redevv/FundamentosProgramacionEOI
 * [new branch]      main       -> origin/main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main

MBPdeMacbook3:00-EOI davidrey$ git branch --set-upstream-to=origin/main main
Branch 'main' set up to track remote branch 'main' from 'origin'.
````

## Crear nombre en hexadecimal y binario:
````
D 44 0010 1100
A 41 0010 1001
V 56 0011 1000
I 49 0011 0001
D 44 0010 1100

Hexadecimal: 44 41 56 49 44
Binario: 0010 1100 0010 1001 0011 1000 0011 0001 0010 1100