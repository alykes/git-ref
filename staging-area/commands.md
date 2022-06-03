The staging area is used to add, delete, and rename files before they are committed into the repository.

Command to use are
- `git add` - add a file
  To initiate the staging individual lines for commit
  - `git add -p`
- `git rm` - remove a file  
  The following two lines achieve the exact same outcome:    
  - `rm a.file` and then `git rm a.file`
  - `git rm a.file`

- `git mv` - move or rename a file
  The following two lines achieve the exact same outcome:
  - `cp a.file new.file` -> `git rm a.file` ->  `git add new.file`
  - `git mv a.file new.file`  

- `git reset` - reset the staging
  Removes any files from the staging area
