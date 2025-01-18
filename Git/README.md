### git init, git status

- working directory (uncommited changes),
- staging area (changes are now tracked by git),
- git repository (commited changes),
- external repository (pushed changes),

`git init` -> to initialize git repository in current folder,
`rm -rf .git/` -> to remove git repository from current folder,
`git status` -> current state of git repository

### git add, git commit

`git add` -> adds files from working directory to git staging area,
`git add .` -> adds all files,
`git add folder/file.txt folder2/file2.txt` -> adds specific file(s),

`git commit` -> adds files from staging area to git repository,
`git commit -m "message"` -> adds file with a git message,

### git log, git diff

`git log` -> displays information about commits (q to quit),
`git log --oneline` -> displays high-level information,

`git diff` -> shows differences between working dir and git repo,
`git diff --name-status` -> shows high level differences,
`git diff --cached` ->

`git diff commitId1..commitId2` -> diff between exact commits,
`git diff commitId1..`, -> diff from a commit downwards,
`git diff --name-status commitId1..` -> shows high level differences,
