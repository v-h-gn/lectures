---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
presenter: true
---

# CS 010A Lab 08: Functions Cont'd 
## 11/4/2025 

---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Announcements

- Check your grades!
- Check your feedback!
- Come to office hours!
- 2 Weeks left until Finals Week

<img src=https://i.imgflip.com/acf42c.jpg v-drag="[455,21,500,500]"/>

---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
addons:
- slidev-addon-cpp-runner
```
::left::
# Functions Review

<v-clicks>

What are the elements of a function definition?

- return type
- function name
- parameters
- code block
- return statement <b>*</b>

<b>\*</b> What is the exception to needing a return statement?

</v-clicks>

::right::
<br><br>

<v-clicks>

```cpp {all}

#include <iostream>
using namespace std;

void prettyPrint(double avg, double std, string data_name) {
    cout << data_name 
    << " mean & std_dev: " 
    << avg << " +/- "<< std << endl;
}

int main() {
    prettyPrint(30.0, 7.5, "Quiz 3 Grades");
    // outputs "Quiz 3 Grades mean & std_dev: 30.0 +/- 7.5
    return 0;
}

```

</v-clicks>

--- 

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Pass By Reference
C++ has two ways we can pass variables to functions


#### Pass by value
Creates a local copy within the function of the argument

#### Pass by reference
Avoids copying, any modifications that occur within the function will also occur to the argument variable


---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
::left::
# Scope
<br>

```cpp {all}{class:'!children:text-xl'}
#include <iostream>

void foo(int arg);

int main() {
    int a = 0;
    foo(a);
    bar(&a);
    cout << "a equals" 
         << a << endl;
    return 0;
}

```

::right::
<br><br>

```cpp {all}{class:'!children:text-xl'}
void foo(int arg) {
    arg = arg + 1;
    cout << arg << endl;
}

void bar(int& arg) {
    arg = arg + 1;
    cout << arg << endl;
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Variable Reference

A **reference** tracks the value of a variable (as opposed to directly storing the value).

#### Ex `int& playerIDReference = &playerID;`



_If `playerID` changes, `playerIDReference` will reflect that change._


# Variable Copy

This is in contrast to when we simply assign a variable to another.

#### Ex. `int playerIDCopy = playerID;`

_Unless you modify `playerIDCopy`, it will never change, even if `playerID` is modified._

---

```yaml
layout: two-cols-header
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Best Practices

- Avoid assigning pass-by-value parameters 
::left::
### Bad ❌
```cpp {all}
int roll(int numSides){
    numSides = rand() % numSides + 1;
    return numSides;
}
```
::right::

### Good ✅
```cpp {all}
int roll(int numSides){
    int result = rand() % numSides + 1;
    return result;
}
```


---

```yaml
layout: two-cols-header
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Best Practices cont'd

- Don't put function calls inside of functions, in this class at least.

::left::
### Bad ❌
```cpp {all}
int roll(int value, int numSides){
    int result = rand() % numSides + 1;
    // retry until we get a result that doesn't equal value
    if(value == result) {
        roll(value, numSides);
    }
    return numSides;
}
```
::right::
### Good ✅
```cpp {all}
int roll(int value, int numSides){
    int result = rand() % numSides + 1;
    // retry until we get a result that doesn't equal value
    while(result == value) {
        result = rand() % numSides + 1;
    }
    return result;
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Brief Intro to Arrays and Vectors

An array is a variable type which stores multiple objects of the same type in a sequential order.

## Ex. `double grades[50];`

A `vector` is an equivalent construct to an array, except that it has lots of special functions we can use that make certain tedious things with arrays simpler.

## Why do we care about these?

Now you can finally store dynamic quantities of data without needing to declare an individual variable for them. 

You can take in a list of items and process them individually.


---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Questions, Comments, Concerns, Quibbles?