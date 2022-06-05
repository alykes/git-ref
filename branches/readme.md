Branch naming conventions  
`git check-ref-format --help`

Checking branches  
`git branch`  

Checking the history of your branch moves  
`git reflognano`

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

Checking the tip (most current) commit_id on a branch  
`git branch -v`

Deleting a branch  
`git branch -d <BRANCH_NAME>`
