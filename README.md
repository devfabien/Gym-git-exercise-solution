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

 ## Bundle3

 ### Exercise 1

 ```bash

 PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Writing objects: 100% (3/3), 1.41 KiB | 288.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/devfabien/Gym-git-exercise-solution.git
   f82c95f..5e29996  ft/service-redesign -> ft/service-redesign
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git status
On branch ft/team-page
Untracked files:
        team.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git add .
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git commit -m "adding team page"
[ft/team-page 7792da2] adding team page
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 436 bytes | 436.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:
To https://github.com/devfabien/Gym-git-exercise-solution.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git log
Author: devfabien <ish001fabi@gmail.com>

    adding team page

commit 492f4ff26e44081676063fa92c9fc7cd609c95b3 (origin/main, origin/HEAD, main, ft/contact-page)
Date:   Fri Jul 28 19:07:46 2023 +0200

    modifying service page from main

commit df965a5884f234bd86c609662bdbb2c6f3829753
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout ft/contact-page
[ft/contact-page 533a6e0] adding team page
 Date: Mon Jul 31 08:27:15 2023 +0200
 1 file changed, 11 insertions(+)
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git add .
[ft/contact-page ac65d57] adding contact us page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Delta compression using up to 4 threads
Writing objects: 100% (6/6), 709 bytes | 354.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/devfabien/Gym-git-exercise-solution/pull/new/ft/contact-page
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git checkout -b "ft/faq-page"
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git add .
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git commit -m "adding faq page"
[ft/faq-page c50f477] adding faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Revert "adding team page"
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 439 bytes | 439.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/devfabien/Gym-git-exercise-solution/pull/new/ft/faq-page
remote:
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git revert 7792da2cb2f7eb7b5d3948ae64916f7e6e142f00     
[ft/faq-page 80fea19] Revert "adding team page"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git status
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution> git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 269 bytes | 269.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/devfabien/Gym-git-exercise-solution.git
   c50f477..80fea19  ft/faq-page -> ft/faq-page
PS C:\Users\The Gym\Documents\Gym\Gym-git-exercise-solution>

 ```