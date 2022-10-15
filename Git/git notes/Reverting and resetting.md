
# Reverting 

- The revert command helps you undo an exiting commit.

- it does not delete any data in this process instead rather git creates a new commit with the includes file reverted to their privious state.
- so, your version control history moves Forward while the state of your file move Backward.

                     git revert  `commit-id`


# Resetting

-  git reset is a powerful command that is used to undo local changes to the state of a Git repo.

- The git reset command is a complex and versatile tool for undoing changes. It has three primary forms of invocation. These forms correspond to command line arguments --soft, --mixed, --hard. The three arguments each correspond to Git's three internal state management mechanism's, The Commit Tree (HEAD), The Staging Index, and The Working Directory.

The default invocation of git reset has implicit arguments of --mixed and HEAD. This means executing git reset is equivalent to executing git reset --mixed HEAD. In this form HEAD is the specified commit. Instead of HEAD any Git SHA-1 commit hash can be used.

## --hard


- This is the most direct, DANGEROUS, and frequently used option. When passed --hard The Commit History ref pointers are updated to the specified commit. 
- Then,  Any previously pending changes to the Staging Index and the Working Directory gets reset to match the state of the Commit Tree. This means any pending work that was hanging out in the Staging Index and Working Directory will be lost.

- the commit will be reset without saving  all those  changes. file in commit now completely gone.

        git reset --hard HEAD~1
## --mixed

- This is the default operating mode. The ref pointers are updated. The Staging Index is reset to the state of the specified commit. Any changes that have been undone from the Staging Index are moved to the Working Directory. 

## --soft

- the reset command also receive the amount of commits that we want to reset 
 
        git reset --soft HEAD~1 


- after it recent a commit and added to  stage area now head point previous commit. you can see by type `git status`


![image](https://user-images.githubusercontent.com/98619865/158058846-2ff2c9dc-8cb0-4dd1-8fde-ff3a44761b72.png)



# git reflog 

- suppose, if you performed  a hard reset it seems like all this data gone forever. 
- well no need to panic  here is a `git reflog` command shows us all the actions that have been taken on your repo. this includes merges,reset,reverts basically any alternation.

- you can easily undo this by resetting HEAD based on the an the information that reflog  gives us

ex:->
-  you want to undo hard reset any reflog see state of before hard reset is that  `HEAD~(?)`.
- and perform git `reset --hard  (hash of bfore hard reset)`

