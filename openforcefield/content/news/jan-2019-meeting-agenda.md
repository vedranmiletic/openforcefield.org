---
date: "2018-10-06T00:00:00+00:00"
title: "Jan 2019 Open Force Field Consortium Workshop Agenda"
tags: ["website","news","consortium","meeting","agenda"]
categories: ["news"]
draft: false
description: "Agenda for the Open Force Field Consortium Workshop in San Diego, January 7-8, 2019."
weight: 10
author: "John D. Chodera"
---

We are hosting the first [Open Force Field Consortium](https://openforcefield.org/consortium/) Workshop in La Jolla, CA on January 7-8, 2019.
Attendance is open to Consortium members and collaborators, but parts of the meeting will be broadcast and recorded for posting online.

## Details at a glance

* *Date:* January 7-8, 2018
* *Location:* [Jacobs Medical Center, UC San Diego, La Jolla, CA](https://goo.gl/maps/VxCtgVb8wst), Rooms 2 and 3
* *Local contact:* Mike Gilson `<mgilson@ucsd.edu>`
* *Last update of this document:* 10:53 AM, Friday, December 28, 2018

## Directions

The workshop will take place at the Jacobs Medical Center Community & Medical Education Center, Rooms 2 and 3, located at [9300 Campus Point Drive, La Jolla, CA 92037](https://goo.gl/maps/VxCtgVb8wst) (mailing address for the entire medical center), about two miles from nearby hotels.

From hotel, take e.g., [Lyft](http://lyft.com) or [Uber](http://uber.com) to the main entrance of the hospital.
Enter there and walk all the way down the long corridor, past the Cove cafeteria on your left, into the modern Jacobs pavilion.
Continue walking past the elevators to the very end, and the meeting room will be on your right.  
See photos of the route below.

![Getting to the meeting rooms](visual-directions.png "Getting to the meeting rooms")

## Meals and breaks

Breakfast, lunch, snacks. and coffee will be provided at the meeting room both days.

The dinner on Day 1 will be held in a private room at the [Rock Bottom Restaurant and Brewery](https://rockbottom.com/locations/la-jolla/), [8980 Villa La Jolla, La Jolla, CA 92037](https://goo.gl/maps/eeFi5YqTWL42), two miles from the meeting location.
Please use Lyft, Uber, or another carsharing or taxi service to get there.  
We ask that each individual or group pay their own portion of the bill.

## Agenda (subject to change)

Comments and questions for discussion during the workshop are invited in the Slack channels indicated after each topic; e.g, `#project-planning` for "Roadmap overview".

### Jan 7

_Research topics: 45 min talk + 15 min discussion_

 Time         | Event | Speaker | Slack channel
 -------------|-------|---------|---------------
 7.45 -  8.00	| [Introduction](00-introduction.pdf) | Gilson |
 8.00 -  8.30 | [Roadmap overview](01-roadmap.pdf) | Shirts | `#project-planning`
 8.30 -  9.30	| [Short-term parameter optimization strategy: ForceBalance](http://doi.org/10.13140/RG.2.2.12894.69449) | Wang | `#forcebalance`
 9.30 - 10.00 | Coffee break | | `#random`
10.00 - 11.00 | [Long-term parameter optimization strategy: Bayesian Fitting](03-bayesian-fitting.pdf) | Chodera | `#bayesian-inference`
11.00 - 12.00 | [Chemical perception and SMIRNOFF typing](http://doi.org/10.13140/RG.2.2.18976.43521) | Mobley/Bannan | `#smirnoff`
12.00 -  1.00 | [Torsion fitting and fragmentation](http://doi.org/10.13140/RG.2.2.17521.53606) | Chodera/Wang | `#torsions`
 1.00 -  2.00	| Lunch (catered) | |
 2.00 -  2.30 | Group discussion to define ad hoc breakouts and breakout leaders/note-takers | |
			        | _Proposed Breakout Session 1_ : typing via chemical perception, torsion fitting | |
			        | _Proposed Breakout Session 2_ : useful physical property data, parameter fitting | |
 2.30 -  3.00 | Breakout Session 1 | |
 3.00 -  3.30 | Coffee break | | `#random`
 3.30 -  4.00 | Breakout Session 2 | |
 4.00 -  5.00 | Reconvene for breakout reports and all-hands discussions | |
              | [Breakout session notes: Benchmarking Accuracy](breakout-benchmarking.pdf) | |
              | [Breakout session notes: Property calculation framework](breakout-property-calculator.pdf) | |
              | [Breakout session notes: Use cases](breakout-use-cases.pdf) | |
 5.00 -  5.15 | Roadmap recap and discussion (reviewing Slack input from remote attendees) | | `#project-planning`
 6.00         | Group dinner in La Jolla at [Rock Bottom Brewing](https://rockbottom.com/locations/la-jolla/) | |

### Jan 8

_Research topics 45 min talk + 15 min discussion_

Time         | Event | Speaker | Slack channel
-------------|-------|---------|---------------
 8.00 -  9.00 | [Charge models](http://doi.org/10.13140/RG.2.2.35543.93608) | Schauperl| `#charge-models`
 9.00 - 10.00 | [Fitting non-torsion valence terms](http://doi.org/10.13140/RG.2.2.11216.97289) | Mobley/Wang | `#valence`
10.00 - 10.30	| Coffee break | | `#random`
10.30 - 11.30	| [Software architecture and infrastructure](08-software-infrastructure.pdf) | Wagner | `#infrastructure`
11.30 - 12.30	| [Fitting condensed-phase properties](09-physical-properties.pdf) | Chodera/Shirts | `#propertycalculator`
12.30 -  1.30	| Lunch (catered) | |
 1.30 -  2.00 | Group discussion to define ad hoc breakouts and breakout leaders/note-takers
              | _Proposed Breakout Sessions:_ electrostatics, software preview / toolkit hands-on
 2.00 -  4.00 | Breakout Session (with coffee)
 4.00 -  5.00	| Reconvene and wrap-up discussion
              | [Breakout session notes: neural network potentials](breakout-neural-networks.pdf)              

### Other discussion topics for the Open Force Field Initiative science team

#### Potential software architecture and infrastructure discussion topics

* Property estimation and automated parameterization (`#propertycalculator`)
* Scaling up property estimation
* If many dependencies are required, do we want to have multiple `conda` packages, or a single monolithic package?
* What should the API for automated parameterization look like to interface with ForceBalance and Bayesian methods?

#### Other potential discussion topics

* Which AMBER biopolymer force field(s) should we target in the first optimized release?
The current recommendation in the AmberTools 18 manual is ff14SB for proteins, so unless there is significant objection, we should probably stick with this.
* Which solvent model should we target in the first optimized release?
TIP3P or TIP4P-Ew?