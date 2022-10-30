# Simple Git Hacks that do the Job
_____________________________________________________

#### => CHANGE COMMIT MESSAGE
* Change commit message if not pushed to remote repo yet(local repo)  
```git commit --amend -m "New commit message."```

* but if pushed to remote repo already:  
<<<<<<< HEAD
```git rebase -i HEAD~3```  
- the above code shows the last 3 commits and an interactive window opens up for you to edit the commit message.(if it is vim, you can use 'i' to insert and 'esc' to exit insert mode and ':wq' to save and quit)  

```git push --force origin main```  
- the above code pushes the changes to remote repo with the new commit message.  
_____________________________________________________

### => REMOVE FOLDER FROM A REMOTE REPO  
``` 
-- git rm -r --cached FOLDERNAME
-- git commit -m "FOLDERNAME removed from remote repo"
-- git push origin main

```
_____________________________________________________  

## => Undo a change with "git add ."  
-- `git reset`
=======
`git rebase -i HEAD~3` 
- the above code shows the last 3 commits and an interactive window opens up for you to edit the commit message.(if it is vim, you can use 'i' to insert and 'esc' to exit insert mode and ':wq' to save and quit)  
 `git push --force origin main`  
- the above code pushes the changes to remote repo with the new commit message.
>>>>>>> b5348b2d72f469ed1cd7c60ad1842f435dcee28f
