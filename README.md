# Git Commands
A list of some useful git commands to know
http://rogerdudler.github.io/git-guide/

1) squashing X commits into one
 ```
 git rebase -i HEAD~X
 ```

"pick" a file, and replace the other "picks" with "squash"

2) undo your last commit without losing your changes

https://stackoverflow.com/questions/927358/how-to-undo-the-last-commits-in-git
```
git reset HEAD~1
```

3) undo your git reset HEAD~X
```
git reset HEAD@{X}
```

4) fix your latest commit without changing the snapshot 

https://www.atlassian.com/git/tutorials/rewriting-history

```
git commit --amend
```

5) look at a comprehensive list of all your git actions. 
```
git reflog
```
If you ever get into a mess, this will save you. 

6) Cherry pick a commit from one branch and apply it to another branch
https://stackoverflow.com/questions/9339429/what-does-cherry-picking-a-commit-with-git-mean
```
git cherry-pick <commit-hash>
```

if cherry-picking from a public branch, use
```
git cherry-pick -x <commit-hash>
```
