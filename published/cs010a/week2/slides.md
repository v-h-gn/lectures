---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
---

# CS 10A Lab 2: Variables, Assignments, and Math
## 10/07/2025 

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Variables

<br>

### A **_variable_** is a named container used to *store data* needed by our program.

<br>

### Variable names can only use alphanumeric characters `(a-Z,0-9)` and underscores. 

<br>

#### **Ex:** `numStudents`, `player1_name`, or `_playerScore`


<br>


### Good variable names are **_critical_**. 
### Two accepted naming styles in C++: camel case and underscore separated. 

<br>

#### Camel Case: `musicVolume`, `isHavingGoodTime`, `arrivalTime`

#### Underscores: `heater_temperature`, `dining_hall_menu`, `wifi_speed`
<br>

### Whichever you choose, or are told to use, you must be **_consistent_**.
---

```yaml
layout: image-right
dragPos:
  square: Left,Top,Width,Height,Rotate
image: https://raw.githubusercontent.com/v-h-gn/lectures/refs/heads/main/published/cs010a/week2/example-code.png
backgroundSize: 25em 95%
```

# Variables (cont'd)

<br>

### Does this code follow good naming style?

<br>

<v-clicks>

- Style changes between different variables

- Does not follow common C++ style

- Undescriptive names (e.g. `joy_x, y`)

</v-clicks>


---

```yaml
layout: full
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Assignment Statements

<br>

### We use `=` to **_assign_** values to variables.

<AdmonitionType type="caution" width="300px" v-drag="[587,76,300,69]">
Do not confuse this symbol with "equals". It does not mean equality!
</AdmonitionType>

<br><br>

### Only variables can go on the left hand side of `=`, and only expressions can go on the right hand side. 

<br>

### Valid   ✅: `goodVariableName = 0`, `x = x + 1`, or `myName = myName` 

### Invalid ❌: `0 = sum`, `counter * 2 = counter`
<br>


<AdmonitionType title="Beyond This Course" type="tip" width="300px" custom="text-lg" v-drag="[68,396,808,77]">
C++ denotes what can go on the left and right hand sides of "=" as l-values and r-values.  L-value or r-value errors mean you are doing an invalid assignment.
</AdmonitionType>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Types of Variables
<br>

### Every variable in C++ has a defined type which never changes. The type defines the format and type of data it can store.

<br>

### What are some of the types we've seen so far?


- char, int, long, long long, short
- float, double
- string

### Why is `char` grouped with the other numeric types and not w/ `string`?

<br>
---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
addons:
  - slidev-addon-cpp-runner
```

# Type Casting

We use `static_cast<type>` to convert between types.

Ex. `double current = static_cast<double>(voltage)/resistance`

In what situations would we need to do this?

<v-clicks>

```cpp {monaco-run}
#include <iostream>
using namespace std;

int main() {
  int numDevicesVahagn = 4;
  int numDevicesPrithviraj = 3;
  int numDevicesMarios = 7; 
  int numDevicesRB = 5;
  int numDevicesYi = 2;

  cout << "Average Number of Devices: " << (numDevicesVahagn + numDevicesPrithviraj 
                                          + numDevicesMarios + numDevicesRB + numDevicesYi) / 5 << endl;
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
addons:
  - slidev-addon-cpp-runner
image: https://github.com/v-h-gn/lectures/blob/main/published/cs010a/week2/orderofoperations.png?raw=true
backgroundSize: 25em 55%
```

# Arithmetic Expressions

C++ supports $+, -, \times{}, /$ and modulo $\%$.  

These standard operators also have compound versions: `+=, -=, *=, /=, %=`

Ex. `a *= b` is equivalent to `a = a * b`

 `#include <cmath>` allows you to use functions like `sin, sinh, log, ln, sqrt(x), pow(x,b)` and others

 That's all you need to do math in C++!

<AdmonitionType title="Fun Fact" type="info" width="300px" v-drag="[102,389,338,99]">
Compound operators in C++ are an example of <b>syntactic sugar</b>. Syntactic sugar is syntax which makes writing code easier w/o introducing new functionality.
</AdmonitionType>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
addons:
  - slidev-addon-cpp-runner
```

# What would this be in C++?
<div v-drag="[130,89,700,392]">

![](https://static.boredpanda.com/blog/wp-content/uploads/2019/08/5d42cc877887a-png__700.jpg)

</div>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
addons:
  - slidev-addon-cpp-runner
```

# Let's Run It

```cpp {monaco-run}
#include <iostream>
using namespace std;

int main() {
  int answer = 8 / 2 * (2+2);
  
  answer = answer;

  float finalAnswer = 0.0 / 0.0;
  
  cout << "Is it 1 or 16?" << endl;
  cout << "Final Answer: " << finalAnswer << endl;
  
  return 0;
}

```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
addons:
  - slidev-addon-cpp-runner
```

# Working w/ Floating Point

Numbers with fractional parts (1.5, 3.14, 2.71828, etc) are represented using `float` and `double` in C++.

`double` is more precise than `float` ($2^{-53}$ vs $2^{-23}$)

We use `fixed` to output floating points in fixed point notation. 

`setprecision(int)` sets the number decimal figures printed equal to the integer you pass into it.

```cpp {monaco-run}
#include <iostream>
#include <iomanip>
#include <cmath>

using namespace std;

int main() {
  cout << fixed << setprecision(3) << sqrt(2) << endl;
  return 0;
}
```

<AdmonitionType title="Note" type="caution" width="300px" v-drag="[593,277,197,152]">
Floating point calculations often have rounding and truncation errors. This can lead to computed answers being off from the real solution.
</AdmonitionType>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
addons:
  - slidev-addon-cpp-runner
```

# Tips for the Labs

Read instructions carefully

Don't worry about formatting outputs with `setprecision()`

# Expected/Common Errors

Not understanding modulo operations

Mixing up integer vs floating point division / not casting correctly.





---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
addons:
  - slidev-addon-cpp-runner
```

# Questions, Comments, Concerns, Quibbles?
