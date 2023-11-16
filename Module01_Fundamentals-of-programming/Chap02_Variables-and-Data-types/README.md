# Introduction to Variables

A variable is a storage place that has some memory allocated to it. It is used to store some form of data. Different types of variables require different amounts of memory.

## Variable Declaration 

In C++, we can declare variables as follows:
```
data_type variable_name;
```
- **data_type:** Type of the data that can be stored in this variable. It can be int, float, double, etc.
- **variable_name:** Name given to the variable.

Example:
```
int x;
```
 
In this way, we can only create a variable in the memory location. Currently, it doesn’t have any value. We can assign the value in this variable by using two ways:
- By using variable initialization.
- By taking input

Here, we can discuss only the first way, i.e., variable initialization. We will discuss the second way later.
```
data_type variable_name = value;
```
Example:
```
int x = 20;
```

## Rules for defining variables in C++
- You can’t begin with a number. Ex- 9a can't be a variable, but a9 can be a variable.
- Spaces and special characters except for underscore(_) are not allowed.
- C++ keywords (reserved words) must not be used as a variable name.
- C++ is case-sensitive, meaning a variable with the name ‘A’ is different from a variable with the name ‘a’. (Difference in the upper-case and lower-case holds true).

## C++ Keywords
![image](https://github.com/tg-quocbao/Learn-Cpp/assets/105618730/c3a5b780-0e9e-441f-b114-1164ff344f00)
