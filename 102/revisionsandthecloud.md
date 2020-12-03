[Main](https://amberfalbo.github.io/learning-journal/)


# Revisions and the Cloud

# What is Git?
Git is a Distributed Version Control System (DVCS) that stores dat in a file system made up of save from your projects mostly from your local computer.

#### but first...
* a Distributed Version Control system addresses the Centralized Version Control System (CVS) and if that went down then collaborators couldn't collab. Luckliy to prevent this type of catastrophic loss, a DVCS allows clients to create mirrored repositories, so if you lose any information then it can be recovered.
* We are using VScode as the DVCS. 
* Contralized Version Control System (CVCS) helped fill the need for collaboration with a developer team on a single fire or a set of files.
* and many many years ago there was just Local Version Control (VCS) which programmers created so they could access one database on your hard disk that stored changes to files.

## **Back to Git**
Git mostly relies on local operations because most necessay information can be found in local resources. Every single change appled to any file or directory is tracked by Git. And, as the **gatekeeper**, Git will always detect file corruption or loss of informaion in transit. 
* **Git can reside in thre main states: committed, modified and staged.**
- Committed - Data is securly stored in a local database.
- Modified - File has been changed but not committed to the database.
- Staged - Flagged a file's changed version to be committed in the next snapshot (save/commit)

## now the fun stuff! **cheat codes**

**Cloning** - You can creat a copy of an already existing Git repository by using the clone command with the repository's URL

```
git clone https://github./test
```

## **ACP** - add - commit - push


Code | Outcome
------------ | ------------
git status | Determins the state of the files. This indicates which branch you're working on, if files have been tracked or modified.
git add . | Tracks all filed in a repository, after using then files are tracked and staged for committing.
git commit -m "made change x,y,z" | Commits staged files and also records a message along with it for yourself and records.
git push origin master | This command pushes changes from the local "master" branch to the  remote repository named "origin". **For cloned repositories, Git will automatically give the name "origin" to the server from which you cloned and the name "master" to your local repository.**

**If you changed anything in GitHub instead of in your DVCS (in this case VScode) even if it ws just a theme then you need the use this commend to reconnect**
*This will bring it back to being synced in other words!*

```
git pull origin master
```




