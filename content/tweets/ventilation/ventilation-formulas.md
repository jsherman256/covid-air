---
title: "Ventilation and Air Quality Formulas"
date: 2022-07-25T00:52:53.000Z
draft: false
description: When fact checking claims, trying to achieve targets and assessing risk, you might need to do some math. Here are the most common formulas you need.
summary: When fact checking claims, trying to achieve targets and assessing risk, you might need to do some math. Here are the most common formulas you need.
categories:
  - Ventilation, Air Quality and CO2
tags:
  - ACH
  - Calculations
  - Ventilation
  - ASHRAE
  - CO2
  - Flow
---
[Source](https://twitter.com/joeyfox85/status/1551369864824201216)

---

### 1. Air changes per hour (ACH)

**How often the air gets changed in a room**

First you need the clean air delivery rate (CADR) from a piece of equipment or know the flow of outdoor air into a room. The formula is:

`ACH = 60 (min/hour) x flow/volume`
or
`Flow = ACH x volume/60`

Ex. Classroom, 7200 cubic ft, HEPA filter 300 cubic ft per minute (CFM) CADR
ACH from the HEPA filter = `60 x 300/7200 = 2.5 ACH`

### 2. Required Ventilation in a room

**Flow of outdoor air**

ASHRAE defines a flow/person and flow/area depending on the space.

`Required outdoor air = # people x flow/person + area x flow/area.`

Details are in [this thread]({{<relref "what-should-your-ventilation-be">}})

### 3. CO2 - Rebreathed fraction

`% Rebreathed air = (CO2/400)-1`

Example: CO2 - 2400 ppm
`% Rebreathed air = (2400/400)-1 = 5%`

{{< tweet user="DavidElfstrom" id="1510798085903069184" >}}

### 4. CO2 and Ventilation

`Ventilation/person = total outdoor air flow/# people`

You need to look up in a table CO2 generated (CO2 gen) based on the age and activity of the occupants.

`Indoor CO2 = Outdoor CO2 + CO2 gen x 1000000/ ventilation/person`

{{<tweet user="joeyfox85" id="1534335303607017473">}}

Alternatively,
`Ventilation/person = CO2 gen x 1000000/(Indoor air CO2 - outdoor air CO2)`

You can also just look this up in the table:

{{<tweet user="joeyfox85" id="1534335316064145409">}}

### 5. Particle Reduction

Every air change [removes 63% of remaining particles]({{<relref "one-air-change">}}) (assuming nothing is being generated).

```
% Particles Remaining = 1/e^(air changes)
% New particles = 1-1/e^(air changes)
```

|Air Change |Fresh Air % |
|-|-|
|1|63|
|2|86|
|3|95|
|4|98|
|5|99|

### 6. Disinfection Claims

Electronic air cleaners or UV claim a % reduced in an amount of time in a room. You can convert that to an equivalent air change:

`Equivalent Air Changes (eAC) = -ln (1-% reduced)`

ex. 99% reduced `eAC = -ln(1-0.99) = 4.6`

{{< tweet user="joeyfox85" id="1520835072286498817" >}}

Once you know the equivalent air changes, you can use the formula above to convert air changes to flow.

`Equivalent flow = Air changes x volume/time`

Ex. 98% reduction, 30 minutes, 500 cubic ft room
```
eAC = -ln(1-0.98) = 3.9
eFlow = 3.9 x 500/30 min = 65 cubic ft/min
```
