---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
---

# CS 010A Lab 06: Functions 
## 11/4/2025 


---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
image: https://raw.githubusercontent.com/v-h-gn/lectures/refs/heads/main/published/cs010a/week6/image.png
```

# Announcements

- Gradescope
- Quiz 2 Grades
- Temporarily Move Office Hours for this Week?
- Mid Quarter Check In

---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
::left::
# What We've Covered

- cin vs cout, formatting
- variables, types, assignment, operations on variables
- branches, booleans, 
- loops (do-while, while, for)
- strings, string operations, character operations, getline

::right::
# What's Left
- Functions (this week and next week)
- File I/O (next week)
- Pass by Reference (Week 8)
- Vectors (Week 9)
- Classes (Week 10)

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Functions

A **_function_** is named block of instructions.

Other terms for functions: **methods, subroutines, routines,** and **procedures**.
<br>

### _Why are functions helpful?_

<v-clicks>

- Help us write cleaner code
- Help us avoid redundancy
- Help us debug
- Help us break down large tasks into smaller easy to solve pieces
- Help us test and verify our program is correct

</v-clicks>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Function Terminology

```cpp {1|14}{class:'!children:text-l'}
double sqrt(double square) {
    
    double current_estimate = square;
    double previous_estimate = 0;

    while(fabs(current_estimate - previous_estimate) < .00001) {
        
        previous_estimate = current_estimate;


        current_estimate = .5 * (current_estimate + (square/current_estimate));
    }

    return current_estimate;
}
```

<v-clicks>

  - `double sqrt(double square)` is called the **function declaration/signature**

<br> 

<AdmonitionType title="Note" type="caution" width="300px" custom="text-xl" v-drag="[21,400,929,55]">
Declarations are <b>ALWAYS</b> written: <b>returnType</b> func_name(<b>type1</b> param1, <b>type2</b> param2, ...) { }
</AdmonitionType>

  - `double sqrt(double square)` paired with `{ /* code statements */ }`, is a **function definition**
  
</v-clicks>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Function Terminology (cont'd)

```cpp {all|1|12}{class:'!children:text-xl'}
int main() {
    double x_0, y_0;
    double x, y;
    cout << "Enter coordinates as separate inputs (e.g 2 5 12 -1):"
    cin >> x >> y >> x_0 >> y_0 >> endl;

    double dx = (x - x_0);
    double dy = (y - y_0);

    cout << "Distance Between Start and Ending Location" 
         << sqrt(dx * dx + dy * dy) << endl;
    return 0;
}
```

- What is the return type of main and what does it return?
- What do we call `sqrt(dx * dx + dy * dy)`?


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Rules for Writing Functions

A VALID function definition includes: 
<v-clicks>

- <b> return type </b>
- <b> function name </b>
- <b> zero or more function parameters </b>
- <b> code block </b>


The code block **must** contain an **accessible** return statement whose argument has the **same type as the return type**.

Accessible means that **every** code path leads to a return statement.

</v-clicks>


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# So You Think You Can Function?

Rules: You will determine if these function definitions are valid or not.

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Counting Character Frequency

```cpp {all}{class:'!children:text-xl'}
int countCharFrequency(char character, string textToSearch) {
    
    int count = 0;

    for(unsigned i = 0; i < textToSearch.length(); i++) {
        if(textToSearch.at(i) == character) {
          count++;
        }
    }

    return count;
}
```


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Hello World

```cpp {all}{class:'!children:text-2xl'}
void helloWorld(string world_name) {
    
    cout << "Hello, " << world_name << "!" << endl;

    return 0;
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Evens and Odds
```cpp {all}{class:'!children:text-2xl'}
bool isEven(num) {
    return num % 2 == 0;
}


bool isOdd(int num) {
    return !isEven(num);
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Integer to String
```cpp {all}{class:'!children:text-2xl'}
string integerToString(int i);


bool isSingleChar(int i) {
  if (integerToString(i).length() == 1) {
    return 1;
  }
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Rules for Calling Functions

- You use a function (known as **calling** a function) by writing `name(arg1, arg2, ...)`.
- Like declaring variables, functions need to be declared before you call them.
- Like with initializing variables, functions need to be defined before you call them. 


---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
::left::
# Tips

<v-clicks>

- **Read the instructions**

- Review C++ fundamentals:
    - Differences between integers, strings, and floats
    - `=` vs `==`
    - Math Operators (specifically `%` vs `/`)
    - String Functions (`at`, `find`, `substr`, `push_back`, `append`)
    - Math Functions (`pow`, `sqrt`, `exp`, etc)

</v-clicks>

::right::

<v-clicks>

- Learn programming templates:
    - Check every character in a string
    - Getting multiple inputs in a row from the user
    - Checking even vs odd
    - Summing and storing a value in a variable
    - Setting and unsetting boolean flags
    - When to use `while` vs `do-while` vs `for`

- Practice, practice, practice.

- Come to Office Hours! 

- Stick around after you're done with lab and ask me questions!

</v-clicks>
