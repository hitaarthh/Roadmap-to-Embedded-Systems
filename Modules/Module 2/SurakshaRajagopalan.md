<div align = "center">
<h1><strong>MODULE 2
</br>
Advanced C</strong></h1>
</div>

</br>

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

## <a href = "https://www.geeksforgeeks.org/how-to-use-algorithms-to-solve-problems/">More about Programs and Algorithm</a>

# __*Basics of C*__
## Operators
There are total of 6 types of operators in C namely, 


 1. Arithmetic Operators 

 An arithmetic operator performs mathematical operations such as addition, subtraction, multiplication, division etc on numerical values (constants and variables).

```C
int A = 8;
int B = 6;
printf("%d\n%d\n%d\n%d\n", A+B, A-B, A*B, A/B);
```

 2. Relational Operators

 A relational operator checks the relationship between two operands. If the relation is true, it returns 1; if the relation is false, it returns value 0. Relational operators are used in decision making and loops.

```C
int num1 = 3;
int num2 = 4;
printf("%d\n%d\n", num1>num2, num1!=num2);
```

 3. Logical Operators

 An expression containing logical operator returns either 0 or 1 depending upon whether expression results true or false. Logical operators are commonly used in decision making in C programming.

```C
int C = 14;
int D = 10;
printf("%d", (C>D && C!=D));
```

 4. Bitwise Operators

 Bitwise operators are used in C programming to perform bit-level operations.

```C
int a = 4;
int b = 3;
printf("%d\n%d\n%d", a^b, a|b, a&b);
```

 5. Assignment Operators 

 This operator is used to assign a value to a variable.
 
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

## <a href = "https://www.tutorialspoint.com/cprogramming/c_operators.htm">Operators link1</a>

## <a href = "https://www.geeksforgeeks.org/operators-c-c/">Operators link2</a>

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

## <a href = "https://www.geeksforgeeks.org/decision-making-c-cpp/">Conditionals</a>

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

## <a href = "https://www.w3schools.com/c/c_arrays.php">Arrays</a>

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

<a href = "https://www.w3schools.com/c/c_pointers.php">Pointers</a>

# __*Structures*__

Arrays allow to define type of variables that can hold several data items of the same kind. Similarly structure is another user defined data type available in C that allows to combine data items of different kinds.
To define a structure, you must use the struct statement. The struct statement defines a new data type, with more than one member. The format of the struct statement is as follows − 

```C
struct [structure tag] {

   member definition;
   member definition;
   ...
   member definition;
} [one or more structure variables];  
```

The structure tag is `nonobligatory` and each member definition is a normal variable definition, such as int i; or float f; or any other valid variable definition.

To access any member of a structure, we use the member access operator `(.)`.

```C
struct Nursery {
   char  Flower_name[50];
   char  Family[50];
   char  colour[15];
   float radius;
} nursery;  
```

## <a href = "https://www.geeksforgeeks.org/structures-c/">Structures</a>

# __*Unions*__ 

A union is a special data type available in C that allows to store different data types in the same memory location. Unions provide an efficient way of using the same memory location for multiple-purpose. The union statement defines a new data type with more than one member for your program. The format of the union statement is as follows −

```C
union [union tag] {
   member definition;
   member definition;
   ...
   member definition;
} [one or more union variables]; 
```
A variable of Data type can store an integer, a floating-point number, or a string of characters. It means a single variable, i.e., same memory location, can be used to store multiple types of data. The memory occupied by a union will be large enough to hold the largest member of the union.

```C
union Data {
   int i;
   float f;
   char str[20];
} data;  
```

## <a href = "https://www.geeksforgeeks.org/union-c/">Unions</a>

# __*Functions*__

A function is a group of statements that together perform a task. Every C program has at least one function, which is main(), and all the most trivial programs can define additional functions.

There are two types of function in C, namely :

1. Standard library

The printf() is a standard library function to send formatted output to the screen (display output on the screen). This function is defined in the stdio.h header file.
Hence, to use the printf()function, we need to include the stdio.h header file using `#include <stdio.h>`.
The sqrt() function calculates the square root of a number. The function is defined in the `math.h` header file.

## <a href = "https://www.programiz.com/c-programming/library-function">Standard Libraries In C</a>

2. User defined library

As the name suggests it is defined by the user. There are two ways in defining a function based on whether it can return a value or not.

```C
int <function name>(<data type> <variable>){
    // the function's work
    return <variable>;
}
```

```C
void <function name>(<data type> <variable>){
    // the function's work
}
```

The void keyword is used when the function is defined if the function has no value to return, while if the function is returning an integer value then int keyword is used when the function is used, if a string is returned then str is used.

## <a href = "https://www.programiz.com/c-programming/c-user-defined-functions">User Defined functions in C</a>


# __*Files*__

A file is a sequence of bites irrespective of whether it is a text file or a binary file. C provides access on high level functions as well as low level (OS level) calls to handle file on your storage devices. 

## Opening a file 

`fopen( )` function to `create a new file` or to `open an existing file`. This call will initialize an object of the type FILE, which contains all the information necessary to control the stream.

Synax of the function is:
```C
FILE *fopen( const char * filename, const char * mode );
```

The modes available for opening the file are: 

<img src = "https://imgs.search.brave.com/rNbsJ7ZtUlpumTV2YjU15JcELcXp5EBArfKwBb4drIU/rs:fit:571:382:1/g:ce/aHR0cHM6Ly9pMS53/cC5jb20vYXRpY2xl/d29ybGQuY29tL3dw/LWNvbnRlbnQvdXBs/b2Fkcy8yMDE5LzA4/L2ZpbGUtbW9kZXMt/bWluLmpwZz9yZXNp/emU9NTcxJTJDMzgy/JnNzbD0x">

</br>

__*The major difference between read, write and append mode :*__

1. __read mode__ : When a file is opened in this mode no changes can be done to the file, it can only be used to read the file or to print its contents. If a file which does not exists is being opened in this mode an error is generated.

2. __write mode__ : The write mode is used when one needs to write into the file. When the file is opened in the write mode and the file does not exists then C creates an empty file with the file name and opens it. If the file already exists with some content in it then the file is opened but when the user tries to modify the content in the file, the previous content is deleted and the fresh data is written.

3. __append mode__ : The append mode is used when the data in the file needs to be modified or updated. If the file does not exist, then a new file is created. While updating the file the previous content is not erased.

## Writing a file

The function `fputc()` writes the character value of the argument c to the output stream referenced by fp. It returns the written character written on success otherwise `EOF` if there is an error.

```C
int fputc( int c, FILE *fip );
```

The function fputs() writes the string s to the output stream referenced by fip. It returns a non-negative value on success, otherwise EOF is returned in case of any error. One can use `int fprintf(FILE *fip,const char *format, ...);` function as well to write a string into a file.

```C
int fputs( const char *s, FILE *fip );
```

## Reading a file

The `fgetc()` function reads a character from the input file referenced by fip. The return value is the character read, or in case of any error, it returns EOF. 

```C
int fgetc( FILE * fip );
```

The functions fgets() reads up to n-1 characters from the input stream referenced by fip. It copies the read string into the buffer buf, appending a null character to terminate the string.

If this function encounters a newline character '\n' or the end of the file EOF before they have read the maximum number of characters, then it returns only the characters read up to that point including the new line character. One can also use int `fscanf(FILE *fip, const char *format, ...);` function to read strings from a file, but it stops reading after encountering the first space character.

```C
char *fgets( char *buf, int n, FILE *fip );
```

## Functions for a binary file

fread() is a function which takes 4 inputs in order to read a binary file which are the a pointer to store the contents of the file, size_of_elements is for the size (in bytes) of the data type of the pointer ptr, number_of_elements is the number of elements that have to read, *a_file is the file pointer. 

```C
size_t fread(void *ptr, size_t size_of_elements, size_t number_of_elements, FILE *a_file);
              
size_t fwrite(const void *ptr, size_t size_of_elements, size_t number_of_elements, FILE *a_file);
```

## Closing a file

`fclose(<file pointer>)` is used inorder to close a file. The fclose(<file pointer>) function returns `zero on success`, or `EOF` if there is an error in closing the file. This function actually flushes any data still pending in the buffer to the file, closes the file, and releases any memory used for the file. The EOF is a constant defined in the header file stdio.h.

```C
int fclose( FILE *fp );
```

__Why do we have to close a file?__

If an opened file is not closed then the consequences are that a file descriptor is `leaked`. The operating system uses some descriptor, and has some resources associated with that open file. If you fopen and don't close, then that descriptor won't be cleaned up, and will persist until the program closes.

This problem is compounded if the file can potentially be opened multiple times. As the program runs more and more descriptors will be leaked, until eventually the operating system either refuses or is unable to create another descriptor, in which case the call to fopen fails.

## Seek and rewind

`fseek()` function helps to find the position of the pointer in a file. 

```C
int fseek(FILE *ptr, long int offset, int whence);
```

Here,

`ptr` − This is the pointer to identify the stream.

`offset` − This is the number of bytes from the position.

`whence` − This is the position from where offset is added.

`whence` is specified by one of the following constants.

`SEEK_END` − End of file.

`SEEK_SET` − Starting of file.

`SEEK_CUR` − Current position of file pointer.

`rewind()` is used to set the position of file to the beginning of given stream. It does not return any value.Syntax of the function is:
```C
void rewind(FILE *ptr);
```
The only parameter of the function is the file pointer.

## <a href="https://www.geeksforgeeks.org/basics-file-handling-c/">File Handling In C</a>


# __*Preprocessor Directives*__

The preprocessor will process directives that are inserted into the C source code. These directives allow additional actions to be taken on the C source code before it is compiled into object code. Directives are `not part of the C language` itself. Preprocessor directives begin with a pound `(#)` symbol and may have several arguments.

</br>

| Directives | Specification     | Examples     |
| ------------- | ------------- | -------- |
| <a href= "https://www.javatpoint.com/c-preprocessor-include">#include</a> | Include another C file into the current file at the location of the #include statement prior to compiling the source code.| #include <math.h>  |
| <a href= "https://www.javatpoint.com/c-preprocessor-define">#define</a> |Define a macro which can be used as a constant throughout the source code.| #define Length 50  |
| <a href = "https://www.techonthenet.com/c_language/directives/undef.php">#undef</a>|Clear a macro which was previously defined.|#undef Length|
| <a href = "https://www.techonthenet.com/c_language/directives/if.php">#if</a>| Conditional expresssion which can be used to include source code for compilation.|#if Length > 50|
| <a href = "https://www.techonthenet.com/c_language/directives/ifdef.php">#ifdef</a>|	Allows the inclusion of source code if the provided macro identifier has been defined. Equivalent to #if defined(identifier).|#ifdef SOLARIS|
| <a href = "https://www.techonthenet.com/c_language/directives/ifndef.php">#ifndef</a>|Allows the inclusion of source code if the provided macro identifier has not been defined.|#ifndef WINDOWS|
| <a href = "https://gcc.gnu.org/onlinedocs/cpp/Elif.html">#elif</a>| Provides an alternate inclusion of source code when used with the #if, #ifdef, or #ifndef directives and the #elif condition evaluates to true.| 	#elif YEARS_OLD > 10|
| <a href = "https://www.javatpoint.com/c-preprocessor-else">#else</a>|Allows the inclusion of source code if the preceeding #if, #ifdef, or #ifndef directive expression evaluates to false.|#else|
| <a href = "https://www.educative.io/answers/what-is-the--sharpendif-directive-in-c">#endif</a>|Signals the end of a #if, #ifdef or #ifndef condition.| 	#endif|
| <a href = "https://gcc.gnu.org/onlinedocs/gcc-4.6.0/gcc/Warning-Options.html">#warning</a>|Report a warning message and continue preprocessing.| 	#warning Non-critical error found|
| <a href = "https://www.techonthenet.com/c_language/directives/error.php">#error</a>| Report error and stop preprocessing.| #error Windows is an unsupported platform|

</br>

# __*Recursion*__

Recursion is the process of repeating items in a self-similar way. In programming languages, if a program allows you to call a function inside the same function, then it is called a recursive call of the function. Recursive functions are very useful to solve many mathematical problems, such as calculating the factorial of a number, generating Fibonacci series, etc.
Here is a basic Factorial program done using recursion.

```C
#include <stdio.h>

int factorial(int i) {

   if(i <= 1) {
      return 1;
   }
   return i * factorial(i - 1);
}

int  main() {
   int i = 5;
   printf("Factorial of %d is %d\n", i, factorial(i));
   return 0;
}
```

## <a href = "https://www.w3schools.com/c/c_functions_recursion.php">Recursion</a>

# __*Project environment*__

Project environment represents a connection, where the design is reused. It impacts the design and is, thus, conditioned. Such an commerce is handed by multitudinous factors as functional, physical, ecological, social, artistic, profitable, cerebral, fiscal, organizational etc. The terrain not only formulates the design but also estimates it. The design terrain analysis is held at the morning of the design.

# __*Makefiles*__

A makefile is a tool for organising or streamlining compilation-related code. Makefile is a collection of commands (similar to terminal commands) that may be used to create and delete object files. We can construct many targets to compile and remove object, binary files in a single make file. Using Makefile, you can compile your project (software) as many times as you want.

The make command allows you to manage large programs or groups of programs. As you begin to write large programs, you notice that re-compiling large programs takes longer time than re-compiling short programs. Moreover, you notice that you usually only work on a small section of the program ( such as a single function ), and much of the remaining program is unchanged.

The make program allows you to use macros, which are similar to variables. Macros are defined in a Makefile as = pairs. An example has been shown below −
```bash
MACROS  = -me
PSROFF  = groff -Tps
DITROFF = groff -Tdvi
CFLAGS  = -O -systype bsd43
LIBS    = "-lncurses -lm -lsdl"
MYFACE  = ":*)"
```

## <a href = "https://www.includehelp.com/c-programming-questions/what-is-makefile.aspx">Makefiles</a>

# __*Libraries*__

## *Standard Libraries:*
C Standard library functions or simply C Library functions are inbuilt functions in C programming.

The prototype and data definitions of these functions are present in their respective header files. To use these functions we need to include the header file in our program. 

<div align = "center">
<img src = "https://imgs.search.brave.com/cNJYgX-B09_u0L9rbSxYdyEoZVaDOAC7JFENS3DmDKo/rs:fit:569:571:1/g:ce/aHR0cHM6Ly9xcGgu/ZnMucXVvcmFjZG4u/bmV0L21haW4tcWlt/Zy01NzIyYzFkMzU1/NGVjODNjNjA0YTIz/MGZjODEyYTVjMQ" width = 350>
</div>

## *Making Own Libraries:*
If you have a bunch of files that contain just functions, you can turn these source files into libraries that can be used statically or dynamically by programs. This is good for program modularity, and code re-use. Write Once, Use Many. A library is basically just an archive of object files.

### Static Library Setup 
First thing you must do is create your C source files containing any functions that will be used. Your library can contain multiple object files. After creating the C source files, compile the files into object files. To create a library:

```shell
ar rcs libmylib.a objfile1.o objfile2.o objfile3.o
```

Remember to prototype your library function calls so that you do not get implicit declaration errors.
When linking your program to the libraries, make sure you specify where the library can be found:

```shell
gcc -o foo foo.o -L. -lmylib
```

Since programs that use static libraries already have the library code compiled into the program, it can run on its own. Shared libraries dynamically access libraries at run-time thus the program needs to know where the shared library is stored. What's the advantage of creating executables using Dynamic Libraries? The executable is much smaller than with static libraries. If it is a standard library that can be installed, there is no need to compile it into the executable at compile time! The key to making your program work with dynamic libraries is through the LD_LIBRARY_PATH enviornment variable. To display this variable, at a shell:
```shell
echo $LD_LIBRARY_PATH
```
Will display this variable if it is already defined. If it isn't, you can create a wrapper script for your program to set this variable at run-time. Depending on your shell, simply use setenv (tcsh, csh) or export (bash, sh, etc) commands. If you already have LD_LIBRARY_PATH defined, make sure you append to the variable. For example:
```shell
setenv LD_LIBRARY_PATH /path/to/library:${LD_LIBRARY_PATH}
```
would be the command you would use if you had tcsh/csh and already had an existing LD_LIBRARY_PATH. An example with bash shells:
```shell
export LD_LIBRARY_PATH=/path/to/library:${LD_LIBRARY_PATH}
```
If you have administrative rights to your computer, you can install the particular library to the /usr/local/lib directory if it makes sense and permanently add an LD_LIBRARY_PATH into your .tcshrc, .cshrc, .bashrc, etc. file.


## <a href = "https://www.cs.dartmouth.edu/~campbell/cs50/buildlib.html">Libraries</a>

# __*Dry Test*__

A dry run is a test or check performed on a computer, hardware, or electrical equipment. This test is run to test the performance or stability of a particular product before it is made available.

Dry run techniques where you step through a program listing away from a computer are very powerful pedagogically as a way to teach programming as well as other computational topics (eg Turing Machines, algorithms, etc).

Two main approaches are

- role play the execution of aspects of a program
- draw dry run tables, showing the changing values of tables with a row for each line executed by the program 

## <a href = "https://cpmadeeasy.blogspot.com/2013/03/dry-run.html">Dry Test</a>
