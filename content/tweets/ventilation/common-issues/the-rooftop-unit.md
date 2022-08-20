---
title: "Common Issues: The Rooftop Unit"
date: 2022-04-11T20:03:07.000Z
draft: false
description: The basic building block of the HVAC world is a ventilation problem?
summary: The basic building block of the HVAC world is a ventilation problem?
categories:
  - Ventilation, Air Quality and CO2
  - Common Ventilation Issues
tags:
  - Ventilation
---
[Source](https://twitter.com/joeyfox85/status/1513608603277545474)

---

Et tu, Brute?

The basic building block of the HVAC world is a ventilation problem?
Unfortunately, RTUs are often incapable of providing sufficient ventilation. Here's the math why:

We'll deal with a typical classroom:
```
25 people, 800 sq ft x 9' ceilings = 7200 cubic ft
```

Current ASHRAE minimums are:
```
(25x10CFM/person+800x0.12CFM/Sq ft)/0.8 = 432 CFM outdoor air
```

`0.8` is a factor for hot air. [See standard 62.1-2019 pg 19,23](https://www.ashrae.org/technical-resources/standards-and-guidelines)

To calculate the air changes/hour:
```
ACH = 60xCFM/Volume = 0.0083xCFM

ASHRAE minimum:
ACH = 0.0083x432 = 3.5
```

Most of our modern installations have `500 CFM/classroom = 4.15 ACH`

Now what can you get out of an [RTU]({{<relref "intro-to-rtu">}})?

---

To start, you have to size the total flow (outdoor air + recirculated air). Here's a description how it's sized, but [the main factor is the cooling load](https://twitter.com/WBahnfleth/status/1503864258630754311). For a typical Canadian classroom it's 2-3 tons. The unit is then sized at 400 CFM/ton.

Taking the middle value of 2.5 tons/classroom (I've seen this a lot), the unit supplies a total of 1000 CFM.

Now we know how much total air is supplied, what % of outdoor air can be supplied?

The limiting factor is the supply air temperature without heating.

Imagine a day where it's cold outside (-5 °C). You can't leave the heating running all the time or you'll overheat. Sometimes it will need to turn off and when this happens, the mixed air temperature is [the same as the supply air temperature]({{<relref "intro-to-rtu">}}).

If the return air temperature is 21 °C (typical space), outdoor air temp is -5 °C and you are supplying 25% Outdoor Air (25% OA), the mixed air temperature will be:
```
MAT = RAT - OA% * (RAT-OAT)
= 21 - 0.25(21 - (-5))
= 14.5 °C
```

When the heating is off, the supply air temperature will be the same temperature as the mixed air temperature. Supplying 14.5 °C air to the space is extremely uncomfortable. People will complain right away. An HVAC mechanic could solve this by reducing the ventilation. 

Even if you were to supply 25% outdoor air, which I've shown cannot be done comfortably on cold days, that's only 250 CFM of outdoor air. ASHRAE minimum is 432 CFM. You're about 58% of the minimum. This also equates to 2.1 ACH. A very low level of ventilation.

---

The point I'm getting at is the simple cheapest option of the packaged rooftop unit is nowhere near capable of comfortably supplying minimum standards of ventilation. Modern classrooms don't use these, but these are common in buildings from the 90s.

You can find these in many places like strip malls. However, those have lower occupancy than classrooms, so it might be okay sometimes.

Next thread I'll show how a more modern unit with heat recovery can fix this problem and the costs involved in upgrading.