
# C: Brief Theory

- C is perhaps the most popular programming languagecreated in 1972 by Dennis Ritchie at the Bell Labs in USA as a part of UNIX operating system. C isused to develop core parts of this operating system. From that time C programming language hasbeen the de facto programming language when fast programs are needed or the software needs tointeract with the hardware in some way.Most of the operating systems like Linux, Windows™, and Mac™ are either developed in C languageor use this language for most parts of the operating system and the tools coming with it.


- C is a general-purpose programming language. It has been closely associated with the UNIX operating system where it was developed, since both the system and most of the programs that runon it are written in C. The language, however, is not tied to any one operating system or machine;and although it has been called a ‘‘system programming language’’ because it is useful for writing compilers and operating systems, it has been used equally well to write major programs in many different domains.

In 1983, the American National Standards Institute (ANSI) established a committee whose goal was
to produce ‘‘an unambiguous and machine-independent definition of the language C’’, while still
retaining its spirit. The result is the ANSI standard for C.








## Scope of Advance/Industrial C:

- C language is used for creating computer applications Used in writing Embedded Firmware/ Software Firmware for various electronics, industrial & communications products which use micro- controller
- It is also used in developing verification software, test code, simulators etc for variousapplications & hardware products. For creating complier of different languages which can take input from other language andconvert it into lower level machine dependent language C is used to implement various Operating Systems & their applications.
- UNIX kernel is completely dependent of C Language
- Operating System
- Network Drivers
- Client-Server Implementation
- Print Spoolers
- Language Compliers
- Assemblers
- Text Editors
- Modern Program
- Database
- Intermediate Language –for portability on machine dependent targets directly or indirectly influenced- C#, D, Go, Java, JavaScript, Limbo, LPC, Perl, PHP, Python,and Unix's C Shell
- GNU Multi-Precision Library, the GNU Scientific Library, Mathematica and MATLAB are completely or partially written in C
- Language Interpreters
- Simulators
- Utilities
- Embedded System
- Aviation
- Military
- Telecom
- Automate
- Healthcare
- ERP
- Banking & Finance




## Features of C
- Robust language, which can be used to write any complex program.
- Has rich set of built-in functions and operators.
- Well-suited for writing both system software and business applications.
- Efficient and faster in execution.
- Highly portable.
- Well-suited for structured programming.
- Dynamic Memory Allocation.

---
---
---

## History of C Language 

#### John Backus: - 
    • Developer of FORTRAN(Formulae Translation)
    • 1957
    • Used for mathematical calculation

#### CODASYL :-
    • Developer of COBOL(Commercial Business Oriented Language)
    •  Around 1959
    • Used for business software

#### Martin Richard:-
    •  Developer of BCPL(basic combined programming language )
    • Around 1966
    • Used for general purpose
#### Ken Thompson:-
    • Developer of B language.
    • Around 1969
    • Also Developer of Unix Operating System.
       
#### Dennis Ritchie: -
    • Developer of C language 
    • 1972
    • at AT&T’s Bell LABs, USA.
    • Co-developer of Unix OS.

## How to execute a programe:-       

![image](https://user-images.githubusercontent.com/98619865/152575140-5af862ca-68a3-4fe0-bcdb-73505d2167e5.png)


## PROGRAMMING

    • Programming is a process of taking an Algorithm and Coding it into a notation.
    • Example:-C, C++, JAVA , PHP , Perl , Python ,SQL  etc.

### Note:-Algorithm is a optimize solution to a particular problem.


---
#### Types of Programming language: -

    • Low-level -> Assembly
    • Procedure Oriented-> C, pascal.
    • Object Oriented-> C++ , Java , C#
    • Programming for Web-> HTML , PHP.
    • Programming for database-> Sql
    • A Scripting-> Shell,  JavaScript
    
### Note:- C is a relatively low-level programming language because c is directly interact with the hardware.# Identifier:---

# Identifier:---

## Constant:- 
    • Any information is a constant
    • Data=information=Constant.

## Variable:-
    • Variable is a name of memory allocation where we store a data.
    • Variable can be  a combination of alphabate,alphanumeric and underscores...
    • A valid Variable name  can not start with digit.
## Rules:-
    • Variable can Capitals and small  alphabeted
    • Number should not come first 
    • Space and special character not allowed
    • Allowed only underscore
## Keywords:--
    • Predefine words 
    • Reserved words
    • There are 32 Keywords in C language acc. To 16 bit architecture  
    -   Ex:-   main() ,calloc(),malloc,sizeof,for,while etc.





# Some Important special character name:---
    • <>  :- Angular bracket 
    • {}    :-  braces
    • ( )   :- bracket or parenthis
    • “is”:- Double Quote
    •  ‘a’ :- Single Quote
    •  %  :- Modulus
    •  &  :- Empersand
    •  *  :- Astrix or pointer or multiple
    •  [] :- Square Bracket
    •  /  :- Forward slash
    • \:- Backword slash
# Escape sequence: -
        ◦ \n  :- used for next line
        ◦ \t  :- used for tab
        ◦ \b:- used for backspace

        ◦ \\:- used to print slash \
        ◦ \”:- used to print double quote
        ◦ \’:- used to print single quote
        ◦ \a:-used to produce alert or beep sound
        ◦ %% :- used to print % 
# Format Specifier:-
![formatspecifier](https://user-images.githubusercontent.com/98619865/153698118-9a036447-2254-4ca7-89e8-01a592a44438.jpg)

- %d print as decimal integer
- %6d print as decimal integer, at least 6 characters wide
- %f print as floating point
- %6f print as floating point, at least 6 characters wide
- %.2f print as floating point, 2 characters after decimal point
- %6.2f print as floating point, at least 6 wide and 2 after decimal point



# Data type in ‘C’: -

   - C language has extensive range of data types which we can use programme. These datatype have different size and capacity.


   - Variables in C are associated with data type. Each data type requires an amount of memory and performs specific operations. There are some common data types in C …

## Integer Types
### The following table provides the details of standard integer types with their storage sizes and value ranges −


![integer](https://user-images.githubusercontent.com/98619865/153698974-c202fade-c5fc-42c7-a2ea-24e33e9b7fc0.jpg)



### Note: - To get the exact size of a type or a variable on a particular platform, you can use the sizeof operator. The expressions sizeof(type) yields the storage size of the object or type in bytes.

## Floating-Point Types
### The following table provide the details of standard floating-point types with storage sizes and value ranges and their precision −

![float](https://user-images.githubusercontent.com/98619865/153698988-6ac7f914-5d65-4964-a62c-602415883a9a.jpg)

### Note:-printf() function by default give precision 6 decimal



# Know this arithmetic while writing simple program of calculator-

- int operator int =  int
- int operator float = float
- float operator int = float
- float operator float = float



# Declaration: -
    • Declaration just explain the entity to compiler
        ◦ EX: - int a;        //a is a type of int;
        ◦ float num1;  // num1 is a type of float 




# Initialization: -
    • At the time of declaration assigning value to it......
     - EX: -int a=10, b=20;



# Definition: -
    • When memory Associated after declaration.
     - EX: -int A;   // define  
            A=10;  // define




# Lvalues and Rvalues in C:


## There are two kinds of expressions in C:


**lvalue** : Expressions that refer to a memory location is called "lvalue" expression. An lvalue may
appear as either the left-hand or right-hand side of an assignment.

**rvalue** : The term rvalue refers to a data value that is stored at some address in memory. An rvalue is
an expression that cannot have a value assigned to it which means an rvalue may appear on the
right- but not left-hand side of an assignment.

- Variables are lvalues and so may appear on the left-hand side of an assignment. Numeric literals are rvalues and so may not be assigned and can not appear on the left-hand side. Following is a valid statement:
    
    
# Internal Typecasting & External Typecasting


- Typecasting is a way to make a variable of one type, such as an int, act like another type, such as a char, for one single operation.


## Internal typecasting
    - float b = 2;
    - printf(“b = %f”,b);
## External typecasting
    - int a = 6;
    - void *ptr = &a;
    - printf(“a = %d” , *(int *)ptr);
    
    
    
#  A S C I I   Table

    • ASCII  stands for American Standard Code for Information Interchange.
    • There are 128 Standard ASCII characters, numbered from 0 to 127. Extended ASCII adds another 128 value and give to 255
    
   ![ascii](https://user-images.githubusercontent.com/98619865/153699563-328020dd-49fc-4783-b70c-9453f16516d3.jpg)


    Note:- ‘A’+32=’a’  , ‘z’-32=’Z’
    Note:- space :- 32
    
    

### - gotoxy(_,_) -> Function shift cursor every position...
    Ex:-
    #include<stdio.h>
    void  gotoxy(int,int);
    Int main()
    {
    clrscr(); // to clear the screen
    gotoxy(40,13); // 40,13 is a co-ordinates of x and y
    printf(“deepak\n”);
    return 0;
    }
    void gotoxy(int x,int y)    
    {
     printf("%c[%d;%df",0x1B,y,x);
    }
    
    
- Note:- 
        ◦ printf() is not a keyword
        ◦ printf() is a pre-define function
- Note:-
        ◦ Unary operator those operators which is used in  single operands. Ex: -   x++;
        ◦ Binary operators those operators which is used two operands Ex :-  x+y; //here x,y is a operand
        ◦ Ternary operator those operators which is used in triple operands Ex: - z?x:y;
- Note:-
        ◦ sizeof() operator used only single operands and it give size of data type of operands
        ◦ sizeof() operator is a compile t
    
    
    
    
    
 
#  Arithmetic Instruction in C Language
    •  Operator: -
                • 3+4 //here 3 and 4 is operands and + is operator

## Arithmetic instruction: -
                • An instruction which is used to manipulate data by using operator, is known as Arithmetic Instruction.

## Types of Operator: -
                • Unary operator-> +, -, ++, --,sizeof()
                • Arithmetic operator ->+ ,- ,*,/,%
                • Relation operator-> <,<=,>,>=,==,!=
                • Logical operator->&& , || , !
                • Bit-wise operator->  & , |  ,  ~ ,  <<  ,  >> , ^
                • Conditional(ternary) operator->  ? : 
                • Assignment operator-> +=,-=,*=,/=,%= (compound operator)
### Note:-
            ▪ ++ and -- are known as iteration
            ▪ There are two iteration.
                        i. Pre-increment-> ++x
                              ->First inc. And then assign 
                        ii. Post-increment-> x++
                              ->First asign and then inc.
            Note:- this concept basically used in printf()
            
            
            
## Precedence & Associativity: - 

                • This rule of priority of operators is called operator precedence.
                • Associativity is only used when there are two or more operators of same precedence.
                
                
![precedence](https://user-images.githubusercontent.com/98619865/153699314-f213910c-86aa-4e8b-af99-f570ece47733.jpg)



### Note:-
            ▪ Real Constant consume memory of 8 bytes like:- 77.18
            ▪ %(modulus) operator only work on integer value 
            ▪ Character in sizeof operator convert into ASCII value which means integer and occupied 4 bytes of memory EX:- sizeof(‘a’)

### Note: -
            ▪ Int/int = int   Ex: - 3/2 = 1
            ▪ Int/float = float Ex: - 3/2.0 = 1.0
            ▪ Float/int = float Ex: - 3.0/2 = 1.0
            ▪ Float /float =float Ex: - 3.0/2.0 = 1.0


### Note: -
     Modulus operator give the sign of numerator always 
            ▪ 4%3 =  1
            ▪ -4%3 =  -1 
            ▪ 4%-3 =  1
            ▪ -4%-3 = - 1




    

    
    
    
    




