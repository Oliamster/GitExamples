But, instead of using a merge commit, rebasing re-writes the project history by creating brand new commits for each commit in the original branch.

``` bash
git checkout feature
git rebase master
```

is equivalent to: rebase feature onto master equivlent to integrate changes from master into feature.


Incorcorate the last  3 commit into new base e rebase of only the last 3 commits.
``` bash
git checkout feature
git rebase -i HEAD~3
```

```
git merge-base feature master 
find the best common ancestor, the best base in practice
```


By default, the git pull command performs a merge, but you can force it to integrate the remote branch with a rebase by passing it the --rebase option.
source: https://www.atlassian.com/git/tutorials/merging-vs-rebasing#conceptual-overview

git checkout feature
Git rebase develop 

in Visual Sudio  Target branch is the Develop branch Source is the current (feature)  branch 