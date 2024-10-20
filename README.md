### Git Commands

## Configuring Git

git config --global user.name ""

git config --global user.email ""

git config --list


## Clone And Status

# Clone- cloning a repository from github to our local machine

git clone <-Link->

# Status - displays the state of the code

git status

untracked, modified, staged, unmodified

## Branch Commands

#### to check branch

git branch

#### to rename branch

git branch -M main

#### to navigate

git checkout <branch name>

#### to create new branch

git checkout -b <new branch name>


#### to delete branch

git branch -d <branch name>


### Undoing Changes

#### Case1: staged changes

git reset <file name>

git reset

#### Case2: commited changes (for one commit)

git reset HEAD-1

#### Case3: commited changes (for many commits)

git reset <commit Hash>

git reset --hard <commit Hash>

### to Initialize

git init



## Most Importent commands

git init

git branch -M main

git add .

git commit -m "all files Added"

>>> git remote # what's our remote 
>>> git remote -v # some more info 


>>> git push origin main / master 

>>> git push -u origin main