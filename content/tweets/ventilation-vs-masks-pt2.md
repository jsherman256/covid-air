---
title: "Comparing Ventilation and Masking"
date: 2022-07-28T03:07:19.000Z
draft: false
description: How much does clean air protect you? How would you convert between mask types and CO2 levels? Here are the calculations. I'll deal with one-way masking.
summary: How much does clean air protect you? How would you convert between mask types and CO2 levels? I'll deal with one-way masking.
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Ventilation
  - Masks
  - CO2
---
[Source](https://twitter.com/joeyfox85/status/1552490859869995008)

---

I've done [a similar thread on this](/tweets/masks-vs-ventilation/) comparing masking or mask mandates with adding HEPA filters here. This is looking at it from a different perspective - what's your risk at different CO2 levels and different types of masks.

The risk of getting infected is based on the virus concentration in the air. Masks filter the air you breathe in and lower the concentration. I'll use the values from [this table](https://twitter.com/brosseau_lisa/status/1449409318412079108).

|Mask|Leakage|
|-|-|
|Cloth|75%|
|Surgical|50%|
|N95|10%|

The math is pretty simple: 

- N95 has 7.5x less leakage than a cloth mask (75%/10%), 
- N95 has 5x less leakage than a surgical mask (50%/10%)
- A surgical mask has 1.5 x less leakage than a cloth mask (75%/50%)

Now you can look up those values in the table I made. I'm assuming that mitigation is purely from ventilation. I'm also dealing with shared room and not short range transmission.

{{< tweet user="joeyfox85" id="1534335316064145409" >}}

---

**Example 1** - Well ventilated classroom with 700 ppm CO2 and wearing a cloth mask.

This translates to 26 CFM/person. The equivalent with a N95 is ventilation rates `7.5 x lower = 26/7.5 = 3.5 CFM/person`. This translates to around 2500 ppm.

So risk in a classroom with 2500 ppm + N95 = risk with 700 ppm + cloth mask.

---

**Example 2**- Office with 700 ppm + surgical mask = 40.7 CFM/person
N95 is 5x better, so 40.7/5 = 8.1 CFM/person which is around 1850 ppm.

So risk of 700 ppm + surgical = 1850 ppm + N95

---

I’ll add on that 10% leakage is not always a valid assumption. With higher leakage, ventilation has an even bigger effect.

In the first case, 20% leakage changes it from 2500 to 1500 ppm. Second case changes from 1850 to 1000 ppm. It shows the importance of good ventilation with imperfect masking. 
