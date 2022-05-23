
## Basic git commands

- get version: `git --version`

## Set settings 

- Name: `git config --global user.name 'Ali Taee'`
- Email:  `git config --global user.email ali.taee.72@gmail.com`
- Editor: `git config --global core.editor 'code --wait'`
- Ending line: Mac/Linux `git config --global core.autocrlf input`
- Ending line: Windows `git config --global core.autocrlf true`

## Help 

Here we search about config:

- Full command: `git config --help`
- Short command: `git config --h`

## Setup project

- `git init`

## Creating snapshots

- Delete command: `git rm "file name or patterns"`
- See files in staging: `git ls-files`
- Add file and commit in same time: `git commit -am "commit message"`
- Move command: `git mv "renamed file name" "old file name"`
- `git status`, `git status -s`
- `git diff --staged`, `git diff`
- `git log`, `git log --oneline`, `git log --oneline --reverse`
- `git show ID`, `git show HEAD`, `git show HEAD~`, `git show HEAD~number to pervious commits`
- `git restore --staged file name`
- `git clean -fd`
- `git restore file name`