---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
---

# CS 10A Lab 3: Branching
## 10/07/2025 

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Announcements
- Grades for labs 1 and 2 should be posted. 
- Good luck on your Quiz!
- Changing my office hours.

<div v-drag="[130,89,700,392]">

![](https://github.com/v-h-gn/lectures/blob/main/published/cs010a/week3/image.png?raw=true)

</div>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Booleans and Boolean Expressions

A Boolean (`bool`) holds a value `true` or `false`.

A Boolean expression is a statement containing Boolean values and logical operators.

Ex. `x > 1`, `true OR (y AND z)`


<AdmonitionType title="Warning" type="caution" width="300px" custom="text-lg" v-drag="[50,261,808,77]">
Booleans in C++ are really just integers, where zero is interpreted as false and anything else is true. Be wary of order of operations in Boolean expressions.
</AdmonitionType>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Branch Syntax

**Branch** instructions are used to change the flow of our program based on state or inputs.

In C++, this is accomplished with `if`-`else` statements.

```cpp {all}{class:'!children:text-2xl'}
if (condition1) {
    // if condition1 is true, run this section
} else if (condition2) {
    // if condition1 was false and condition2 is true
    // run this section
} else {
    // if condition1 and condition2 were both false
    // run this section
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# C++ Logical Operators: AND, OR, NOT

AND (`&&`) - evaluates to TRUE when both operands are TRUE.

OR (`||`) - evaluates to TRUE when at least one operand is TRUE.

NOT (`!`)- evaluates to TRUE when input is FALSE and FALSE when input is TRUE.

Ex. Let `a` be TRUE, `b` be false, and `c` be false.

<br>

`a && b` evaluates to FALSE.

`a || c` evaluates to TRUE.

`b || c` evaluates to FALSE.

`!(a && b)` evaluates to TRUE.

`a && !c` evaluates to TRUE.

<AdmonitionType title="Beyond This Course" type="tip" width="300px" custom="text-lg" v-drag="[548,352,373,144]">
AND, OR, and NOT are computed in hardware via gates made of transistors. These three gates are all you need to build a universal computer that can do any other instruction.
</AdmonitionType>

---

```yaml
layout: full
transition: slide
addon:
  - slidev-addon-cpp-runner
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Comparison Operators

C++ allows us to use comparison operators like `>`, `>=`, `==`, `<=`, `<` to compare values and return a bool.

```cpp {all}{class:'!children:text-2xl'}
// ropeLength is a float
if (ropeLength > 50) {
  // invalid state, apply small force to shrink rope length
} else if (ropeLength = 50) {
  // apply rotational force and tension force
} else {
  // don't apply tension
}
```

<v-clicks>

<AdmonitionType title="Warning" type="caution" width="300px" custom="text-2xl" v-drag="[460,197,383,159]">
We never use == to compare floating point numbers. They are often inexact due to precision limits!
</AdmonitionType> 

</v-clicks>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Comparison Operators

C++ allows us to use comparison operators like `>`, `>=`, `==`, `<=`, `<` to compare values and return a bool.

```cpp {all}{class:'!children:text-2xl'}
// ropeLength is a float
if (ropeLength >= 50) {
  // invalid state, apply small force to shrink rope length
} else if (fabs(ropeLength - 50) < .00001) {
  // apply rotational force and tension force
} else {
  // don't apply tension
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Practice Example:

```cpp {all}{class:'!children:text-2xl'}
// packetSize is 512 and transmitReady has value false
if (transmitReady && packetSize > 250) {
    cout << "[INFO] Large packet encountered, " 
         << "size: " << packetSize << " MB. " 
         << "Splitting packet before transmitting."
         << endl;
} else if (transmitReady && packetSize <= 250) {
    cout << "[INFO] Transmitting packet, "
         << "size: " << packetSize << " MB." 
         << endl; 
} else {
    cout << "[INFO] Antenna not ready or in use." << endl;
}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Testing Programs w/ Branches

You need test cases which account for every path your code can take. 

1 test case per branch path minimum.

Exercise: Generating full coverage test cases for previous example.


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Nesting Branch Statements

We can put if-else statements inside of existing if-else statements to create more complex logic.

```cpp {all}{class:'!children:text-2xl'}
if(smokeAlarmOn) {
  if(fireIsSmall)
    useFireExtinguisher();
  else
    callFireDept();
} else {
  // do nothing
}
```

_How many possible branch paths do we have in this code?_ 

_Is this code robust? Would this be good to use in a real life system?_

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# In Lab Exercise 3 Guidelines

Follow instructions IN ORDER and read them CAREFULLY.

One test case per branch-path. 

You must use if-else statements to accomplish the lab.

# Tips on the Zybooks Labs

Review the sections of the Zybooks for branching statements w/ intervals.




---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```


# Questions, Comments, Concerns, Quibbles?
