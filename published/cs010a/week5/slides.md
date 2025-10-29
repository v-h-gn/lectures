---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
---

# CS 010A Lab 05: Strings and For Loops
## 10/28/2025 


---

```yaml
layout: iframe-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
url: https://cutiehack.com
```

# Announcements

- Quizzes
- Fixed Grades
- Cutie Hack

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Strings

A _string_ is a sequence of characters. 

When we see strings represented by double quotation marks, we call them _string-literals_.

Ex. `"Hello, World!"`, `"Happy Halloween!"`, `"Spooky Scary Skeletons"`

We can also declare strings as variables. 

```cpp {hidden|all}
#include <string>
// more above

  string text;

// more below
```


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Checking, Parsing, and Mutating Strings

<table class="table-auto border-collapse w-full text-center">
  <thead>
    <tr class="bg-gray-200">
      <th class="border px-4 py-2">Task</th>
      <th class="border px-4 py-2">C++ Syntax</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="border px-4 py-2">Checking string equality</td>
      <td class="border px-4 py-2" v-click> string1 == string2 </td>
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
      <td class="border px-4 py-2">Check if character is alphabetical</td>
      <td class="border px-4 py-2" v-click>isalpha(string1.at(i))</td>
    </tr>
  </tbody>
</table>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# For Loops

We use for loops when we have an exact number of times we need to iterate.

```cpp {hidden|all}{class:'!children:text-2xl'}
//loop variable init   loop condition   loop variable update
for(    int i = 0;         i <= number;         i++          ) {
  // loop body
}
```

Example: Loop N times
```cpp {hidden|all}{class:'!children:text-2xl'}
for(int i = 0; i < N; i++) {

}
```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Strings and Loops
<br>

```cpp {all}{class:'!children:text-2xl'}
// ... 
  for (int i = 0; i <= userString.length(); i++) {
      char currentChar = _______; // what do we assign to currentChar if we want currentChar to be character at index i.
  }
// ...

```

```cpp {all}{class:'!children:text-2xl'}
// ... 
  for (int i = 5; i > 0; i++) {
      // if current char is the character at index i

      cout << currentChar << " " endl;
  }
// ...

```

 
---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Common Errors / Bad Practices with For Loops

- Incorrect loop variable update, e.g. adding when you meant to subtract
- Off by one bugs (OBOBs), usually caused by using `<=` when you need `<` or vice versa.
- Iterator errors (caused when using strings w/ for loops incorrectly)
- Concurrently modifying your loop variable in your loop expression **not an error, but can lead you to problems in many cases

```cpp {all}{class:'!children:text-2xl'}
for (int i = 0; i < N; i++) {
    // some code here
    i--; // try not to do this EVER
}
```


---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Advice on the Labs

Work incrementally, start by making sure your loop runs the correct number of times, then build more functionality.

Don't forget about while loops! They are still useful!

Use variables, don't just inline expressions, use variables to store things.

Make sure you understand string indexing and your loops don't go beyond the valid indices of your string!


---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Questions, Comments, Concerns, Quibbles?