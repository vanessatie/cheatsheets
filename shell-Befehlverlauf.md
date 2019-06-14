## Bei Merge-Konflikt zwischen zwei Branches, die auf den Master wollen: (Branches rewritten-main und )

➜ git-playground git:(master) git checkout -b main-text
Switched to a new branch 'main-text'
➜ git-playground git:(main-text) code .
➜ git-playground git:(main-text) git add .
➜ git-playground git:(main-text) ✗ git commit -m "add main plus font-size"
[main-text 1310a0b] add main plus font-size
2 files changed, 12 insertions(+)
➜ git-playground git:(main-text) git push
fatal: The current branch main-text has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main-text

➜ git-playground git:(main-text) git push --set-upstream origin main-text
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 550 bytes | 550.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0)
remote:
remote: To create a merge request for main-text, visit:
remote: https://gitlab.com/vanessatie/git-playground/merge_requests/new?merge_request%5Bsource_branch%5D=main-text
remote:
To gitlab.com:vanessatie/git-playground.git

- [new branch] main-text -> main-text
  Branch 'main-text' set up to track remote branch 'main-text' from 'origin'.

## Erster Branch wurde schon gemerged. Nun gehts um den Zweiten. Dieses Problem muss lokal gelöst werden:

➜ git-playground git:(master) git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0)
Unpacking objects: 100% (1/1), done.
From gitlab.com:vanessatie/git-playground
4e0792f..77f3b62 master -> origin/master
Updating 4e0792f..77f3b62
Fast-forward
index.html | 8 ++++++++
styles.css | 4 ++++
2 files changed, 12 insertions(+)
➜ git-playground git:(master) git checkout rewritten-main
Switched to branch 'rewritten-main'
Your branch is up to date with 'origin/rewritten-main'.
➜ git-playground git:(rewritten-main) git merge master
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.
➜ git-playground git:(rewritten-main|MERGING) ✗ code .
➜ git-playground git:(rewritten-main|MERGING) ✗ git add .
➜ git-playground git:(rewritten-main|MERGING) ✗ git commit
[rewritten-main 197617c] Merge branch 'master' into rewritten-main
➜ git-playground git:(rewritten-main) git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 371 bytes | 371.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote:
remote: View merge request for rewritten-main:
remote: https://gitlab.com/vanessatie/git-playground/merge_requests/4
remote:
To gitlab.com:vanessatie/git-playground.git
ddd14da..197617c rewritten-main -> rewritten-main
➜ git-playground git:(rewritten-main)
