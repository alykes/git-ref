Tagging commits can be achieved by issueing the following command  
`git tag <TAG_NAME> -m "some message about the commit" <COMMIT_ID>`  

Once the commit is tagged, use the tag instead of the commit id

Push all local tags to a remote  
`git push --tags`  

Tag a commit, 2 back  
`git tag -a two_back -m "Two behind the HEAD" HEAD^^`  
Push the change to the remote  
`git push origin two_back`  

Delete a local tag  
`git tag -d two_back`  

Delete a remote tag  
`git push origin :two_back`
