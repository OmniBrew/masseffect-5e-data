---
name: Slam
version: 1
level: 0
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
    damage:
      - dieCount: 2
        dieType: 8
        type: bludgeoning
    duration:
      length: 0
      unit: instant
    concentration: false
    range:
      short: 90
    detonates: false
advancements:
  - id: stun
    name: Stun
    text: If the target is a creature, it must pass a Constitution saving throw or becomes stunned until the end of your next turn.
    casting:
      - dc:
          base: 8
          proficient: true
          save: con
        notes:
          - CON save (DC {{ dc }}) or stunned
  - id: reaction
    name: Reaction
    text: When a creature or object you can see becomes lifted, you may cast Slam on it as a reaction.
    casting:
      - altCasting:
          - length: 1
            unit: reaction
            reaction: When a creature you can see becomes lifted
---
Target a lifted creature or object and slam it to the ground dealing 2d8 bludgeoning damage and knocking it prone. The
target is no longer lifted.

The number of targets increases by 1 when you reach 5th level (2), 11th level (3) and 17th level (4).
