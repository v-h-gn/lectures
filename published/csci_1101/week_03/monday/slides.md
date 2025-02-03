---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
---

## Booleans and Asking Questions <twemoji-red-question-mark />

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Booleans

:: content ::

<br>

# A boolean or `bool` is a ==primitive== data type that is only represented by either `True` or `False`.

<br>

#### In Python, they are always capitalized: `True` and `False`.

<br>

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on', fontSize:16}}
# Assigning Boolean literals to variables
is_snowing: bool = True
is_sunny: bool = False

print("Is it snowing? ⛄", is_snowing)
print(f"Is it sunny? 🌞 {is_sunny}")
```

---
layout: section
color: bowdoin
---

### Okay, but how often will I use `True` or `False`?

<br>

#### By themselves? Probably not very often.. However, `True` and `False` are used heavily because they are the result of a new type of expression!

<twemoji-thinking-face v-drag="[825,376,90,90]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Relational Operators

:: content ::

## Relational operators allow us to ask basic questions about the state of our program's data. Here are the questions we can ask:

<br>

| Human Operator           | Python Symbol | Example Expression |
| :----------------------: | :-----------: | :----------------: |
| Equal to                 | `==`          | `5 == 5.0`           |
| Not equal to             | `!=`          | `True != False`           |
| Greater than             | `>`           | `7.0 > 3`            |
| Less than                | `<`           | `"A" < "B"`            |
| Greater than or equal to | `>=`          | `4 >= 4`           |
| Less than or equal to    | `<=`          | `3.5 <= 5.0`           |

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Relational Operators

:: content ::

<br>

## The result of these relational expressions will be a `bool` value.

<br>

## This allows us to store the result of asking a question and potentially use that answer later in our program.

<br>

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on', fontSize:16}}
word_1: str = "Apple"
word_2: str = "Banana"

in_order: bool = word_1 < word_2

print(f"{word_1} comes before {word_2}? {in_order}")
```
---
layout: section
color: bowdoin
---

### Okay, so we can get meaningful `bool` values..

<br>

### But what can we actually do with them?

<twemoji-thinking-face v-drag="[825,376,90,90]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# The `if` Statement

:: content ::

#### An `if` statement, also called a "conditional" statement, allows us to ask questions about the state of data and *"conditionally"* execute code based the result.

<br>

#### `if` statements can evaluate <u>any</u> `True` or `False` expression!

<br>

#### Any indented code under the if statement only executes if the expression (also called the condition) evaluates to `True`. If the condition is `False`, the code doesn't run!


```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on', fontSize:14}}
temperature: float = 31.5 # Try changing the temp to see what happens!

if temperature < 32.0:
    print("It is freezing! 🥶")
    print("Maybe it will snow! ⛄")
print("Not inside of the if! 🤪")
```

---
layout: top-title
color: bowdoin-title
---

:: title ::

# The `else` Clause

:: content ::

#### We can optionally add an `else` clause to `if` statements that defines alternative code to runs in the event that the `if` statement's condition evaluates to `False`.

<br>

#### Each `if` statement can only have one `else` clause.

<br>

#### An `else` must be at the same indentation level as its corresponding `if` statement.

<br>

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on', fontSize:14}}
password: str = "1234"

if password == "1101S25":
    print("Welcome to our CodeRunner! ✅")
else:
    print("That password is incorrect! ❌")
    print("Please try again!")
```

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Nesting

:: content ::

<twemoji-nesting-dolls v-drag="[854,86,90,90]" />

#### We can ==nest== conditional statements inside of other conditional statements!

<br>

#### We can also put conditional statements inside of functions!

<br>

```python {monaco-run} {autorun:true, editorOptions: { lineNumbers:'on'}}
def check_number(num: int) -> bool:
    if num == 0:
        return f"{num} is zero!"
    else:
        if num > 0:
            return f"{num} is positive!"
        else:
            return f"{num} is negative!"

print(check_number(10))
print(check_number(-5))
print(check_number(0))
```
