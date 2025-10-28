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

A string is a sequence of characters. 

A string literal is when we take text and surround it with `""`

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
      <td class="border px-4 py-2" v-click>string1.substring(startIndex, numChars)</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Appending a character</td>
      <td class="border px-4 py-2" v-click>string1.push_back('X')</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Appending a string</td>
      <td class="border px-4 py-2" v-click>string1.append("Boo!")</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Check if character is a digit</td>
      <td class="border px-4 py-2" v-click>isdigit()</td>
    </tr>
    <tr>
      <td class="border px-4 py-2">Check if character is alphabetical</td>
      <td class="border px-4 py-2" v-click>isalpha()</td>
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
# Another Example: Last Week's Lab
<br>

```cpp {all}{class:'!children:text-2xl'}
// ... 
  cout << userNum << " ";
  for(int i = userNum - 1; i % 11 != 0; i++)
      cout << i << " ";
  cout << endl;
  cout << userNum - i << endl;
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
- Off by one bugs (OBOB), usually caused by using `<=` when you need `<` or vice versa.
- Iterator errors (caused when using strings w/ for loops incorrectly)
- Concurrently modifying your loop variable in your loop expression (not an error, but bad program design)

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

# Spooky Cypher 

You were invited to a Halloween murder mystery party. The host, who is playing the butler, Vahobgoblin Toothmummyan, asked you to help him make a cryptographic message via a simple substitution cypher. 

(Ex. "HELLO WORLD" becomes "AYFFM DMPFK")

1. Given the input message on one line,
2. For each alphabetical character, generate a random character to replace it in the encoded version.
3. Output the new encoded string.

<br>

#### What are some clues in the prompt that guide us towards which functions to use?
<br>

#### Should we try to do the modification in place, or should we create a new variable?
<br>

#### What are some possible bugs that can happen if we aren't careful?


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