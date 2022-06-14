`git push origin master` -- Push the master branch to the remote named origin.  
`git push`               -- Push the current branch to the default remote-tracking branch set up by `git checkout` or `git push --set-upstream`.  
`git push --set-upstream origin new_branch` -- Create a remote-tracking branch to new_branch on the remote named origin.  
`git config --get-regexp branch`  -- List all Git configuration settings that have the word branch in the variable name.  
`git branch -d localbranch` -- Remove the local branch named localbranch.  
`git push origin :remotebranch` -- Remove the branch named remotebranch from the remote named origin.  


`git tag -a TAG_NAME -m TAG_MESSAGE SHA1ID` -- Create a tag to the SHA1ID with the name TAG_NAME and the message TAG_MESSAGE.  
`git push origin TAGNAME` --  Push the tag named TAGNAME to the remote named origin.  
`git push --tags` -- Push all tags to the default remote.  
`git push origin :TAGNAME` -- Delete the tag named TAGNAME on the remote named origin.  
`git tag -d TAGNAME` -- Remove the tag named TAGNAME from your local repository.  
