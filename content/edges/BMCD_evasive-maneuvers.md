---
name: Evasive Maneuvers
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: When an ally moves, you can expend one Command die, rolling the die and adding the number rolled to your AC until they stop moving.
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
When an ally moves, you can expend one Command die, rolling the die and adding the number rolled to your AC until they stop moving.
