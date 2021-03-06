# Git commands đģ

## Basic git commands

- Get version: `git --version`
- Help: here we search about config: âšī¸
  - Full command: `git config --help`
  - Short command: `git config --h`
- Initial new git project: `git init`

## Set settings

- Name: `git config --global user.name 'Ali Taee'`
- Email: `git config --global user.email ali.taee.72@gmail.com`
- Editor: `git config --global core.editor 'code --wait'`
- Ending line: Mac/Linux `git config --global core.autocrlf input`
- Ending line: Windows `git config --global core.autocrlf true`

## Creating snapshots đ¸

- Delete and add staging command: `git rm "file name or patterns"`
- See files in staging đī¸: `git ls-files`
- Add file to staging and commit in same time: `git commit -am "commit message"`
- Move command: `git mv "old file name" "renamed file name"`
- Get last state of files:
  - `git status`
  - `git status -s`
- Review what is changed đ:
  - `git diff`
  - `git diff --staged`
- Show git history đ:
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
