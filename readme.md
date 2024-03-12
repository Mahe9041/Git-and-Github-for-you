# Git and GitHub Beginners Guide
#### Welcome to the Git and GitHub Beginners Guide! This repository is your one-stop resource for learning everything you need to know about Git and GitHub. Whether you're new to version control or looking to expand your knowledge, this guide will provide you with all the commands and instructions you need to get started.

## What is Git and GitHub ?
#### In present situaton when anyone want to contribute or two individuals wants to work on a same project remotly How can we do so?

#### For suppose we are working on a project and we did some changes that later we regret and want to revort back, How can we do so?

#### To do all that and along with it to solve many more problem there is a tool required. That requirement is fulfilled by __Git and GitHub__.

## Start with cmd command basics.
#### __ls__ : list files in the current directory. <br> __mkdir__ : make new directory.<br> __touch name.text__ : to create files.<br> __git status__ : Tracking changes. <br> __vim *file name*__ : to make changes to the file contents. <br> __cat *file name*__ : to see the file contents. <br> __git log__ : to check the log or complete history. <br> __rm -rf *file name*__ : to delete a file. <br> __git reset *hash id*__ : It is to reset ur changes till the id you give.(The hash id is not included and the above changes will be removed). <br>__git stash__ : it will same uncommited changes at backstage and give you new clean status to do experiment.<br>__git stash pop__ : To bring back the changes we kept back at backstage. <br>__git stash clean__ : The backstaged changes will be clenaed permanently. <br> __git remote -v__ : this will list out all the remote repo that the current file is connected.<br> __git checkout *branch name*__ : creating a new branch. <br> __git checkout *branch name*__ : the feature branch will be seletected. <br> __git merge *branch name*__ : to merge the branch with main. <br> __git clone *url*__ : copy the project of other. <br> __git remote add *url of the copy project*__ : to add the main repo form where we copied the project. <br> __git remote push *origin* -f__ : the -f is force push that is necessary because the commits on github is now not present in git. <br> __git fetch --all --prune__ : this will update our main branch according to the main project bramch from where we have forked.<br> __git reset --hard upstream/main__ : next dtep for the prev one. <br> __git push origin main__ : the next step of prev. <br> __git pull upstream__ : alternative of the above steps. <br> __git rebase -i *hash id*__ : this will give us the opertunity to merge all the commites into one. <br> 

## Starting with actuall work.
#### __Step 1__<br> git init : initiation of git. <br> we can see those files using __ls -a__ command
#### __Step 2__<br> git add __.__ / *fileName* : adding untracked files to the tracked before commit.
#### __Step 3__<br> git commit -m "some message" : to commit changes along with(-m) adding message.
#### __Step 4__<br> git remote add origin *github url* : to connect the local git to an github repo.
#### __Step 5__<br> git push origin master : to push the changes to the origin repo with branch master.

#### *To remove elements after add command and before commit command : __git restored --staged filename__*
#### *To see te complete history log of the git we use command : __Git log__*
##### *Note : .git file stores all the history and its hidden*

## Merge conflicts.
#### This occur when there are two pull requests made on the same line or bassically there are changes made on same line by two parties. This is resolved only by manually deleting which is required part and which is not.