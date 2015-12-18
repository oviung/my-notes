## Commands

### Initial settings
* `git config --global user.name [Your Name]` - add your GitHub name (not username)
* `git config --global user.email [your@email.ex]` - add your GitHub email
* `git config --global user.username [USERNAME]` - add your GitHub username
* `git config user.[name/email/username]` - view a specific setting like name, email or username
* `git config --list` - show all config settings

Store the username & password for working with HTTPS:  
https://help.github.com/articles/caching-your-github-password-in-git/#platform-linux  
Linux:  
1. `git config --global credential.helper cache` -  set git to use the credential memory cache  
2. `git config --global credential.helper 'cache --timeout=[n]'` - git will cache  for [n] seconds

### Local
* `git reset [FILE]` - remove file from staging area
* `git diff` - show changes before staging
* `git branch` - list branches
* `git branch [BRANCH_NAME]` - creat a branch
* `git checkout [BRANCH_NAME]` - switch to another branch
* `git branch -d [BRANCH_NAME]` - delete local branch
* `git push origin --delete [BRANCH_NAME]` - delete remote branch
* `git show HEAD~[n]` - show changes at a specific commit ([n] = integer number)
* `git log` - show commit history

### Remote
* `git remote add origin [REMOTE_REPO_URL]` - add remote URL to the local repository
    * `git remote set-url origin [REMOTE_REPO_URL]` - if URL is already set and you want to change it
* `git remote -v` - show remote name (it's origin by default)
* `git push origin [BRANCH_NAME]` - push branch to remote
* `git clone [REMOTE_URL]` - create local copy of remote repository
* `git remote add upstream [ORIGINAL_REPO_URL]` - link original repo from where you forked to pull changes
* `git pull [REMOTE_NAME/origin] [REMOTE_BRANCH]` - pull changes from forked remote
* `git pull upstream [BRANCH_NAME]` - pull branch from original repo to local
* `git fetch` - view changes before pulling
* `git merge origin/master` - done after `fetch` to bring the changes from the remote master to local

### Merge branches
1. Checkout to the brench you want to merge into (ex: master)
2. `git merge [BRANCH_TO_MERGE]` - merge the branch you want with master

### Reverting changes
* `git checkout SHA/HEAD-[n] [filename]` - reset the state of the file to a specific commit (if it existed back then)  
The SHA only needs the first 7 characters (list commits with `git log`). Alternatively you can use HEAD  
HEAD = HEAD~0  
The index of HEAD starts from 0 (this being the last commit)  
To go back more commits use HEAD~[n]
* `git reset SHA/HEAD~[n]` - reset the commit history back to a desired commit  
OPTIONS:  
`--soft` - won't remove the changes to the files  
`--hard` - removes the changes done after the commit you want to reset to
