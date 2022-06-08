## Viewing the history

- Show the list of modified files: `git log --stat`
- Show the actual changes (patches): `git log --patch`
- Shows the commits that touched file.txt: `git log file.txt`

- Viewing a commit: `git show HEAD~2`
- Viewing a specific file in a commit: `git show HEAD~2:file1.txt`

- Viewing contributors: `git shortlog`
- Viewing contributors in a specific file: `git blame file.txt` or `git blame -e -L 1,3 file.txt`

## Filtering the history

- Shows the last 3 entries: `git log -3`
- Show Range of Commits: `git log hash1(older)..hash2(newer)`
- Formatting the log output: `git log --pretty=format:"%an committed %H"`
- Filter logs by:
  - Author name: `git log --author="Ali"`
  - Date: `git log --before="2020-08-17"` or `git log --after="one week ago"`
  - A word in (is case sensitive):
    - Message: `git log --grep="GUI"`
    - Changes: `git log -S"GUI"`

## Comparing commits

- Between two commits: `git diff HEAD~2 HEAD --name-only`
- Specific file between commits: `git diff HEAD~2 HEAD file.txt`

## Checking out

- To a commit: `git checkout dad47ed`
- To a branch: `git checkout master`
