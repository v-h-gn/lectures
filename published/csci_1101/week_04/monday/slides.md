---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
---

## Slices and String Methods <twemoji-scissors />

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Recall we can access parts of strings

:: content ::

<br>

#### We can access individual pieces of data inside a string using the `[]` (brackets)

<br>

#### Remember, we start counting from 0!

<br>


|  C  |  h  |  r  |  i  |  s  |
| :-: | :-: | :-: | :-: | :-: |
|  0  |  1  |  2  |  3  |  4  |

<br>

```python {monaco-run} {editorOptions: {lineNumbers:'on', fontSize:20}}
name = "Chris"

print(name[0], name[1], name[2], name[3], name[4])
```

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Slices

:: content ::

#### We can access multiple pieces of data inside a string using the `[]` (brackets) like so:

<br>

#### `my_str[start:end]` where `start` is inclusive and `end` is exclusive!

- #### `start` defaults to 0 if it is not provided!

- #### `end` defaults to the length of the string if it is not provided!

```python {monaco-run} {editorOptions: {lineNumbers:'on', fontSize:16}}
name = "Christopher Martin"

print(name[5:9])
print(name[:5])
print(name[12:])
```

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Slices

:: content ::

|  C  |  h  |  r  |  i  |  s  |  t  |  o  |  p  |  h  |  e  |  r  |    |  M  |  a  |  r  |  t  |  i  |  n  |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
|  0  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 |
