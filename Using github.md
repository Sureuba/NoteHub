# **GitHub - Basics**
Connect your folder to the repo <br/>
Pull from the current one to your branch<br/>
Create your own branch so then you push it to your branch and then compare it to the main to ensure the changes can be made without any matching errors <br/>
For more on [editing style](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)

### Steps to SetUp
(1) Connect Local to Remote(GitHub):<br/>
git init = project root command<br/>
git remote add origin <Repo Location> = pushing local to the remote<br/>

(2) Create your branch:<br/>
git branch = lists out all the existing branches in a repo<br/>
git branch new-branch-name = create a new branch mirroring the commits on the active branch<br/>
git checkout new-branch-name = switches to the new branch - new branch will become the active one<br/>

### Steps to make changes to code (FOLLOW EVERY TIME):
Updating your Branch with the master: <br/>
git status = see changes made to local branch <br/>
git stash = stash changes in your local branch <br/>
git checkout master = go back to og <br/>
git pull origin master = update master branch to get all the remote branch changes <br/>

### Merging Branches (after you have made changes):
Changes made to the new branch can be merged into og branch <br/>
git add.<br/>
git commit -m “Message (what did you change)”<br/>
git checkout master = change back to og branch<br/>
git merge new-branch-name = merge branch into the master **need to be on the branch we are merging into<br/>

### Pushing to Remote Repo
**git push origin master(or main)** = push back to remote repo <br/>


### Cloning from Github to Local Repo (SSH):
**git clone <git@github.com:username/repository.git>** <br/>







****IGNORE****
**git status** = see changes made to local branch<br/>
**git stash** = stash changes in your local branch<br/>
**git checkout master** = go back to og<br/>
**git pull origin master** = update master branch to get all the remote branch changes<br/>
origin is the URL of the remote repo<br/>

**git checkout <new-branch-name>** = go back to working branch<br/>
**git status** = <br/>
**git merge master** = merge working branch to master<br/>
**git stash pop** = get changes from stash<br/>
**git status** = changes made earlier in the working directory<br/>
**git push origin <new-branch-name>** = push back to remote repo<br/>
 
