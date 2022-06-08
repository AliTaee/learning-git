## Branching

- Creates a new branch called bugfix: `git branch bugfix`
- Switches to the bugfix branch: `git checkout bugfix` or `git switch bugfix`
- Creates and switches: `git switch -C bugfix`
- Deletes the bugfix branch: `git branch -d bugfix`

## Comparing branches

- Lists the commits in the bugfix branch not in master: `git log master..bugfix`
- Shows the summary of changes: `git diff master..bugfix`

## Stashing

- Creates a new stash: `git stash push -m “New tax rules”`
- Lists all the stashes: `git stash list`
- Shows the given stash: `git stash show stash@{1}` or `git stash show 1 `
- Applies the given stash to the working dir: `git stash apply 1`
- Deletes the given stash: `git stash drop 1`
- Deletes all the stashes: `git stash clear`

## Merging

- Merges the bugfix branch into the current branch: `git merge bugfix`
- Creates a merge commit even if FF (fast forward merge) is possible: `git merge --no-ff bugfix`
- Merges the bugfix branch into the current branch: `git merge bugfix`
- Performs a squash merge: `git merge --squash bugfix`
- Aborts the merge: `git merge --abort`

## Viewing the merged branches

- Shows the merged branches: `git branch --merged`
- Shows the unmerged branches: `git branch --no-merged`

## Rebasing

- Changes the base of the current branch: `git rebase master`
- Open our merge tool during rebase process if we have any conflict: `git mergetool`
- Skip a rebase process: `git rebase --skip`
- Stop rebase process: `git rebase --abort`

## Cherry picking

- Applies the given commit on the current branch: `git cherry-pick dad47ed `
