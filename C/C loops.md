# C Loops 
Loops are very basic and very useful programming facility that facilitates programmer to execute any
block of code lines repeatedly and can be controlled as per conditions added by programmer. It saves
writing code several times for same task.

# There are three types of loops in C.
-  For loop
- Do while loop
- While loop

- Entry control loops:

         While loop
         For loop
- Exit control loops:

         Do while loop
         
  
  

## 1. For Loop Examples

- Basic syntax to use ‘for’ loop is:
```
for (variable initialization; condition to control loop; iteration of variable)
{
statement 1;
statement 2;
..
..
}
```
- In the pseudo code above :

      Variable initialization is the initialization of counter of loop.
      Condition is any logical condition that controls the number of times the loop statements are executed.
      Iteration is the increment/decrement of counter.
      It is noted that when ‘for’ loop execution starts, first variable initialization is done, then condition is
      checked before execution of statements; if and only if condition is TRUE, statements are executed;
      after all statements are executed, iteration of counter of loop is done either increment or decrement.  
      
  
# 2. Do While Loop Examples

It is another loop like `for` loop in C. But do-while loop allows execution of statements inside block of
loop for one time for sure even if condition in loop fails.

- Basic syntax to use `do-while` loop is:
```
variable initialization;
do {
statement 1;
statement 2;
..
..
iteration of variable;
} while (condition to control loop)
```
- In the pseudo code above :

      Variable initialization is the initialization of counter of loop before start of ‘do-while’ loop.
      Condition is any logical condition that controls the number of times execution of loop statements
      Iteration is the increment/decrement of counter
      Here is a basic C program covering usage of ‘do-while’ loop in several cases:  
      
   
   
# 3. While Loop Examples

It is another loop like ‘do-while’ loop in C.
The `while` loop allows execution of statements inside block of loop only if condition in loop succeeds.

- Basic syntax to use `while` loop is:

```
variable initialization;
while (condition to control loop)
{
statement 1;
statement 2;
iteration of variable;
} 


```






# Break and continue

To exit a loop you can use the break statement at any time. This can be very useful if you want to
stop running a loop because a condition has been met other than the loop end condition. Take a look
at the following example:

```

#include<stdio.h>
int main()
{
int i;
i = 0;
while ( i < 20 )
{
i++;
if ( i == 10)
break;
}
return 0;
}

```
---
In the example above, the while loop will run, as long i is smaller then twenty. In the while loop there
is an if statement that states that if i equals ten the while loop must stop (break).
With `continue` it is possible to skip the rest of the commands in the current loop and start from the top again. (the loop variable must still be incremented). Take a look at the example below:

---
``` 

#include<stdio.h>
int main()
{
int i;
i = 0;
while ( i < 20 )
{
i++;
continue;
printf("Nothing to see\n");
}
return 0;
}

```

- In the example above, the printf function is never called because of the `continue;`.
