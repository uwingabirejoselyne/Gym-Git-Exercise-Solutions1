
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

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout -b 'ft/bundle-2'
Switched to a new branch 'ft/bundle-2'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)
$ touch services.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)
$ git commit -m 'adding service page'
[ft/bundle-2 081f2bb] adding service page
 1 file changed, 1 insertion(+), 4 deletions(-)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 667 bytes | 667.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/ft/bundle-2
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)

```

# Git exercise
# bundle 02
# exercise 02


```bash
User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout ft/bundle-2 
Switched to branch 'ft/bundle-2'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)
$ git chekout main
git: 'chekout' is not a git command. See 'git --help'.

The most similar command is
        checkout

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git pull
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), 1.39 KiB | 26.00 KiB/s, done.
From https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1
   c8c1cc2..f95e3d8  main       -> origin/main
Updating c8c1cc2..f95e3d8
Fast-forward
 about.html    | 11 +++++++++++
 services.html |  5 +----
 2 files changed, 12 insertions(+), 4 deletions(-)
 create mode 100644 about.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout -b 'ft/service-redesign'
Switched to a new branch 'ft/service-redesign'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git commit -m 'Making some change on service page using ft/service-redesign branch '
[ft/service-redesign 7d91ac0] Making some change on service page using ft/service-redesign branch
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 410 bytes | 410.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/ft/service-redesign  
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

 User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
M       README.md
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git add services.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git commit -m 'Making some change on service page using main branch '
[main a4cd4e1] Making some change on service page using main branch
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 573 bytes | 573.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   f95e3d8..a4cd4e1  main -> main

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout  'ft/service-redesign'
Switched to branch 'ft/service-redesign'
M       README.md

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git diff main
diff --git a/README.md b/README.md
index ecf890f..5ee9168 100644
--- a/README.md
+++ b/README.md
@@ -276,4 +276,76 @@ To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git

 User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/bundle-2)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign|MERGING)     
$ git add services.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign|MERGING)     
$ git commit -m 'solving conflict '
[ft/service-redesign df06311] solving conflict

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git merge main
Already up to date.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 395 bytes | 395.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   7d91ac0..df06311  ft/service-redesign -> ft/service-redesign
```

# Git exercise
# bundle 03
# exercise 01

```bash


User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout -b 'ft/team-page'
Switched to a new branch 'ft/team-page'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ touch team.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git add team.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git commit -m 'Creation of Team page'
[ft/team-page 1a6a3d0] Creation of Team page
 1 file changed, 11 insertions(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 431 bytes | 431.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/ft/team-page     
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      ft/team-page -> ft/team-page

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout -b 'ft/contact-page'
Switched to a new branch 'ft/contact-page'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout ft/team-page 
Switched to branch 'ft/team-page'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git log
commit 1a6a3d06a5201e8e208559df88573677fbf4c464 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Joselyne uwingabire <uwingajoselyne@gmail.com>
Date:   Fri Jul 28 10:51:14 2023 +0200

    Creation of Team page

commit 27f5e57ceeaa9403b644e427f5c35169c5420b07 (origin/main, origin/HEAD, main, ft/contact-page)        
Author: Joselyne uwingabire <uwingajoselyne@gmail.com>

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ git cherry-pick 1a6a3d06a5201e8e208559df88573677fbf4c464
[ft/contact-page e15930d] Creation of Team page
 Date: Fri Jul 28 10:51:14 2023 +0200
 1 file changed, 11 insertions(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ git push origin ft/contact-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 436 bytes | 436.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/ft/contact-page  
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      ft/contact-page -> ft/contact-page

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ touch contact.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ git add contact.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ git commit -m 'Creation of contact page'
[ft/contact-page 58159d0] Creation of contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ git push origin 'ft/contact-page'
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 452 bytes | 452.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   e15930d..58159d0  ft/contact-page -> ft/contact-page

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/contact-page)
$ git checkout -b 'ft/faq-page'
Switched to a new branch 'ft/faq-page'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ touch faq.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git add faq.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git push origin ft/faq-page
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/ft/faq-page      
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      ft/faq-page -> ft/faq-page

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git checkout main
Switched to branch 'main'
M       README.md
A       faq.html
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
M       README.md
A       faq.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git add faq.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git commit -m 'Saving faq page'
[ft/faq-page 2207c30] Saving faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 440 bytes | 440.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   58159d0..2207c30  ft/faq-page -> ft/faq-page

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
M       README.md

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git log
commit 1a6a3d06a5201e8e208559df88573677fbf4c464 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Joselyne uwingabire <uwingajoselyne@gmail.com>
Date:   Fri Jul 28 10:51:14 2023 +0200
# On branch ft/team-page

    Creation of Team page

commit 27f5e57ceeaa9403b644e427f5c35169c5420b07 (origin/main, origin/HEAD, main)
Author: Joselyne uwingabire <uwingajoselyne@gmail.com>

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git revert 1a6a3d06a5201e8e208559df88573677fbf4c464
[ft/team-page 1c61c2c] Revert "Creation of Team page"
 1 file changed, 11 deletions(-)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 289 bytes | 289.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   1a6a3d0..1c61c2c  ft/team-page -> ft/team-page

```
# Git exercise
# bundle 03
# exercise 02

```bash
User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/faq-page)
$ git checkout -b 'ft/home-page-redesign'
Switched to a new branch 'ft/home-page-redesign'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git add index.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git commit -m 'Adding paragraph on main branch'
[main 0f3f1f9] Adding paragraph on main branch
 1 file changed, 1 insertion(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 615 bytes | 615.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   bbbc1dc..0f3f1f9  main -> main

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (main)
$ git checkout ft/home-page-redesign 
Switched to branch 'ft/home-page-redesign'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign)
$ git commit -m 'saving readme'
[ft/home-page-redesign f28e962] saving readme
 1 file changed, 7 insertions(+), 6 deletions(-)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 356 bytes | 356.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   f676f10..f28e962  ft/home-page-redesign -> ft/home-page-redesign

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign)
$ git rebase main
dropping e15930d3e29e24216eec62698813324c602abaed Creation of Team page -- patch contents already upstream
dropping 58159d0806c9182862b764182d34786bca64c569 Creation of contact page -- patch contents already upstream
dropping 2207c30612b4d781f8c3b4a4fd21201fca00c80f Saving faq page -- patch contents already upstream
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply a9499b9... changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
Could not apply a9499b9... changes

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git commit -m 'saving readme'
[detached HEAD a9427e7] saving readme
 1 file changed, 1 insertion(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git push origin ft/home-page-redesign
Everything up-to-date
```
# Git exercise
# bundle 04
# exercise 01
```bash

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git remote add git-copy https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1Copy.git


User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git commit -m 'Change home page'
[main 6a913cb] Change home page
 1 file changed, 1 insertion(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 442 bytes | 442.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
   6372384..6a913cb  main -> main

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 9/10)
$ git push git-copy main
Enumerating objects: 124, done.
Counting objects: 100% (124/124), done.
Delta compression using up to 12 threads
Compressing objects: 100% (120/120), done.
Writing objects: 100% (124/124), 19.52 KiB | 1.30 MiB/s, done.
Total 124 (delta 66), reused 13 (delta 3), pack-reused 0
remote: Resolving deltas: 100% (66/66), done.
```

# Git exercise
# bundle 04
# exercise 02

```bash
User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git commit -m 'Creating footer section'
[ft/footer f794332] Creating footer section
 1 file changed, 4 insertions(+)


User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git commit -m 'Adding paragraph to the footer'
[ft/footer cc5ac46] Adding paragraph to the footer
 1 file changed, 1 insertion(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git push origin ft/footer
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 761 bytes | 761.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/ft/footer
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      ft/footer -> ft/footer

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git checkout -b 'ft/squashing'
Switched to a new branch 'ft/squashing'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git merge --squash ft/footer
Updating d170d99..cc5ac46
Fast-forward
Squash commit -- not updating HEAD
 index.html | 5 +++++
 1 file changed, 5 insertions(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git commit -m "footer changes squashing"
[ft/squashing fead992] footer changes squashing1~
 1 file changed, 5 insertions(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git commit -m "footer changes squashing"
[ft/squashing 07c7228] footer changes squashing
 1 file changed, 1 insertion(+)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git push origin ft/footer
Everything up-to-date

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/Gym-Git-Exercise-Solutions1 (ft/home-page-redesign|REBASE 10/10)
$ git push origin  ft/squashing
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 785 bytes | 785.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1/pull/new/ft/squashing
remote:
To https://github.com/uwingabirejoselyne/Gym-Git-Exercise-Solutions1.git
 * [new branch]      ft/squashing -> ft/squashing

```
# Git exercise
# bundle 05
# exercise 01
```bash
https://uwingabirejoselyne.github.io/Gym-Git-Exercise-Solutions1/
```

# Git exercise
# bundle 05
# exercise 02
```bash

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (main)
$ git add index.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (main)
$ git commit -m 'Editing index Page'
[main 3a3d013] Editing index Page
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 322 bytes | 322.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/uwingabirejoselyne/git-cafe-exercise.git
   4873d22..3a3d013  main -> main


```
# Git exercise
# bundle 06
# exercise 01
```bash
User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (main)
$ git checkout -b feature 
Switched to a new branch 'feature'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (feature)
$ touch menu.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (feature)
$ git add menu.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (feature)
$ git commit -m 'Creating menu page'
[feature c61ed45] Creating menu page
 1 file changed, 14 insertions(+)
 create mode 100644 menu.html

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (feature)
$ git push origin feature
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 737 bytes | 368.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To https://github.com/uwingabirejoselyne/git-cafe-exercise.git
   4cf4815..a6e5e47  feature -> feature
   
```
# Git exercise
# bundle 06
# exercise 02
```bash
User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (feature)
$ git  checkout -b bug_fix
Switched to a new branch 'bug_fix'

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (bug_fix)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (bug_fix)
$ git commit -m 'Fixing bug on bundle 6 exercise 2'
[bug_fix da00e4a] Fixing bug on bundle 6 exercise 2 
 1 file changed, 203 insertions(+), 203 deletions(-)
 rename index-4.html => contact.html (97%)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (bug_fix)
$ git push origin bug_fix
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 2.51 KiB | 1.25 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'bug_fix' on GitHub by visiting:
remote:      https://github.com/uwingabirejoselyne/git-cafe-exercise/pull/new/bug_fix
remote:
To https://github.com/uwingabirejoselyne/git-cafe-exercise.git
 * [new branch]      bug_fix -> bug_fix
```

# Git exercise
# bundle 06
# exercise 03
```bash

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (bug_fix)
$ git add .

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (bug_fix)
$ git commit -m 'making small hotfix on the contact page'
[bug_fix a2d3875] making small hotfix on the contact page
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-Q9JB4D6 MINGW64 ~/Desktop/The Gym/git-cafe-exercise (bug_fix)
$ git push origin bug_fix
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 320 bytes | 320.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0        
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/uwingabirejoselyne/git-cafe-exercise.git
   da00e4a..a2d3875  bug_fix -> bug_fix
```
# Git exercise
# bundle 06
# exercise 04
```bash


```