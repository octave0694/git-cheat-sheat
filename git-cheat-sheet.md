# GodOfBinary's ![git-48](https://user-images.githubusercontent.com/9167445/187039273-6d5474fb-f00e-4ed5-bf89-59f95cf269ce.png) cheat-sheet 

icon from [icons8](https://icons8.fr)

The purpose of this document is to reference some git usefull commands and serve as cheat-sheet. 
It save me from dealing with long searches amoung documentation pages.
This document will be update frequently to add new ✨Tips✨

### A simple diagram that shows how git works
![how-git-work](https://user-images.githubusercontent.com/9167445/187041457-f2824f67-59a0-4407-9d2c-aacc8ae3028d.png)

### How to install git
Click the link bellow for full git installation tutorial.
[How to install git](https://github.com/git-guides/install-git)

### 🪄 Check git version 🪄
`git --version`

### 🪄 Git Configuration 🪄
For more details about git configuration, check the [official documentation](https://git-scm.com/docs/git-config).

##### Git config
`git config --list` get current git global configuration.  
`git config --local -l` get the configuration values of the current git repository.  This configuration can also be found and updated in the file .git/config.  
Change some global configuration.  
`git config --global user.name "myName"`  
`git config --global user.email "hello@email.com"`  
`git config --global color.ui auto`  

### 🪄 Repository 🪄
For more details about repository initialization, check the [official documentation](https://git-scm.com/docs/git-init).

##### Git init
`git init` initialize a new local repository.  
`git init -b [branch-name]` initialize a new local repository with the initial branch name.  

### 🪄 Staging zone 🪄
For more details, check the official documentation links bellow:
[git status](https://git-scm.com/docs/git-status)  
[git add](https://git-scm.com/docs/git-add)  
[git diff](https://git-scm.com/docs/git-diff)  
[git restore](https://git-scm.com/docs/git-restore)  

##### Git status
`git status` show the current files on the working directory.  
`git status -s` show the working tree in short format description.  

##### Git add
`git add .` add all files from the working directory (untracked files) to the staging zone.  
`git add [file-name] [...]` add all specified files from the working directory to the staging zone.  
`git add -A` add every single file within the working repository to the staging zone.  

##### Git rm
`git rm --cached [file-name]` remove file from the staging zone and put it back to the working directory (untracked files).  
`git rm -r --cached .` untrack all the files from the staging zone.  

##### Git diff
`git diff` show changes between a commit and the working directory.  

##### Git restore
`git restore [file-name]` restore file to the state of the last commit.  

### 🪄 Save point/Snapshot 🪄
For more details about git commit, check the [offcial documentation](https://git-scm.com/docs/git-commit).

##### Git commit
`git commit -m "commit message"` make a commit with a specified message.  
`git commit --amend -m "new commit message` change the message of the previous commit.  

### 🪄 Log history 🪄
For more details, check the official documentation links bellow:
[git log](https://git-scm.com/docs/git-log)
[git show](https://git-scm.com/docs/git-show)

##### Git log and show
`git log` show the commits history of the repository.  
`git log --oneline` show the commits history in pretty mode (one line for each commit).  

##### Git show
`git show [commit-hash]` show details about a specified commit.  

### 🪄 Sync with remote repository 🪄
For more details, check the official documentation links bellow:
[git remote](https://git-scm.com/docs/git-remote)  
[git push](https://git-scm.com/docs/git-push)  
[git pull](https://git-scm.com/docs/git-pull)

##### Connect with SSH key
Check [this link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) for more details about how to use git with ssh key connection.  

##### Git remote
`git remote add [repo-name] [repo-url]` add a remote repository to synchronize with.

##### Git push
`git push -u [remote-repo-name] [branch-name]` push the local branch to the remote repository and start tracking to this branch.  
`git push -u [repo-name] [branch-name]` push a newly created branch to the remote server repository and set tracking for that branch. (A simple `git push` on a newly created local branch won't work).  

##### Git pull
`git pull` get the latest changes from the remote server.

### 🪄 Branching 🪄
For more details, check the official documentation links bellow:  
[git-branch](https://git-scm.com/docs/git-branch)  
[git checkout](https://git-scm.com/docs/git-checkout)  

##### Git branch
`git branch` list all branches in the local repository, and show the current branch you are working on.   
`git branch -r` list all branches from the remote server.   
`git branch -a` list both local and remote branches.  
`git branch -M [branch-name]` force rename the current branch.  
`git branch [branch-name]` create a new branch in local repository.  
`git branch -d [branch-name]` delete a fully merged branch.  
`git branch -D [branch-name]` force delete a branch even if it's not merged.

##### Git checkout
`git checkout [branch-name]` switch to a branch.  
`git checkout -` switch to the previous branch.  
`git checkout -b [branch-name]` create a new branch and checkout on this branch. 

##### Git merge
`git merge [branch-name]` merge changes from another branch into the current branch.  
``

