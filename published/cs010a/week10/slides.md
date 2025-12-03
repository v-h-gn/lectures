---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
presenter: true
---

# CS 010A Lab 10: Review
## 11/25/2025 

---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Announcements

- IEvals
- Grades

<img src="https://raw.githubusercontent.com/v-h-gn/lectures/refs/heads/main/published/cs010a/week10/qr-code.png" v-drag="[-8,0,0,0]">

<img src="https://www.meme-arsenal.com/memes/ca21a3770c05da1a7bb8fcb8119191ca.jpg" v-drag="[638,288,303,224]">

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Variables and Naming

<br>

### A **_variable_** is a named container used to *store data* needed by our program.

<br>

### Variable names can only use alphanumeric characters `(a-Z,0-9)` and underscores. 

<br>

#### **Ex:** `numStudents`, `player1_name`, or `_playerScore`

<br>

Which of these is/are valid variable declarations?

A. string 1stName; 
B. int numStudents[10]; 
C. ifstream for;
D. vector data;
E. int& intRef;

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Operator Precedence

<v-clicks>

1. Unary operators: `!` (logical not), `-` (unary minus)

2. Multiplication, modulo, and division (`*, %, /`)

3. Addition, subtraction (`+, -`)

4. Logical AND (`&&`)

5. Logical OR (`||`)

6. Assignment and compound operators (`=`, `*=`, `+=`, `/=`, `-=`, `%=`)

</v-clicks>


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

<table class="table-auto border-collapse w-full text-center">
  <thead>
    <tr class="bg-gray-200">
      <th class="border px-4 py-2">String Operation</th>
      <th class="border px-4 py-2">C++ Syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="border px-4 py-2">Checking string equality</td>
      <td class="border px-4 py-2" v-click> string1 == string2 </td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Getting string length</td>
      <td class="border px-4 py-2" v-click>string1.length() or string1.size()</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Getting character at index i</td>
      <td class="border px-4 py-2" v-click>string1.at(i)</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Getting a substring between two indices</td>
      <td class="border px-4 py-2" v-click>string1.substr(startIndex, numChars)</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Appending a character</td>
      <td class="border px-4 py-2" v-click>string1.push_back('X')</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Appending a string</td>
      <td class="border px-4 py-2" v-click>string1.append(string2)</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Check if character is a digit</td>
      <td class="border px-4 py-2" v-click>isdigit('9')</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Check if character is alphanumeric</td>
      <td class="border px-4 py-2" v-click>isalphanum('a')</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Check if character is alphabetical</td>
      <td class="border px-4 py-2" v-click>isalpha(string1.at(i))</td>
    </tr>
  </tbody>
</table>

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

void prettyPrint(const double& avg, 
                 const double& std, 
                 const string& data_name) {
    cout << data_name 
    << " mean & std_dev: " 
    << avg << " +/- "<< std << endl;
}

int main() {
    prettyPrint(30.0, 7.5, "Current (mA)");
    // outputs "Current (mA) mean & std_dev: 30.0 +/- 7.5
    prettyPrint(85.2, 11.3, "Lab Attendance (%)")
    return 0;
}

```
</v-clicks>

---

```yaml
layout: full
transition: slide
```
# Pass By Reference
C++ has two ways we can pass variables to functions

#### Pass by value
Creates a local copy within the function of the argument

#### Pass by reference
Avoids copying, any modifications that occur within the function will also occur to the argument variable


#### When do we use pass by value?

<v-clicks> 

Small data types: ints, bools, chars, floats, etc 

</v-clicks>

#### When do we use pass by reference?

<v-clicks> 

Big data types: vectors, strings, classes/objects

</v-clicks>



---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Questions, Comments, Concerns, Quibbles?
