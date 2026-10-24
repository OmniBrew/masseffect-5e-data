---
name: Stimulant Pack
version: 1
level: 0
powerType: combat
classes:
  - infiltrator
  - soldier
  - vanguard
  - explorer
tags:
  - buff
casting:
  - castingTime:
      length: 1
      unit: bonus_action
    duration:
      length: 1
      unit: minute
    concentration: false
    range:
      short: 0
    detonates: false
    resource:
      reset: long
      max:
        type: flat
        value: 1
advancements:
  - id: friendly
    name: Friendly
    text: You can inject a willing creature within melee range with the stimulant pack.
    casting:
      - range:
          short: 5
  - id: high-tolerance
    name: High Tolerance
    text: You can use stimulant pack twice per long rest.
    casting:
      - resource:
          max:
            value: 2
---
Inject yourself with a stimulant pack. For the next minute, whenever you make an attack roll or saving throw,
you can roll a d4 and add the number rolled to the attack roll or saving throw.

You must finish a long rest before you can use this feature again.
