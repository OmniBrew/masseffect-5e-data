---
name: Ambush
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: When you make a Dexterity (Stealth) check or an initiative roll, you can expend one Command die and add the die to the roll, provided you aren’t incapacitated.
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
type: commands
---
When you make a Dexterity (Stealth) check or an initiative roll, you can expend one Command die and add the die
to the roll, provided you aren’t incapacitated.
