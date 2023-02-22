- ### Command to delete all (expect few) local branches 
  ```sh
  git branch | grep -v "master" | grep -v "dev" | grep -v "main" | xargs git branch -D
  ```
  - Get all branches (except for the master/dev/main) via `git branch | grep -v "master" | grep -v "dev" | grep -v "main"` command
  - Select every branch with `xargs` command
  - Delete branch with `xargs git branch -D`
