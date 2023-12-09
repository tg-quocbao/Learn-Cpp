# Input/Output in C++

## Taking Input from Console

### Cin

To take input from the user via console, we use the **cin** statement. 

cin is a predefined variable that reads data from the keyboard with the extraction operator (**>>**).

**Example1:**
```
int x; 
cin >> x; // Get user input from the keyboard
cout << x;
```
Input: 5
Output: 5


**Example2:**
```
string x; 
cin >> x; // Get user input from the keyboard
```
Input1: “Hello”
Output1: “Hello”
 
**Question:** Calculate the Simple Interest.
```
#include<iostream>
using namespace std;
int main() {
    int principal, time;
    double rate, si;
    cout << "Enter Principal Amount: ";
    cin >> principal;
    cout << "Enter Rate of Interest: ";
    cin >> rate;
    cout << "Enter Time period ";
    cin >> time;
    si = (principal * rate * time) / 100;
    cout << "Simple Interest: " << si;
}
```

Output:
```
Enter Principal Amount: 3000
Enter Rate of Interest: 2
Enter Time period: 3
Simple Interest: 180
```

**Question:** Add two numbers.
```
#include <iostream>
using namespace std;

int main() {
    int n1, n2, addition;
    cout << "Enter two integers: ";
    cin >> n1 >> n2;
    addition = n1 + n2;
    cout << "Sum of the numbers is: " << addition;
    return 0;
}
```

Output:
```
Enter two integers: 5 10
Sum of the numbers is: 15
```

### Getline

**getline()** is a standard library function used to read a string or a line from an input stream.

It is used when input strings with spaces between them or process multiple strings at once.

The **getline()** function extracts characters from the input stream and appends them to the string object until the delimiting character is encountered. While doing so, the previously stored value in the string object str will be replaced by the input string, if any.

**Syntax 1:**
```
istream& getline(istream& is, string& str, char delim);
```
**Parameters:**
- **is:** is an object of the istream class that tells the stream’s function the input that needs to be read.
- **str:** is the string object that stores the input after the stream’s reading process is finished.
- **delim:** defines the delimitation character, which commands the function to stop processing the input. The reading process will stop once the written code reads this command.
 

**Syntax 2:**
```
istream& getline (istream& is, string& str);
```
The second declaration is almost the same as that of the first one. The only difference is that the latter have a delimitation character by defaulting a new line(\n)character.

**Example:**
```
#include<iostream>
#include<string>
using namespace std;

int main() {
    string s;
    getline(cin, s);
    cout << s;
    return 0;
}
```
Input: Hello world
Output: Hello world
 
## Printing to the Console

### Cout

The C++ **cout** is used to produce output on the standard output device, usually the display screen or console. 

**cout** is a pre-defined variable that displays some output or text using the insertion operator(<<).

**Example:**
```
cout << “Hello World!”;
```
Output: Hello World!

**endl**: It is used to insert a new line character.

**Example:**
```
cout << “Hello” << endl;
cout << “World”;
```
Output: 
Hello 
World!

To print the variable value, the syntax is as followed 
```
cout << Variable_name;
```

**Example:**
```
#include <iostream>
using namespace std;
int main() {
    int age = 21;
    string firstName = "King";
    string lastName = "Kong";
    cout << "My name is " << firstName << " " << lastName << endl;
    cout << "My age is " << age << endl;
    return 0;
}
```
Output: 
My name is King Kong
My age is 21
 