# Remote-repository

- we can push code to the remote repository that is hosted somewhere else and get this code again our local machine by pulling this information.

- there are several plateform on which we can host our remote repository.

ex:-> `Github` , `Gitlab`, `Bitbucket` etc.


- after initialized a remote repository in one of those platform. we can get access to something called a `connection string`.


### Connection string 
- it is a url that we can use in order to let Git know.

## How to add Local repo to remote  Repo.

- use `git remote add origin`. the origin is a alias that make sure that always know which remote repo we are pushing to.
   
      git remote add origin 'connection string' 


- How list remote repo.
  
     git remote -v 


## pushing 

-   when local and remote repo are sync we can push data for a local to remote repo.

            git push origin master or main
- `master` or `main` is a default branch on remote repo 



# Cloning
-  When a new member gets added to the project and should access all the data that  person can clone the repository in order to get this data on their local machines.

- When you clone a repository you copy the repository from Github.com to your local machine.

- cloning a repository pulls down a full copy of all the repository that Github.com has at that point in time , including all the version of every file and folder for the project. 

- You can clone a repo with a git clone command followed by `ssh link` of the remote repo.
   
       git clone [ssh link]


- By default that command will create a folder locally with same name as the remote Repository.

And you can now get start work on this project locally and intract with remote repository.

NOTE:->
-   After cloning you should create a new branch and working on them and push on remote repository `git push origin  master/max.`

- But, to push all changes just you have made you need to collobrate as a team to remote repository . just tell the remote repo owner to add as a collaborater of their repository and after that you will able to push your code.

- After pushing on github plateform will have a notification and you can creating somthing called `pull request (PR)`  to merge into the master branch. And owner and who have write access master branch  will approve your request and merge them.

- After creating a pull request other team member can see the changes that you have made coments on them.

