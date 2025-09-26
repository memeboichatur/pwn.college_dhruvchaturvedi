# GitHub Commands : 

***repository*** -where we store code 
we can create branches to a main file, which are copies of the main code for us to play with 
if needed, we can then merge a branch to the main file

a few git commands : 

``` 
git init
git add
git commit -m "commit message"
git branch -M main
git remote add origin <GitHub link>
git push -u origin main

git checkout -b my-new-branch
git add
git commit -m "new branch"
git push -u origin my-new-branch 
```



------
How to push a folder to github -->
1. Staging
2. Committing 
3. Pushing

***Staging*** - Selecting the files we need to push
use the command to add all files 
``` git add . ``` 
to add a specific file, use 
``` git add <path> ```

***Committing*** - Save your staged changes into your local repository's history with a descriptive message. This is called a commit.Your commit message should briefly explain what you changed.
 
use the following command :

``` git commit -m "<description here>" ```

***Pushing*** - Upload your new commit(s) from your local computer to your remote repository on GitHub. This is called pushing.
You'll need to specify the remote name (usually origin) and the branch name (commonly main or master).

```git push origin main ``` 



