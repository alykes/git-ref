### git configuration variables and order of precedence  

| Scope        | Description  | Precedence (1 Highest)|
|--------------|--------------|--|
| local        | Current Repo |1|
| global       | All repos you have control over  |2|
| system       | System-Wide  |3|

- #### git config scope listings
To get a listing of each you can run the commands below  
`git config --local --list`  (You must be in a repo to run the command with the local switch)  
`git config --global --list`    
`git config --system --list`  

- #### git config naming conventions
Some examples on the naming system below  
|section|sub-section|key|value|entry|
|-|-|-|-|-|
|user||name|alykes|user.name=alykes|
|remote|origin|url|https://github.com/alykes/git-ref.git|remote.origin.url=https://github.com/alykes/git-ref.git|

_Note:_ section + key can be referred to as the **Name**  

- #### git config changes
To preview a configuration change before you apply it, us the `-c` argument  
`git -c log.date=relative log -n 2`  

To save a value in git config  
`git config --local log.date relative`  
To unset a value in git config  
`git config --local --unset log.date`  
