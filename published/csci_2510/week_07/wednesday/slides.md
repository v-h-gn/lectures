---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
---

## Social Engineering and Disclosure <twemoji-smirking-face /> <twemoji-megaphone />
#### Module 3: Security

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: section
color: bowdoin
---

### During this module, we have reviewed many different reasons why security is important as well as how serious malware / cyberattacks can be!

<br>

### Today, we will finish up our discussion by looking at how we can exploit the non-technical factors of a system and our responsibility of disclosure!

<br>

### Before we move on:

<br>

#### ==We have seen that many issues are caused by malware and cyberattacks,==
#### ==should users be legally required to install anti-virus software?==

<twemoji-thinking-face v-drag="[861,419,96,89]" />

---
layout: two-cols-title
color: bowdoin
---

:: title ::

### ==Social Engineering== is hacking that exploits the human aspects of a system!
### You can think about this like 'conning' your way in!

:: left ::

- #### Phishing
  Using deceptive means to steal sensitive information from unsuspecting victims
- #### Spear phishing
  Highly targeted phishing
- #### Vishing
  Voice-based phishing
- #### Smishing
  SMS-based phishing
- #### Quid Pro Quo
  Exchanging information or services to convince the victim to act

:: right ::

- #### Pretexting
  Tricking victims into giving up information by assuming a false identity
- #### Baiting
  Manipulating a victim by promising a reward in return for sensitive information
- #### Tailgating
  Following someone in to a secure building or area to get physical access to infrastructure
- #### Water-holing
  Infecting a frequented website and its visitors with malware

<twemoji-smirking-face v-drag="[868,63,96,89]" />

---
layout: section
color: bowdoin
---

### ==What dangers do you think social engineering poses?==

<br>

### ==How can we mitigate social engineering threats?==
### ==Is it our responsibility to mitigate them?==

<twemoji-thinking-face v-drag="[861,419,96,89]" />

---
layout: section
color: bowdoin
---

<Youtube id="ETOVI7NCLG4" height='500' width='800'/>

<twemoji-zany-face v-drag="[866,419,96,89,26]" />

---
layout: section
color: bowdoin
---

<Youtube id="fHhNWAKw0bY" height='500' width='800'/>

<twemoji-face-screaming-in-fear v-drag="[866,419,96,89,9]" />

---
layout: section
color: bowdoin
---

### ==How you do you feel after watching real examples==
### ==of social engineering?==

<br>
<br>

### ==How could this affect you as an individual?==

<br>
<br>

### ==How might you be a target for spear phishing?==

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Disclosure Responsibility

:: content ::

## If you discover a vulnerability in a system, you have an ethical obligation to disclose that weakness and not exploit it
### However, how we do this is very important!

<br>

## We must confidentially report the issue! ==Why?==
### We must operate in good faith to ensure the company knows about it safely!

<br>

### You and the company should agree on a time period before you release details about the vulnerability!

<br>

### ==What if the company refuses to fix the issue?==

<br>

### ==What if the company doesn't fix the issue in the agreed upon period?==

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Case Study

:: content ::

## Goatse Security (a hacker group) collected the email addresses of more than 100,000 iPad owners from a public AT&T website in 2010
- #### The website displayed the email address of an iPad owner to anyone who entered the iPad ID number; it did not require a password
- #### The vulnerability was discovered by just sending GET requests to the AT&T website
- #### "Weev", a member of the hacker group, notified media organizations about the security ﬂaw and discussed it on a chat channel before AT&T knew about it

<br>

#### Weev was sentenced to 41 months in federal prison and $73,000 in restitution.

<br>

#### He spent 13 months in prison before his conviction was vacated by a higher court

---
layout: section
color: bowdoin
---

#### In December of 2015, Syed Rizwan Farook and Tashfeen Malik killed 14 and wounded 22 others at holiday gathering in San Bernardino, California

- Farook and Malik died in shootout with police

- FBI recovered Malik's work-issued iPhone 5C but it was locked


- Due to the built-in security features of iPhone 5C all of Malik's personal data encrypted
  - After 10 consecutive incorrect passcode entry attempts, the encryption key would be deleted rendering all personal data inaccessible

<br>

#### In February of 2016, the FBI asked Apple to create a new version of iOS that disabled the passcode security features
- Apple refused to cooperate
- The FBI convinced a US magistrate to issue an order for Apple to comply

---
layout: section
color: bowdoin
---

#### Apple’s argued that if the backdoored version of iOS that disabled security features fell into wrong hands, criminals would be able to unlock any iPhone

- This could seriously harm all iPhone users

<br>

#### Department of Justice's argued that Apple could maintain custody of software and even destroy software after being used by the FBI

<br>

#### In March of 2016, the Department of Justice withdrew its request, declared it had gotten into locked iPhone

- The Inspector General later determined the FBI had made request of Apple before exploring whether FBI had other means to unlock iPhone

#### ==What do you think Apple should have done? Why?==

<br>

#### ==If you were told to create backdoors in your code, would you?==
#### ==How would the situation effect your answer?==

---
layout: section
color: bowdoin
---

# Questions?

<twemoji-thinking-face v-drag="[851,287,96,89]" />
