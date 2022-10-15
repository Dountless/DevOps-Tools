
# What is Git

**Git  is a ` version-control system` for tracking changes in computer files and coordinating work on those files among multiple people.”**

actually, Git is a`Distributed Version Control System`. So Git does not necessarily rely on a central server to store all the versions of a project's file.Instead ,every user `clone` a copy of a repository(a collection of files) and has the `full` history of the project on their own hard drive.

## Version Control System

Version control system basically mean that we can go back in time and work with a different version of our code base since `git` stored it all and work with branches

There are two types of version control: centralized and distributed

**Centralized version control**

With centralized version control systems, you have a single “central” copy of your project on a server and commit your changes to this central copy. You pull the files that you need, but you never have a full copy of your project locally.

**Distributed version control**

Distributed means that it has a remote repository which is stored in a server and a local repository which is stored on computer of every developer working on a project so, every developer has access to the full copy of the code base.


# Why use Git ?

- Undo mistake
- Distributed developement
- **Don't mix things up**
- Community Support

# What is a GIT Repository?

Repositories in GIT contain a collection of files of various different versions of a Project.

### **Git has two repository**
- **local repository** : basically in your own  machine so you have direct access to it and it has three stages.
- **remote repository** : repository usually in a `centralized server` and is entirely optional.

![repository](https://i.stack.imgur.com/UvZ0M.png)

### Note: local repository containing a three stages

- **Working area:** The Working Tree is the area where you are currently working. It is where your files live. This area is also known as the “untracked” area of git. Any changes to files will be marked and seen in the Working Tree.
- **The Staging Area (Index):** The Staging Area is when git starts tracking and saving changes that occur in files. These saved changes reflect in the .git directory. That is about it when it comes to the Staging Area. You tell git that I want to track these specific files, then git says okay and moves them from you Working Tree to the Staging Area and says “Cool, I know about this file in its entirety.” 

- **The Local Repository:** The local repository contains `committed`files. The files in this area will be pushed to the origin.The Local Repository is everything in your .git directory. Mainly what you will see in your Local Repository are all of your checkpoints or commits. It is the area that saves everything (so don’t delete it). That’s it.

  `Note: Storing changes in a local Git repository is called commiting.`

# Let's start Working with a Repository 

![Screenshot from 2022-02-11 13-20-21](https://user-images.githubusercontent.com/98619865/153555352-93c06330-71d1-4a4b-97cf-e4193a70bf4d.jpg)

- First you need to install a git tool on your machine :-

  [` https://github.com/git-guides/install-git`](https://github.com/git-guides/install-git)
  
  
  ----
 After installing git you need to perform a some command to work on it ....
- Initialize  empty Git repository 
``` 
   git init 
```
*You can see that after initialized `.git` folder created automatically, use `ls -a` to see `.git` folder.*

---
- check status of your git repo
``` 
   git status
```

----
- To add file in staging area

``` 
   git add 'file.txt'
```
----

- To commit all  file that are in staging area 

``` 
   git commit -m "initial commit"
```
--- 

*Note:-> Before committing git need to know who you are because all commits are recorded by name of an author.*

So, you must use the `git config` command

``` 
   git config user.name "deepak"
   git config user.email "deepak@example.com" 
```

*when you type git commit command without any option git open a text editor which is always the default, here you provide a commit message*

Note:-> Every commit needs to have a meaningful message that tells exactly what that commit does very briefly.

- What exactly a commit?
--- 
   commit stores a copy of the file in its current state, one file or a set of file  that were committed.
   so, its save a copy of files within the `.git` folder  so,our work is safe... 

--- 

- Restore the privious version of file from the previous commit

``` 
   git restore 'file.txt' 
```

----
Note:-> its always recommended to keep your commit `atomic` and name your commits  with a message that tells exactly what commit does. 

Note:-> when you stage a file in git by `git add` command it caches the state of file when it was staged .

----
- Remove a file from the staging area 

``` 
   git restore --staged 'file.txt'
```
----

- remove a tracked file and retain the file in our directory

``` 
   git rm --cached 'file.txt' 
```
- remove a tracked file(untrack) and delete the file permanently.

``` 
   git rm -f 'file.txt' 
```
----

Note:-> add a file name in a .gitignore file so, its basically instruct the git to permanently ignore this file.

----

- Show the information that you need to know about all the commits
``` 
   git log 
```
this command show the information such as , `commit hash` , `author name` , the `date of commit` and the `commit message`

- see the privious commit history along with branch they were committed on.

``` 
   git rm --graph --decorate  
```

use `--oneline` option to sort the  information.

----




