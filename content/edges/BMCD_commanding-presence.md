---
name: Commanding Presence
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: When you make a Charisma (Intimidation), a Charisma (Performance), or a Charisma (Persuasion) check, you can expend one Command die and add the Command die to the ability check.
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
When you make a Charisma (Intimidation), a Charisma (Performance), or a Charisma (Persuasion) check,
you can expend one Command die and add the Command die to the ability check.
