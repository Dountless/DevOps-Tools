
# Git Branches

Lets say a new developer joins the project and want to add new story(file). we dont want to developer to directly make changes to our production code but instead give them a seperated version where they can change code and commit to until their work is done.
- The seperate version that give developer called Branches.
- A branch is basically a pointer to the last commits.
- master or main is a default Branches.

![image](https://user-images.githubusercontent.com/98619865/158058441-d5eadb67-e223-4f1a-a3bd-96753b95d06e.png)## command 

- *create a new branch*

       git branch feature

- *switch to an exiting branch*

      git checkout feature 

- *create a new branch and switch to it* 
      
       git checkout -b max 

- *delete a branch*
    
       git branch -d max 


- *list all  branches.* 
 
       git branch 


## Head
- A head is a where you are right now in the git repo. 
- the head point to the last commit in the branch that you are currently on. 
- where you switch branch the head moves with you.

## Merging branch 

-  we can merge branch with  a `git merge` command.
- git merge command receives the name of the branch that. we want to merge into our current branch.

- *Two types of merge git can perform*
    
    ### fast-forward 

    - this type of merge does not create a new commit but rather merge to commit on the branch that we are merging right into the current branch.

    ### no-fast forward 
    - rarely the case if we commit changes on the current branch that the branch we want to merge does not have git will perform a no-fast forward merge.
    - with a no-fast forward merge git creates a new

![image](https://user-images.githubusercontent.com/98619865/158058501-3afdbfd2-55d0-45a4-b619-ec1c9b92f03c.png)


### Working with multiple branch at the same time. 
there can be case where we want to work with multiple branch at the same time. for that we can use the worktree which allows us to access the different branch of the same application at the same time. 
 git worktree add [<options>] <path> [<commit-ish>]
 git worktree list [<options>]
 git worktree lock [<options>] <path>
 git worktree move <worktree> <new-path>
 git worktree prune [<options>]
 git worktree remove [<options>] <worktree>
 git worktree repair [<path>...]
 git worktree unlock <path>

