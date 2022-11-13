$ git init
Initialized empty Git repository in C:/Users/EUGEN/eugen/.git/

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git remote add origin https://github.com/Ezarne01/TestBranch.git

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ touch FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git commit -m "Commit 0"
[master (root-commit) 9a4da70] Commit 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git checkout -b bug-fix
Switched to a new branch 'bug-fix'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git switch master
Switched to branch 'master'

Eugen@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ alias graph="git log --all --decorate --oneline --graph"

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ graph
* 9a4da70 (HEAD -> master, bug-fix) Commit 0

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git commit -m "Commit 1"
[master c376b42] Commit 1
 1 file changed, 1 insertion(+)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git commit -m "Commit 2"
[master 88d845c] Commit 2
 1 file changed, 3 insertions(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git switch bug-fix
Switched to branch 'bug-fix'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ graph
* 88d845c (master) Commit 2
* c376b42 Commit 1
* 9a4da70 (HEAD -> bug-fix) Commit 0

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git commit -m "Commit 3"
[bug-fix ae454bf] Commit 3
 1 file changed, 2 insertions(+)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git commit -m "Commit 4"
[bug-fix 9b9ab3c] Commit 4
 1 file changed, 1 insertion(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git checkout -b bug-fix-experimental
Switched to a new branch 'bug-fix-experimental'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git switch bug-fix
Switched to branch 'bug-fix'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git merge master
Auto-merging FILE.md
CONFLICT (content): Merge conflict in FILE.md
Automatic merge failed; fix conflicts and then commit the result.

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix|MERGING)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix|MERGING)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix|MERGING)
$ git commit -m "Commit 5"
[bug-fix 798841e] Commit 5

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ code F

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git commit -m "Commit 6"
[bug-fix d2e3b66] Commit 6
 1 file changed, 1 insertion(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git switch bug-fix-experimental
Switched to branch 'bug-fix-experimental'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git commit -m "Commit 7"
[bug-fix-experimental 26d89e2] Commit 7
 1 file changed, 1 insertion(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git commit -m "Commit 8"
[bug-fix-experimental 321c36f] Commit 8
 1 file changed, 1 insertion(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git commit -m "Commit 9"
[bug-fix-experimental a73be38] Commit 9
 1 file changed, 1 insertion(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix-experimental)
$ git switch master
Switched to branch 'master'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ code F

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git commit -m "Commit 10"
[master cb04525] Commit 10
 1 file changed, 1 insertion(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git switch bug-fix
Switched to branch 'bug-fix'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git merge bug-fix-experimental
Auto-merging FILE.md
CONFLICT (content): Merge conflict in FILE.md
Automatic merge failed; fix conflicts and then commit the result.

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix|MERGING)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix|MERGING)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix|MERGING)
$ git commit -m "Commit 11"
[bug-fix 8be61c9] Commit 11

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git commit -m "Commit 12"
[bug-fix f221456] Commit 12
 1 file changed, 1 insertion(+), 1 deletion(-)

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (bug-fix)
$ git switch master
Switched to branch 'master'

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ git merge bug-fix
Auto-merging FILE.md
CONFLICT (content): Merge conflict in FILE.md
Automatic merge failed; fix conflicts and then commit the result.

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master|MERGING)
$ code FILE.md

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master|MERGING)
$ git add .

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master|MERGING)
$ git commit -m "Commit 13"

EUGEN@DESKTOP-4P2EJC5 MINGW64 ~/eugen (master)
$ graph
*   bea4781 (HEAD -> master) Commit 13
|\
| * f221456 (bug-fix) Commit 12
| *   8be61c9 Commit 11
| |\
| | * a73be38 (bug-fix-experimental) Commit 9
| | * 321c36f Commit 8
| | * 26d89e2 Commit 7
| * | d2e3b66 Commit 6
| * |   798841e Commit 5
| |\ \
| | |/
| |/|
| * | 9b9ab3c Commit 4
| * | ae454bf Commit 3
* | | cb04525 Commit 10
| |/
|/|
* | 88d845c Commit 2
* | c376b42 Commit 1
|/
* 9a4da70 Commit 0
