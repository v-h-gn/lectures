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
layout: image-right
image: https://github.com/v-h-gn/lectures/blob/main/published/cs010a/week1/vhgn-formatted.png?raw=true
```

# About Me

- va-HAH-gun, like va-Haagen Dazs.

- Email: vtovm002@ucr.edu

- Office Hours: TBD

- 2nd Year PhD Student, B.S. in CEN & Pure Math from UCR 

- Research: computational biochemistry, lab tech automation

- 6 years of C++ experience

- Fun Fact: I can speak 4 languages. 

---

```yaml
layout: full
```
# About the Lab

- Meets once a week for the entire quarter.
- Reinforces what you learn in lecture via TA presentation and **In Lab Exercises (ILE)**
- **ILEs** will be done in pairs on a worksheet I give you. 
- **ILEs** will be graded based on **completion** and **effort**, not correctness.
- There will be an opportunity to make up a missed lab later in the quarter.
- You may attend another scheduled lab section **ONCE** this quarter by notifying us on EdStem, more details will be given later.

---

```yaml
layout: full
```
# Student Expectations

- Being on time, attending every week. 
- Engaging with the material.
- Collaborating with peers. One person should not be doing all of the work. 
- Respecting your peers.

# TA Expectations
- Helping you learn C++ and succeed in this class.
- Maintaining a safe and productive learning environment.
- Providing effective and prompt feedback.

---

```yaml
layout: full
```

# Review: Hello, CS010A! - C++ Output

```cpp {hide|1-3|4-5|7,10|8|9}{lines:true}
/*  Author: Vahagn Tovmasian
 *  Date: 9/30/2025
 */
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, CS010A!" << endl; // prints Hello to the class
    return 0;
}
```
<v-clicks>

- Block comment, group comment
- `#include` directive and `namespace`
- `main` function -> the first function to execute in any C++ program
- Print statement, output statement, and line comment
- `return` statement

</v-clicks>

---

```yaml
layout: full
```

# Review: Complex I/O - C++ Input
I want to design a program which given 3 inputs, `sectionNumber`, `endingHour`, and `ending Minute` of my lab section, greets and tells the user how long until the lab is over in hours and also total minutes.

I want the output to look like the following:

For `28`, `1`, and `50`:

```
Hello, CS 010A Lab Section 28!
Your lab ends in 1 hour(s) 50 minute(s).
Total minutes: 110
```

<v-clicks>

- Can you help me come up with a plan for how to program this?
- How can we test that the program is correct? 

</v-clicks>


---

```yaml
layout: full
```

```cpp {hide|1-5|6,7|6-13|16|18|19|all}{lines:true}
#include <iostream>

using namespace std;

int main() {
    int sectionNumber;
    cin >> sectionNumber; // why are we using sectionNumber here?
    
    int endingHour;
    cin >> endingHour;

    int endingMinute;
    cin >> endingMinute;

    // output Hello for specific lab section
    cout << "Hello, CS010A Lab Section " << sectionNumber << "!" << endl;
    // output lab ending time and total minutes to user
    cout << "Your lab ends in " << endingHour << " hour(s) " << endingMinute << " minute(s)." << endl;
    cout << "Total minutes: " << endingHour * 60 + endingMinute << endl; 
    return 0;
}
```

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