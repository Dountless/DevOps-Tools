
# Understanding Git

## How it actually work 
 - Git is nothing more than key value store.
 - When we added a file to a commit the content of a file are `hashed` using `SHA-1` algorithm.
 - The `hash` is then used as a key name for the folder and store store a file using that key name 

 ### Git has two type of command 
   - porcelain command 

         git add , git status , git commit , git stash etc. 

   - plumbing commands:-> used to access to the internal of git 

          git hash-object , git ls-files , git rev-parse , git ls-remote etc.



#### To understand more clearly what is internally git see that video:->  https://www.youtube.com/watch?v=MyvyqdQ3OjI 

#### Also read that blog :-> https://www.freecodecamp.org/news/git-internals-objects-branches-create-repo/
