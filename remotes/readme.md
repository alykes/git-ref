Show the remote name  
`git remote`  

Show more verbose information about remotes  
`git remote -v`   

Show all branches (including remotes if they exist)  
`git branch --all`

Renaming a remote  
`git remote rename <ORIGINAL_REMOTE_NAME> <NEW_REMOTE_NAME>`  
eg `git remote rename origin start`  

Adding a second remote to a cloned repo  
`git remote add <NEW_REMOTE_NAME> <REPO_URL|REPO_DIRECTORY>`  
`git remote add remote-2 ../another_clone_of_the_same_repo`
