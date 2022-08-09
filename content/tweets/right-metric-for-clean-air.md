---
title: "What's the right metric for clean air?"
date: 2022-05-30T19:03:58.000Z
draft: false
description: We know we want cleaner air, but it's not completely clear how to measure it.
summary: We know we want cleaner air, but it's not completely clear how to measure it. Here's a detailed analysis of the different metrics.
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Ventilation
  - Calculations
---
[Source](https://twitter.com/joeyfox85/status/1531350723841118208)

---

I give [a shorter version in this thread](/tweets/calculating-ventilation/), but here's a more detailed analysis of the different metrics.

First, indoor pollutants come from 3 places: **people, the space and outdoors** (I'm not dealing with outdoors here).

People create CO2, body odor and can also bring viruses to the space. Volatile organic compounds (VOCs) can come from perfume or deodorant.

The space can give off pollutants as well. VOCs can come off paint from walls, cleaning products or chemicals on furniture. Construction materials can contain asbestos and other materials. Carpets are also sources of pollutants.

Here are 5 metrics:

### 1. Flow per area

This metric ignores ceiling height. The people and majority of objects emitting chemicals are on the ground. If the ventilation supplied is properly going to the breathing zone, then you don't care about the ceiling height or volume of the room.

Imagine two spaces with the exact same people and objects, but one had a 10 ft higher ceiling. Does the ventilation need to change there? With proper air mixing - no.

This metric also ignores how many people are there.

### 2. Air changes per hour (ACH)

ACH is how many times the air in a room is changed every hour. In 1970, [CDC set 6 ACH for infection control](https://www.cdph.ca.gov/Programs/CCDPHP/DEODC/EHLB/IAQ/CDPH%20Document%20Library/School_ventilation_and_filtration_ADA.pdf). The only factor is volume. ACH is used by indoor air quality experts and in medical settings.

This ignores how many people are there. It's useful if you care about clearing a hazard from the air in a room like flushing out a room from COVID once someone leaves it. You want to wait a certain amount of air changes before the coast is clear.

It might also be relevant if it's a high ceiling and you need more ventilation because of stratification (poor mixing between upper and lower rooms). But usually if you double the ceiling height, you don't need to double the ventilation.

### 3. Flow per person

When people are equally emitting pollutants, you care about the flow per person. Since CO2 is a pollutant per person, CO2 levels are an indication of the flow per person. This also relates to body odor.

### 4. Virus removal per infectious aerosol generation

This is what you've been waiting for - how to use ventilation to mitigate against COVID. The probability of getting infected is related to the concentration of virus in the air. 

```
Concentration = Generation/Removal

Generation = # infected ppl x activity x infectiousness
Removal = deposition (landing on surfaces) + decay (virus inactivating over time) + ventilation flow + filtration flow + UV
```

Generally, ventilation is the most significant factor of the removal mechanisms.

Some of these factors are difficult to know to fully assess risk, but the main point is the ventilation is not dependent on the number of uninfected people and the size of the space.

We've been using ACH as the metric, but I think it's misguided. I'll explain:

Remember this study? [6 ACH reduces school outbreaks 82%](https://www.reuters.com/world/europe/italian-study-shows-ventilation-can-cut-school-covid-cases-by-82-2022-03-22/). That might be the wrong metric. Assuming 1 infected source in a classroom (typical for an outbreak) and a typical volume of 7000 cubic ft, you get: `7000x6/60=700 cubic ft/minute (CFM)`. 

The study showed that 700 CFM of outdoor air in a classroom can reduce outbreaks by 82% - the volume of the room wasn't necessarily the correct metric. Perhaps more outbreaks occurred in smaller classrooms since they had less total flow. (We don't know)

We can also see the issue with comparing this to flow per person. Let's say you have 30 people and 1 is infected and you have 23 CFM/person - that's 700 CFM/infected person. Outbreak chances reduced by 82%.

Now half of them leave and you keep the same flow per person (this is called demand control ventilation). Now your flow is 350 CFM total, so 350 CFM/infected person. Outbreak chances have now significantly increased.

This is why ACH (not dependent on # people) is better than flow/person for airborne mitigation (I state this in the thread about good ventilation). Although the truth is, if you care about airborne mitigation, the real metric is flow/infected person.

### 5. ASHRAE 62.1.

This is how design ventilation rates are currently calculated. It's a combination of flow per area and flow per person. The goal of this was to address sick building syndrome - when 20% or more of people complained about the air quality. 

These rates (ventilation per person and per square foot) are adjustable based on the type of space since gyms, nail salons, classrooms and food processing facilities all have different types of occupants, activities and contaminants.

However, these rates were not designed to prevent infection from airborne disease.

---

### So why does this matter?

We need to know what our goals are. If the goal is to stop COVID in public spaces, then flow/infected person is what matters.

It can also be from ventilation, filtration or ultraviolet germicidal irradiation (UVGI)-makes no difference.

If we want better test scores, attentiveness and productivity, that's been related to CO2 levels which is outdoor air flow/person. Filtration and UVGI don't help.

If you're providing ventilation to a one person office, no need to mitigate airborne exposure.

If there are plenty of pollutants from the space, the area matters.

If you're flushing a space between uses, you care about ACH.

If there are high ceilings and poor mixing between the upper and lower rooms, then you'll need higher airflow to compensate which means volume is more important than just the area. This can also be mitigated with a destratification fan.

ACH is a straightforward metric, but I don't think there is a basis in physics to use it as an infection control metric which is done in medical settings. This could cause underventilation of small rooms and overventilation of large rooms.

If we want to improve air quality, assess risk and protect people from COVID, we need to use the correct metrics and tools to achieve the desired goals. Other factors like room size, activity and humidity also matter. I'll deal with that in an upcoming thread.