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
**Code**: git push -m "<ins>*Commit message*</ins>" -m "<ins>*Commit Description*</ins>"
**Notes**: Commit message is mandatory, Commit descripton is optional, smth to do with what and why you committed

## SSH Keys
**Decription**:Used to prove you are the owner of github account/ Connect local machine to github account </br>
**Code**: ssh-keygen -t rsa -b 4096 -C "<ins>*Github email address*</ins>"
**Notes**: Code generates SSH key, -t: type of encryption, -b: strength of encryption </br>
There is a file for key and key.pub, key.pub is going to be uploaded to github interface (pub stands for public) </br>
Testkey is private (dont show to anyone) this key shows github you are the person that generated that public key </br>
Last step we just need to do is that let the local git cmd line know about the ssh key (search on internet)

