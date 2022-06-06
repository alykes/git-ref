To perform a simple merge into a local branch  
`git checkout main`  
`git merge bugfix`  
This will merge bugfix into main

To determine the common ancestor between two branches  
`git merge-base <BRANCH_1> <BRANCH_2>`


### Conflicts
If you run into conflicts, as below:
```
<<<<<<< HEAD
printf "The answer is %d" $c
=======
echo $c
>>>>>>> bugfix
```  
The `<<<<<<<` denotes changes in HEAD (local change, in relation to the checked out branch)  
The `=======` is a separator  
The `>>>>>>>` denotes the conflicted line in the "bugfix" branch (remote change in relation to the checkout branch)  
To fix the conflict, remove the code that you don't want and then perform an add/commit


### Fast Forward Merges  
Just means that the branch you are merging into doesn't have any commits, so it becomes an FF merge.
If git determines that the feature branch is a direct descendant of the branch being merged (eg main), then merge rolls up the local (main) branch to the remote (feature) branch. This is what is meant by a fast forward.


### Aborting a merge
To abort a merge  
`git merge --abort`  
_note:_ Generally because you’ve selected the wrong branch to merge into or you forgot to check out the correct branch to use as the starting point.
