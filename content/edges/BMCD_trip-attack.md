---
name: Trip Attack
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: When you hit a creature with a weapon attack, you can expend one Command die to attempt to knock the target down. You add the Command die to the attack’s damage roll, and if the target is Large or smaller, it must make a Strength saving throw. On a failed save, you knock the target prone.
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
When you hit a creature with a weapon attack, you can expend one Command die to attempt to knock the target down. You
add the Command die to the attack’s damage roll, and if the target is Large or smaller, it must make a Strength saving
throw. On a failed save, you knock the target prone.
