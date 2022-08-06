---
title: "Comparing Masks and Ventilation/Filtration"
date: 2022-05-17T23:16:32.000Z
draft: false
description: What's more effective - a CR box in the classroom or everyone wearing a cloth mask? Here's how they can be compared.
summary: What's more effective - a CR box in the classroom or everyone wearing a cloth mask? Here's how they can be compared.
categories:
  - Engineering Methods
tags:
  - Masks
---
[Source](https://twitter.com/joeyfox85/status/1526703242578739200)

---

There are different metrics to measure ventilation or filtration, but I'll use clean air delivery rate (CADR). For a new classroom, minimum required CADR is around 400 CFM. Typical is 250 CFM (poor). Really good air quality would be around 750 CFM.

Masks reduce the concentration of the virus you inhale. This table shows the concentration reduction for the different masks. The values I'll use for remaining virus:
Cloth: 75%
Surgical: 50%
Non-fit-tested (NFT) N95: 20%
Fit-tested (FT) N95: 10%

{{< tweet user="brosseau_lisa" id="1449409318412079108" >}}

How much does ventilation reduce the virus in the air?

Concentration is inversely proportional to virus removal. This includes flow from ventilation, filtration, decay and deposition. Decay and deposition makeup around 20-30% as a rough estimate.

{{< tweet user="joeyfox85" id="1526657312001343489" >}}

I'll ignore those effects to simplify the math and assume virus is removed only through ventilation or filtration. The estimate will still give a fairly accurate result.

With this assumption, if you double the ventilation, the virus concentration gets cut in half.

So change in virus concentration = airflow 1/airflow 2

or New Airflow = Old Airflow/% of virus remaining.

For a cloth mask, where 25% removed & 75% of the virus remains, the new airflow = old airflow/0.75 = 1.33 x old airflow.

So in a typical classroom with 250 CFM, the cloth mask would create the equivalent of a classroom with 250x1.33 = 332 CFM. The difference is 332-250=82 CFM.

So wearing a cloth mask in a classroom has the equivalent effect as [a tiny 82 CFM HEPA](https://www.amazon.ca/Purifier-Bedroom-Portable-Replacement-Reminder/dp/B09NLQ9ZPN/ref=sr_1_1_sspa).

Another example: 2-way surgical masks.

They each reduce the concentration by 50%, so total virus remaining is 0.5^2=0.25
New airflow=old airflow/0.25
Using 250 CFM
New airflow = 1000 CFM
The difference is 750 CFM.

So 2-way surgical masking is like having an extra 750 CFM.

I've run the numbers for all the different scenarios here. I've used typical CFMs of 100, 250, 400 and 500 for classrooms.

The table shows what size HEPA filter you would need  to get the equivalent benefit.

---

| Equivalent CFM | | | | | |
|-|-|-|-|-|-|
|Ventilation CFM in Classroom| | 100 | 250 | 400 | 500 |
| | Leakage % | | | | | 
| Cloth Mask | .75 | 33 | 83 | 133 | 167 |
| 2-way Cloth | .56 | 78 | 194 | 311 | 389 |
| Surgical | .5 | 100 | 250 | 400 | 500 |
| 2-way Surgical | .25 | 300 | 750 | 1200 | 1500 |
| Non-Fit-Test Respirator | .2 | 400 | 1000 | 1600 | 2000 |
| 2-way NFT Respirator | .04 | 2400 | 6000 | 9600 | 12000 |
| Fit-Tested Respirator | .1 | 900 | 2250 | 3600 | 4500 |
| 2-way FT Respirator | .01 | 9900 | 24750 | 39600 | 49500 |

| Air Cleaning Method | Equivalent CFM |
| - | - |
| Ventilation | 100-500 |
| Filtration | 100-300 each |
| Upper Room UVGI | 1000-2000 |
| Far UV | 1000-40000 |

---

To compare in a classroom setting:
- CR Box (275 CFM) is better than a surgical mask (250)

- Great ventilation 750 CFM (that's 6 ACH) + CR box is equal to 2-way surgical masking

- Upper room UV which is equivalent to 1600 CFM is better than a non-fit-tested respirator

There were a bunch of assumptions here and it's not a 100% fair comparison. For example, I used a poor (but common) ventilation of 250 CFM. If you have a room that is at modern standards, a surgical mask will provide the equivalent of an extra 400 CFM. (That's a lot)

Conversely, if you are in a really poorly ventilated room with 100 CFM (still common), a surgical mask will provide only an extra 100 CFM, like a medium size HEPA filter. A cloth mask will give you 33 CFM - barely anything. 2-way cloth masking is 78 CFM. Still minimal.

This all assumes consistent and proper masking.

Some important takeaways:
If you are indoors, there is no better option to protect against infection than a proper fitting respirator.

But respirators don't remove the virus, they only reduce the concentration you inhale.

**Masks are the best tool against short range transmission.** Initially when you breathe out, respiratory aerosols are more concentrated. Ventilation can help in that situation, but is less effective. Masks stop short range transmission. 

For masks in schools - if kids are wearing cloth masks in a poorly ventilated room and not wearing them properly, a CR box or HEPA filter would be much more effective.

It shows the importance of air quality and how that amplifies the effectiveness of masks. It also shows why if there is masking, it should be respirators and not cloth masks.

This isn't one or the other, you can do both. But this is a rough comparison between them.

IMHO: This demonstrates that there is low benefit for mask mandates in poorly ventilated schools where cloth masks are allowed. Especially if not worn properly.

If you want an effective way to reduce transmission, you need respirators with good air quality.

---

Fair criticism of this analysis. I discuss the importance of masks for short range transmission, but here’s the math behind it.

{{< tweet user="PrasadKasibhat1" id="1526945047861764096" >}}
