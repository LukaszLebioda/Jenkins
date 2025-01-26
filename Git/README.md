### vocabulary, aliases, basic commands

- working directory (uncommited changes),
- staging area (changes are now tracked by git),
- git repository (commited changes),
- external repository (pushed changes),

git aliases
-> ~/.gitconfig
create new group [alias] and create aliases for git (git ch = git checkout etc.)
[alias]
        ch = checkout
        st = status

`git init` -> to initialize git repository in current folder,
`rm -rf .git/` -> to remove git repository from current folder,
`git status` -> current state of git repository
`git clone` -> to clone remote git repo (e.g. grom GitHub),

### git add, git commit

`git add` -> adds files from working directory to git staging area,
`git add .` -> adds all files,
`git add folder/file.txt folder2/file2.txt` -> adds specific file(s),

`git commit` -> adds files from staging area to git repository,
`git commit -m "message"` -> adds file with a git message,

### git log, git diff, git show

`git log` -> displays information about commits (q to quit),
`git log --oneline` -> displays high-level information,
- when in vim log output, type `/` to search for any string,

`git diff` -> shows diff between workdir and git_repo (with staging),
`git diff --name-status` -> shows high level differences,
`git diff --cached` or `git diff --staged` -> shows diffs between staging area and the state of git repo (last commit),

`git diff commitId1..commitId2` -> diff between 2 particular commits,
or `git diff commitId1 commitId2`
`git diff commitId1..`, -> diff from 1 commit downwards,
`git diff --name-status commitId1..` -> shows high level differences,
- first 7 signs of commit sha identifier is enough,

`git show commitId` -> git log + git diff combined,
