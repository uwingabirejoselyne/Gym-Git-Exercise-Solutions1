
# Git exercise
# bundle 01
# exercise 01
```bash

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1
$ git init
Initialized empty Git repository in D:/The gym/Gym-Git-Exercise-Solutions1/.git/

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (master)
$ git branch main
fatal: not a valid object name: 'master'

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (master)
$ git branch -m main

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git add .

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git commit -m 'my first commit'
[main (root-commit) 6d47a36] my first commit
 2 files changed, 12 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git remote add origin origin https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from


Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git remote add origin https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$  git push --set-upstream origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 466 bytes | 155.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout -b dev
Switched to a new branch 'dev'

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout dev
Switched to branch 'dev'

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git branch -d test
error: branch 'test' not found.

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git checkout -b test
Switched to a new branch 'test'

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (test)
$ git checkout dev
Switched to branch 'dev'

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git branch -d test
Deleted branch test (was 6d47a36).
```
# Git exercise
# bundle 01
# exercise 02
```bash

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout dev
Switched to branch 'dev'
D       index.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ touch home.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git add home.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 6d47a36 my first commit

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash list
stash@{0}: WIP on dev: 6d47a36 my first commit
stash@{1}: WIP on main: dc2236c Second committ

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ touch about.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git add about.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 6d47a36 my first commit

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash list
stash@{0}: WIP on dev: 6d47a36 my first commit
stash@{1}: WIP on dev: 6d47a36 my first commit
stash@{2}: WIP on main: dc2236c Second committ

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ touch team.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git add touch
fatal: pathspec 'touch' did not match any files

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git add  team.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 6d47a36 my first commit

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash list
stash@{0}: WIP on dev: 6d47a36 my first commit
stash@{1}: WIP on dev: 6d47a36 my first commit
stash@{2}: WIP on dev: 6d47a36 my first commit
stash@{3}: WIP on main: dc2236c Second committ

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (8816192e7667063796ab653cbeeb8c91610eea61)

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash pop stash@{2}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{2} (a1ca8fe53a815ce2902b8d8ec8b8c998d886e0e1)

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git add .

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git commit -m "second commit"
[dev cf5d4d0] second commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 about.html

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git push --set-upstream origin dev
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 285 bytes | 95.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/dev
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (4761177fc83269c61e2a93981e7bdec6cb771328)

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git log
commit cf5d4d0d3808cef721f84a812da8e99641ce5666 (HEAD -> dev, origin/dev)
Author: Joselyne Uwingabire <uwingajoselyne@gmail.com>
Date:   Tue Jul 11 12:00:41 2023 +0200

    second commit

commit 6d47a36a9676f805637f4e63f897aa4087d8901b
Author: Joselyne Uwingabire <uwingajoselyne@gmail.com>
Date:   Tue Jul 11 11:19:20 2023 +0200

Uwing@DESKTOP-DHVDNUL MINGW64 /d/The gym/Gym-Git-Exercise-Solutions1 (dev)
$ git reset -- hard commit cf5d4d0d3808cef721f84a812da8e99641ce5666

```
# Git exercise
# bundle 02
# exercise 01
```bash


```