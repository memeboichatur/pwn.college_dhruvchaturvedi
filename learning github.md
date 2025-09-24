repository-where we store code 
we can create branches to a main file, which are copies of the main code for us to play with 
if needed, we can then merge a branch to the main file

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