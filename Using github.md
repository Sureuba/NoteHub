# **GitHub - Basics**
Connect your folder to the repo <br/>
Pull from the current one to your branch
Create your own branch so then you push it to your branch and then compare it to the main to ensure the changes can be made without any matching errors
For more on [editing style](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

### Steps to SetUp
(1) Connect Local to Remote(GitHub):
git init = project root command
git remote add origin <Repo Location> = pushing local to the remote

(2) Create your branch:
git branch = lists out all the existing branches in a repo
git branch new-branch-name = create a new branch mirroring the commits on the active branch
git checkout new-branch-name = switches to the new branch - new branch will become the active one

### Steps to make changes to code (FOLLOW EVERY TIME):
Updating your Branch with the master:
git status = see changes made to local branch
git stash = stash changes in your local branch
git checkout master = go back to og
git pull origin master = update master branch to get all the remote branch changes   

### Merging Branches (after you have made changes):
Changes made to the new branch can be merged into og branch
git add .
git commit -m “Message (what did you change)”
git checkout master = change back to og branch
git merge new-branch-name = merge branch into the master **need to be on the branch we are merging into

### Pushing to Remote Repo
git push origin master(or main) = push back to remote repo 


### Cloning from Github to Local Repo (SSH):
git clone git@github.com:username/repository.git







****IGNORE****
git status = see changes made to local branch
git stash = stash changes in your local branch
git checkout master = go back to og
git pull origin master = update master branch to get all the remote branch changes
origin is the URL of the remote repo

git checkout new-branch-name = go back to working branch
git status = 
git merge master = merge working branch to master
git stash pop = get changes from stash
git status = changes made earlier in the working directory
git push origin new-branch-name = push back to remote repo
 
