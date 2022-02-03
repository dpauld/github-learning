# github-learning
https://stackoverflow.com/questions/7106012/download-a-single-folder-or-directory-from-a-github-repo

## Pushing or Adding new resources
```
git add .
git commit -m "your message"
git push 'remote_name' 'branch_name' => [eg: git push origin main]
```
## Removing a file
If you want to remove the file from the remote repo, first remove it from your project with --cache option and then push it:
```
git rm --cache /path/to/file
git commit -am "Remove file"
git push
```
## Reverting
```
git reset --hard <commidId> && git push --force
git revert HEAD~2
```
-------------- Worked -----------
```
git reflog
git checkout <commit id> // now you are in where you want but you cannot push from detached branch to master
manually copy and paste changes from detached branch to master or working branch
git reset --hard HEAD // if needed
git add ... > git commit ... > git push ...
```
--------------Undo the checkout------------
```
git checkout -
or
git checkout <branch_name>
```
