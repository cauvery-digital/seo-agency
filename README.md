# Git Commands

## Configuring Git

git config --global user.name ""

git config --global user.email ""

git config --list


## Clone And Status

### Clone- cloning a repository from github to our local machine

git clone <-Link->

## Status - displays the state of the code

git status

untracked, modified, staged, unmodified

## Branch Commands

### to check branch

git branch

### to rename branch

git branch -M main

### to navigate

git checkout <branch name>

### to create new branch

git checkout -b <new branch name>


### to delete branch

git branch -d <branch name>


## Undoing Changes

### Case1: staged changes

git reset <file name>

git reset

### Case2: commited changes (for one commit)

git reset HEAD-1

### Case3: commited changes (for many commits)

git reset <commit Hash>

git reset --hard <commit Hash>

## to Initialize

git init



# Quick setup — if you’ve done this kind of thing before

or	

https://github.com/cauvery-digital/seo-agency.git


Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

## …or create a new repository on the command line


echo "# seo-agency" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/cauvery-digital/seo-agency.git

git push -u origin main

## …or push an existing repository from the command line
git remote add origin https://github.com/cauvery-digital/seo-agency.git
git branch -M main
git push -u origin main

git switch master

git --help
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
           [--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
           [--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

geeta@DESKTOP-JGVT41G MINGW64 ~/Documents/WebDesign/QuickStart (main|MERGING)
$ git switch master
fatal: cannot switch branch while merging
Consider "git merge --quit" or "git worktree add".

geeta@DESKTOP-JGVT41G MINGW64 ~/Documents/WebDesign/QuickStart (main|MERGING)
$ git pull
error: You have not concluded your merge (MERGE_HEAD exists).
hint: Please, commit your changes before merging.
fatal: Exiting because of unfinished merge.

geeta@DESKTOP-JGVT41G MINGW64 ~/Documents/WebDesign/QuickStart (main|MERGING)
$ git commit -m "merge"
[main 564a2e1] merge

geeta@DESKTOP-JGVT41G MINGW64 ~/Documents/WebDesign/QuickStart (main)
$ git switch master
branch 'master' set up to track 'origin/master'.
Switched to a new branch 'master'
