# Types of Variables, Overflow and Underflow

## Types of Variables

There are three types of variables based on the scope of the variable in C++:
- Local Variables
- Instance Variables
- Static Variables

### 1. Local Variables

The variables declared within the body of a function or block are known as local variables and are created(occupy memory) when the program enters the block or makes a function call. The local variables get destroyed(memory is released) after exiting from the block or return from the function call. They can be used only by the statements inside the body of the function or the block they are declared within.

**Example:**
```
void function() {
    //local variable marks
    int marks = 90;
    marks = marks + 2;
    cout << "Student obtained "<<marks<<" marks."
    return;
}
```
Output:
```
Student obtained 92 marks.
```

### 2. Instance Variables

Instance variables are non-static variables and belong to an instance of a class and are declared in a class outside any method, constructor, or block. These variables are created when an object of the class is created and destroyed when the object is destroyed and are accessible to all the constructors, methods, or blocks in the class. Each object of the class within which the instance variable is declared will have its own separate copy or instance of this variable.

Unlike local variables, we may use access specifiers for instance variables.

**Example:**
```
class A {
    int a; // by default private instance variables
    int b;
    public:
        int c; // public instance variable
    Void
    function () {
        a = 10;
        cout << a;
    }
};
```

### 3. Static Variables

Static variables are declared using the keyword ‘static’, within a class outside any method, constructor, or block. Space is allocated only once for static variables i.e we have a single copy of the static variable corresponding to a class, unlike instance variables. The static variables are created at the start of the program and get destroyed at the end of the program i.e the lifetime of a static variable is the lifetime of the program. Static variables are initialized only once and they hold their value throughout the lifetime of the program. 

**Example:**
```
class A {
    static int
    var; //static variable
    Void func() {
        ++var;
    }
};
```