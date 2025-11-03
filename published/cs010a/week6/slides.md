---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
---

# CS 010A Lab 06: Functions 
## 10/28/2025 


---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
url: image.png
```

# Announcements

- Quiz 2 
- Temporarily Move Office Hours for this Week?
- Gradescope
- Mid Quarter Check In

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
# Brief Review

- cin vs cout, formatting
- variables, types, assignment, operations on variables
- branches, booleans, 
- loops (do-while, while, for)
- strings, string operations, character operations, getline,

# What's Left?
- Functions (this week and next week)
- File I/O (next week)
- Pass by Reference 
- Vectors
- Classes

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# What is a function? Why do we need them?

A function is named block of instructions.

<AdmonitionType title="Note" type="note" width="300px" custom="text-lg" v-drag="[44,413,866,84]">
Other common terms for a function include: <b> method, subroutine, routine, and procedure </b>
</AdmonitionType>

_Why are functions helpful?_

<v-clicks>
    - Help us write cleaner code
    - Help us avoid redundancy
    - Help us debug
    - Help us break down large tasks into smaller easy to solve pieces
    - Help us test&verify our program is correct
</v-clicks>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Function Terminology

```cpp {2|15|25}{class:'!children:text-2xl'}

double sqrt(double square) {
    
    double current_estimate = square;
    double previous_estimate = 0;

    while(fabs(current_estimate - previous_estimate) < .00001) {
        
        previous_estimate = current_estimate;


        current_estimate = .5 * (current_estimate + (square/current_estimate));
    }

    return current_estimate;
}

int main() {
    double x_0, y_0;
    double x, y;

    cout << "Enter coordinates as separate inputs (e.g 2 5 12 -1):"
    cin >> x >> y >> x_0 >> y_0 >> endl;

    cout << "Distance Between Start and Ending Location" << sqrt((x - x_0)*(x - x_0) + (y - y_0)*(y - y_0)) << endl;
    return 0;
}

```

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```