---
title: "Common Issues: Broken Dampers"
date: 2022-04-21T19:05:40.000Z
draft: false
description: Broken Dampers. This is probably the most common issue. Ventilation gets cut off, no one notices and it remains unfixed for many years.
summary: Broken Dampers. This is probably the most common issue. Ventilation gets cut off, no one notices and it remains unfixed for many years.
categories:
  - Ventilation, Air Quality and CO2
  - Common Ventilation Issues
tags:
  - Ventilation
---
[Source](https://twitter.com/joeyfox85/status/1517218027644854274)

---

### Broken Dampers

The mixed air dampers/economizer are [dampers that modulate to select](/tweets/intro-to-rtu/) between supplying return air or outdoor air. When they are fully "closed", it's 100% return air and 0% outdoor air. When they are "open", it's 0% return air and 100% outdoor air.

![Diagram of an RTU. Motorized dampers are closed, preventing recirculation of indoor air. 100% of the supplied air is outdoor air](/rtu-diagram-100-outdoor.png)

Dampers are designed to fail in the "closed" position - no outdoor air. Why? [This protects the equipment](/tweets/hvac-priorities/) and the people in the space. Bringing in 100% outdoor air can damage the equipment and freeze or overheat the occupants.

If the heating or cooling system are broken, people will notice and complain. If ventilation isn't working, [most people don't notice](https://twitter.com/DavidElfstrom/status/1513903768185753611). This even happens when fans are broken for long periods of time. If dampers break, they remain broken.

Preventative maintenance should fix this, but it doesn't. A school I investigated (not from work) in August 2020 had 16 RTUs. 9 of them had broken dampers. The maintenance contractors didn't bother checking or fixing them since no one complained.

---

### How To Diagnose

The only way a non-professional can do this is by monitoring the CO2. If you check the flow from the diffusers, it will look normal. You'd expect CO2 levels to rise since outdoor air isn't being supplied.

There might be days that the CO2 looks okay. There could be some outdoor air leakage through the dampers, low capacity or if the windows are open, it would be fine. But that's why it's important to constantly monitor the CO2.

In my job, I can easily diagnose this from the building automation system. From the temperatures inside the unit, if the dampers are supposed to be open, but the mixed air temperature (MAT) equals the return air temperature (RAT), [they have failed](/tweets/intro-to-rtu/).

When I commission units, I also check the flow going into the outdoor air damper and also visually confirm it's moving from the outside. You can also see the backdraft dampers flapping from the exhaust air. HVAC technicians can check by opening up the unit. 

![Picture of a rooftop unit with arrows showing where air enters and leaves](/rtu-annotated.jpg)

---

This is typical of a constant problem with the industry. There is no incentive to fix broken dampers.
- It costs money
- Costs effort and time
- Increases utilities bill
- No one will notice
- No oversight or enforcement

Why bother? And so they remain broken.

Two things we can do is work on regulations to fix this (good luck) and educating people to advocate for themselves. If there's high CO2 levels or smells linger for too long, first check the air flow. If it's fine, ask the building operator to ensure the dampers are working.