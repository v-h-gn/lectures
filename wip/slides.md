---
layout: cover
transition: slide
theme: neversink
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
image: image.png
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
C++ denotes what can go on the left and right hand sides of "=" as l-values and r-values.  Errors with these words in them mean you're assigning something incorrectly.
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
# Functions & Math

--- 