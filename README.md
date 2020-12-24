# how-to-git
## SSH
- Create key rename if desired
```
ssh-keygen
```
- Copy new key.pub to source control console (github)

## Clone repo With SSH Specific Key
```
GIT_SSH_COMMAND="ssh -i ~/.ssh/<PRIVATE_KEY_RSA> -F /dev/null" git clone <GIT_SSH_URI>
```

## Set core.sshCommand in Git config
```bash
# While in directory 
git config core.sshCommand "ssh -i ~/.ssh/<PRIVATE_KEY_RSA> -F /dev/null"
# Make changes 
git add .
git commit -m "new change"
git push
```

## Pull/Merge Request
1. git clone desired repo
```
git clone git@github.com:SOMEAWESOMEREPO.git
```
2. Change Directory
```
cd SOMEAWESOMEREPO
```
3. Checkout new Local Branch
```
git checkout -b mycool-testing-branch
```
4. Make Changes
```
touch SOMENEWFILE
```
5. Add/Commit Changes
```
git add .
git commit -m "my sweet changes"
```
6. Push back to orgin 
```
git push origin mycool-testing-branch
```
7. Create Pull Request
Go to the browser UI and visit the repo and create pull request from pushes


## Create new Repo
1. Create repo in UI do not initialize or create readme.md
2. Back on the cli in project folder 
```bash
git init
git add . 
git commit -m "First commit"
git remote add origin remote <REPOURL>
git remote -v 
git push -u origin master
```

## References 
- [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)
