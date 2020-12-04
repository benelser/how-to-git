# how-to-git
## SSH
- Create key rename if desired
```
ssh-keygen
```
- Copy new key.pub to source control console (github)

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

## References 
- [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)
