---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
---

## Introduction to Vulnerabilities <twemoji-unlocked /><twemoji-fearful-face />
#### Module 3: Security

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: section
color: bowdoin
---

## Last class, we began to look into why security is important

<br>

### Today, we will discuss different types of exploits and showcase different examples of how very avoidable mistakes can lead to serious vulnerabilities!

<br>

### ==To you, what is "hacking"?==

<br>

### ==What does it mean to "hack"?==

<br>

### ==What does "hacking" consist of?==

<twemoji-thinking-face v-drag="[861,419,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# A History of Hacking

:: content ::

## To many, ==hacking== refers to intentionally gaining unauthorized access to computer systems
### However, this is not the original meaning of the term!

<br>

#### In the early 1960s and 1970s, "hacking" was a positive term!
- A "hacker" was a creative programmer who wrote elegant or clever code
- A "hack" was an especially clever piece of code

<br>

#### From the 1970s to 1990s, "hacking" began to take on a more negative connotation..
- Started being equated with breaking into systems without authorized access because that required a deep understanding of computers and finding exploitations to make them do what you wanted

#### ==What factors do you think led to this transition? What made the 1970s special?==


<twemoji-laptop v-drag="[755,111,154,143]" />
<twemoji-unlocked v-drag="[803,150,61,57]" />
<twemoji-smirking-face v-drag="[867,181,96,89]" />

---
layout: two-cols-title
color: bowdoin
---

:: title ::

# The late 1960s and 1970s were an extremely exciting time!

### They marked the beginning of the digital era through the rise in personal computers and computers being able to communicate over a network!

:: left ::

## Network Communication

- ARPANET (1969)

- Email (1972)

- Ethernet (1973)

- Fiber optics (1973)

- TCP/IP (1977)

:: right ::

## Personal Computing

- Intel 4004 (1971)

- Altair 8800 (1974)

- Apple I (1976) and Apple II (1977)

- TRS-80 (1977)

- Commodore PET 2001 (1977)

:: default ::

#### Both of these factors led to more people having access to computers and a greater reach for software! However, with increased reach and wider access..

<twemoji-star-struck v-drag="[857,143,96,89]" />

---
layout: section
color: bowdoin
---

# We see the first ==malware== <twemoji-bug />
# and ==viruses== <twemoji-microbe /> !

<br>

<br>

### ==What do you think malware is?==

<br>

### ==What do you think a computer virus is?==

<br>

### ==What is the difference between them?==

<twemoji-face-screaming-in-fear v-drag="[861,419,96,89,9]" />

---
layout: two-cols-title
color: bowdoin
---

:: title ::

# Malware (short for Malicious Software) is any software that is designed to damage or steal data from computers!

### There are many different types of malware!

:: left ::

- #### Virus <twemoji-microbe />
  Malware that copies itself by modifying programs on a computer
- #### Worm <twemoji-bug />
  Malware that spreads by replicating itself on other computers
- #### Trojan Horse <twemoji-horse />
  Malware that tricks users into thinking it's a harmless file

#### ==Had you heard of any of these before?==

#### ==Which are new?==

:: right ::

- #### Spyware <twemoji-eye />
  Malware that secretly collects information
- #### Adware <twemoji-newspaper />
  Malware that displays unwanted advertisements
- #### Ransomware <twemoji-locked />
  Malware that prevents you from accessing your device and the data stored on it, usually by encrypting your files
- #### Remote Access Trojan (RAT) <twemoji-rat />
  Malware that allows an attacker to remotely control an infected computer

:: default ::

<twemoji-fearful-face v-drag="[849,95,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Creeper

:: content ::

# Creeper, the first worm, was released onto ARPANET in 1971
### While the worm wasn't harmful and was developed to test if programs could replicate themselves, it still infected the network and took effort to remove

<br>

## Infected systems would see the following message displayed:
### `I'M THE CREEPER : CATCH ME IF YOU CAN`

<br>

## Lead to the development of the first anti-virus, Reaper, in 1972
### Reaper was specifically meant to study the removal of viruses from a system or network that was infected

<br>

### ==How do you think viruses and worms would even work programmatically?==

### ==What do you think the code for that would even look like?==

<twemoji-bug v-drag="[850,192,124,115]" />

---
layout: section
color: bowdoin
---

# Let's see for ourselves!

<twemoji-microbe v-drag="[843,64,96,89]" />
<twemoji-bug v-drag="[90,401,96,89]" />
<twemoji-zany-face v-drag="[620,223,96,89]" />

---
layout: section
color: bowdoin
---

### ==How would you feel if you accidentally ran virus.py==
### ==on your computer?==

<br>
<br>

### ==How much work do you think it would take to==
### ==‘disinfect’ your system?==

<twemoji-grinning-face-with-sweat v-drag="[861,419,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Non-Malicious Hacking

:: content ::

# Hacking, whether it is malicious or not has repercussions!
### Responding to non-malicious or prank hacking uses resources!
#### Hackers could accidentally do significant damage!

<br>

### Samy - A worm developed by Samy Kamkar for MySpace in 2005.

- #### Appended the text `"but most of all, samy is my hero"` to victim's MySpace profile bio and sent Samy a friend request
- #### When a new user viewed an infected profile page, the payload would then be replicated onto their own profile page continuing the distribution of the worm
- #### Spread to over one million users within 24 hours
  Making it the fastest spreading virus of all time!

### ==What are your thoughts about the Samy MySpace worm?==

<twemoji-bug v-drag="[827,134,124,115]" />

---
layout: section
color: bowdoin
---

### MySpace had to be taken offline to stop the worm!

<br>

### Samy was raided by the United States Secret Service!

<br>

### Samy pled guilty to a felony charge resulting in him paying a fine of $20,000, serving three years of probation (limited computer access), and working 720 hours of community service!

<br>

### ==Do you think this was fair or too extreme?==


<twemoji-astonished-face v-drag="[861,419,96,89]" />

---
layout: section
color: bowdoin
---

# Questions?

<twemoji-thinking-face v-drag="[851,287,96,89]" />
