Show the log history  
`git log`

`git log --oneline`

To show more detailed information about file changes  
`git log --stat`

To show the parents of each commit  
`git log --parents`  
To make the output more readable  
`git log --parents-abbrev-commit`

To show all patches of each file during a commit  
`git log --patch`  
`git log --patch --stat`  
`git log --patch-with-stat`  

To view commits that pertain to a specific file  
`git log --oneline specific.file`  

To view branches and commits  
`git log --graph --decorate --pretty=oneline --all --abbrev-commit` 
alternatively, use `gitk` to get a visual presenation of the same.  

List branches and/or tags only  
`git log --oneline --decorate --simplify-by-decoration --all`

List the last change  
`git log -1`  
`git log max-count=1`
