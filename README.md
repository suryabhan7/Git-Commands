# GitCommands
Useful git command for daily use

### Getting started
 - git init
 - git status
 - git add . (add all file to staging area)
 - git reset FILE_NAME.extension  (Unstage file froms staging area)
 - git commit -m "meaningful comment"
 - git branch -M master  (Create master branch)
 - git remote add origin https://github.com/sadabnepal/GitCommands.git  (add remote url to local)
 - git push -u origin master  (push newly created master branch to remote)
 - git pull (pull changes from remote to local)


 ### Show commit logs
  - git log --stat
  - git log --oneline --graph --decorate --all
  
 ### working with tag
  - git tag -a v0.1 -m "meaningful comment" COMMIT_ID  (creates tag locally)
  - git push --tags (push all created tags to remote)


### Git config
 - git config --list  (view all config setting)
 - git config --global user.name "Your name"
 - git config --global user.email "yourname@provider.com"
 
### Local and remote repp
 - git remote -v (list all linked remote repo)
 - git remote set-url origin repo-url  (set new remote repo)
 
### Branches
 - git branch
 - git checkout branchname
 - git branch --merged (check if any branch merged with current)
 - git checkout -b dev (create new branch and switch to it)
 - git branch -d dev   (Delelet local branch)
 - git branch -D dev   (Delelet local branch forcefully)
 - git push --delete origin dev  (Delete remote branch)
 
### Revert commit
 - git revert commit_id

### Changes in file
- git diff  (difference in file)

### Stash
- git stash
- git stash list
- git stash apply stash@{0}
- git stash pop entryIndex  ((apply and delete)
- git stash apply entryIndex 
- git stash drop entryIndex  (delete)
- git stash clean

### Create alias
- git config --global alias.am "!git add -A && git commit -m"
- git am "new message"  (will do samething as above two command using am alias)
- git config --global --unset alias.am (unset alias created in config file)
 
