<div align = "center">
<h1><strong>MODULE 2</strong></h1>
</div>

# __*Problem solving and Algorithms*__
Though a problem can be solved in numerous ways a proper algorithm is required. An algorithm is a sequence of steps to solve a problem. There are numerous ways in which an algorithm can be written for one problem. Algorithm develops the framework to aid in instructing the computer for a specific task. The ability to breakdown a large problem into small parts assist in understanding the problem. The common steps to write down an algorithm are-
 - Get the Specification of the problem
 - Evaluate and interpret the problem
 - Develop a effective algorithm
 - Process the algorithm with additional details
 - Inspect the algorithm

</br>

<div align = "center">
<img src="https://user-images.githubusercontent.com/91787553/194767515-0104f626-20e8-4088-b9ec-b866a29f2d6a.png" height=250>
</div>
</br>

# __*Basics of C*__
## Operators
There are total of 6 types of operators in C namely, 


 1. Arithmetic Operators

```C
int A = 8;
int B = 6;
printf("%d\n%d\n%d\n%d\n", A+B, A-B, A*B, A/B);
```

 2. Relational Operators

```C
int num1 = 3;
int num2 = 4;
printf("%d\n%d\n", num1>num2, num1!=num2);
```

 3. Logical Operators

```C
int C = 14;
int D = 10;
printf("%d", (C>D && C!=D));
```

 4. Bitwise Operators

```C
int a = 4;
int b = 3;
printf("%d\n%d\n%d", a^b, a|b, a&b);
```

 5. Assignment Operators 
 
 ```C
 int x = 10;
 ```
 
 6. Misc Operators
 
 Misc operators or the Miscellaneous operators consists of operators such as, sizeof(), pointers(*), conditional expressions (?:), address of the variable (&).
 
 ```C
 int x = 10;
 int *p;
 p = &x;
 ```
 </br>

 <div align = "center">
<img src="https://user-images.githubusercontent.com/91787553/194767579-22f71fd7-052b-4d5f-b592-bbdde52e676d.png" height=250>
</div>
</br>

## Conditionals

Conditionals or the decision making statements aid in taking decisions by a boolean expression. They include: if-else statements, switch cases.

The if-else if-else conditionals:

```C
if (<condition1>)
{
//If <condition1> is true this part of the code is executed.
}
else if (<condition2>)
{
//If <condition2> is true this part of the code is executed.
}
else
{
//If neither <condition1> nor <condition2> is true this part of the code is executed.
}
```

switch-cases conditionals:

```C
Switch (expression)
{
 case value1:
 // if (expression==value1) this part of code is executed. 
 break;
 case value2:
 // if (expression==value2) this part of code is executed. 
 break; 
 case valuen:
 // if (expression==valuen) this part of code is executed. 
 break;
 Default:
 // if none of them are satisfying the necessary conditions then this block is executed.
}
```

## Arrays

A data structure that can store a fixed-sized sequence. The intialization of an integer array can be done by -

```C
// 1-D array initialization.
int arr1[5] = {1,4,5,7,9};  
// or
int arr2[5];

// 2-D array initialization.
int arr3[10][4];

// n-D array initialization.
type name[size1][size2]...[sizen];
```

Arrays can be accessed using loops. An array is a contiguous piece of memory that holds enough space for a number of items of a certain type. For instance, integers are 4 bytes, and so an integer array with 4 elements would be 16 bytes long. Since arrays are `not mutable`. To resize and array, you would have to make a new array of the desired size and copy the memory from the old array to the new array.

## Pointers
A pointer is a variable whose value is the address of another variable, i.e., direct address of the memory location. Like any variable or constant, you must declare a pointer before using it to store any variable address.

```C
int    *ip;    //pointer to an integer
double *dp;    //pointer to a double
float  *fp;    //pointer to a float
char   *ch     //pointer to a character
```

**How pointers are used in string arrays?**

A string is a 1-D array of characters, so an array of strings is a 2-D array of characters.

The string array ends with an null character `\0`.

```C
char *sports[] = {<element1>, <element2>, ........ <elementn>};
```

