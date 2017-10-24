# git_commands
useful git commands

1) squashing X commits into one

git rebase -i HEAD~X

"pick" a file, and replace the other "picks" with "squash"

2) undo your last commit without losing your changes
https://stackoverflow.com/questions/927358/how-to-undo-the-last-commits-in-git

git reset HEAD~1

3) undo your git reset HEAD~X

git reset 'HEAD@{X}'
