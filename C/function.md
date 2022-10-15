
# Function in  C 

- Function is a piece of code to accomplish certain operation and it has a name for identification.

- A function is a group of statements that together perform a task. Every C program has at least one function, which is main(), and all the most trivial programs can define additional functions.

- Function are used to divide a large programme into a smaller pieces.

    You can divide up your code into separate functions. How you divide up your code among different
    functions is up to you, but logically the division usually is so each function performs a specific task.

- A function is known with various names like a method or a sub-routine or a procedure, etc.




## Defining a Function:
- The general form of a function definition in C programming language is as follows:
```
return_type function_name( parameter list )
{
body of the function
}
```

- A function definition in C programming language consists of a function header and a function body.
*Here are all the parts of a function:*

*`Return Type:`*   A function may return a value. The return_type is the data type of the value the function
returns. Some functions perform the desired operations without returning a value. In this case, the
return_type is the keyword `void`.

*`Function Name:`* This is the actual name of the function. The function name and the parameter list
together constitute the function signature.

*`Parameters:`*  A parameter is like a placeholder. When a function is invoked, you pass a value to the
parameter. This value is referred to as actual parameter or argument. The parameter list refers to the
type, order, and number of the parameters of a function. Parameters are optional; that is, a function
may contain no parameters.


*`Function Body:`* The function body contains a collection of statements that define what the function
does.



![image](https://user-images.githubusercontent.com/98619865/154440031-7c0af339-ab6b-4172-a940-f7aea9fa9997.png)



## Function Declarations/prototype/signature:->
- A function declaration just tells the compiler about the function name, function datatype, parameter and how to call the function.
- A function tell the compiler about this existence.
- Explain:-> `int fun(int,int);`

        fun  is a function with two argument as int and int and it will return int .
## Function Calling:->
- A function is called in order to be used.
- While creating a function , you give define of what the function has to do. To use a function you will have to call that function to perform the defined task.
    Ex:-> `Functionname (pass by value /Reference)` 

- When a program calls a function, program control is transferred to the called function. A called function performs defined task and when its return statement is executed or when its function-ending closing brace is reached, it returns program control back to the main program.



## Function Definition:->
- A function is define to get some task done.
-  Some function perform the desired operation without returning a value, in this case the return type is void.






# Parameter & Argument:->
## Function parameter
- Function  parameter are the listed in the function definition.
- it must declare variables that accept the values of the arguments. These variables are called the formal parameters of the function. 
- The formal parameters behave like other local variables inside the function and are created upon entry into the function and destroyed upon exit.

## Function argument
- Function Argument are the Real value passed to the function .

- While calling a function, there are two ways that arguments can be passed to a function:

  - #### Call by value
    This method copies the actual value of an argument into the formal parameter of the function. In this case, changes made to the parameter inside the function have no effect on the argument.
  - #### Call by reference

    This method copies the address of an argument into the formal parameter. Inside the function, the
    address is used to access the actual argument used in the call. This means that changes made to the
    parameter affect the argument.


# Recursion: (Equivalent to loop)
#### Recursion is a programming technique that allows the instructions is to "repeat the process" like loops. If a programming allows you to call a function inside the same function that is called recursive call of the function.

- Best example to understanding of recursion function is factorial of any no.

    Ex:->Factorial of a number

                #include<stdio.h>
                int fact(int);
                int main()
                {
                    int num=4,Result;
                    Result=fact(num);
                    printf(“factorial of %d no. is:”,Result);
                    return 0;
                }
                int fact(int a)
                {
                    if (a==0);
                        return 1;
                    else
                    {
                        return (a*fact(a-1));
                    }
                }

![image](https://user-images.githubusercontent.com/98619865/154439860-93751624-7589-4cb0-b5bc-62fd9844b036.png)
