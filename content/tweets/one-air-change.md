---
title: "1 air change only removes 63% of the virus particles. Why?"
date: 2022-02-08T01:38:15.000Z
draft: false
description: "Warning: Math"
summary: "Warning: Math"
categories:
  - Ventilation, Air Quality and CO2
tags:
  - Ventilation
  - Calculations
  - Theory
---
[Source](https://twitter.com/joeyfox85/status/1490862509112365056)

---

### Thought Experiment 1:

- Start with 100 virus particles (VPs).
- Remove all the air in the room (100 VPs).
- Refill the room with air.
- You have 0 VPs left - 100% removal.

### Thought Experiment 2:
- Start with 100 virus particles (VPs).
- Remove half the air in the room (50 VPs).
- Refill half the room with air and let it mix.
- You have 50 VPs left.
- Remove half of the air again (25 VPs).
- Refill the room.
- You have 25 VPs left - 75% removal

### Thought Experiment 3:
- Start with 27 VPs.

- Remove 1/3 of the air (9 VPs).
18 VPs remain. Refill the room.

- Remove 1/3 of the air (6 VPs).
12 VPs remain. Refill the room.

- Remove 1/3 of the air (4 VPs).
8 VPs remaining, 19 removed total.
Refill the room.

- `19/27=70%` of VPs removed.

### How it's really done: calculus

The rate of virus removal is proportional to the concentration of the virus:

`-d(virus removed)/d(volume removed)= C * virus concentration`

`C` is a constant.

This is the classic mixing problem - a differential equation. 

Once you solve it, you get:
```
Old air remaining %=1/e^(air changes)

Fresh air % = 1-old air%=1-1/e^(air changes)
```

|Air Change |Fresh Air % |
|-|-|
|1|63|
|2|86|
|3|95|
|4|98|
|5|99|
