---
name: Gravity Field
version: 1
level: 1
powerType: biotic
classes:
  - adept
  - vanguard
tags:
  - control
casting:
  - castingTime:
      length: 1
      unit: action
    dc:
      base: 8
      proficient: true
      save: str
    conditions:
      - restrained
    duration:
      length: 1
      unit: minute
    concentration: true
    range:
      short: 90
      aoe:
        type: cube
        size: 15
    detonates: false
    primes: force
advancements:
  - id: pulsing-field
    name: Pulsing Field
    text: As a bonus action, for the duration of the power, you can force a number of creatures equal to twice the power level that are within the gravity field to make a Strength saving throw or be restrained until the power ends.
    casting: []
  - id: warping-field
    name: Warping Field
    text: A creature takes 1d6 necrotic damage per power level when it enters the gravity field for the first time on a turn or ends its turn there.
    casting:
      - damage:
          - dieCount: 1
            dieType: 6
            type: necrotic
---
You create a field of unstable gravity in a :distance{length="15" adj} cube starting from a point within range.  For the duration, this
space becomes difficult terrain.

A creature in the area when you cast the power must succeed on a Strength saving throw or be :condition{id="restrained"}
until the power ends. A creature restrained by this power can use its action to make a Strength check against your
power save DC. On a success, it frees itself.

When the power ends, the gravity field dissipates.
