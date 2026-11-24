---
name: Protection
mechanics:
  - type: reaction
    shortDesc: When a creature you can see attacks a target other than you that is within :distance{length="5"} of you, expend one barrier tick to impose disadvantage on the attack roll. If the attack hits, the damage is reduced by your barrier tick roll.
    resource:
      reset: off
      displayType: barrier-ticks
      label: Barrier Ticks
    damage:
      - dieCount:
          type: me:barrier-die-count
        dieType:
          type: me:barrier-die-type
        label: Damage reduced
type: fighting-styles
---
When a creature you can see attacks a target other than you that is within :distance{length="5"} of you, you can use your reaction and expend one barrier tick to impose disadvantage on the attack roll. If the attack hits, the damage is reduced by your barrier tick roll.
