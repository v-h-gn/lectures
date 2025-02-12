---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
---

## DRM and Copyright Protection <twemoji-warning />
#### Module 2: Intellectual Property

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: section
color: bowdoin
---

### Copyright protects our tangible works of expression..

<br>

### However, that doesn't actually prevent people from using things other people have made!

<br>

### Most copyrighted material is digital now, could _we_ somehow enforce its protections?

<br>
<br>

#### ==Reflecting on our past discussions, what are some _hypothetical_ ways the copyright==
#### ==of digital materials could be violated?==

<br>

#### ==As developers, could _we_ somehow enforce copyright protections?==

<twemoji-thinking-face v-drag="[868,270,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Digital Rights Management

:: content ::

#### ==Digital Rights Management== (DRM) is a category of restrictions that are applied to digital copyrighted content in an attempt to limit how it can be accessed or used

<br>

### Many types of systems constitute DRM, but some common examples are:

- #### User authentication
  Requiring the verification of users to access content
- #### Geoblocking
  Requiring content to be accessed in certain regions
- #### Licensing agreements
  Limiting users rights over the content they access
- #### Encryption
  Requiring a special key to access content

<div v-drag="[537,323,357,28]" ><h4><mark>Have you ever encountered DRM?</mark></h4></div>

<div v-drag="[535,378,439,28]" ><h4><mark>What are some specific examples of DRM?</mark></h4></div>

<div v-drag="[533,433,408,28]" ><h4><mark>How would you feel to have to program</mark></h4><h4><mark>limits into your software?</mark></h4></div>

<twemoji-warning v-drag="[848,205,96,89,14]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# DRM Weaknesses

:: content ::

# Copyright holders want to protect their IP but DRM can negatively impact the experience of consumers..

<br>

# Some of the cons:
- #### Any technological “fix” is bound to fail sooner or later
- #### DRM undermines fair use and could reduce competition / stifle innovation
- #### DRM can make anonymous access impossible
- #### Can be very inconvenient to average consumers who wouldn't violate copyright


### ==What happens when required DRM technology is no longer==
### ==supported or maintained?==



<twemoji-balance-scale v-drag="[864,81,96,89]" />

---
layout: top-title
color: bowdoin-title
---

:: title ::

# DCMA

:: content ::

# The ==Digital Millennium Copyright Act (DCMA) of 1998==
### Aimed to protect copyright holders and remove liability from content hosts

<br>

#### Requires Internet Service Providers (ISPs) and content hosts to take down or block access to infringed materials upon notice from a copyright holder!

<br>

#### Outlines criminal and civil penalties for violating copyright:
- Minimum fine of $750 for a downloaded file
- Criminal penalties of up to $250,000 and five years in prison

<br>

### Makes it illegal to try to circumvent DRM!

<br>

### Makes it illegal to remove or alter copyright management information!

---
layout: section
color: bowdoin
---

### ==What are the strengths and weaknesses of DMCA?==

---
layout: section
color: bowdoin
---

### Imagine you were developing a downloadable desktop application that enabled users to compose music

<br>

#### ==If you wanted to require users to buy a license to use your software,==
#### ==how could you build that into your software without making it easy for them to bypass?==

<br>
<br>

#### Really think about this and come up with a strong technical design!

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Case Study: Sony Rootkit

:: content ::

# Sony BMG Music Entertainment Rootkit

### In 2005, Sony sold CDs with additional Extended Copy Protection software installed called XCP-Aurora that prevented users from:
- #### _"Ripping"_ audio tracks into MP3 format
- #### Making more than 3 copies of their music

#### Upon inserting one of these CDs into a Windows computer, the user would be prompted with an End User License Agreement.

- If they did not accept, they could not listen to their music.

- If they accepted, software was installed that monitored the computer ensuing they did not copy the music.

#### Relied on a Windows rootkit to hide files and processes on the users computer!

---
layout: section
color: bowdoin
---

### ==What do you think about Sony’s use of a rootkit to implement their DRM?==

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Case Study: Apple FairPlay

:: content ::

# Apple FairPlay

### In 2003, all iTunes music was protected with Apple's ==FairPlay== DRM

<br>

#### FairPlay stopped users from exchanging purchased music in the following ways:
- #### Songs couldn’t be played on more than 5 different computers
- #### Songs couldn’t be copied onto CDs more than 7 times
- #### Songs purchased from iTunes Store wouldn’t play on non-Apple devices
- #### DRM-protected music purchased from other retailers couldn’t be played on the iPod

#### FairPlay relied on encryption that was linked to specific iTunes enabled devices

<br>

### ==What do you think about Apple's implementation of FairPlay?==

---
layout: section
color: bowdoin
---

# Questions?

<twemoji-thinking-face v-drag="[813,227,96,89]" />
