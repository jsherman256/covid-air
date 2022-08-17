---
title: "Intro to the Packaged Roof Top Unit (RTU)"
date: 2022-03-11T01:41:21.000Z
draft: false
description: I want to do a few tweets about common ventilation issues, but first I need to do an intro to the basic system - the RTU. 
summary: I want to do a few tweets about common ventilation issues, but first I need to do an intro to the basic system - the RTU. It's essentially a home furnace with dampers.
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Basics
  - RTU
  - Ventilation
---
[Source](https://twitter.com/joeyfox85/status/1502097313896046593)

---

It's essentially a home furnace with dampers. Here's what they look like:

||||
|-|-|-|
|![Picture of an RTU. It's a large rectangular box on a rooftop](/rtu1.jpg)|![Picture of an RTU. It's a large rectangular box on a rooftop](/rtu2.jpg)|![Picture of an RTU. It's a large rectangular box on a rooftop](/rtu3.jpg)|

This is a schematic of what it looks like inside. Here are the steps:

1. Air is returned from the space into the unit.
2. The exhaust damper - air leaves here. It's usually a backdraft damper. Air can only flow out and not in. It isn't motorized. 

![Diagram of an RTU. Motorized dampers are partially open allowing 75% recirculated air. The other 25% of air supplied is outdoor air](/rtu-diagram-25-outdoor.png)

3. The mixed air dampers/economizer - these control the ventilation. When they are "open", it means the outdoor air damper is open and the return air damper is closed. This brings in 100% outdoor air. The return damper closing forces the air out through the exhaust damper.

![Diagram of an RTU. Motorized dampers are closed, preventing recirculation of indoor air. 100% of the supplied air is outdoor air](/rtu-diagram-100-outdoor.png)

When they are "closed" the outdoor air damper is closed and the return damper is open. 100% of the air is recirculated. No fresh air.

For safety, dampers always fail to the closed configuration.

![Diagram of an RTU. Motorized dampers are fully open and the outdoor air damper is completely closed. All supply air is recirculated air. No fresh air is being provided](/rtu-diagram-0-outdoor.png)

4. After the dampers, the air is a mix of return and outdoor air, it passes through a replaceable bank of filters like in your home furnace. This catches dust and prevents it from clogging up the coils or being supplied to the space.

5. The air passes through a direct expansion (DX) cooling coil. It works similar to your furnace through compression and expansion of a refrigerant. When it's on, it cools down the air.
6. The air passes through a gas fired heating coil. When it's on, it heats up the air.

7. The fan is what pushes the air.
8. The air is supplied back to the space.

If it is computerized, there are usually 5 temperature sensors:
- a. Space Temp (SPT)
- b. Return Air Temp (RAT)
- c. Outdoor Air Temp (OAT)
- d. Mixed Air Temp (MAT)
- e. Supply Air Temp (SAT)

![Diagram of RTU showing locations of temperature sensors. SPT is in the classroom. RAT is just inside the return air vent. OAT is just before the vent bringing in outdoor air. MAT is just past the junction where return air and outdoor air are mixed, and prior to heating and cooling. SAT is in the duct providing heated/cooled air to the classroom](/rtu-sensors.png)

How the temperatures work:
- If dampers are closed, `MAT = RAT`
- If dampers are open, `MAT = OAT`
- If heating and cooling are off, `SAT = MAT`
- cooling on, `SAT < MAT`
- heating on, `SAT > MAT`

SPT should be close to RAT, but due to stratification, RAT might be a bit higher.

---

### General sequence of operations for the equipment:

### Fan:
- always runs during occupied hours
- at night during the winter, the space temperature is allowed to get colder. If it gets too cold, the fan will turn on to heat the space (night setback).
- before occupancy, the fan will turn on early to heat up the space so when people arrive, it won't be cold. This is called optimal start or morning warmup.
- some places might have morning cooldown and night setback for cooling. Generally not common in Canada.

### Cooling: 
when it's hot outside, if the space is too warm, turn on the cooling. Supply cold air to the zone until it's satisfied.

### Heating: 
when it's cold outside, if the space is too cold, turn on the heating. Supply hot air to the zone until it's satisfied.

### Dampers:
- when the fan is off or unoccupied (night setback or morning warmup), dampers are closed.
- during normal operation, dampers open to a position to provide the minimum amount of required air to the space.
- Free cooling/economizer mode: if it's cooler outside than inside and the space is too hot, the dampers open even more to cool down the space.

---

That's the basics. When all this is computerized, it's put on a building automation system (BAS). That's what I do for a living.

If you want to know the simple ways to improve the system, it's here.

{{<tweet user="DavidElfstrom" id="1488881727862976518">}}
