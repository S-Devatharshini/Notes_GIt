# An introduction to Git and Github
## Git

It is free and open source "CONTROL SYSTEM"

## Version Control

It is the process of managing the changes to the documents,computer programs,large web-sites and other collections of information.

## Git Commands

| **S.NO**      | **Command**       | **Use**                                       |
|:-------------:|:-----------------:|:----------------------------------------------|
| 1             | clone             | Bring repository that is hosted somewhere     |
| 2             | add               | Track the files and changes in Git            |
| 3             | commit            | Save your files in Git                        |
| 4             | push              | Upload Git commands to remote repository      |
| 5             | pull              | Download changes from remote repository       |

## Cloning

Cloning can be done by executing the "Clone command".

    git clone link

## Steps to push project from local machine to remote repository
#### (When the repository is intialized)

### 1) Cloning

First cloning has to done.

    git clone link

### 2) Check the status

Execute the status command to view the status of the repository.

    git status

### 3) Track the changes

The following command is executed to track all the changes.

    git add filename

### 4) Commit the changes

Next, inorder to save the changes execute the commit command.

    git commit -m "message" -m "message description"

### 5) Push and Upstreaming

The push command is executed to to push the changes from local machine to the repository.

    git push -u origin main

## Steps to push project from local machine to remote repository
#### (When the repository is not intialized)

### 1) Initialize the repository 

Intialization can be done by executing 

    git init

### 2) Check the status

The status of the repository can be known by executing

    git status

### 3) Commit the changes 

The changes can be commited by executing

    git add . 
    git commit -m " message" -m " message description"

### 4) Creating a repository

A empty repository is created in github and its url is copied(either http or ssh).

### 5) Add the origin

Origin to the repository is done by executing 

    git remote add origin link

### 6) Push and Upstreaming

Finally push the repository to remote using

    git push -u origin master

## GIT Branching

### 1) Current Branch

First check the current branch you are working on by executing

    git branch

##### Note: All the branches will be displayed and the current branch is highlighted.

### 2) Create a feature branch

Create a feature branch of the current master repository using

    git checkout -b branchname

### 3) Track and Commit the changes

Track and commit the changes which are done in the feature branch using 

    git add .
    it commit -m " message" -m " message description"

## GIT Merging

Merging is done to commit the changes which are done in feature branch to its respective master branch

### 1) Switch to Master Branch

After commiting changes in feature branch switch to master branch by executing

    git checkout master

### 2) Find the difference

Inorder to find the difference between the master and feature branch execute the command

    git diff branchname

### 3) Push and Upstreaming 

Pushing and upstreaming can be done by executing the following commands

    git status
    git push --set-upstream origin branchname
    git push
    git push -u origin branchname

### 4) Pull request

Inorder to reflect the changes to master branch execute the pull command

    git checkout master
    git pull

### 5) Delete the feature branch 

Once merging is done the feature branch is deleted to avoid redudancy and conflict.

    git branch -d branchname

## Undoing in git

It is used to undo the unnecessary commits.

### 1) Eliminate unnecessary commits

Unecessary commits are eliminated and resetted by executing

    git reset filename
    git reset HEAD`~1

##### Note:HEAD is a pointer to the most recent commit

### 2) Display the commits 

All the commits can be listed in chronological order by executing the command

    git log

## GIT Forking 

- A fork is a copy of a repository that you manage. 
- Forks let you make changes to a project without affecting the original repository. 
- You can fetch updates from or submit changes to the original repository with pull requests.