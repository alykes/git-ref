Branch naming conventions  
`git check-ref-format --help`

Listing branches  
`git branch`  
`git branch --all`  
`git log --simplify-by-decoration --all --oneline`  
`git branch --column` 

Checking the history of your branch moves  
`git reflog`  
`git reflog <branch>`

Creating a branch  
`git branch dev`  
Creating a branch at specific commit point
`git branch <NEW_BRANCH_NAME> <COMMIT_ID|EXISTING_BRANCH_NAME|TAG>`

Creating a branch and switching to it immediately  
`git checkout -b <NEW_BRANCH_NAME>`  
Creating a branch from another branch and checking it out immediately  
`git checkout -b <NEW_BRANCH_NAME> <EXISTING_BRANCH_NAME|TAG>`

Renaming a branch  
`git --move <BRANCH_NAME> <NEW_BRANCH_NAME>`  

Switching to a branch  
`git checkout <BRANCH_NAME>`  
Switching to a branch and throwing away changes  
`git checkout -f main`  

Checking the tip (most current) commit_id on a branch  
`git branch -v`

Deleting a branch  
`git branch -d <BRANCH_NAME>`  
Deleting a remote branch (BE CAREFUL WITH THIS COMMAND)
`git push origin <src>:<dst>`  
`git push origin :<BRANCH_NAME>`  

Find a branch name from a commit  
`git name-rev <COMMIT_ID>`  
`git branch -r --contains <COMMIT_ID>`  
`git branch --contains <COMMIT_ID>`  
