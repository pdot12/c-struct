# c-struct

## Variables
- char
- int
- float
- double
- void

`type variable_list;`

## Integer Literals
- 'c'
- "hello"
- 1
- 3.14

`#define identifier value`
`const type variable = value;`

## Storage Class
- auto
- register
- static
- extern

## Operators
---------------+------------------------------------+---------------
Postfix        | () [] -> . ++ --                   | Left to right
Unary          | + - ! ~ ++ -- (type)* & sizeof     | Right to left
Multiplicative | * / %                              | Left to right
Additive       | + -                                | Left to right
Shift          | << >>                              | Left to right
Relational     | < <= > >=                          | Left to right
Equality       | == !=                              | Left to right
Bitwise AND    | &                                  | Left to right
Bitwise XOR    | ^                                  | Left to right
Bitwise OR     | |                                  | Left to right
Logical AND    | &&                                 | Left to right
Logical OR     | ||                                 | Left to right
Conditional    | ?:                                 | Right to left
Assignment     | = += -= *= /= %=>>= <<= &= ^= |=   | Right to left
Comma          | ,                                  | Left to right
---------------+------------------------------------+---------------

## Decision Making
- if ...
- if ... else ...
- if ... else if ... else ...
- Exp1 ? Exp2 : Exp3;
- switch 

## Loops
- for 
- while
- do ... while

## Functions
`return_type function_name( parameter list );`
```
return_type function_name( parameter list ) {
   body of the function
}
```
**Arguments**
- Call by value
- Call by reference

## Scope Rules
- local variables
- global variables
- formal parameters

## Arrays
`type arrayName [ arraySize ];`
- Multi-dimensional arrays
- Passing arrays to functions
- Return array from a function
- Pointer to an array

## Pointers
`type *var-name;`
- Pointer arithmetic
- Array of pointers
- Pointer to pointer
- Passing pointers to functions in C
- Return pointer from functions in C

## Strings
`char greeting[6] = {'H', 'e', 'l', 'l', 'o', '\0'};`

## Structures
- Defining a Structure
- Accessing Structure Members
- Structures as Function Arguments
- Pointers to Structures
- Bit Fields

## Unions
- Defining a Union
- Accessing Union Members

## Bit Fields
- Bit Field Declaration
```
struct {
   type [member_name] : width ;
   type [member_name] : width ;
};
```

## typedef
`typedef unsigned char BYTE;`

## Input and Output
- The Standard Files
---------------+--------+----------
Standard input | stdin  | Keyboard
Standard output| stdout | Screen
Standard error | stderr | Your screen
---------------+--------+----------

## File I/O
- Opening Files
	FILE *fopen( const char * filename, const char * mode );
- Closing a File
	int fclose( FILE *fp );
- Writing a File
	int fputc( int c, FILE *fp );
	int fputs( const char *s, FILE *fp );
- Reading a File
	int fgetc( FILE * fp );
	char *fgets( char *buf, int n, FILE *fp );
- Binary I/O Functions
	size_t fread(void *ptr, size_t size_of_elements, size_t number_of_elements, FILE *a_file);
	size_t fwrite(const void *ptr, size_t size_of_elements, size_t number_of_elements, FILE *a_file);

## Preprocessors
--------------+---------------------------------------------------------------------
`#define`     |Substitutes a preprocessor macro.
`#include`    |Inserts a particular header from another file.
`#undef`      |Undefines a preprocessor macro.
`#ifdef`      |Returns true if this macro is defined.
`#ifndef`     |Returns true if this macro is not defined.
`#if`         |Tests if a compile time condition is true.
`#else`       |The alternative for #if.
`#elif`       |#else and #if in one statement.
`#endif`      |Ends preprocessor conditional.
`#error`      |Prints error message on stderr.
`#pragma`     |Issues special commands to the compiler, using a standardized method.
--------------+---------------------------------------------------------------------

- Predefined Macros
-----------+-----------------------------------------------------------------
`__DATE__` |The current date as a character literal in "MMM DD YYYY" format.
`__TIME__` |The current time as a character literal in "HH:MM:SS" format.
`__FILE__` |This contains the current filename as a string literal.
`__LINE__` |This contains the current line number as a decimal constant.
`__STDC__` |Defined as 1 when the compiler complies with the ANSI standard.
-----------+-----------------------------------------------------------------

- Preprocessor Operators
	The Macro Continuation (\) Operator
	The Stringize (#) Operator
	The Token Pasting (##) Operator
	The Defined() Operator
	Parameterized Macros

## Header Files
`#include <file>`
`#include "file"`
```
#ifndef HEADER_FILE
#define HEADER_FILE

the entire header file file

#endif
```
## Type Casting
- (type_name) expression
long double <- double <- folat <- unsigned long long <- long long <- unsigned long <- long <- unsigned int <- int


