---
layout: top-title
color: bowdoin-title
---

:: title ::

# Repetition

:: content ::

#### As we program, we may find ourselves rewriting the same code over and over again.

<br>

For example, say we were writing a calculation program to help us check some of our math homework.

<br>

Using the midpoint formula:

$$
M = \left( \frac{x_1 + x_2}{2}, \frac{y_1 + y_2}{2} \right)
$$

<br>

1. Find the midpoint of the line segment connecting the points $A(2, 3)$ and $B(6, 7)$.

2. Find the midpoint of the line segment connecting $P(-4, -1)$ and $Q(2, 5)$.

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Repetition

:: content ::

#### We could implement our program like so:

```python {monaco-run} {editorOptions: { lineNumbers:'on'}}
a_x = 2
a_y = 3

b_x = 6
b_y = 7

ab_x = (a_x + b_x) / 2
ab_y = (a_y + b_y) / 2
print("The midpoint is (", ab_x, ",", ab_y, ")")

p_x = -4
p_y = -1

q_x = 2
q_y = 5

pq_x = (p_x + q_x) / 2
pq_y = (p_y + q_y) / 2
print("The midpoint is (", pq_x, ",", pq_y, ")")
```