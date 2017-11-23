---
title: "Details"
bg: green
color: black
fa-icon: align-left
ref: "details"
lang: "en"
---

## Principle

<div class="i4x3">
  <div id="slideshow">

<div markdown="1">
### La romaine de base
![1](img/principe01.png)
</div>
    
<div markdown="1">
### On motorise le déplacement du contrepoids
![2](img/principe02.png)
</div>
    
<div markdown="1">
### Une fourche optique détecte l'équilibre
![3](img/principe03.png)
</div>
    
<div markdown="1">
### Un microcontrôleur quelconque pilote l'ensemble
![4](img/principe04.png)
</div>

<div markdown="1">
### Envoi de la donnée...
![5](img/principe05.png)
</div>

  </div>
</div>.


## Why a mechanical scale, and not a load cell?

- Because load cell are not supposed to be under continuous constraint.
  * A creep phenomen make measurement unstable after some time, this is well documented
  * Load cells manufacturers don't communicate on creep over 30 minutes...
  * Typical use case implies a tare between each measurement, not possible in hive monitoring scenario
  * We check this on our first prototype using load cells, it was worse than expected
  * Mechanical scale is not subject to this phenomena. Even if structure creeps, measurement doesn't change.

- Because we don't depend on any complicated part that we must outsource
  * This makes possible to keep price low
  * Easier to understand what could go wrong and repair
  * DIY-ers friendly

- Principle is simple and old as ancient Rome

- 


-------------------------

## Connectivity

- WiFi
  * Included in every board
  * Cheapest option if you have a hotspot accessible
  * User-friendly configuration with a smartphone or laptop
  * Master-slave scenario, for sharing a single GSM or Sigfox endpoint

- Sigfox (optional)
  * Best option for battery life if no hotspot
  * Subscription cheaper than GSM
  * Network coverage complementary with GSM
  * [World roll-out in progress](https://www.sigfox.com/en/coverage)

- GSM (optional)
  * Best coverage all around the world

-------------------------
  
## Autonomy

Best energy is the one you don't use...

- First, highly optimized electronic
  * 100nA sleep current
  * Motor driving strategy
  * Modulable measurement frequency and data send along the year
  * ...

- Then we look for the best trade-off between environmental impact, cost, availibility of batteries
  * We managed to achieve a good autonomy with simple alkaline batteries
  * On a 10 years lifecycle, rechargeable battery, Li-ion or Ni-MH, with or without solar panel as an higher cost and impact
  * AA alkaline batteries are the most available battery all around the world

With 3xAA alkaline batteries, we expect 2-5 years autonomy, depending on climate, measurement frequency etc...

-------------------------

## Construction

We designed an easy to assemble kit, made of aluminium profiles and laser cut stainless steel, joint mainly with rivet.
Very few 'other' parts, a simple motor, a belt, linear bearing, optical end stop. That's it.



To be continued....