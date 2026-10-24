---
name: Riposte
mechanics:
  - type: reaction
    resource:
      reset: off
      displayType: barrier-ticks
      label: Barrier Ticks
    damage:
      - dieCount:
          type: me:barrier-die-count
        dieType:
          type: me:barrier-die-type
    shortDesc: When a creature misses you with a melee attack, you can use your reaction and expend one barrier tick to make a melee attack against the creature. If you hit, you add <strong>{{ damage }}</strong> to the attack’s damage roll.
type: maneuvers
---
When a creature misses you with a melee attack, you can use your reaction and expend one barrier tick to make a melee
attack against the creature. If you hit, you add the barrier tick to the attack's damage roll.
