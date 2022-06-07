When cloning, only the active branch is cloned (The one that HEAD points to)  

Cloning locally  
`git clone <SOURCE_DIR> <DESTINATION_DIR>`  

Cloning from a remote  
`git clone <REMOTE_URL> <DESTINATION_DIR>`  
_Destination Dir can be ommitted when cloning from a remote_

To change the name from "origin"  
`git clone --origin <new_name> <repo_to_clone> <repo_destination>`  


Creating a bare directory with git clone  
`git clone --bare <repo> <REPO_NAME>.git` (added the .git to signify that this is a bare directory)
_Note:_ There is no working directory, this is can be known as the official copy of the repo.  
This is what is hosted on places like github.
