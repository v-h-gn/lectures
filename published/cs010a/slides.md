---
layout: cover
transition: slide
theme: neversink
---

# CS 10A Lab 1: Intros and I/O

## 9/30/2025

---

```yaml
# The first yaml block will be treated as the frontmatter of that slide
layout: image-left
image: vhgn-formatted.png
```

# Who am I?

- Va-HAH-gun, like Va-Haagen Dazs.

- 2nd Year PhD Student 

- Research: computational biochemistry, lab tech automation

- B.S. in CEN & Pure Math @ UCR 

- 6 years of C++ experience

- Former Supplemental Instructor (SI) and tutor.

- Email: vtovm002@ucr.edu

- Office Hours: TBD

---

```yaml
layout: full
```
# Student Expectations

- Being on time, attending every week. (Excessive lateness (>15 min) will get you points docked.)
- Working in pairs. (assigned by TA via icebreaker, randomly, or hat-pull.)
- Turn in your worksheet once you are done. (Don't use phones or laptops to look up answers.)
- Leave only once you are done or stay and work on your Zybooks labs and exercises.

# TA Expectations
- Helping you learn C++ and succeed in this class.
- Being prompt about submitting your grades.
- Maintaining a safe and productive learning environment.
---

```yaml
layout: full
```

# Review: Hello, CS010A! - C++ Output

Let's review some of the basic elements of a C++ program before your exercises.

```cpp {hide|1-4|6|8|10,12|11}{lines:true}
/*
    Author: Vahagn Tovmasian
    Date: 9/30/2025
*/

#include <iostream>

using namespace std;

int main() {
    cout << "Hello, CS10A!" << endl;
}
```



---

```yaml
layout: full
```

# Review: Multiple Sections? - C++ Input

A lot of times, we want to be able to get data from the external world and give it to our program. 

We do this via **input** statements, like `cin`. 


```cpp {all|6,8|6,10}{lines:true}
#include <iostream>

using namespace std;

int main() {
    int sectionNumber;

    cin >> sectionNumber;
    
    cout << "Hello, CS10A Lab Section " << sectionNumber << "!" << endl;
}

```

**TIP:** The _operator_ you use with  `cin` or `cout`, corresponds to the _direction_ you want to move data.

`cin` takes data from the console and puts it into a *variable*, so `cin >> variableName;`

`cout` takes data from your variables/values and outputs it to the console. `cout << outputResult;`


---

# Advice On The In Lab Exercise and ZyBooks Labs

- Read instructions carefully, _precision_ is key. 
- Do not sabotage your learning by looking up the answer online or asking AI.

## Common/Expected Mistakes
- Forgetting semicolons `;`
- Using the wrong stream operator `<<` vs `>>`for `cout` and `cin`
- Whitespace errors ex. `Hello World! `  vs `Hello World!`
- Not using `endl` to print to a new line.

---

```yaml
layout: center
```

# Questions, Comments, Concerns, Quibbles?