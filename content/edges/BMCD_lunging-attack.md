---
name: Lunging Attack
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: When you make a melee weapon attack on your turn, you can expend one Command die to increase your reach for that attack by :distance{length="5"}. If you hit, you add the Command die to the attack’s damage roll.
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
When you make a melee weapon attack on your turn, you can expend one Command die to increase your reach for that
attack by :distance{length="5"}. If you hit, you add the Command die to the attack’s damage roll.
