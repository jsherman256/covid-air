---
title: "What is Good Ventilation?"
date: 2022-04-18T20:21:45.000Z
draft: false
description: 3 Ways of Calculating It
summary: If we want to have "good ventilation" we need to know how to define it. The different definitions tell you different information.
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Ventilation
  - Calculations
---
[Source](https://twitter.com/joeyfox85/status/1516150008059514881)

---

If we want to have "good ventilation" we need to know how to define it. The different definitions tell you different information.

Imperial units for air flow is cubic ft/minute (CFM)
Metric is liters/sec (LPS)

### 1. CFM (LPS)/Person

If you are worried about the air quality issues created by every person, this is the metric to use. My first boss told me that a room with 50 people has 50 bums and 100 arm pits. This is relevant for body odor and CO2 levels.

### 2. Air Changes per Hour (ACH) 

`ACH = 60xCFM/Volume or 3600xLPS/Volume`

This doesn't take occupancy into account - only the volume of the room. It's relevant for COVID. If there is one infected person in the room, it makes no difference how many other people are there. 

You care about how quickly the ventilation system can clear the virus out of the room.

### 3. ASHRAE 62.1 Ventilation Guidelines
`(10 x # ppl + 0.12 x sq ft.)/0.8 (in CFM)`

This has [more details](https://www.ashrae.org/technical-resources/standards-and-guidelines). It takes both occupancy and the area into account.

The values are different depending on the situation, but I've used the numbers for classrooms with heating (pg 17,23). A discussion of the basis of 62.1 can [be found here](https://twitter.com/DavidElfstrom/status/1503402659046469637).

It doesn't count the volume of the room (only area) which is relevant for rooms with high ceilings.

### Demand Control Ventilation (DCV)

DCV is a energy saving method based on occupancy. When there are fewer people and lower CO2 levels, you reduce the ventilation.

From what I just explained, the issue is obvious. CO2 measures the ventilation/person, so with DCV ventilation will be reduced, even though the prevention of airborne transmission is related to the ACH. 2 different metrics relating to different uses.

If we want to use ventilation to mitigate airborne virus transmission, then DCV might be a thing of the past. An alternative is to reduce ventilation only to spaces with no occupancy. This requires room by room control with motion sensors - more complicated and expensive.

This also shows [the limitation of CO2 monitoring](https://twitter.com/joeyfox85/status/1510785191857508357). CO2 monitoring tells you the flow/person and not ACH. It can alert you to issues with ventilation. But low occupancy can still lead to low CO2, even if there is a low ACH - poor ventilation.

So what is good ventilation? For airborne transmission risk: **4-6+ ACH**.
Now that we live in the COVID era, we need more data. A higher ACH might be necessary going forward - especially in places prone to super-spreader events.

![Chart comparing adequacy of different ACH rates. 6 is ideal; 5-6 is excellent; 4-5 is good; 3-4 is bare minimum; less than 3 is low](/covid-air/ach-chart.jpg)

**Assuming 800 sq ft classroom, 9' ceilings, 25 ppl. What is ASHRAE minimum?**

```
(10x25 + 0.12x800) / 0.8 = 433 CFM, 204 LPS
60x433 / 800 / 9 = 3.6 ACH
= 17.5 CFM/person, 8.2 LPS/Person
```

**What is common ventilation?**

I've seen a lot of old classrooms designed for 250 CFM, 118 LPS.

```
250 / 433 = 58% of modern ASHRAE minimum
60x250 / 800 / 9 = 2 ACH
= 10 CFM/person, 4.7 LPS/person
```

**Ideal ventilation = 6 ACH**

```
6 / 60*800*9 = 720 CFM, 340 LPS
= 29 CFM/person, 13.7 LPS/person
720/433 = 166% of ASHRAE minimum
```

This is similar to the old standard for environmental tobacco smoke (ETS). What's the analogy for COVID spread again?

{{< tweet user="joeyfox85" id="1482797712928034822" >}}

### Ventilation Summary:

| | |
|-|-|
| Poor/Common | 10 CFM/person, 4.7 LPS/person, 58% of modern minimum, 2 ACH |
| Modern Minimum | 17.5 CFM/person, 8.2 LPS/person, 3.6 ACH |
| Ideal | 29 CFM/person, 13.4 LPS/person, 166% of modern minimum, 6 ACH |

![Graph showing different levels of ventilation.](/covid-air/vent-level-graph.png)