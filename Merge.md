# Merge develop into feature

``` bash
git merge feature master 
```


Equivalent to: 

``` bash
git checkout  feature 
git merge master
```

# Merge feature into develop


``` bash
git merge develop feature  
```

Equivalent to:

``` bash
git checkout  develop 
git merge feature
```

our => ignore changes from all others branches an prefer "our" changes in case of conflicts


in Visual Studio, when I do  git merge --merge squash, in the tool for resolving conflicts 
Ours = MyBranch in wich I want to merge the source branch, so the target branch 
Thiere is the source.