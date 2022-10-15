# Stashing

Suppose you are implementing a new feature for your product. your code is in progress and suddenly a customer escalation comes.

Because of this, you have to keep aside your new feature work for few hours.

You don't want to commit your partial code also won't throw away your changes. 

so, you need some temprory storage, where you can store partial changes and later on commit it.

`that is stash(temprory storage)`

Note:-> To stash an item only applies to modified files not new files.

## command of Stashing
-  put all work in stash
   
       git stash

- get the changes back into working area that you are currently stash
   
      git stash pop 

- list all  stashes files

      git stash list 

- see the content of the stash file 

       git stash show stash@{0} 

- pop for specific stash 
   
       git stash pop stash@{0}


- to clear stash 

      git stash clear 



Note:-> After  stash pop the data will copy stash to working Directory not copy paste.


![image](https://user-images.githubusercontent.com/98619865/158058911-2f3c9519-e223-4d48-b2b6-58f8f3866e98.png)
