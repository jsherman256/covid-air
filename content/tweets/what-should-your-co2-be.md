---
title: "What should your CO2 be?"
date: 2022-07-03T19:24:38.000Z
draft: false
description: If you intend to speak up when CO2 levels are too high, you need to know when that happens. 
summary: If you intend to speak up when CO2 levels are too high, you need to know when that happens. Here, a ventilation expert claims classrooms should be around 1500 ppm. Is that correct? What should it really be?
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Ventilation
  - CO2
  - School
---
[Source](https://twitter.com/joeyfox85/status/1543677113051582466)

---

Here, [a ventilation expert claims](https://twitter.com/mjb302/status/1433721407423328276) classrooms should be around 1500 ppm. Is that correct? What should it really be?

It's takes three steps:

### Step 1: Find out what your ventilation should be. 

You have to calculate it as shown in [this thread](https://twitter.com/joeyfox85/status/1542959661829312512).

For a classroom, I'll assume 800 sq ft and 25 people.

The ventilation should be:
```
10 x 25 + 0.12 x 800 = 346 cubic feet/minute (CFM)
```
or
``` 
5 x 25 + 0.6 x 74.3 sq m = 169 Litres/second (lps)
```

### Step 2: Find the ventilation per person. 

Divide the answer in step 1 by the number of people:

```
Ventilation/person = 346 CFM/25 = 13.8 CFM/person
```
or 
```
169 lps/25 = 6.8 lps/person
```

### Step 3: Look it up in this table

||Low activity adults||High activity adults||Low activity children||High activity children||
|-|-|-|-|-|-|-|-|-|
|**CO₂  (ppm)**|**LPS**|**CFM**|**LPS**|**CFM**|**LPS**|**CFM**|**LPS**|**CFM**|
|**600**|30.0|63.3|85.6|180.5|19.4|41.0|55.6|117.2|
|**700**|19.3|40.7|55.0|116.1|12.5|26.4|35.7|75.4|
|**800**|14.2|30.0|40.5|85.5|9.2|19.4|26.3|55.5|
|**900**|11.3|23.7|32.1|67.7|7.3|15.4|20.8|44.0|
|**1000**|9.3|19.6|26.6|56.0|6.0|12.7|17.2|36.4|
|**1100**|7.9|16.8|22.6|47.8|5.1|10.9|14.7|31.0|
|**1200**|6.9|14.6|19.7|41.7|4.5|9.5|12.8|27.1|
|**1300**|6.1|12.9|17.5|36.9|4.0|8.4|11.4|24.0|
|**1400**|5.5|11.6|15.7|33.2|3.6|7.5|10.2|21.5|
|**1500**|5.0|10.6|14.3|30.1|3.2|6.8|9.3|19.5|
|**1600**|4.6|9.7|13.1|27.5|3.0|6.3|8.5|17.9|
|**1700**|4.2|8.9|12.0|25.4|2.7|5.8|7.8|16.5|
|**1800**|3.9|8.3|11.2|23.5|2.5|5.4|7.2|15.3|
|**1900**|3.6|7.7|10.4|22.0|2.4|5.0|6.8|14.3|
|**2000**|3.4|7.2|9.7|20.6|2.2|4.7|6.3|13.4|
|**2200**|3.0|6.4|8.7|18.3|2.0|4.1|5.6|11.9|
|**2400**|2.7|5.8|7.8|16.4|1.8|3.7|5.1|10.7|
|**2600**|2.5|5.2|7.1|14.9|1.6|3.4|4.6|9.7|
|**2800**|2.3|4.8|6.5|13.7|1.5|3.1|4.2|8.9|
|**3000**|2.1|4.4|6.0|12.6|1.4|2.9|3.9|8.2|
|**3200**|1.9|4.1|5.5|11.7|1.3|2.7|3.6|7.6|
|**3400**|1.8|3.8|5.2|10.9|1.2|2.5|3.4|7.1|

For this case, 13.8 CFM/person or 6.8 lps/person for kids puts you around 950 ppm. If you are in a classroom and your average CO2 is much higher than 1000 ppm, it's likely is not complying with modern ASHRAE ventilation requirements.

---

We can also do this the long way. Kids sitting at desks is [around 1.3 Met](/tweets/calculating-ventilation-from-co2/). This translates to [0.0033 lps of CO2 for elementary and 0.0045 lps for high school](/tweets/calculating-ventilation-from-co2/). 

|||
|-|-|
|![Chart listing metabolic rates for various activities. Available in text form in the previous link](/metabolic-sitting.png)|![Large chart showing CO2 generation rates based on age, sex and metabolic rates](/co2-elementary.png)|

Elementary:
`420 + 0.0033*1000000/6.8 = 905 ppm`

High School:
`420 + 0.0045*1000000/6.8 = 1081 ppm`

Well below 1500 ppm quoted earlier.

---

Note: I dealt with mechanical ventilation in this thread. Natural ventilation is slightly higher. Still well below 1500 ppm.