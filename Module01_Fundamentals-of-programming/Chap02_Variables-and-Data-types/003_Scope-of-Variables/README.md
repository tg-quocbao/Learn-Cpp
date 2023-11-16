# Scope of a Variable

Scope of a variable refers to the region of visibility or availability of a variable i.e the parts of your program in which the variable can be used or accessed.

There are mainly two types of variable scopes:
- Local Scope
- Global Scope

### 1. Local Scope

Variables declared within the body of a function or block are said to have local scope and are referred to as **‘local variables’**. They can be used only by the statements inside the body of the function or the block they are declared within.

**Example:**
```
void person() {
    string gender = "Male";
    //This variable gender is local to the function person()
    //and cannot be used outside this function.
}
```

### 2. Global Scope

The variables whose scope is not limited to any block or function are said to have global scope and are referred to as **‘global variables’**. Global variables are declared outside of all the functions, generally on the top of the program, and can be accessed from any part of your program. These variables hold their values throughout the lifetime of the program.

**Example:**
```
#include <iostream>
using namespace std;

// Global variable declaration: and can be used anywhere in code
int g;

int main() {
    g = 10; // Using global variable
    cout << g;
    return 0;
}
```