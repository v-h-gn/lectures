---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
drawings:
  persist: true
addons:
  - slidev-addon-python-runner
---

## Ethics and Cybersecurity <twemoji-locked />
#### Module 3: Security

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: section
color: bowdoin
---

## Last week, we talked about what security is and the different types of malware!

<br>

### Now, our focus will be to contextualize this knowledge to showcase the importance of your ethical / security obligations as a developer!

<br>

#### ==What obligations do you think you have as a developer in regards to security?==

<twemoji-thinking-face v-drag="[861,419,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Computer Fraud and Abuse Act of 1986

:: content ::

# Computer Fraud and Abuse Act (CFAA) of 1986
##### Criminalized the intentional use of a computer without authorized access!

<br>

#### Has been amended to treat the following as computer crimes:
- Knowingly accessing a protected computer without authorized access
- Knowingly exceeding authorization access to obtain confidential information
- Knowingly participating in the transmission of a program, code, or series of digital information with the intent to harm a computer system
- Intentionally causing damage to a protected computer system
- Knowingly using another individual’s password or access key to access a protected system
- Trafficking passwords related to a protected computer
- Extortion that involves the use of a computer

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Types of Hackers

:: content ::

# Recall that ==hacking== involves intentionally gaining unauthorized access to computer systems


<br>

## Accessing a system without permission is still
## considered hacking even if your goal is to do good!
### There are three main categories of "hackers" distinguished by this idea:
- #### White Hat
  Hack into systems <u>with permission</u> to uncover weaknesses in order to fix them
<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-02-1.svg" v-drag="[185,308,45,45]">
- #### Grey Hat
  Hack into systems <u>without permission</u> to explore, usually without malicious intent
<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-03-1.svg" v-drag="[185,379,45,45]">
- #### Black Hat
  Hack into systems <u>without permission</u> to uncover weaknesses and exploit them
<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-01-1.svg" v-drag="[185,452,45,45]">

<twemoji-laptop v-drag="[753,107,154,143]" />
<twemoji-locked v-drag="[796,138,71,66]" />
<twemoji-astonished-face v-drag="[857,168,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Some more types of Hackers!

:: content ::

- #### Blue Hat
  Employed White Hat hackers who test the security of their employer's systems
- #### Red Hat
  Vigilante Grey Hat hackers who fight back against Black Hat hackers
- #### Hacktivists
  Black Hat hackers who gain access to systems with the goal of expose secrets for a "just" cause
- #### Cyberterrorists
  Black Hat hackers who disrupt critical infrastructure to advance an ideology or spread fear
- #### State-sponsored Hackers
  Employed by governments to hack the systems of rival governments and organizations
- #### Malicious Insiders
  Black Hat hackers with a personal goal of acting maliciously towards their employer

<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-04-1.svg" v-drag="[170,82,45,45]">

<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-06-1.svg" v-drag="[170,155,45,45]">

<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-08-1.svg" v-drag="[197,226,45,45]">

<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-14-1.svg" v-drag="[242,301,45,45]">

<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-18-1.svg" v-drag="[345,369,45,45]">

<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-17-1.svg" v-drag="[269,441,45,45]">

<twemoji-fearful-face v-drag="[871,71,96,89]" />

---
layout: section
color: bowdoin
---

# Script Kiddies
  ### Amateur hackers who use tools created by others

<br>

#### Script kiddies are still dangerous!
They often don’t fully understand the damage they can do with the tools they use

<img src="https://www.avast.com/hubfs/New_Avast_Academy/white_hat_vs_black_hat_hackers_academy_refresh/icon-09-1.svg" v-drag="[384,180,64,64]">

<div v-drag="[457,191,141,41]"><h3>(You <twemoji-index-pointing-at-the-viewer/>)</h3></div>

---
layout: section
color: bowdoin
---

### These are just some of the classifications!

<br>

#### ==What factors distinguish an ethical hacker from an unethical hacker?==

<br>

#### ==What can we do to prevent some of these types of malicious hackers==
#### ==from accessing the systems we create?==

<br>

#### ==Which was the most surprising type of hacker to learn about?==

<br>

#### ==Which type of hacker do you think is the most dangerous?==

<twemoji-thinking-face v-drag="[861,419,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Cyberattacks

:: content ::

# Last class we discussed many different types of malware
### These only represent a small portion of attack methods hackers use!

<br>

### After the rise of the internet in the late 1980s and 1990s, many hackers began to leverage weaknesses in network communications and websites!

<br>

# This led to the rise of ==cyberattacks==
### Malicious and deliberate attempt by an individual or organization to breach or disrupt a system or a system's data

---
layout: section
color: bowdoin
---

### Today, we are going to discuss different types of vulnerabilities and the cyberattacks that exploit them with the goal of showing how they are avoidable!

<br>

#### During upcoming demonstrations, I will be facilitating these types of attacks on you!
<u>You are not required to participate if you do not feel comfortable with the idea of me "hacking" you!</u>

<br>

#### I received special permission to showcase these topics to you in an educational way!
Without permission, performing these types of activities is considered <u>**unethical**</u> and <u>**illegal**</u> hacking!

---
layout: top-title
color: bowdoin-title
---

:: title ::

# First time offence punishments under CFAA

:: content ::

<div v-drag="[55,73,398,52]">
<h4>Obtaining national security information</h4>
<h5>10 years</h5>
</div>

<div v-drag="[55,141,626,52]">
<h4>Intentionally damaging a computer through data transmission</h4>
<h5>1 to 10 years</h5>
</div>

<div v-drag="[55,233,513,80]">
<h4>Accessing a computer to defraud and obtain value</h4>
<h4>Extortion involving computers</h4>
<h5>5 years</h5>
</div>

<div v-drag="[55,327,600,80]">
<h4>Recklessly damage through intentional computer access</h4>
<h4>Accessing a protected computer and obtaining information</h4>
<h5>1 to 5 years</h5>
</div>

<div v-drag="[55,422,709,108]">
<h4>Trespassing in a government computer</h4>
<h4>Negligent damage or loss caused by deliberate access</h4>
<h4>Trafficking in passwords</h4>
<h5>1 year</h5>
</div>

<twemoji-face-screaming-in-fear v-drag="[861,419,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Denial of Service Attack

:: content ::

# A Denial of Service (DoS) Attack
#### One of the most common types of network-based cyberattacks that consists of an attacker attempting to overwhelm a target system through repeated network traffic!

<twemoji-desktop-computer v-drag="[750,280,96,89]" />

<twemoji-laptop v-drag="[150,280,96,89]" />

<twemoji-smirking-face v-drag="[113,317,61,57]" />

<twemoji-file-folder v-drag="[880,220,61,57]" />

<twemoji-file-folder v-drag="[880,300,61,57]" />

<twemoji-file-folder v-drag="[880,380,61,57]" />

<twemoji-laptop v-drag="[150,370,96,89]" />

<twemoji-loudly-crying-face v-drag="[113,397,61,57]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Dedicated Denial of Service Attack

:: content ::

# A Dedicated Denial of Service (DDoS) Attack
#### A more advanced cyberattack where multiple systems are being used to facilitate a DoS attack to overwhelm a target system through repeated network traffic!

<twemoji-desktop-computer v-drag="[750,280,96,89]" />

<twemoji-laptop v-drag="[150,280,96,89]" />

<twemoji-laptop v-drag="[150,190,96,89]" />

<twemoji-laptop v-drag="[150,370,96,89]" />

<twemoji-smirking-face v-drag="[113,227,61,57]" />

<twemoji-smirking-face v-drag="[113,397,61,57]" />

<twemoji-smirking-face v-drag="[113,317,61,57]" />

<twemoji-file-folder v-drag="[880,220,61,57]" />

<twemoji-file-folder v-drag="[880,300,61,57]" />

<twemoji-file-folder v-drag="[880,380,61,57]" />

<twemoji-laptop v-drag="[500,440,96,89]" />

<twemoji-loudly-crying-face v-drag="[468,476,61,57]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Dedicated Denial of Service Attack (Botnet)

:: content ::

## More often than not, DDoS attacks are facilitated by a ==botnet==!
#### A collection of controllable computers that have been infected with malware

<twemoji-desktop-computer v-drag="[750,280,96,89]" />

<twemoji-laptop v-drag="[100,280,96,89]" />

<twemoji-laptop v-drag="[300,280,96,89]" />

<twemoji-laptop v-drag="[300,190,96,89]" />

<twemoji-laptop v-drag="[300,370,96,89]" />

<twemoji-smirking-face v-drag="[63,318,61,57]" />

<twemoji-smirking-face v-drag="[63,318,61,57]" />

<twemoji-rat v-drag="[325,205,43,40]" />

<twemoji-rat v-drag="[325,295,43,40]" />

<twemoji-rat v-drag="[325,385,43,40]" />

<twemoji-file-folder v-drag="[880,220,61,57]" />

<twemoji-file-folder v-drag="[880,300,61,57]" />

<twemoji-file-folder v-drag="[880,380,61,57]" />

<twemoji-laptop v-drag="[500,440,96,89]" />

<twemoji-loudly-crying-face v-drag="[468,476,61,57]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Slowloris Attack

:: content ::

# A Slowloris Attack
#### A DoS attack where the attacker overwhelms a target system through purposefully slow network traffic that results in the target system slowing down too!

<twemoji-desktop-computer v-drag="[750,280,96,89]" />

<twemoji-laptop v-drag="[150,280,96,89]" />

<twemoji-smirking-face v-drag="[113,317,61,57]" />

<twemoji-file-folder v-drag="[880,220,61,57]" />

<twemoji-file-folder v-drag="[880,300,61,57]" />

<twemoji-file-folder v-drag="[880,380,61,57]" />

<twemoji-sloth v-drag="[203,289,56,52]" />

<twemoji-laptop v-drag="[500,440,96,89]" />

<twemoji-loudly-crying-face v-drag="[468,476,61,57]" />

---
layout: section
color: bowdoin
---

### Denial of Service Attacks have a severe impact on the internet and services we use today!

<br>

#### ==What are the repercussions of preventing legitimate users from accessing a service?==

<br>

#### ==How do you think these types of cyberattacks are prevented?==

---
layout: section
color: bowdoin
---

# Demo time!

<twemoji-smiling-face-with-horns v-drag="[861,419,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# SQL Injection

:: content ::

# SQL Injection
### SQL injection is a code injection technique used to attack applications by manipulating them into executing malicious database queries

<br>

# SQL or Structured Query Language
### A standard language used to access and manipulate data in databases!

<br>

```sql {monaco} {editorOptions: {fontSize:16}}
SELECT * FROM users WHERE email = '{email}' AND password = '{password}'
```

<br>

## But what if we could change the query to something like this:

```sql {monaco} {editorOptions: {fontSize:16}}
SELECT * FROM users WHERE email = '{email}' AND password = '{password}' OR '1'='1
```

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Cross Site Scripting

:: content ::

# Cross Site Scripting or XSS enables code to be injected into a website's source code and any connected clients!

### This is the technique used by Samy's MySpace worm!

<br>

## To make user input safe, we need to ==sanitize== them!

```python {monaco-run} {editorOptions: {lineNumbers:'on', fontSize:18}}
import bleach

user_input = "<script>alert('Hi!')</script>"

print(user_input)
print(bleach.clean(user_input))
```

---
layout: section
color: bowdoin
---

### ==What was the most surprising aspect of today?==

<br>

### ==What was the most scary aspect of today?==

<br>

### ==What obligations do you think you have==
 ### ==as a developer in regards to security?==

---
layout: section
color: bowdoin
---

# Questions?

<twemoji-thinking-face v-drag="[851,287,96,89]" />
