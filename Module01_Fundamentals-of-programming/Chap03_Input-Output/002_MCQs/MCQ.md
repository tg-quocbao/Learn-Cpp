# Multiple Choice Questions

## 1. Find x
Easy

**Problem Statement :** What value of 'x' will generate an error?
```
#include <iostream>
#include <string>

using namespace std;

int main() {
    string x;
    cin >> x;

    return 0;
}
```

- [ ] "4513"
- [ ] "Hello"
- [ ] "Hello world"
- [ ] None of the above

## 2. cin input
Medium

**Problem Statement :** Where does 'cin' stop its extraction of data?

- [ ] By seeing a blank space
- [ ] By seeing a newline (\n)
- [ ] By seeing a ()
- [ ] Both a and b


## Solutions
1. None of the above
> Since we have defined our variable 'x' as a string, it can't take space character as input.

2. Both a and b
> 'cin' stops its extraction when it encounters a blank space or a new line.
