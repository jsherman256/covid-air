---
title: "Comparing Electronic Air Cleaning Equipment and HEPA Filters"
date: 2022-05-01T18:38:30.000Z
draft: false
description: Electronic air cleaning equipment producers make claims like 99.9% reduction of contaminants in 60 minutes. What does that mean? How does it compare to stand-alone HEPA filters?
summary: Electronic air cleaning equipment producers make claims like 99.9% reduction of contaminants in 60 minutes. What does that mean? How does it compare to stand-alone HEPA filters?
categories:
  - HEPA Filters and the Corsi-Rosenthal Box
---
[Source](https://twitter.com/joeyfox85/status/1520835065646915584)

---

This is inspired by an article that just came out in April 2022 ASHRAE journal by Stephens et al where they used regressions for comparing them. I'm going to derive a formula here. 

But first, what are we comparing? 
HEPA filters use passive or subtractive cleaning.

They remove particles from air that passes through them and deliver clean, particle-free air.

The electronic air cleaners discussed here do not provide clean air. They are active or additive cleaners and they put ions, hydroxyl radicals or other particles into the air.

The goal is to eliminate pollutants in the space. They can't measure a clean air delivery rate (CADR), only a % reduction in particles in a certain space and time, but you can use this to calculate an equivalent clean air delivery rate. Here's how:

---

Here, I give a non-rigorous derivation of [the relationship]({{<relref "one-air-change">}}) between % clean air and air changes (AC).

The formula is: `% reduction = 1-e^-(AC)`

This can be rearranged so that: `Equivalent AC = -ln (1-% reduction)`

So a 99% reduction = `-ln(0.01)=4.6 AC`

Here's a table:

|AC|% Reduction|
|-|-|
|1|63|
|2|86|
|3|95|
|4|98|
|5|99.3|
|6|99.7|
|10|99.995|
|15|99.99997|

Once you get above 5 air changes, it's just 99 with a bunch of 9s afterwards. In a small chamber, lots of air changes isn't that meaningful.

---

CADR = volume x AC/time, so

```
Equivalent CADR for air cleaner = - volume x ln(1-% reduction)/time
```

You need these 4 pieces of data: % reduction with equipment on, % reduction with off (control), volume & time. Otherwise it's meaningless.

Example from ASHRAE:
`95% reduction, 500ft^3 chamber, 60 minutes.` Sounds good?
`Equivalent CADR = -500 x ln (0.02)/60=25 CFM`

**CR Box is 275 CFM, 11 times better.**

What % would a CR Box give you in these conditions?

`AC = 60x275/500 = 33`

The number would be `1-e^-33= 99.999999999999999999...%` . It's too close to 1 to calculate.

The point is, these numbers can sound good, but really suck.

I'm also ignoring here the possible creation of harmful byproducts like formaldehyde or ozone.

Go look at their websites - if they don't tell you the volume of the test chamber or the % reduction from when the unit is off, it's garbage data. It's as helpful as saying that a HEPA filter can filter 99.97% of particles and not telling you how powerful the fan is.