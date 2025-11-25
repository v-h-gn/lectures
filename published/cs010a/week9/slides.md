---
layout: cover
transition: slide
theme: neversink
addons:
- slidev-addon-cpp-runner
presenter: true
---

# CS 010A Lab 09: Vectors
## 11/25/2025 

---

```yaml
layout: image-right
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Announcements

- Week 10 Lab 
- Thanksgiving Holiday -> No Office Hours
- IEvals



---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```
::left::
# Vector Type

A **vector** is a finite list of items arranged in some kind of order. All items must have the same data type.

Items in the vector are called **elements**.

#### Declaring a vector: 
`vector<type> myVector(numElements);`

#### Accessing an element at index `i`: 
`myVector.at(i);`

#### Appending an element `e`: 
`myVector.push_back(e);`

::right::

# Array Type

Arrays are also finite ordered lists, but with less supported operations. All items in an array must have the same data t ype.

Array items are also called elements.

#### Declaring an array: 
`<type> myArray[numElements];`
#### Accessing an element at index `i`: 
`myArray[i];`
#### Appending an element `e`: 
Not directly possible in C++

---

```yaml
layout: two-cols
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

::left::
# Vector Pros
- Lots of helpful functions for appending, equality, etc
- Automatic resizing
- Automatic bounds checking & security
- Automatic memory management

# Vector Cons
- Slightly slower than array
- Slightly more memory than array
- Not available in certain environments

::right::
# Array Pros
- Fast
# Array Cons
- Can cause security bugs
- Cannot resize
- No boundary checking
- No functions to help
- Need to manage memory yourself

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Iterating through a Vector

Who remembers how we iterate through a string?

Given a vector of integers named `scoreData`, can you write a function that will visit all of the elements and return the maximum element?

<v-clicks>

```cpp {all}{class:'!children:text-xl'}
int max(const vector<int>& scoreData) {
    int maxInteger = scoreData.at(0);
    for(unsigned i = 0; i < scoreData.size(); i++) {
        if(scoreData.at(i) > maxInteger) {
            maxInteger = scoreData.at(i);
        }
    }
    return maxInteger;
}
```

</v-clicks>

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Putting Data Into a Vector

```cpp
#include <iostream>
#include <vector>
using namespace std;

int max(const vector<int>& scoreData);

void collectUserInput(vector<int>& values, const unsigned numElements) {
    cout << "Enter " << NUM_ELEMENTS << " integer values..." << endl;
    for (unsigned i = 0; i < NUM_ELEMENTS; ++i) {
        cout << "Enter value for next element: ";
        cin >> val;
        userVals.push_back(val);
    }
}

int main() {
    const int NUM_ELEMENTS = 8;      // Number of elements to add
    vector<int> userVals;            // Empty vector for user values

    collectUserInput(userVals, NUM_ELEMENTS);
    cout << "Maximum element is: " << max(userVals) << endl;
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

# Other Operations on Vectors

<br>

#### Checking last element: `myData.back()` 

<br>

#### Removing and retrieving last element: `myData.pop_back()` 

<br>

#### Checking equality: `myVector1 == myVector2`

<br>

#### Copying a vector: `myVector1 = myVector2`

<br>

#### Resizing a vector: `myVector1.resize(newSize)`

---

```yaml
layout: full
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Tips For Vectors

- Be careful when removing elements in a vector while simultaneously iterating.
- If you want a function to modify a vector, use pass by reference
- If don't want or need modification, use `const` + pass by reference (why?)
- Always always always use `vector::at()`.

# Tips on Labs and Quizzes
- Read the Zybooks.
- Practice using Additional Labs and Optional Labs
- Email or post on Edstem if you get stuck.


---

```yaml
layout: center
transition: slide
dragPos:
  square: Left,Top,Width,Height,Rotate
```

# Questions, Comments, Concerns, Quibbles?

