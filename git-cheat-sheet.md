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
`git log` show the commit history of the repository.  

##### Git show
`git show [commit-hash]` show details about a specified commit.  

### 🪄 Sync with remote repository 🪄
For more details, check the official documentation links bellow:
[git remote](https://git-scm.com/docs/git-remote)
[git push](https://git-scm.com/docs/git-push)

##### Git remote
`git remote add [repo-name] [repo-url]` add a remote repository to synchronize with.
##### Git push
