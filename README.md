
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