 # Fetching and merging

- You and your team have changed in remote repo and mergeed in the master branch then now local repo is not automatically aware of these changes. in order to have changes into local repo by use `git fetch` command 

          git fetch origin master 

- In order to update the origin master branch in  our local repo . we can merge origin master into the local master branch.

## Pulling

Instaed of individually fetching and then merging. we can also pull the origin master branch with `git pull` command

- Git pull is actually two command in one -> `git fetch` and `git merge`.

                git pull origin master 
- By typing this command actually we are doing  fetch and merge the remote  changes directly into your local master branch.


# Merge Conflict
Merge conflicts happen when you merge branches that have competing commits, and Git needs your help to decide which changes to incorporate in the final merge.Git can often resolve differences between branches and merge them automatically.

- Merge conflict error is also occure at the time of pushing -> The remote repo contains work that you do not have locally.
-  this error because someone has pushed changes to the remote. that need to be pulled first and result of pull is merge conflict 
- we are now in a merge conflict look like there was a already a file named `file_name.txt`.

## How to resolve Merge Conflict

see:->https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-using-the-command-line




# Fork

A fork is a copy of a repository that you manage. Forks let you make changes to a project without affecting the original repository. You can fetch updates from or submit changes to the original repository with pull requests.

- After using GitHub by yourself for a while, you may find yourself wanting to contribute to someone else’s project. Or maybe you’d like to use someone’s project as the starting point for your own. This process is known as forking.
- Creating a "fork" is producing a personal copy of someone else's project. Forks act as a sort of bridge between the original repository and your personal copy. You can submit pull requests to help make other people's projects better by offering your changes up to the original project.

     see:-> https://docs.github.com/en/get-started/quickstart/contributing-to-projects
