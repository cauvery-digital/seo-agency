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



## Quick setup — if you’ve done this kind of thing before

or	

https://github.com/cauvery-digital/seo-agency.git


Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

# …or create a new repository on the command line


echo "# seo-agency" >> README.md

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin https://github.com/cauvery-digital/seo-agency.git

git push -u origin main

# …or push an existing repository from the command line
git remote add origin https://github.com/cauvery-digital/seo-agency.git
git branch -M main
git push -u origin main