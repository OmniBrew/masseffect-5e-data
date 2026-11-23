---
name: Disarming Strike
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: When an ally hits a creature with a weapon attack, you can expend one Command die to command them to attempt to disarm the target, forcing it to drop one item of your choice that it’s holding. You add the Command die to the attack’s damage roll, and the target must make a Strength saving throw. On a failed save, it drops the object you choose. The object lands at its feet.
    damage:
      - dieCount: 1
        dieType:
          type: progressive
          limit: tracker
          value:
            3: 8
            10: 10
            14: 12
        label: Command die
    notes:
      - Save DC {{ 8 + profBonus + intMod }} (synthetic beast) or {{ 8 + profBonus + chaMod }} (organic beast)
type: commands
---
When an ally hits a creature with a weapon attack, you can expend one Command die to command them to attempt to
disarm the target, forcing it to drop one item of your choice that it’s holding. You add the Command die to the
attack’s damage roll, and the target must make a Strength saving throw. On a failed save,
it drops the object you choose. The object lands at its feet.
