---
name: Slow Fall
version: 1
level: 0
powerType: biotic
classes:
  - adept
  - vanguard
tags:
  - movement
casting:
  - castingTime:
      length: 1
      unit: reaction
      reaction: when you or a creature within :distance{length="30" abbr} of you falls
    duration:
      length: 1
      unit: minute
    concentration: true
    range:
      short: 30
    detonates: false
advancements:
  - id: improved-duration
    name: Improved Duration
    text: Increase the duration to 5 minutes
    casting:
      - duration:
          length: 5
          unit: minute
  - id: navigate
    name: Navigate
    text: As you fall, you can direct your fall by :distance{length="5"} in any direction except up. You may do this once per round.
    casting: []
---
When you or a creature within :distance{length="30"} of you falls, choose up to five falling creatures within range. Create a negative mass
effect field around each creature, slowing the rate of descent to :distance{length="60"} per round. If the creature lands before the power
ends, it takes no Falling damage and can land on its feet, and the power ends for that creature.
