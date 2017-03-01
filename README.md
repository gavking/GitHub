# Getting starter with GitHub
Checkout this Repo Wiki for further information on how to get started with GitHub

## Basics

`git`  //lists Git commands  
`git command --help`  //opens the manual for the command

General workflow is:  
* Clone the remote repo to make a local copy
* Change to new directory
* [optional] Make a new branch
* [optional] Switch to new branch 
* Make edits
* Add the changes
* Commit the changes
* Push changes to (remote) repo
* [optional] Merge branches

## Copying (cloning) a remote repo 

* `git clone URL`  //get the URL from GitHub repo home page

## Starting a local repo

* `git init`  //initialize a new git repo in the current directory 

## Adding files to be tracked

* `git add filename.ext`  //adds a single file to commit
* `git add .` or `git add -A` //adds all files in current directory to commit

## Commit tracked changes

* `git commit`  //opens a Vim session to add a long description for the commit
* `git commit -m "message_text"`  // combines commit changes and giving a simple description
* `git status`  //shows currently tracked changes that can be committed

## Pushing changes to repo
* `git push`

## Pull down the latest repo changes
* `git pull`

## Creating  and Working in Branches - Master is also a branch!

* `git branch branch_name`  //creates a branch
* `git checkout branch_name`  //switch to using branch
* Make edits, add them to tracking and commit
* `git push --set-upstream origin branch_name` //push new branch to remote repo
* `git checkout master`  //switch back to master
* `git branch`  //show all branches and highlights current working branch

## Merge branches

* `git checkout master`  //switch back to master if in a branch
* `git merge branch_name` //merge the branch with local master
* `git push`  // push the merge to the (remote) repo

## View contents of a branch

* `git ls-tree branch_name` //lists contents of branch

## Add existing project to a repo

* Create new repo in github.com
* Create a folder to hold the repo and cd into it
* git init   //initialize the local directory as a Git repo
* git add -A  //Stages all files in folder for commit, use "git reset HEAD your-file" to unstage a file
* git commit -m "message"  //commits tracked changes and preps them to be pushed to github 
* git remote add origin "Repo URL from github"  //sets the new remote
* git remote -v //verifies the new remote URL
* git push -u origin branch  //pushes changes to github to selected branch

