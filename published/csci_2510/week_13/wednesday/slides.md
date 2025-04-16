---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
---

## Why Systems Fail <twemoji-no-entry />
#### Module 6: Safety and Reliability

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: section
color: bowdoin
---

### Last class, we discussed the difference between safety and reliability

<br>

#### Today, we are going to review how software can be unsafe, unreliable, or both along with the different ways failure can occur!

<br>
<br>

### ==What are some of the ways a system can fail?==

---
layout: top-title
color: bowdoin-title
---

:: title ::

# User Errors

:: content ::

## User Errors are issues caused by user mistake, misuse, or misunderstanding as opposed to the system itself being unreliable

<br>

### User errors account for a significant portion of system failures
#### In many cases, systems not being clear to their users results in these types of issues

- #### Overreliance on legacy / outdated systems
- #### Data-entry or integrity errors
- #### Inadequate training or understanding of a system
- #### Misinterpreting system results or output
- #### Inadequate attention / response to problems
- #### Overconfidence in software by users

---
layout: section
color: bowdoin
---

### ==How can we reduce user errors?==

<twemoji-thinking-face v-drag="[868,420,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Avoid User Errors

:: content ::

## In many cases, user errors are the result of systems being unclear or by assuming users know what they are doing <twemoji-zany-face />

<br>

### Here are <u>some</u> ways we can avoid them through UI/UX:

- #### Provide clear instructions and error messages
- #### Be consistent
- #### Ensure the system behaves as a user would expect
- #### Include appropriate input validation to reduce major system failures caused by typos or other errors a person will likely make
- #### Provide users with feedback to understand what the system is doing at any time

==What are some UI/UX features you have encountered that you disliked or felt didn’t work well?==

---
layout: top-title
color: bowdoin-title
---

:: title ::

# "Soft" Developer Errors

:: content ::

## While we hate to admit it, sometimes system failures are our fault...


- #### Incorrect assumptions about how the software will be used
- #### Lack of clear / well-thought-out goals and specifications
- #### Poor management and poor communication among customers, designers, programmers, etc.
- #### Institutional and political pressures that encourage unrealistically low bids, low budget requests, and underestimates of time requirements
- #### Refusal to recognize or admit a project is in trouble
- #### Not planning or designing code to handle unexpected inputs or situations
- #### Going too fast resulting in sloppy work

---
layout: top-title
color: bowdoin-title
---

:: title ::

# "Hard" Developer Errors

:: content ::

- #### Implementation logic mistakes
- #### Insufficient testing
  - Reuse of software from another system without adequate verification
  - Incompatibility between software and hardware or between the application software and the target platform / operating system

- #### Creating inflexible / rigid systems or writing 'unreadable' code

- #### Missing or poor documentation

- #### Overreliance on system dependencies or the use of very new technology with unknown reliability, security, and limited support

- #### Improper use of standardized tooling such as version control

---
layout: section
color: bowdoin
---

### ==How can we reduce developer errors?==

<twemoji-thinking-face v-drag="[868,420,96,89]" />

---
layout: section
color: bowdoin
---

<div v-drag="[80,15,805,503]">

![Software Development Methodologies](https://cdn.brocoders.com/Frame_1206_c584824f9d.png)

</div>

<div v-drag="[79,17,818,53]"><h2>Software Development Methodologies</h2></div>

<div v-drag="[37,464,928,53]"><h3><mark>Research one of these methodologies and summarize it!</mark></h3></div>

---
layout: section
color: bowdoin
---

![Software Development Lifecycle](https://cdn.brocoders.com/6_phases_of_software_development_life_cycle_ce25a52c62.png)

---
layout: section
color: bowdoin
---

<div v-drag="[118,-44,757,627]">

![Types of Software Testing](https://www.techtarget.com/rms/onlineimages/sorftware_quality_test_types-f.png)

</div>

---
layout: top-title-two-cols
color: bowdoin-title
---

:: title ::

# Validation vs Verification

:: left ::

# Validation
### The process of checking whether a system / its design meet the customer's required specifications

<br>

#### Are we building the right system?

:: right ::

# Verification
### The process of checking that a system correctly achieves its specific function without any issues

<br>

#### Are we building the system right?

---
layout: section
color: bowdoin
---

<div v-drag="[137,-7,711,621]">

![Verification vs Validation](https://www.technolush.com/uploads/2019-04-05/banner/verification-validation-medium.png)

</div>

---
layout: section
color: bowdoin
---

# Questions?

<twemoji-thinking-face v-drag="[813,227,96,89]" />
