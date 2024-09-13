---
layout: cover
theme: neversink
color: bowdoin
routerMode: hash
---

## Data Types

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Types of Data

:: content ::

<br>

Data makes up every fundamental aspect of a program but not all data is the same. Some forms of data are complex or ==composite== while others are more simple.

An example of this could be an image. In an image, each pixel is stored as three color values and the combination of all them makes up what we see. The image itself is complex while the individual color values are simple.

<br>

We say that types of data that are so simple they cannot be broken down any further are ==primitive==.

<br>

So far, we have seen some examples of simple data but there are many more types of data to come!

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Primitive data

:: content ::

<br>

<u>Computers store different kinds of primitive data in different ways, for example:</u>  

A whole number / integer, or just ==int== for short,  is stored as an ascending scale of values in binary:

- `0000` is `0`, `0001` is `1`, `0010` is `2`, `0011` is `3`, etc

A real number / floating-point value, or just ==float== for short, is stored in scientific notation.   
This goes outside the scope of our class but here is how `10.5` is stored:

- `0 10000010 01010000000000000000000` 🤔❓ 

Text / string data, or just ==str== for short, is stored in a similar way but each binary arrangement corresponds to a character. Then, these characters are 'strung' together to form sequences.

- `1000001` is `A`, `1000010` is `B`, `1000011` is `C`, etc

Some of you may note that it is the individual characters that are primitive, not the string itself!

---
layout: top-title
color: bowdoin-title
---

:: title ::

# The `type` Statement

:: content ::

In Python, we can determine the type of a value using the `type()` statement.

The `type()` statement will evaluate to the final data-type of whatever expression is provided to it.

<br>

Let's see some examples!

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
print(type(5))
print(type(1.5))
print(type("Hello!"))
```

<br>

For right now, we can ignore the `class` part of the output and focus on the right-hand section.  

In it, we see our familiar `int`, `float`, and `str`!

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Types of Variables

:: content ::

<br>

Variables store the type of data they hold but will update as their data changes:

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
answer = 5 + 5
print("answer's type is", type(answer))

answer = 7.5 - 2.3
print("answer's type is", type(answer))

answer = "I don't know"
print("answer's type is", type(answer))
```

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Expressions with Different Types

:: content ::

<br>

Sometimes, expressions involve multiple types.

When this happens, the result will usually be the "larger" of the types.  

This ensures that if you end up outside the range of the "smaller" type you will still get a valid answer.

<br>

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
answer = 7.5 - 2 # 7.5 is a float and 2 is an int
print(answer, type(answer))
```

<br>

`int` is considered "smaller" than `float` because it can't store as many unique values.

Due to this,  we will always get a `float` when evaluating an arithmetic operation that mixes the two.

---
layout: side-title
titlewidth: is-2
align: cm-lm
color: bowdoin-title
---

:: title ::

# Division

:: content ::

The division breaks this rule slightly.

<br>

Whenever we use the `/` operator, we will always get back a `float` result.

This happens even if the two operands are `int`.

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
answer = 4 / 2
print(answer, type(answer))
```

<br>

If you want the possibility of getting an `int`, you must use the `//` operator:

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
answer = 4 // 2
print(answer, type(answer))
```

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Different behavior for different things

:: content ::

<br>

Sometimes, we reuse the same operators for different types of data.

<br>

A simple example of this is how we can use the `+` operator on `str` data!

This "joins" or ==concatenates== the two strings together!

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
answer = "Mon" + "day"
print(answer)
```

<br>

This is kind of similar to what `+` does to numbers but acts differently for a different type of data.

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Type incompatibilities

:: content ::

<br>

Sometimes, we run into a situation where we cannot perform the operation we want because some of the data isn't the matching type for what we want to do:

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
# It is not possible to 'add' strings and other types
answer = "The temperature is " + 58.5
```

<br>

In these situations, we can ask the computer to convert a value from one type to another.

This is referred to as ==type casting==.

---
layout: side-title
titlewidth: is-2
align: cm-lm
color: bowdoin-title
---

:: title ::

# Type casting

:: content ::

To type cast in Python, we use the name of the type we want to convert to like a function and pass in what we want to convert.

For example:

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
print(type(str(5)))       # Converts the int value 5 into the string "5"
print(type(float("3.5"))) # Converts the string "3.5" into the float value 3.5
print(type(int(3.0)))     # Converts the float value 3.0 into the int value 3
```

<br>

This becomes especially important when the data coming into our program is being entered as text because the user is typing it in or it is coming from a file.

We will need to convert those strings into their actual values in the correct type before we can use them

---
layout: side-title
titlewidth: is-2
align: cm-lm
color: bowdoin-title
---

:: title ::

# Limitations

:: content ::

Type casting only works if the value you are attempting to convert can be represented somehow as a value in the other type:

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
# The string value "Hello" cannot be represented as an int
int("Hello")
```
