# Typecasting

Converting an expression of a given data type into another data type is known as **type-casting** or **type-conversion**. There are two types of type conversions:

- Implicit Type Conversion
- Explicit Type Conversion
 

### 1. Implicit Type Conversion

It is automatically performed by the compiler itself to ensure that the calculations between the same data types take place and avoid any loss of data. Such types of conversions take place when more than one data type is present in an expression. The rule associated with implicit type conversions involves upgrading the data type of all the variables to the data type of the variable with the **“largest data type”**.

The order of automatic type conversion or the sequence for smallest to largest data type(left to right) for this type conversion is given as:

bool -> char -> short int -> int -> unsigned int -> long -> unsigned -> long long -> float -> double -> long double

**Example:**
```
#include <iostream>
using namespace std;

int main() {
    int number = 200;
    char letter = 'c';
    float dec = 0.7;
    int res1 = number + letter; // here letter is implicitly converted to int and its value is the             
    //  ASCII value of ‘c’ i.e. 99
    cout << res1 << " ";
    float res2 = res1 + dec; // here res1 is implicitly converted to float.
    cout << res2;
}
```
Output: 
```
299 299.7
```

### 2. Explicit Type Conversion:

This process is also called typecasting, and it is user-defined. Here the user can typecast the result to make it of a particular data type which may lead to data loss and is also known as forceful casting.

**Syntax:** 
```
(type) expression
```

**Example**:
```
int main() {
    double dbl = 5.6;
    int res = (int)dbl + 10; // Here dbl is explicity converted to int i.e value of 
    // dbl becomes 5.
    cout << "Result = " << res; 
}
```
Output: 
```
Result = 15
```