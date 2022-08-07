---
title: "What Should Your Ventilation Be?"
date: 2022-07-01T19:53:44.000Z
draft: false
description:
summary: You can use CO2 sensors to make sure the ventilation is working, but first you need to know what the CO2 should be. To understand that, you need to calculate the ventilation. Here's how you do it.
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Ventilation
  - ASHRAE
  - Calculations
---
[Source](https://twitter.com/joeyfox85/status/1542959661829312512)

---

You can use CO2 sensors to make sure the ventilation is working, but first you need to know what the CO2 should be. To understand that, you need to calculate the ventilation. Here's how you do it.

First a caveat, there are tons of exceptions for systems like stratified air distribution, personalized ventilation, high supply air temperature, multizone systems and others, but these calculations work most of the time, so you can use it as an estimate.

Here are the steps:

### 1. Find out 3 things:

- The area of the room
- The number of people
- The type of room.

### 2. Look up numbers in the ASHRAE table.

- Go to this link: https://ashrae.org/technical-resources/standards-and-guidelines
- Click on "Standard 62.1-2019", about half way down the page.
- Pages 19-23 (labelled 17-21 in the document) contain table 6-1. You need to find the area and person flows from the table for the room type. They are labelled as `Rp` and `Ra`.

Example - barber shop: on page 22/92, `Rp = 7.5 cfm/person`, `Ra = 0.06 cfm/ft^2`.

### 3. Once you have the info, use the formula:

`Rp x # people + Ra x area`

Example, 1000 sq ft barbershop with 15 people:
`7.5 x 15 + 0.06 x 1000= 172.5 CFM` of outdoor air.

I'll show you how to estimate the CO2 levels in an upcoming thread.

---

Now try it yourself:

- Classroom, 25 people, 800 sq ft
- Place of worship, 300 people, 4000 sq ft
- Gym, 15 people, 3500 sq ft
