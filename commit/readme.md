Get the SHA1 ID of head and main  
```
git rev-parse head
git rev-parse main
```
Get the commit ID of 4 commits past
`git rev-parse main~4`

Go to a specific commit version  
`git checkout <SHA1_ID>`

To go back to main  
`git checkout main`


To amend a commit message  
`git commit --amend -m "Fixed commit" -m "Second paragraph" -m "Wall of text"`
