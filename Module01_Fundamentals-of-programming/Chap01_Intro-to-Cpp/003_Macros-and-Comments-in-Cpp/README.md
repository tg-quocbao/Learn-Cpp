# Macros and Comments in C++

## Macros
 
Macros are a piece of code in a program that is given some name. Whenever the compiler encounters this name, the compiler replaces the name with the actual piece of code. The ‘#define’ directive is used to define a macro.

**Note:** There is no semicolon(‘;’) at the end of the macro definition.

**Example:**
```
#include <iostream>
using namespace std;

// macro definition
#define LIMIT 5

int main() {
    for (int i = 0; i < LIMIT; i++) {
        cout << i << " ";
    }
    return 0;
}
```

Output:
```
0 1 2 3 4
```

**Macros with arguments:** We can also pass arguments to macros. Macros defined with arguments work similarly as functions.

**Example:**

```
#include <iostream>
using namespace std;

// macro with parameter
#define Area(l, b)(l * b)

int main() {
    int l = 10, b = 5, a;
    a = Area(l, b);
    cout << "The Area of the rectangle is: " << a;
    return 0;
}
```

Output:
```
The area of the rectangle is: 50
```

## Comments
 
C++ comments are hints that a programmer can add to make their code easier to read and understand. They are completely ignored by C++ compilers.

There are two ways to add comments to code:

**//**        - Single Line Comment

**/* */ **   - Multi-line Comments

**Example: Single line comment.**
 
```
#include <iostream>
using namespace std;

int main() {
    // This is a comment
    cout << "Hello World!";
    return 0;
}
```

Output:
```
Hello World!
```

**Example: Multi-line Comment.**

```
#include <iostream>
using namespace std;

int main() {
    /* The code below will print - Hello World!
    to the screen*/
    cout << "Hello World!";
    return 0;
}
```

Output:
```
Hello World!
```