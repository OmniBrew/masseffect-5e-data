---
name: Collector SMG
rarity: spectre
weaponType: smg
cost: 59000
weight: 7
damage:
  dieCount: 2
  dieType: 8
  type: piercing
range:
  short: 25
  long: 75
image: https://vignette.wikia.nocookie.net/masseffect/images/6/68/ME3_Collector_SMG.png/revision/latest/scale-to-width-down/350?cb=20121009204046
andromeda: false
properties:
  - id: special
  - id: two-handed
  - id: burst-fire
  - id: light
  - id: vented
  - id: heat
    value: 6
slots: 2
---
The Collector SMG does not use thermal clips. Instead, use a d6 to track the "heat". Whenever you 
make a ranged attack with the weapon, spin down the die 1 face. Every round that you don't fire the 
weapon, spin the die up 1 face. This represents the weapon internally cooling off. If you ever spin 
down the die to 0, the weapon jams and cannot be fired again this combat.
