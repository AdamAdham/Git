# Git Notes

## Cloning
**Decription**: Getting downloading the repository </br>
**Code**: git clone <ins>*link of repository*</ins>

## Status
**Decription**: Knowing which files are modified, not modified or untracked and not saved in a commit yet</br>
**Code**: git status

## Add
**Decription**: Track an untracked file </br>
**Code**: git add <ins>*name of file*</ins> / <ins>*.*</ins> </br>
**Notes**: . is to track all files in current directory

## Commiting
**Decription**: Saving the project LOCALLY </br>
**Code**: git commit -m "<ins>*Commit message*</ins>" -m "<ins>*Commit Description*</ins>" </br>
**Notes**: Commit message is mandatory, Commit descripton is optional, smth to do with what and why you committed

## Push
**Decription**: Uploading to remote repository where my project is hosted </br>
**Code**: git push origin master
**Notes**: Origin is the location of the git repository, master is the branch </br>
Shortcut: set smth called upstream so we use git push only by </br>
git push -u origin master

## SSH Keys
**Decription**:Used to prove you are the owner of github account/ Connect local machine to github account </br>
**Code**: ssh-keygen -t rsa -b 4096 -C "<ins>*Github email address*</ins>"
**Notes**: Code generates SSH key, -t: type of encryption, -b: strength of encryption </br>
There is a file for key and key.pub, key.pub is going to be uploaded to github interface (pub stands for public) </br>
Testkey is private (dont show to anyone) this key shows github you are the person that generated that public key </br>
Last step we just need to do is that let the local git cmd line know about the ssh key (search on internet)

## Start a git repository
**Decription**: create repository locally </br>
**Code**: git init </br>
**Notes**: Error will occur if we push (because was not cloned)

## Connect to a Repository on Github
**Decription**: To be able to push and pull </br>
**Code**: git remote add origin <ins>*link*</ins>

## Commiting
**Decription**: Saving the project LOCALLY </br>
**Code**: git commit -m "<ins>*Commit message*</ins>" -m "<ins>*Commit Description*</ins>"
**Notes**: Commit message is mandatory, Commit descripton is optional, smth to do with what and why you committed

## Undo Commit
**Decription**: Switch between branches </br>
**Code**: git reset HEAD~1 </br> / git reset <ins> *hash of commit*</ins> / git reset --hard <ins>*hash of commit*</ins>


**Notes**: 
1. HEAD: Last commit
2. ~1: Go back 1 commit
3. To hash of commit: Resets any change after that commit
4. Hard: Doesnt only unstage, it completely removes anything after that commit
## Log
**Decription**: List of commits in reverse chronological order </br>
**Code**: git log </br>

## Basic steps for uploading repository
1. git add .
2. git commit
3. git push
4. pull request (if a review or permission is needed)

## Branch
**Decription**: See branches of repository </br>
**Code**: git branch </br>
**Notes**: The one with astrisk is one currently on

## Checkout
**Decription**: Switch between branches </br>
**Code**: git checkout <ins>*name of branch*</ins> </br>

## Difference
**Decription**: See difference between current and specified branch </br>
**Code**: git diff <ins>*name of branch*</ins>/*nothing to see diff of last commit*

## Pull Request
**Decription**: Code from pulled in from another branch </br>
**Code**: Did on github </br>

## Pull
**Decription**: Get updated code from branch from remote repository </br>
**Code**: git checkout <ins>*name of branch*</ins> </br>

## Delete Branch
**Decription**: self explanatory </br>
**Code**: git branch -d <ins>*name of branch*</ins> </br>

## Merge Conflicts
**Decription**: When same branch is being changed at same time  </br>
**Code**: do on vs code/github

## Unstage
**Decription**: Make git not take into consuderation specified file</br>
**Code**: git reset <ins>*name of file*</ins> </br>

## Notes
When working on a branch every once in a while merge master to not get too far behind to not make the merge hard
