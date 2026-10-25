---
name: Sentry Turret
version: 1
level: 3
powerType: tech
classes:
  - engineer
  - musician
  - tracker
tags:
  - summon
casting:
  - castingTime:
      length: 1
      unit: action
    duration:
      length: 1
      unit: minute
    concentration: false
    range:
      short: 5
    detonates: false
advancements:
  - id: cryo-turret
    name: Cryo Turret
    text: The turret's mass accelerator machine gun deals 7 (2d6) piercing and 7 (2d6) cold damage. Instead of flamethrower, the turret can innately cast cryo beam 5 times per day.
    casting: []
  - id: shields
    name: Shields
    text: The turret has 30 shield points (regen 0).
    casting: []
---
Construct a sentry turret (stats can be found in the bestiary) in an unoccupied space within :distance{length="5"}. You have complete control over the turret. Any hacking
attempts on the turret are rolled against your Intelligence, not the turret's.

The turret has its own turn in the initiative order, which occurs immediately following your turn.

The turret lasts until its hit points become 0 or lower or until you use a bonus action to destroy it.

__At Higher Levels__: When you cast this power using a power slot of 4th level or higher, the turret deals an additional
1d6 piercing and 1d6 radiant damage with its mass accelerator machinegun and gains 10 additional hit points for
each power slot above the 3rd.
