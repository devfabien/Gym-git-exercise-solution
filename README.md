 # THE GYM Git Exercise

 ## Bundle1

 ### Exercise1

 ```bash
FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise
$ git init
Initialized empty Git repository in C:/Users/FABIEN/Documents/TheGym/Gym git exercise/.git/

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (main)
$ git branch -M main

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (main)
$ git add .

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (main)
$ git commit -m "add readme"
[main (root-commit) 745a93c] add readme
 1 file changed, 30 insertions(+)
 create mode 100644 README.md

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (main)
$ git remote add origin https://github.com/devfabien/Gym-git-exercise-solution.git

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 531 bytes | 265.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/devfabien/Gym-git-exercise-solution.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (main)
$ git checkout -b dev
Switched to a new branch 'dev'

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/devfabien/Gym-git-exercise-solution/pull/new/dev
remote:
To https://github.com/devfabien/Gym-git-exercise-solution.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git checkout -b test
Switched to a new branch 'test'

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (test)
$ git push --set-upstream origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/devfabien/Gym-git-exercise-solution/pull/new/test
remote:
To https://github.com/devfabien/Gym-git-exercise-solution.git
 * [new branch]      test -> test
branch 'test' set up to track 'origin/test'.

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git branch -D test
Deleted branch test (was 745a93c).

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git push origin --delete test
To https://github.com/devfabien/Gym-git-exercise-solution.git
 - [deleted]         test

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)

 ```

 # Exercise2

 ```bash

 ```