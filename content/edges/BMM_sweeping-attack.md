---
name: Sweeping Attack
mechanics:
  - type: other
    resource:
      reset: off
      displayType: barrier-ticks
      label: Barrier Ticks
    damage:
      - dieCount:
          type: me:barrier-die-count
        dieType:
          type: me:barrier-die-type
        type: force
    shortDesc: When you hit a creature with a melee attack, you can expend one barrier tick to attempt to damage another creature. Choose another creature within :distance{length="5"} of the original target and within your reach. If the original attack roll would hit the second creature, it takes <strong>{{ roll }} force</strong> damage.
type: maneuvers
---
When you hit a creature with a melee attack, you can expend one barrier tick to attempt to damage another creature
with the same attack. Choose another creature within :distance{length="5"} of the original target and within
your reach. If the original attack roll would hit the second creature, it takes force damage equal to the number you roll on your barrier tick.
