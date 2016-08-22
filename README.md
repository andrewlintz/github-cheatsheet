# github-cheatsheet

<strong>Setting up a New Repo on Github.</strong>

1) Create repo on Github  
  - check "initialize this repo w/ a readme.md 
  
2) copy the HTTPS clone URL  

3) in terminal navigate to the directory you want to clone the repository  

  - cd = change directory  
  - cd .. = navigate up in hierachy  
  - ls = shortlisting  
  - More commands found here = https://github.com/0nn0/ter)minal-mac-cheatsheet 
<br> </br>

<strong>Common Commands</stron>

$git clone [URL]  
  - makes a copy of the remote repo locally

$git pull   
  - pull will take anything from the remote repo and add it to your local repo. 

$git status  
  - shows the difference between the local repo & the remote 

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

<stron>Merge Conflicts</stron>
