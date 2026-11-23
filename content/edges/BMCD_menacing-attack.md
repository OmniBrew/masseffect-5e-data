---
name: Menacing Attack
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: When you hit a creature with a weapon attack, you can expend one Command die to attempt to frighten the target. You add the Command die to the attack’s damage roll, and the target must make a Wisdom saving throw. On a failed save, it is frightened of you until the end of your next turn.
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
When you hit a creature with a weapon attack, you can expend one Command die to attempt to frighten the target.
You add the Command die to the attack’s damage roll, and the target must make a Wisdom saving throw. On a failed save,
it is frightened of you until the end of your next turn.
