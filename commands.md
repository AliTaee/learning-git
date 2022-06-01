# Git commands 💻

## Basic git commands

- Get version: `git --version`
- Help: here we search about config: ℹ️
  - Full command: `git config --help`
  - Short command: `git config --h`
- Initial new git project: `git init`

## Set settings

- Name: `git config --global user.name 'Ali Taee'`
- Email: `git config --global user.email ali.taee.72@gmail.com`
- Editor: `git config --global core.editor 'code --wait'`
- Ending line: Mac/Linux `git config --global core.autocrlf input`
- Ending line: Windows `git config --global core.autocrlf true`

## Creating snapshots 📸

- Delete and add staging command: `git rm "file name or patterns"`
- See files in staging 🗃️: `git ls-files`
- Add file to staging and commit in same time: `git commit -am "commit message"`
- Move command: `git mv "old file name" "renamed file name"`
- Get last state of files:
  - `git status`
  - `git status -s`
- Review what is changed 🔍:
  - `git diff`
  - `git diff --staged`
- Show git history 📜:
  - With details: `git log`
  - Focus is on git message: `git log --oneline`
  - Focus is on git message with reverse timeline: `git log --oneline --reverse`
- Show a commit:
  - Showing a commit with ID: `git show ID`
  - Showing head commit: `git show HEAD`
  - Showing pervious head commit: `git show HEAD~`
  - Showing pervious head commit with specific number: `git show HEAD~number to pervious commits`
- Undo work on a file:
  - on stage: `git restore --staged file name`
  - on working environment: - `git restore file name`
- `git clean -fd`
- Restore a file from pervious head commit with specific number: `git restore --source=HEAD~1 full path name`

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
- Show Range of Commits: `git log hash1..hash2`
- Formatting the log output: `git log --pretty=format:”%an committed %H”`
- Filter logs by:
  - Author name: `git log --author=“Ali”`
  - Date: `git log --before=“2020-08-17”` or `git log --after=“one week ago”`
  - A word in:
    - Message: `git log --grep=“GUI”`
    - Changes: `git log -S“GUI”`

## Comparing commits

- Between two commits: `git diff HEAD~2 HEAD --name-only`
- Specific file between commits: `git diff HEAD~2 HEAD file.txt`

## Checking out

- To a commit: `git checkout dad47ed`
- To a branch: `git checkout master`
