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

 ### Exercise2

 ```bash
FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git add home.html

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 4514fce readme for first exercise

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git add about.html

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 4514fce readme for first exercise

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git add team.html

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash
Saved working directory and index state WIP on dev: 4514fce readme for first exercise

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash list
stash@{0}: WIP on dev: 4514fce readme for first exercise
stash@{1}: WIP on dev: 4514fce readme for first exercise
stash@{2}: WIP on dev: 4514fce readme for first exercise

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash pop stash@{1}:
fatal: 'stash@{1}:' is not a stash-like commit

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (5541382476a43c35d029ad74f00d3f3f21314a55)

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (79a9ee8e624f25e68dce6df1fccb3bb9e5ccadbe)

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git add .

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git commit -m "adding home and about page"
[dev e7bc9bc] adding home and about page
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 536 bytes | 268.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/devfabien/Gym-git-exercise-solution.git
   4514fce..e7bc9bc  dev -> dev

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash list
stash@{0}: WIP on dev: 4514fce readme for first exercise

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (dd7c54376cfe41f5b8022b9637ffab129fb20163)

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git reset --hard
HEAD is now at e7bc9bc adding home and about page

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

 ```

 ## Bundle2

 ### Exercise1

 ```bash
FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        service.html

nothing added to commit but untracked files present (use "git add" to track)

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (ft/bundle-2)
$ git add service.html

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (ft/bundle-2)
$ git commit -m "adding service page"
[ft/bundle-2 31a66e8] adding service page
 1 file changed, 11 insertions(+)
 create mode 100644 service.html

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 442 bytes | 442.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/devfabien/Gym-git-exercise-solution/pull/new/ft/bundle-2
remote:
To https://github.com/devfabien/Gym-git-exercise-solution.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

FABIEN@DESKTOP-1HATNBG MINGW64 ~/Documents/TheGym/Gym git exercise (ft/bundle-2)


 ```
  ### Exercise 2

  ```bash
The Gym@DESKTOP-249BB42 MINGW64 ~/Documents/Gym/Gym-git-exercise-solution (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

The Gym@DESKTOP-249BB42 MINGW64 ~/Documents/Gym/Gym-git-exercise-solution (main)
$ git pull
Already up to date.

The Gym@DESKTOP-249BB42 MINGW64 ~/Documents/Gym/Gym-git-exercise-solution (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

The Gym@DESKTOP-249BB42 MINGW64 ~/Documents/Gym/Gym-git-exercise-solution (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

no changes added to commit (use "git add" and/or "git commit -a")

The Gym@DESKTOP-249BB42 MINGW64 ~/Documents/Gym/Gym-git-exercise-solution (ft/service-redesign)
$ git add .

The Gym@DESKTOP-249BB42 MINGW64 ~/Documents/Gym/Gym-git-exercise-solution (ft/service-redesign)
$ git commit -m "adding services"
[ft/service-redesign 79dc58f] adding services
 1 file changed, 5 insertions(+)

The Gym@DESKTOP-249BB42 MINGW64 ~/Documents/Gym/Gym-git-exercise-solution (ft/service-redesign)

S C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 495 bytes | 165.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/devfabien/Gym-git-exercise-solution/pull/new/ft/service-redesign
remote:
To https://github.com/devfabien/Gym-git-exercise-solution.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout main
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git status
On branch main

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git add .
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git commit -m "modifying service page from main"
 1 file changed, 1 insertion(+)
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 348 bytes | 348.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/devfabien/Gym-git-exercise-solution.git
   df965a5..492f4ff  main -> main
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git merge main
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git diff
index 88b6010,2e75ad6..0000000
--- a/service.html
@@@ -7,10 -7,6 +7,14 @@@
  </head>
  <body>
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git merge main
fatal: You have not concluded your merge (MERGE_HEAD exists).
Please, commit your changes before you merge.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.
All conflicts fixed but you are still merging.

Changes to be committed:
        modified:   service.html

PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git commit -m "updated service"
[ft/service-redesign f82c95f] updated service
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 363 bytes | 363.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/devfabien/Gym-git-exercise-solution.git
   79dc58f..f82c95f  ft/service-redesign -> ft/service-redesign
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution>

  ```

  