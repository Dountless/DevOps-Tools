# Pointer and Function
## Functions returning Pointers
- We have already learnt that a function can return an int, a double or any other data type. Similarly it can return a pointer. However, to make a function return a pointer it has to be explicitly mentioned in the calling function as well as in the function declaration.
- While retaining pointer, return the pointer to global variables or static or dynamically allocated address. Do not return any address of local variable because stop to exit after function call.
```
/*Example: Function returning pointers*/
/*Program to accept two numbers and find greater number*/ #include<stdio.h>
int main(void)
{
   int a, b,*c;
   int*check(int,int);
   printf(“Enter two numbers:”);
   scanf(“%d%d”,&a,&b);
   c=check(&a,&b);
   printf(“\n Greater numbers: %d”,*c);
}
int*check(int*p,int*q)
{
   if(*p>=*q)
       return(p);
   else
       return(q);
}
```
- The address of integer being passed to check() are collected in p and q.
- Then in the next statement the conditional operators test the value of *p and *q and return either the address stored in p or the address stored in q.
- This address gets collected in c in main().


## Pointers to Functions
1. Functions have addresses just like data items. A pointer to a function can be defined as the address of the code executed when the function is called. A function’s address is the starting address of the machine language code of the function stored in the memory.
2. Pointers to functions are used in
3. writingmemoryresidentprograms.
4. writing viruses, or vaccines to remove the viruses


## Address of a Function
- The address of a function can be obtained by only specifying the name of the function without the trailing parantheses.
- For example, if CalcArea is a function already defined, then CalcArea is the address of the function CalcArea().
## Declaration of a Pointer to a Function
- The declaration of a pointer to a function requires the function’s return type and the function’s argument list to be specified along with the pointer variable.
- The general syntax for declaring a pointer to a function is as follows:

      return-type(*pointer variable)(function’s argument list);
- Thus , the declaration

      int(*fp)(int i,int j);
- declares fp to be a variable of type “pointer to a function that takes two integer arguments and return an integer as its value.” The identifiers i and j are written for descriptive purpose only,
- The preceding declaration can, therefore also be written as

        int(*fp)(int,int);

- Thus declarations
```
int i(void).   :- declares i to a function with no parameters that return an int.
int*pi(void).  :- declares pi to a function with no parameters that returns a pointer to an int.
int(*ip)(void).:- declares ip to be a pointer to a function that returns an integer value and takes no argument.
```

```       
/*Example: Pointer to Function*/
#include<stdio.h>
int func1(int i)
{
return(i); 
}
float func2(float f)
{
return(f); 
}

int main(void)
{
int(*p)(int); /*declaring pointer to function*/ float(*q)(float);
int i=5;
float f=1.5;
p=func1; /*assigning address of function func1 to p*/ q=func2; /*assigning address of function func2 to q*/ printf(“i=%d f=%f\n”,p(i),q(f));
}
```
 
- After declaring the function prototypes and two pointers p and q to the function; p is assigned the address of function func1 and q is assigned the address of function func2.
## Invoking a Function by using Pointers
- In the pointer declaration to functions, the pointer variable along with operator(*) plaays the role of the function name. Hence, while invoking function by using pointers, the function name is replaced by the pointer variable.
```
/*Example: Invoking function using pointers*/ #include<stdio.h>
int main(void)
{
unsigned int fact(int);
unsigned int ft,(*ptr)(int);
int n;
ptr=fact; /*assigning address of fact() to ptr*/ printf(“Enter integer whose factorial is to be found:”); scanf(“%d”,&n);
ft=ptr(n); /*call to function fact using pointer ptr*/ printf(“Factorial of %d is %u \n”,n,ft);
}
unsigned int fact(int m)
{
   unsigned int I,ans;
   if(m==0)
       return(1);
   else
   {
       for(i=m,ans=1;i>1;ans*=i--)
       return(ans);
} }

```
```
Output:
    Enter integer whose factorial is to be found: 8
    Factorial of 8 is 40320
```
