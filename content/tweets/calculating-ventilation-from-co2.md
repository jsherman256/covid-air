---
title: "Calculating Ventilation from CO2 Levels"
date: 2022-06-08T00:43:37.000Z
draft: false
description: 
summary: People breathe out CO2 at a rate depending on their age and activity. Here's a table of the CO2 rate based on the activity
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Ventilation
  - Calculations
  - CO2
---
[Source](https://twitter.com/joeyfox85/status/1534335303607017473)

---

Outdoor air CO2 is around 420 ppm. People breathe out CO2 at a rate depending on their age and activity. Here's a table of the CO2 rate based on the activity:

|Activity|M (met)|Range|
|-|-|-|
|Calisthenics--light effort|2.8||
|Calisthenics--moderate effort|3.8||
|Calisthenics--vigorous effort|8||
|Child care||2.0 to 3.0|
|Cleaning, sweeping--moderate effort|3.8||
|Custodial work--light|2.3||
|Dancing--aerobic, general|7.8||
|Health club exercise classes--general|5||
|Kitchen activity--moderate effort|3.3||
|Lying or sitting quietly||1.0 to 1.3|
|Sitting reading, writing, typing|1.3||
|Sitting at sporting event as spectator|1.5||
|Sitting tasks, light effort (e.g. office work)|1.5||
|Sitting quietly in religious service|1.3||
|Sleeping|0.95||
|Standing quietly|1.3||
|Standing tasks, light effort (e.g. store clerk, filing)|3||
|Walking, less than 2 mph, level surface, very slow|2||
|Walking, 2.8 mph to 3.2 mph, level surface, moderate pace|3.5||

![Large chart showing how much CO2 people exhale depending on their age, sex, and activity level. CO2 generation increases roughly linearly with physical activity level (met in above table). Female infants have the lowest generation rate at 0.0008 liters per second for met of 1.0. Males aged 21 to 30 have the highest rate at 0.0039 liters per second for met of 1.0.](/CO2_Emission_Rate.PNG)

First determine average age and activity. If you are in a low risk setting, with a range of people, I'd assume a metabolic rate of `1.4 met`. A large age range gives around `0.0054 litres/sec (lps)`.

The indoor CO2 = `the outdoor CO2 + amount CO2 generated per person /outdoor flow per person` (x 1 million if you are using PPM)

With the outdoor air CO2 being around 420 parts per million and rearranging, you get:

`Ventilation/person = CO2 generated per person x 1000000/(Indoor CO2-Outdoor CO2)`

Ex. You're in a waiting room. 10 people there and CO2 levels are 1200:

```
0.0054 x 1000000/(1200-420) = 6.9 lps/person = 14.6 cubic ft/min (CFM)/person.
```

Total with `10 ppl = 69 lps or 146 CFM`.

Here's a table I made so you can avoid calculations. Look up the CO2 levels based on the age and activity and multiply it by the number of people to calculate the total air flow.

I'll tell you how to use this for risk assessment in an upcoming thread.

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

You can also find it in [the 3rd tab here](https://docs.google.com/spreadsheets/d/1AjFzhqM_NILYvZjgE8n0CvGZzYh04JpF_DO0phrOcFw/edit#gid=0)