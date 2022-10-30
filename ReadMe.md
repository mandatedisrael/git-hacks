# Simple Git Hacks that do the Job
_____________________________________________________

#### CHANGE COMMIT MESSAGE
* Change commit message if not pushed to remote repo yet  
`git commit --amend -m "New commit message."`

* but if pushed to remote repo already:  
`git rebase -i HEAD~3` 
- the above code shows the last 3 commits and an interactive window opens up for you to edit the commit message.(if it is vim, you can use 'i' to insert and 'esc' to exit insert mode and ':wq' to save and quit)  
 `git push --force origin main`  
- the above code pushes the changes to remote repo with the new commit message.
