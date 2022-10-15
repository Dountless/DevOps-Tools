

# Rebase

-  When we are rebasing branches. we are basically putting one branch on top of another one.

lets rebase the max branch on top of the master branch 

image



## difference between merge and rebase 

- In git each commit has unique identifier this unique identifier is `hash` . that can contains information about the commit and it possible for us to intract with specific commits.

- When we merge branches. these unique identifier won't be modified .` In other words we are not modified the history of our git commits when we are merging.`

But,

- when we  rebase branches however we are actually the commits from one branch to another. since we are creating new copied commits the hash is update.`In other words we are modified the git history when we are rebasing the branches.`

Note:-> for Rebashing it can be annoy . when you are working with a team because its not clear when certain branch get rebash because there is no merge commit.

![image](https://user-images.githubusercontent.com/98619865/158058764-9332fc5e-2ee6-40a2-822d-2bea20da04bd.png)

# Intractive Rebashing

It allow us to modified a git history.

ex:-> how can merge two or more commits.
 
- 
  
    git rebase -i HEAD~4


this command basically squash and meld commit 
- output that command show vi editor and leave first line and chose second and more for replace pick to squash.



# Cherry Picking

Cherry picking is the act of picking a commit from a branch and applying it to another. git cherry-pick can be useful for undoing changes. For example, say a commit is accidently made to the wrong branch. You can switch to the correct branch and cherry-pick the commit to where it should belong.

see:-> https://www.atlassian.com/git/tutorials/cherry-pick#:~:text=Cherry+picking+is+the+act,to+where+it+should+belong.

