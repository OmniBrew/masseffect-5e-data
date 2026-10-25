---
name: Vortex
version: 1
level: 3
powerType: biotic
classes:
  - adept
  - sentinel
  - vanguard
  - explorer
tags:
  - damage
casting:
  - castingTime:
      length: 1
      unit: action
    dc:
      base: 8
      proficient: true
      save: str
    damage:
      - dieCount: 6
        dieType: 10
        type: force
    conditions:
      - prone
    duration:
      length: 0
      unit: instant
    concentration: false
    range:
      short: 0
      aoe:
        type: cone
        size: 30
    detonates: false
  - damage:
      - dieCount: 8
  - damage:
      - dieCount: 10
advancements:
  - id: radial
    name: Radial
    text: You may cast the vortex in a :distance{length="15" adj}-radius sphere centered on you instead.
    casting: []
  - id: damage
    name: Damage
    text: Increase the damage to d12
    casting:
      - damage:
          - dieType: 12
---
You intertwine negative and positive mass effect fields to create a swirling vortex. Creatures within a :distance{length="30" adj} cone must
make a Strength saving throw. On a failed save a creature takes 6d10 force damage, or half as much damage on a successful one.

Creatures that fail the saving throw are thrown 1d6 + :distance{length="5"} away from you and become prone.

__At Higher Levels__: When you cast this power using a power slot of 4th level or higher, increase the damage by 2d10 for
each slot level above the 3rd.
