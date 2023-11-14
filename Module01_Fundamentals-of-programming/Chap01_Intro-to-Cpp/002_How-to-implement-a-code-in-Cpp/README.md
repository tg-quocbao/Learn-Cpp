# How to implement a code in Cpp

## Headers

C++ code begins with the inclusion of header files. There are many header files available in the C++ programming language, which will be discussed while moving ahead with the course.

So, what are these header files?

The names of program elements such as variables, functions, classes, and so on must be declared before they can be used. For example, you can’t just write x = 42 without first declaring variable x as:

```
int x = 42;
```

The declaration tells the compiler whether the element is an int, a double, a float, a function, or a class. Similarly, header files allow us to put declarations in one location and then import them wherever we need them. This saves a lot of typing in multi-file programs. To declare a header file, we use **#include** directive in every .cpp file. This #include is used to ensure that they are not inserted multiple times into a single .cpp file.

Now, moving forward to the code:

```
#include <iostream>

using namespace std;
```
 
**iostream** stands for Input/Output stream, meaning this header file is necessary to take input through the user or print output to the screen. This header file contains the definitions for the functions:

**cin**: used to take input

**cout**: used to print output
 
**namespace** defines which input/output form is to be used. You will understand these better as you progress in the course.

**Note:** semicolon (;) is used for terminating a C++ statement. i.e., different statements in a C++ program are separated by a semicolon.

## main() function

Look at the following piece of code:

```
int main() {

      Statement 1;

      Statement 2;

      ...

}
``` 

You can see the highlighted portion above. Let’s discuss each part stepwise.

Starting with the line: 

```
int main()
```
 
- **int:** This is the return type of the function. You will get this thing clear once you reach the Functions topic.

- **main():** This is the portion of any C++ code inside which all the commands are written and executed.

This is the line at which the program will begin executing. This statement is similar to the start block of flowcharts.

As you will move further in the course, you will get a clear glimpse of this function. Till then, just note that you will have to write all the programs inside this block.

- **{}:** all the code written inside the curly braces is said to be in one block, also known as a particular function scope. Again, these things will be clear when you will study functions.

For now, just understand that this is the format in which we are going to write our basic C++ code. As you will move forward with the course, you will get a clear and better understanding.

## Compile and run a C++ code

**For compiling and running a CPP program in Linux following are the command lines:**

Compile: g++ Filename.cpp
Run or execute: ./a.out
 
**For compiling and running a CPP program in Windows following are the command lines:**

Compile: gcc Filename.cpp
Run or execute: filename