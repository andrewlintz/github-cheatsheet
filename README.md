# github-cheatsheet

<strong>Common Commands</strong>

$git clone [URL]  
  - downloads a copy of the remote repo locally

$git pull   
  - downloads any changes made on the master remote repo and to update your local repo. 

$git status  
  - shows a summary of files differences between the local repo & the remote 

$git add [file name]  
  - queues that file to be ready to be committed to the remote repo.   

$git add .  
  - queues everything in the directory to be commited  

$git add -A  
  - queues all

$git commit -m "[your commit message]"  
  - means you are locking it it, it is committing to the change, and ready into what will be pushed, -m is the message.  

$git push   
  - going to take anything committed locally and add it to the remote repo.  
  
<br>  

<strong>Setting up a New Repo on Github.</strong>

1) Create repo on Github  
  - check "initialize this repo w/ a readme.md 
  
2) copy the HTTPS clone URL  

3) in terminal navigate to the directory you want to clone the repository  

  - cd = change directory  
  - cd .. = navigate up in hierachy  
  - ls = shortlisting  
  - More commands found here = https://github.com/0nn0/ter)minal-mac-cheatsheet 

<br>


<strong>Pushing up an existing local repo to a new github repo</strong>

$ git init

$ git add .  
  # Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
  
$ git commit -m "First commit"  
  # Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
  
$ git remote add origin remote repository URL  
  # Sets the new remote
  
$ git remote -v  
  # Verifies the new remote URL
  
$ git push -u origin master  
  # Pushes the changes in your local repository up to the remote repository you specified as the origin

<br>

<stron>Merge Conflicts</stron>

Manually revise the conflict, save file, enter 
$ git add -A
$ git commit"    [with no comment]
$ git push

If ever in the strange zone after commiting with out message:
hit esc:wq



Pull Requests

$ git pull  
$ git branch  
- lists all the branches

$ git branch [give a name for branch]  
- makes a complete copy of the Master for you to work on.  

$ git checkout [specify which branch]  
- switches you to whatever banch you want to switch to.

Make changes and develop you code.  
$ git add -A  
$ git commit -m "message"  
- now it's ready for you make a pull request, but before you do that, go back to master and make sure that the code hasn't change since your last pull.  
$ git checkout master  
- switches back to master  
$ git pull
- to update to current code  
$ git checkout [name of the branch you just completed updating.  
$ git merge master
- will take all the changes & update of master  and try to merge into [designated branch]

Merge conflitch  
- go back to file and manually resolve the differences.  
$ git status  
$ git add -A  
$ git commit -m "message"  
$ git push   
- now the branch is pushed up to Github repo  
- review and comment.  
- the merge



