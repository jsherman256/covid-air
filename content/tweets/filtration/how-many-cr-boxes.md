---
title: "How Many Corsi-Rosenthal Boxes Do You Need?"
date: 2022-04-24T18:50:32.000Z
draft: false
description: 
summary: 
categories:
  - HEPA Filters and the Corsi-Rosenthal Box
tags:
  - CR Box
---
[Source](https://twitter.com/joeyfox85/status/1518301381106577414)

---

### Formula
```
Air changes/hour (ACH) = 60 x CADR/Volume
```

### Assumptions
- CR Box `CADR = 275 CFM`
- Goal is `6 ACH`
- Already have `1.5 ACH` from ventilation, so you need `4.5 ACH`

### Imperial units
```
# boxes = 4.5 x volume/(60x275) = 2.7e-4 x volume (cb ft)
```

### In metric (under-ventilated)
```
# boxes = volume (m^3)/100
```

### Examples

1. Typical under-ventilated classroom - 800 sq ft, 9' ceilings = 7200 c.ft
```
# boxes = 2.7e-4 x 7200 = 2
```

2. Classroom with minimum ASHRAE standards:
```
Ventilation = 3.5 ACH
Need 2.5 ACH
# boxes = 2.5 x 7200/(60x275) = 1.1
```

### See Also

{{<tweet user="joeyfox85" id="1481775099271393280">}}