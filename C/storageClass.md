# STORAGE CLASS
	•	It tells about the allocation of variable in memory .
	•	MEMORY:->
	•	Basically memory are three type  CPU register, RAM, secondary storage .

## RAM:-> RAM(Random access memory) have Four Segment
- STACK
- HEAP
- DATA
- CODE/TEXT
		

## Storage Class tells about four property:->
	•	auto/Automatic
	•	register
	•	static
	•	global/extern

## Automatic storage class:-( auto)
	•	initial value/Default value->garbage value
	•	storage->stack			
	•	scope->with in block
	•	life->block end

	•	Note:-> optional (keyword:-> auto )

```
Ex:->	#include<stdio.h>
	Int main()
	{
		Int x=5;
		printf(“%d\n”,x);
		{
			Int x=2;
			printf(“%d\n”,x);
//the x variable which is more local it will reference 
		}
		printf (“%d\n”,x);
		return 0;
	}
Output:-> 	5
		2
		5	
```

## Register storage class:	(register)
	•	initial value/Default value->garbage value
	•	storage->CPU Register/stack,( if register not available.)
	•	scope->with in block
	•	life->block end


  programme will become fast slightly







```
•	Ex:->
#include<stdio.h>
Int main()
{	register int x=4;
	Int y;
	y=x++;
	x--;
	y=x+5;
	printf(“%d %d”,x,y);
	return 0;
}
Output:->4,9

```
# Static storage class:(static)
	•	initial value/Default value->Zero(0)
	•	storage->data segment
	•	scope->with in block
	•	life->programme end

```
Ex:->
	#include<stdio.h>
	void F1(void);
	int main()
	{
		F1();
		F1();
		return 0;
	}

	void  F1()
	{
		static int i;
		i++;
		printf(“%d\n”,i);
	}
Output:->	1
		    2
```
# Global/Extern storage class: (global/extern)
	•	initial value/Default value-> Zero(0)
	•	storage-> data segment
	•	scope->across the  block
	•	life-> programme end
```

Ex:-1
	#include<stdio.h>
	void  f1();
	void f2();
	Int x;//globally
	Int main()
	{
		printf(“%d\n”,x);
		f1();
		f2();
		print(“%d\n”,x);
		return 0;
	}
	void f1()
	{
		x++;
		printf(“%d\n”,x);
	}
	void f2()
	{
		static int x=5;
		x++;
		printf(“%d\n”,x);
	}

	Output:-> 0
			1
			6
			1
Ex:2-
	#include<stdio.h>
	void g1();
	Int main()
	{
		extern int x;
		printf(“%d\n”,x);
		g1();
		printf(“%d\n”,x);
		return 0;
	}
	Int x;
	void g1()
	{
		x++;
		printf(“%d\n”,x);
	}
	Output:->	0
			1		
			1
```			
	•	The extern Storage Class 
	•	The extern storage class is used to give a reference of a global variable that is visible to ALL the program files. When you use 'extern', the variable cannot be initialized as all …..
	•	it does is point the variable name at a storage location that has been previously defined. 
	•	When you have multiple files and you define a global variable or function, which will be used in other files also, then extern will be used in another file to give reference of defined variable or function. 
	•	Just for understanding, extern is used to declare a global variable or function in another file. 

- The extern modifier is most commonly used when there are two or more files sharing the same global variables or functions as explained below. 
```
First File: main.c 

#include <stdio.h>
int count ;
extern void write_extern();
main() {
   count = 5;
   write_extern();
}

Second File: support.c

#include <stdio.h>
extern int count;
void write_extern(void)
{
   printf("count is %d\n", count);
}   
   

Here, extern keyword is being used to declare count in the second file where as it has its definition in the first file, main.c. Now, compile these two files as follows:
 $gcc main.c support.c
This will produce a.out executable program, when this program is executed, it produces the following result:
5

```   
![Screenshot 2022-03-09 at 9 59 56 PM](https://user-images.githubusercontent.com/98619865/157486006-4c600d93-e209-4faa-a408-7e45dd511763.png)


   
   
