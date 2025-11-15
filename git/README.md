### Git

1. Config tips
    - git config --global init.defaultBranch _BranchName_
    - git config --global alias.st status
    - git config --global alias.co checkout
    - git config --list  (_Show config_)
    - git config --global alias.ls "log --oneline --graph --decorate"
    
2. Create repo
    - git init
  
3. Index
    - git add .
    - git add _FileName_
    - git reset HEAD _FileName_  (_Delete file from index_)
    
4. Commit
    - git commit -m "desc of changes"  (_Make commit with desc_)
    
5. Branch
    - git branch  (_Show branches_)
    - git branch -m _BranchName_ (_Change name of current branch_)
    - git branch _BranchName_  (_Create branch_)
    - git checkout/switch _BranchName_  (_Switch to specific branch_)
    - git checkout -b _BranchName_  (_Create and switch to branch_)
    - git switch -c _BranchName_  (_Create and switch to branch_)
    - git branch -d _BranchName_  (_Delete branch_)
    
6. Restore/Reset/Revert
    - git restore _FileName_  (_To discard changes in the working directory_)
    - git checkout -- _FileName_  (_To discard changes in the working directory_)
    - git reset --soft HEAD~1  (_Delete commit and leave stagging_)
    - git reset --mixed HEAD~1  (_Delete commit and stagging, leave working directory_)
    - git reset --hard HEAD~1  (_Delete all and back to previous commit state_)
    - git revert _commit-hash_
    - git revert commit head  (_Revert last commit_)
    - git revert HEAD~2..HEAD  (_Revert two last commits_)
    
7. Merge/Rebase
    - git merge _BranchNameMergedInToCurrent_
    - git status  (_Show files which are in conflict_)
    - git merge --abort  (_Decline merge if smth went wrong_)
    
8. Log
    - git log
    - git log --oneline --graph --decorate
  
9. Diff
    - git diff
    
10. Remote

### Extra

1. git rev-parse --short HEAD >>> get current hash of commit
2. git rev-parse HEAD~ (HEAD~1) >>> get commit of first parent
3. git rev-parse HEAD~~ (HEAD~2) >>> get commit of second parent
4. git cat-file -p hash >>> show parents of commit
5. git rev-parse --short HEAD^2 >>> switch to another parent and get current commit aka HEAD
6. git rev-parse --short HEAD^2~ (HEAD^2^) >>> switch to another parent and get commit of 1st parent of its
7. git config
    - git config --unset user.***
    - git config --remove-section user 

### Python

1.  sudo apt update && sudo apt upgrade -y
2.  sudo add-apt-repository ppa:deadsnakes/ppa
3.  sudo apt update
4.  sudo apt install python3.x
5.  sudo apt install python3.x-dev python3.x-venv
6.  python3.x --version
7.  python3.x -m venv venv
8.  source myproject_env/bin/venv

