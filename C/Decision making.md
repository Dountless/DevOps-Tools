# Decision making/Conditional statement/Selection statement

    • If statement (single selection statement)
    • If-else statement (double selection statement)
    • If elseif...elseif..........else (multiple selection)
    • Switch (choice/case based selection)
    • Conditional/Ternary ( ? : )
    
## If statement

``` #include<stdio.h>
Int main()
{
Int x;
printf(“enter  a no\n”);
scanf(“%d”,&x);
If(x>0)
printf(“no. Is positive”);
return 0;
}
```
- Note:- 

                • don’t put semicolon after if()
                • We can remove braces in if() when  in block single statement


# If-else statement

``` #include<stdio.h>
Int main()
{
Int age;
printf(“enter your age\n”);
scanf(“%d”,&age);
If(age>=18)
printf(“you are valid to play game”);
Else
printf(“you are not a valid to play “);

return 0;

}
``` 

# If-elseif statement

``` 
#include<stdio.h>
Int main()
{
float p ;
printf(“enter a percentage of marks\n:”);
scanf(“%f”,&p);
If (p>0 && p<33)
{
printf(“fail\n”);
}
elseif (p>=33 && p<45)
{
printf(“3rd division\n”);
}
elseif(p>=45&&p<60)
{
printf(“2nd division\n”);
}
elseif(p>=60)
{
printf(“1st division\n”);
}
else
{
printf(“ invalid percentage input\n”);
}
return 0;

}

``` 

# Nested if-else
``` 
Syntax:
If (condition)
{
If (condition)
{
//statement;
}
}
else
{
//statements;
}
``` 

- Note: -
 
        ◦ If  float a=3.4 it means a assign value is 3.3999999999..... that means if assing float  value is bit decrease.


- Note:- use of goto keyword
   
        Syntax:
        goto  there;   // there is a lable..
         …...............
          ................
            …...........................
        there:
           printf(“deepak\n”);




# Switch

``` 
Syntax:
switch (expression)
{
case  constant:
//statement;
break;
case  constant:
//statement;
break;
case  constant:
//statement;
break;
case  constant:
//statement;
break;
case  constant:
//statement;
break;
default:
//statement;
}
``` 
-  Note:- 

            ▪ constant is anything just like a digit,alphabate etc.
            ▪ The keyword break can be used in loop body or in switch body.
            ▪ The purpose of break is to terminate loop execution immediately as it encounters.
            
            


---
# CALCULATOR USING SWITCH
---


    /*Note:-> to use this calculator use -lm when you compile this program
          :->command to use compile this programe is `gcc filename.c -lm`*/


    #include<stdio.h>
    #include<stdlib.h>
    #include<math.h>
    int main()
    {
            int a,b,c,ch;
            float d;
            char cha;
            printf("**************************WELCOME TO DOUNTLESS CALCULATOR*******************************\n(press enter):");
            scanf("%c",&cha);
            while(1)
            {
                	printf("\n\t\tEnter the choice in the given below:\n");
                    printf("Addition:1\nSubstraction:2\nmultiplication:3\nDivision:4\nmodulation(Reminder):5\nSquare_root:6\nexit:7\n\n:->");
                	scanf("%d",&ch);
                	switch(ch)
                    {
    
                            case 1:
                                    printf("enter two no: ");
                                    scanf("%d%d",&a,&b);
                                    c=a+b;
                                    printf("Addition of %d and %d is %d\n",a,b,c);
                                    break;
                            case 2:
                                    printf("enter two no: ");
                                    scanf("%d%d",&a,&b);
                                    c=a-b;
                                    printf("Substraction of %d and %d is %d\n",a,b,c);
                                    break;
                            case 3:
                                    printf("enter two no: ");
                                    scanf("%d%d",&a,&b);
                                    c=a*b;
                                    printf("Multiplication of %d and %d is %d\n",a,b,c);
                                    break;
                            case 4:
                                    printf("enter two no: ");
                                    scanf("%d%d",&a,&b);
                                    d=(float)a/b;
                                    printf("division of %d and %d is %6.2f\n",a,b,d);
                                    break;
                            case 5:
                                    printf("enter two no: ");
                                    scanf("%d%d",&a,&b);
                                    c=a%b;
                                    printf("Addition of %d and %d is %d\n",a,b,c);
                                    break;
                            case 6:
                                    printf("enter a no.:");
                                    break;
                            case 7:
                                exit(0);
                            default:
                                    printf("enter a valid choice\n");
                    }
            }
    return 0;
    }	
---


