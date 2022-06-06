To perform a simple merge into a local branch  
`git checkout main`  
`git merge bugfix`  
This will merge bugfix into main


### Conflicts
If you run into conflicts, as below:
```
<<<<<<< HEAD
printf "The answer is %d" $c
=======
echo $c
>>>>>>> bugfix
```  
The <<< HEAD denotes the changes in HEAD (local change, in relation to the checked out branch)  
The === is a separator  
The >>> bugfix is the conflicted line in the bugfix branch (remote change in relation to the checkout branch)  

To fix the conflict, remove the code that you don't want and then perform an add/commit

To abort a merge  
`git merge --abort`
