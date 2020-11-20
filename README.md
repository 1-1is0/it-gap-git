# summary

## list of command used it for this repo


`$ git init` Create an empty Git repository  

`$ git remote add origin git@github.com:1-1is0/it-gap-git.git`
adding the remote repository to the local git repo  

To list all the remote repo.

```shell
$ git remote -v
origin  git@github.com:1-1is0/it-gap-git.git (fetch)
origin  git@github.com:1-1is0/it-gap-git.git (push)
```

`git add` git-add - Add file contents to the index  

never use `$ git add .` or `$ git add -all` if you don't know what you are doing.  
`$ git add -i` opens up an interactive shell to add and update your files and see the diffs
so you don't have to write the long command for each file.

```shell
$ git add -i

*** Commands ***
  1: status       2: update       3: revert       4: add untracked
  5: patch        6: diff         7: quit         8: help
```

before adding files with `git add`

```shell
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        README.md

nothing added to commit but untracked files present (use "git add" to track)
```

after adding files

```shell
$ git add .gitignore README.md

$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   .gitignore
        new file:   README.md
```

`$ git commit -m "<message>"` create a commit with all the files added (staged)  
or just use `$ git commit` to open a text editor and write your message in there.

```shell
$ git status 
On branch master
nothing to commit, working tree clean
```

to push the changes to a remote repository.

`$ git push origin master`

