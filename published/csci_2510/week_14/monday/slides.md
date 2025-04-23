---
layout: intro
theme: neversink
color: bowdoin
routerMode: hash
favicon: https://avatars.githubusercontent.com/u/9260792
---

## Notable System Failures <twemoji-fearful-face />
#### Module 6: Safety and Reliability

<br>

<hr><br>

Christopher Martin - _Bowdoin College_ <a href="https://bowdoin.edu/" class="ns-c-iconlink"><mdi-open-in-new /></a>
<Email v="c.martin@bowdoin.edu" />

---
layout: section
color: bowdoin
---

### Today, we are going to discuss some of the most historically notable system failures to analyze how they failed and learn from their mistakes

<br>

#### Please understand that this is not a complete list!

<br>

#### Over the weekend, you probably saw many different examples - share them with the people around you

<br>

#### ==Did you choose the same event? If so, was it for the same reasons?==

<br>

#### ==What were some of the patterns you noticed while researching different==
#### ==software failures?==

---
layout: top-title
color: bowdoin-title
---

:: title ::

# AirAsia Flight 8501

:: content ::

## In December of 2014, AirAsia Flight 8501 crashed into the Java Sea, killing all 162 of the people on board as a result of operator error

- #### One of the two flight computer sent repeated false warning messages to crew believed to be caused by a loosely soldered wire

- #### Captain Iriyanto had experienced a similar error while performing a systems check in the same plane 3 days earlier and observed maintenance reseating the circuit breaker to reset computer

- #### Captain Iriyanto repeated the process of reseating the primary flight computer's circuit breaker as he saw maintenance do not realizing this didn't automatically reengaged autopilot functionality on that primary computer

- #### Captain Iriyanto reseated the backup flight computer's circuit breaker while the primary was still offline resulting in an immediate loss of auto-pilot and auto-thrust

---
layout: section
color: bowdoin
---

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

### In the ensuing moments, the pilots miscommunicated resulting in the plane diving directly into the Java Sea

<div v-drag="[441,11,532,366]">

![](https://i.imgur.com/kDnSinL.png)

</div>

<div v-drag="[60,34,424,292]">

![](https://i.imgur.com/KSWF5wK.png)

</div>

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Doctors Without Borders

:: content ::
## In October of 2015, a US Air Force AC-130 gunship mistakenly fired at a Doctors Without Borders hospital in Afghanistan repeatedly over the course of 30 minutes, killing 30 and injuring 34 as a result of a networking crash

- #### A networking outage onboard eliminated the <br>ability of the aircraft crew to transmit video,<br> send and receive e-mail, or send and <br>receive electronic messages

- #### Information Technology Systems available <br>to the commanding officers responsible for <br>the gunship failed to alert those on duty in <br>the operations center that the target selected by the aircraft was on a no-strike list

<div v-drag="[541,202,424,292]">

![](https://s.abcnews.com/images/International/AP_doctors_without_borders_airstrike_hb_151124_16x9_992.jpg?w=1600)

</div>

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Patriot Missile Failure

:: content ::
## In February of 1991, a Patriot missile battery in Saudi Arabia failed to track and intercept an incoming Iraqi Scud missile resulting in the death of 28 US soldiers and over 100 more being wounded

- #### The Patriot Missile was a mobile anti-aircraft system designed to only operate idly for a few hours at a time due to its reliance on time-sensitive range calculations

- #### Time was tracked by incrementing a 24-bit integer value every 0.1 seconds after system startup but needed to be converted to a float for these range calculations

- #### The Alpha Patriot battery was kept in operation for over 100 hours, significantly longer than the recommended operating time of 8 hours

- #### 1/10th cannot be represented exactly in IEEE 754 floating-point format, this imprecision caused a rounding error of `0.000000095` every tenth of a second

---
layout: section
color: bowdoin
---

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

### Running the system for 100+ hours caused these rounding errors compounded to roughly 0.34 seconds causing the Patriot Missile system to misjudge the position of the incoming Scud missile by 687 meters

<div v-drag="[497,19,474,326]">

![](https://import.viva64.com/docx/blog/0445_Patriot/image3.png)

</div>

<div v-drag="[60,34,424,292]">

![](https://import.viva64.com/docx/blog/0445_Patriot/image9.png?ver=03-31-2025-12-33-29)

</div>

---
layout: top-title
color: bowdoin-title
---

:: title ::

# AT&T Network Outage

:: content ::
## In January of 1990, an innocuous one line change to a switch statement in a 4 million line codebase was prematurely deployed without proper testing

- #### This one change caused a race condition allowing messages sent in quick succession to overwrite one another
- #### This issue caused a massive service outage resulting in over half of AT&T's long distance network switches being unavailable for over 9 hours
- #### During this period, 70 million calls failed and over 60,000 people lost all service
  Disrupted consumers, businesses, and emergency services
- #### AT&T suffered an estimated loss of 60 million dollars in revenue

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Ariane 5 Rocket

:: content ::
## In June of 1996, the first unmanned Ariane 5 rocket launched to deliver Cluster, a collection of4 research satellites, into orbit

<br>

<Youtube id="A1gGGDG580E" height='350' width='800'/>

---
layout: section
color: bowdoin
---

### Failure of the Ariane 5 rocket was due to reused software that was developed for the earlier Ariane 4

<br>

#### However, the new rocket design was faster than the older rocket

<br>

#### Code in this system relied on undocumented assumptions made based on the specifications of the Ariane 4 that were no longer accurate for the Ariane 5

<br>

#### 37 seconds into launch, this old code attempted to convert a 64-bit floating-point number to a 16-bit signed integer resulting in an integer overflow exception which could never have happened in the Ariane 4 rocket

<br>

#### This crashed the navigation system and backup navigation system causing the rocket to tear itself apart trying to correct incorrect readings that it was horizontal

<br>

#### The explosion resulted in an equipment loss of over $500 million dollars

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Mars Climate Orbiter

:: content ::
## In September of 1999, NASA lost contact with the Mars Climate Orbiter, a satalite meant to study the Martian atmosphere and serve as a communications relay between surface rovers and Earth

<br>

- #### Different aspects of the orbiter were developed by<br>different agencies (Lockheed Martin and NASA's JPL)

- #### The Orbiter disintegrated in Martian atmosphere<br>after a navigational error caused by receiving a<br>command from NASA resulting in a mission loss of<br>over $327 million dollars..

- #### Lockheed Martin designed one piece of software to<br>use English units (pound seconds) while NASA's<br>JPL designed expected metric Newton seconds

<div v-drag="[638,196,322,222]">

![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/Mars_Climate_Orbiter_2.jpg/1024px-Mars_Climate_Orbiter_2.jpg)

</div>

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Mars Polar Lander

:: content ::
## In December of 1999, NASA lost contact with the Mars Polar Lander, a probe meant to collect samples and study the south pole of Mars

<br>

- #### The probe's landing engines shut off early resulting<br>in the rover crashing into the surface of the planet..

- #### This resulted in a mission loss of over $165 million

- #### Engines shut off too early when vibrations from<br>deploying the stowed probe legs was interpreted<br>as touchdown, this was a known issue but was not<br>properly accounted for in the software because<br>backup sensors to verify touchdown had happened<br>were found to give false positives in ambient<br>conditions during leg deployment

<div v-drag="[638,196,322,222]">

![](https://upload.wikimedia.org/wikipedia/commons/thumb/9/96/Mars_Polar_Lander_-_artist_depiction.png/1024px-Mars_Polar_Lander_-_artist_depiction.png)

</div>

---
layout: top-title
color: bowdoin-title
---

:: title ::

# THERAC-25

:: content ::

<Youtube id="Ap0orGCiou8" height='400' width='800'/>

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Tokyo Stock Exchange

:: content ::
## In December of 2005, J-Com (the largest cable television company in Japan) had their IPO on the open Tokyo Stock Exchange

- #### A Mizuho Securities employee mistakenly entered an order to sell 610,00 shares of J-Com at 1 yen each instead of 1 share at 610,000 yen

- #### The employee bypassed the computer warning message and performed the trade

- #### After the sell order posted on the stock exchange’s display board, Mizuho tried to cancel order several times but a software bug caused all attempts to fail

- #### Mizuho lost $225 million as a result of buying back the posted shares

## This is one example of 'fat-finger' errors

---
layout: top-title
color: bowdoin-title
---

:: title ::

# Never meant to be

:: content ::
## Sometimes, mistakes just don't stop resulting in software costing more than it is worth to continue developing...

- ### Denver International Airport Automated Baggage System ($600M)
- ### FBI Virtual Case File System ($170M)
- ### Sainsbury Automated Supply-chain management system ($526M)
- ### Ford Motor Purchasing System ($400M)
- ### California Child-Support System ($100M) + ($1B in penalties)

<br>

## Each of these systems were ultimately abandoned..

---
layout: section
color: bowdoin
---

# Questions?

<twemoji-thinking-face v-drag="[813,227,96,89]" />
