# Recruitment for E-Agle TRT | Electronics division

Welcome to the recruitment _test_ for the electronics team of E-Agle Trento Racing Team.

This _test_ is meant to give us the possibility to have a first understanding of the capabilities of our applicants without them having the pressure of seeing it as an exam.

Moreover it's studied so that the applicants get a first taste of the tools used, so that once in the team, they can get up and running quickly into the team's workflow without having to learn stuff under pressure when it's needed.

## What we'll look into

 - Understanding of basic electronics
 - Components choice and their suitability
 - KiCad
   - Schematic choices, tidyness and good practices
   - Board layout understanding and, again, good practices
 - `git` usage: fork, branch, clone, commit, push, pull
 - Not only _tecnical correctness_ but also actual usability.

## Assignment

Develop an overcurrent monitoring system (**monitor**) to perform plauysibility checks of a secondary system (**load**).

### Overview
The **monitor** has the following specs:
- It is supplied by an unstable DC voltage line, ranging from 9V to 17V
- Has a normally open relay connected in series with the load
- Has a hall effect sensor that measures the current through the load

The **load** has the following specs:
- Voltage range: $24[V] \div 48[V]$
- Current range: $-3[A] \div 25[A]$

### Specs
The **monitor** must ensure that the relay is open if the power obsorbed by the **load** is above $500[W]$.
Once open, it must not be possible to close the relay unless the **monitor** is power cycled.

No programmable logic is allowed.

The Hall effect based sensor can be chosen from the _Allegro ACS781xLR_ family of devices. Other sensors may be used as long as the specs are met and equivalency is proven.

Below you can find a general diagram of the system

<p align="center">
<img src=".\general-diagram.png" width="400">
</p>

## KiCad instructions
- In the schematic use also a hierarchical sheet
  - _It's not a good practice for such a small project, but it's for letting you learn about hierarchy without the hassle of a more complex assignment_

- Add comments for the necessary calculations of values

- Consider JLC PCB as the board manufacturer

## General instructions

 - Create a repository on your GitHub account (if you don't have it, create one) and copy this project in it. **Do not clone this repository!**
 - Branch the master into one called `name_surname` and commit your progress in this branch
 - Commit your progress along the way. **Do not commit just the finished project**, use Git for what it's made for!
 - When you are done, generate the schematic output inside `docs/` and the production (gerber) files in `output/`
 - If you haven't already, submit your application form [here](https://eagletrt.it/apply)
 - If you have any questions feel free to contact us at [electronics@eagletrt.it](mailto:electronics@eagletrt.it)
 - Feel free to also come to our lab (Povo 2 floor -2) if we are slow at replying
 - You have **2 weeks** (14 days) to work on this project (**This is a hard deadline and we evaluate if you meet deadlines**)

## Links
:globe_with_meridians: [Website](https://www.eagletrt.it)

:iphone: [Instagram](https://www.instagram.com/eagletrt)

:computer: [LinkedIn](https://www.linkedin.com/company/eagletrentoracingteam)