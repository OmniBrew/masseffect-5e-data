---
name: Unlimited Power
level: 18
klass: vanguard
subclass: ravager
mechanics:
  - type: attack-augment
    ask: Spend a barrier tick (target within :distance{length="5"})?
    augmentTypes:
      - damage
    addDamage:
      - dieCount: 2
        dieType: 8
        type: force
---
At 18th level, you've mastered using your unstable barrier in both defense and offense. Whenever you make a successful
attack roll on an enemy within :distance{length="5"} of you, you may spend one barrier tick to add your barrier's
damage reduction roll (2d8) as bonus Force damage. On a critical hit, this force damage dice also doubles.
