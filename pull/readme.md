- Pull consists of two commands  
`git fetch` and `git merge FETCH_HEAD`

- Pull **only** commits that can be automatically fast forward merged locally  
`git pull --ff-only`
  - Configure git so that this is the default behaviour  
    `git config pull.ff only`
