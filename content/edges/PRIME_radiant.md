---
name: Radiant
type: primers
mechanics:
  - type: me:primer-detonation
    levels:
      - 1
      - 5
      - 11
      - 17
    tiers:
      - damage:
          - dieCount: 3
            dieType: 4
            type: radiant
        dc:
          base: 15
          save: con
        shortDesc: Each creature within :distance{length="10"} of the detonated creature suffers {{ damage }} must succeed on DC 15 Constitution saving throw or become :condition{id="poisoned"} for 1 hour.
      - damage:
          - dieCount: 4
      - damage:
          - dieCount: 5
      - damage:
          - dieCount: 6
---
A creature that is primed: radiant is also :condition{id="poisoned"} until the primed: radiant condition ends.
When a creature that is primed: radiant detonates, each creature within :distance{length="10"} of it suffers
3d4 radiant damage and must succeed on DC 15 Constitution saving throw or become :condition{id="poisoned"} for 1 hour.
