```bash
git branch -m <new_name>
git push origin :<old_name>
git push origin <new_name>:refs/heads/<new_name>

```

rename branch and update origin refs 

delete branch remote
git push <remote_name> --delete <branch_name> or $ git push <remote_name> :<branch_name>

or
$ git push -d origin branch_name  //remote
$ git branch -d branch_name //local

-d = delete only if it has been merged, 
-D = use force


find the branches that contain specific commit 
git name-rev <SHA>

git branch --contains <commit> (list all branches that contain this commit)

HEAD^ means the first parent of the tip of the current branch.





# Rename the local branch to the new name
git branch -m <old_name> <new_name>

# Delete the old branch on remote - where <remote> is, for example, origin
git push <remote> --delete <old_name>

# Or shorter way to delete remote branch [:]
git push <remote> :<old_name>

# Push the new branch to remote
git push <remote> <new_name>

# Reset the upstream branch for the new_name local branch
git push <remote> -u <new_name>