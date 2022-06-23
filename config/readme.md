git configuration variables have orders of precedence  

| Scope        | Description  | Precedence (1 Highest)|
|--------------|--------------|--|
| local        | Current Repo |1|
| global       | All repos you have control over  |2|
| system       | System-Wide  |3|

To get a listing of each you can run the commands below  
`git config --local --list`  (You must be in a repo to run the command with the local switch)  
`git config --global --list`    
`git config --system --list`  

Some examples on the naming system below
|section|sub-section|key|value|entry|
|-|-|-|-|-|
|user||name|alykes|user.name=alykes|
|remote|origin|url|https://github.com/alykes/git-ref.git|remote.origin.url=https://github.com/alykes/git-ref.git|

_Note:_ section + key can be referred to as the **Name**  

To preview a configuration change before you apply it, us the `-c` argument  
`git -c log.date=relative log -n 2`  
