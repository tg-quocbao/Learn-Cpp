# Multiple Choice Questions

## 1. Local scope
Easy

**Problem Statement :** Which of the following is a local scope variable?
```
#include <iostream>
using namespace std;

int g;
int local

int main() {
    int global;
    double b, c;
}
```

- [ ] local, b
- [ ] global, b, c
- [ ] g, b, c
- [ ] local, global

## 2. Bool variable
Easy

**Problem Statement :** Which of the following is a global scope variable?
```
#include <iostream>
using namespace std;

int g;
int local

int main() {
    int global;
    double b, c;
}
```

- [ ] local, g
- [ ] global, c
- [ ] g, b, c
- [ ] local, global

## Solutions
1. global, b, c
> It's the only option that contains only local scope variables; the rest all the options have at least one global scope variable.

2. local, g
> It's the only option that contains only global scope variables; the rest all the options have at least one local scope variable.
