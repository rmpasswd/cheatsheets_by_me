### Branching
- `git switch anotherBranch` : switch  command saves the current un-commited changes to `.git` and  moves the HEAD to  'anotherBranch'
- `git checkout anotherBranch`
- `git checkout -b newBranch` : creates a changes to a  new branch, local of course.
- `git branch -d branchName` : deletes the branch & gives warning if branch contains changes that have not been marged with current branch/upstream branch. Use capital -D  to force delete.

### Upload & Sync Code
- 'origin' is a traditional name given to the remote link  using command `git  remote add origin URL`
- Lets say i named mine 'githubb'! `git remote add githubb git@github.com:rmpasswd/fullstack-blog-FastAPI.git ` Get the link from big '<> code' button. Now i'm mansplaining to myself -_- !
- `git push -u githubb newBranch` : All future `git push` command will push to newBranch  in remote(Github). The branch will be created if do not exists.
- `git push githubb local_branch:remote_branch`: Stateless, does not affect how the  next `git push` will behave.
- 

### Merging and 🍒 Picking

- **I made a bugfix/feature that should be merge to all other branches as well**
  - **Commit** the changes in current branch, get the commit ID
