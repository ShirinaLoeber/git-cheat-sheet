# Git Cheat Sheet
  
First `init` a new respository to work with:

```
$ git init REPO_NAME
$ cd REPO_NAME
```

***Note***  directories not tracked
To ignrore files add them to git ignrore

```
log/*.log
```

to add just parts to index use git add -p 

disaster recovery 
in case of deleted commits use it reflog and git cherry-pick to recover 

git cherry-pick lostcommitsha1

cleaned up after git gc ran 

git blame to see last change for each line 
use git show commitsha1 to get detailled inforamtion about this commit 

use git log --online --graph to get condensed log view 

branaches are essential for any git workflow 
git checkout -b branchname anlegen oder switchen 
git branch shows all branches 

add commits as usuall in your branch --> git rebase -interactive master to cleanup ur commits 
to merge branach into master use git merge --ff banchname (ff = fast forward)
squash by git merge --squash 
git reset --soft if u accidently added commits to master 
make sure to merge rebase master berfore mergeing ur branch into master 
