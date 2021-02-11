# Useful git commands

List of useful git commands with some context around each command.

## Setting up git
```git config --global user.name "first.last"```
```git config --global user.email "user@domain.com"```

* To set values for a specific project, drop --global
```git user.name "first.last"```
```git user.email "user@domain.com"```


## Listing variables
```git config --List```

* To list specific variables
```git config user.name``` 
```git config user.email```

## Help
```git help <config/commit/etc>```

## Initialising a new repo
Run the command from the directory you wish to host the new repo in
```git init```

## Set up a repo on github
Add the remote origin to the local repo, so that you can push/pull changes

```git remote add origin https://github.com/alykes/git-ref.git```

## Push changed up to the remote repo
```git push -u origin main```

## Status of the local repo in comparison to the origin/master
The results will let you know if there is anything to commit and what has and hasn't been staged.
```git status``
For a briefer response
```git status --short``` or ```git status -s```

## Add file(s) to the repo
* Add a single file
```git add <file.name>```
* Add multiple files
```git add .```

### Reminder Tip
When you *add* a file, it is in a _STAGED_ state
When you *commit* a file it is in the _COMMITED_ state

## Diff command
* To compare files STAGED (*add*ed) with the last commit snapshot
```git diff --staged```
* To tell git not to treat files as copies of one another
```git diff --staged --no-renames```

* To compare the difference in the working directory with what is STAGED (*add*ed)
```git diff```

## Commit changes
```git commit -m "A description of the changes made"```
* Shortcut to skip stages -a
```git commit -a -m "A description of the changes made"```

## Push changes
* Push locally commited changes up to the remote master
```git push origin master``` ```git push origin main```

## Log command
* view local commit history in reverse chronological order
```git log```
* Limit output, latest commit
```git log -1 ```
* shows commits in a single line format, good for summarising
```git log --oneline```
* Shows stats of each file modified and grouped by commit
```git log --stat```
* Shows a detailed view of each commit, including changes
```git log --patch```

## Remove files from the local repo
* To delete the file from disk and from the respo
```git rm <file.name>```
* To remove the file from the working directory but leave it on disk
```git rm --cached <file.name>```

## Renaming files
```git rn old.file.name new.file.name```

## Branches
* List Branches
```git branch```
* Create a new branch
``git branch new.branch```
* Create a new branch and checkout to it
``git checkout -b new.branch```

## Stash
* If you are switching branches and have uncommitted changed, stash them to save the working directory as WIP
``git stash```
* List the stash
``git stash list```
* Show a more detailed view of the files stashed
```git stash show```
* Put the changes back into your working directory
```git stash pop```

## Merge a branch
* from main or master (or wherever you want to merge into)
```git merge new.branch```
* Add a message and save
``git merge new.branch```
* If you receive an error about unrelated histories
```git merge master --allow-unrelated-histories```

## Reset
Moves commits from history back into the staging area or throw changes away, don't reset after a push to the remote origin as you could disrupt other peoples work flow
* Move commits back into the staging area
```git reset --soft <commit.id>```
* Move commits back into the working directory
```git reset --mixed <commit.id>``` OR ```git reset <commit.id>```
* Moves changes to the bin (also deletes changes in your working directory or staging directory)
```git reset --hard <commit.id>```

## Pull
```git pull``` or ```git pull --all```
