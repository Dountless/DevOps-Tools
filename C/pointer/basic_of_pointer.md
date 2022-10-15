
# Pointer

 A pointer is a variable whose value is the address of another variable, i.e., direct address of the memory location. Like any variable or constant, you must declare a pointer before you can use it to store any variable address. The general form of a pointer variable declaration is:
 `  type *var-name;`
# What is a pointer variable?
 The address of a data item is called a pointer to the data item and a variable that holds an address is called a pointer variable.


### Uses of pointers
- Keep track of address of memory location.
-  By changing the address in pointer type variable you can manipulate data in different memory allocation.
- Allocation of memory can be done dynamically.


```
	Int X=5			
		x
		5
		2048	
	X is a name of memory location
	5 is the content of memory block 
	2048 is the Address of the memory block 
```
```
Ex:->	main()
	{
		Int x=5;
		printf(“%d\n”,x);
		printf(“%d”,&x);
	}
	Output:-> 5
		2048
```
### Address of operator :->
	•	& is known as address of operator 
	•	It is an unary operator 
	•	Oprands must be name of the variable 
	•	& give address number of variable
	•	& is also known as referencing operator 
### Indirection operator
	•	* is a indirection operators
	•	It is also known as dereferencing operator 
	•	It is an unary operator 
	•	It takes address as an argument
	•	* return the content whose address is argument
```
Ex:-> main()
	{
		Int x=5;
		Printf(“%d\n”,x);
		Printf(“%d\n”,&x);
		Printf(“%d”, *&x);
	}

Note:-> reference %u to print address because address is not negative.
```
```	
Ex:->1
	Int x=5				
	&x=7

Output:->L value error because &x means 2048 that means 2048=7 not allowed because its constant.

Ex:->2
	Int *j ,x=5;
	J=&x;
	•	 J is not an ordinary variable like any other intiger variable 
	•	J is a variable which  contains the address of another variable.

Ex:->	#include<stdio.h>
	{
	Int x=5,*j;
	J=&x;
	Printf(“%d %u\n”,x,j);
	Printf(“%d %u”,*j,&x);
	Printf(“%u”,*&j);
	}
	Output:-> 	5     2048 
			5	2048
			2048


```

## Base Address
	
	Int a , *j;	
	J			a
	1000		
			1000              1001

	float b , *k;
	k			b
	2000		
			2000		2001		2002		2003

	char  c , *r;
	r			c
	3000		
				3000


J=&a,k=&b,r=&c;


 ## Extended Concept of Pointer :-> 

	x			p			q			r	
	
	5			1000			2000			3000
	1000			2000			3000			4000	
```
void main()
{
	Int x=5 , *p ,**q ,***r;
	p=&x;
	q=&p;
	r=&q;
	***r=7;// that means x=7;
}

```

```
Ex:->
	p		  q	          	r
	6		 0x100	      0x200 
	0x100	0x200		0x300

	Int p=6;					
	Int *q=&p;
	Int **r=&q;
	printf(“%d\n”,p);
	p=6				&p=0x100 
q=0x100                        &q=0x200			
r=0x200			&r=0x300	

*p=illigle			**p=illigle	    
*q=6				**q=illigle	
*r=0x100			**r=6              

*&p=6
*&q=0x100
*&r=0x200

```

## Pointers Arithmatic
	
	•	We can not add,multiply,divide two addresses(Substraction is possible)
	•	We can not multiply an intiger to an address and similarly we cannot divide an address with an intiger value
	•	We can only add or substraction intiger to /form as address

- Formulae:->Pointer + n =pointer + sizeof(type of pointer) * n

```		
Int *p;
		p
		1000

	p+1 = 1004
	p+2 = 1008
	p+3 = 10012

substraction=Pointer -n =>pointer  - sizeoff(type of pointer ) * n
	1000 – 4 *2
	1000 – 8 = 1992

	p-1 = 996
	p-2 = 992
	Pointer1 – pointer2 = Literal substraction  / size of (type of pointer)
	•	1020 – 1000 => 20(address)/4(size of memory block)  = 5 (make five memory block) 
		
```


## Pointer type Declaration

Pointers are also variables and hence, must be defined in a program like any other variable. The Rules for declaring pointer variable names are the same as ordinary variables.
- type *variable_name;

Where, 
```  
               For example,

type             Data type of the variable pointed variable.
variable_name    Name of the pointer variable.
*(asterisk)      Signifies to the compiler that this variable has to be considered a pointer to the data type indicated by type.
```
```
  int*int_ptr :-      int_ptr is a pointer to the data of type integer
   char*ch_ptr :-      ch_ptr is a pointer to data of type character
   double*db_ptr :-   db_ptr is a pointer to data of type double
   ```
Note: All the pointer variables will occupy 4 bytes of memory regardless of the type they point to.


## Pointer Comparison
- The relational comparison ==,!= are permitted between pointers of the same type.
- The relational comparison <, <=, >, >= are permitted between pointers of the same type and the result depends on the relative location of the two data items pointed to.
```
For example,
   int a[10],*ap;
the expression
    ap==&a[9];
is true if ap is pointing to the last element of the array a, and the expression
    ap<&a[10];
is true as long as ap is pointing to one of the element of a.
```
