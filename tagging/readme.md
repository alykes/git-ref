Tagging commits can be achieved by issueing the following command  
`git tag <TAG_NAME> -m "some message about the commit" <COMMIT_ID>`  

Once the commit is tagged, use the tag instead of the commit id

Tag a commit, 2 back  
`git tag -a two_back -m "Two behind the HEAD" HEAD^^`  
