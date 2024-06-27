# GIT - Some commonly used commands

## What is GIT ?
 - GIT is a distributed version control system that is used to track changes in source code during software development.
 - It allows multiple developers to work on same codebase simultaneously.
 - It keeps  record of all the changes made to a codebase overtime.
## Different areas in git 
  - understanding different areas in git can be helpful in understanding the commands easily
![image of different areas in git](https://miro.medium.com/v2/resize:fit:1204/1*zpvd5fjZAFGsVAEsvMGKxA.png)

**working area** - this is the area where new files are added, old files are deleted and modify the existing files.

**staging area** - sometimes it is also called as index.this is the area where all the file changes are ready to commit to a local repo.

**local repo** - this is the area where you can find all the commited code.

**remote repo** - this is where all developers collaborate. remote simply means online or available over internet. 

## Some commonly used commands 

| command | description |
|:-------:|:------------|
| git --version | this command is ued to find the version of git in your system |
| git init | used to initialize a empty git repository |
| git config | - used to configure details like name, email etc  --global flag can be used to config the global details line name and email|
| git config --list | to find all configuration details |
| git add | used to stage the newly added or modified files into the staging area |
| git status | used to know which files are in staging area and which are not |
| git status --short | to gve status in compact way |
| git rm <filename> | to remove file from index and working area |
| git rm --cached <filename> | to remove file from indexx but not in working area |
| git commit -m 'message' | to commit the changes from index to local repo with a message describing why we are doing a commit |
| git commit --amend | to change the last commit message promptly from text editor |

## Branching related commands 

| command | description |
|:-------:|:------------|
| git branch | to list all the branches and shows current branch we are in with * symbol |
| git branch <branchName> | to create a branch from current branch |
| git branch -m [<oldBranchName>] <newBranchName> | to modify branch name if we dont mention oldBranchName the current branch name will get modified |
| git checkout <branchname or commit-hash> | allows to switch from different branches or versions of a repository |
| git checkout -b <branchName> | create and switch to new branch at the same time |

## some commands which are related to pushing or fetching the code from/to internet

| command | description | 
|:-------:|:------------|
| git fetch | used to download all the content from remote repository |
| git pull | used to fetch and merge the code from remote repository |
| git push | used to push the code from local repo to remote repository |

## Some useful resources
 - git cheatsheet [https://education.github.com/git-cheat-sheet-education.pdf](https://education.github.com/git-cheat-sheet-education.pdf)
 - official git documentation [https://git-scm.com/docs](https://git-scm.com/docs)
 - video tutorial [https://www.youtube.com/watch?v=RGOj5yH7evk&t=179s](https://www.youtube.com/watch?v=RGOj5yH7evk&t=179s)
