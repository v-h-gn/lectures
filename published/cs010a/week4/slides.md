---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
---

# CS 10A Lab 4: Loopy Randomness
## 10/21/2025 

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Announcements

- Lab 3 Grades 
- Quiz 1
- Office Hours

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Random Number Generation in C++ (RNG)
<v-clicks>

Random numbers are important for simulating lots of things.

<br></br>

In C++, we use `rand()` (requires `#include <cstdlib>`) to _pseudorandomly_ generate number.

`rand()` generates an integer between `0` and `RAND_MAX`. 

<br></br>

How can we restrict its output to a desired set of integers?

Ex. Randomly output numbers between 11-110

_Hint 1: How many integers are in $[11,110]$ and how many are in $[0,99]$?_

_Hint 2: When dividing an integer $x$ by another integer $n$, what values can the remainder have?_

_Hint 3: What C++ operator computes the remainder, and how can we turn $[0,99]$ into $[11,110]$?_


</v-clicks>


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Loops and Iterative Programming
<v-clicks>

A _loop_ is used to repeatedly perform instructions. We'll focus on `do`-`while` and `while` loops for now.

<br>`do`-`while` loops runs the code in the loop body FIRST, then check the loop condition.</br>

`while` loops check the loop condition FIRST, then they run the code in the loop body.

</v-clicks>

---

```yaml
layout: two-cols
transition: slide
addon:
  - slidev-addon-cpp-runner
dragPos:
  square: Left,Top,Width,Height,Rotate
```

<AdmonitionType title="Beyond This Course" type="tip" width="300px" custom="text-lg" v-drag="[44,413,866,84]">
In hardware, all loops are usually implemented as do-while loops. This is because it needs less machine instructions.
</AdmonitionType>


::left::

# Do-While Syntax

<br>

```cpp
int difficultClass = 10;
int successes = -1;

do {
    // loop body
    successes += 1;
    cin >> playerRoll;
} while(playerRoll >= difficultyClass)
```

## Notes
- Always runs at least once
- Can feel more natural for certain programs/algorithms

::right::

# While Syntax
```cpp
int difficultClass = 10;
int successes = 0;
cin >> playerRoll;
while(playerRoll >= difficultyClass) {
    // loop body
    successes += 1;
    cin >> playerRoll; 
}
```

## Notes
- May not run at all (sometimes this is desired)
- Can require repetition

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# ILE Rubric

- On Time and On Task / Effort (2)
- Code Plan (1)
- Test Cases (1) 
- Executable Code (1)

# Comments on Lab 3

A handful of you lost points because you didn't have any code plan or test cases. 

Partial points were docked for major syntax errors, not matching the output exactly, or not having enough testcases.

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Elements of a Good Code Plan

- Written in plain English 
- Easy to understand
- Avoids C++ specific terminology (cout/cin, if-else, etc)
- Performs according to client specification.

# What I am Looking For 

Did you read the instructions and come up with a plan before you started writing your code/test cases? 

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Elements of Good Testing
- Provides both Input and Expected Output
- Sufficient in number to verify execution of your program
- Verifies edge cases and normal cases

# Questions To Ask Yourself
What happens if some of my inputs are non-existent?

What happens if some of my inputs are bigger or smaller than I expect? 

What happens if some inputs are equal?

# What I am Looking For
Did you think about how to verify that your program is correct before you actually wrote it? Did you think about what are good test cases before you wrote them? (i.e not just random numbers)

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Tips for In Lab Exercise & Zybooks

- Read the instructions VERY carefully
- Write down important information from the instructions. (This will help with your code plan!)
- Break down the task into smaller more manageable pieces. (This will help with your code plan and writing code!)

# Tips for Zybooks Specifically
- Remember the structure of getting input before the while loop and also at the very end of the loop body.
- Loops execute their loop body when the condition is TRUE.


---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Questions, Comments, Concerns, Quibbles?
