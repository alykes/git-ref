- Show the remote name  
`git remote`  

- Show more verbose information about remotes  
`git remote -v`   

- Show all branches (including remotes if they exist)  
`git branch --all`

- Renaming a remote  
`git remote rename <ORIGINAL_REMOTE_NAME> <NEW_REMOTE_NAME>`  
eg `git remote rename origin start`  

- Adding a second remote to a cloned repo  
`git remote add <NEW_REMOTE_NAME> <REPO_URL|REPO_DIRECTORY>`  
`git remote add remote-2 ../another_clone_of_the_same_repo`

- Setting a new remote location  
`git remote set-url <EXISITNG_REMOTE_NAME> <NEW_REMOTE_LOCATION_DIR|NEW_REMOTE_LOCATION_HTTPS>`  
`git remote set-url partner ../math.alykes`

- Adding multiple repos to a single remote  
`git remote set-url --add <EXISITING_REMOTE> <NEW_REMOTE_LOCATION_DIR|NEW_REMOTE_LOCATION_HTTPS>`  

- Removing a remote  
`git remote remove <REMOTE_NAME>`  
`git remote remove start`  

- Interrogating a remote  
`git ls-remote`  
`git ls-remote origin`  
`git ls-remote origin-2`

- Showing verbose information about a remote  
`git remote -v show origin`  

- To get more verbose network activity information wqhen issuing an `ls-remote`  
`GIT_TRACE_PACKET=1 git ls-remote`
