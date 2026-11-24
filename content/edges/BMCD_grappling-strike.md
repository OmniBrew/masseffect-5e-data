---
name: Grappling Strike
mechanics:
  - type: other
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: Immediately after your beast hits a creature with a melee attack on your turn, you can expend one Command die and then have your beast try to grapple the target as a bonus action (see the Player’s Handbook for rules on grappling). Add the Command die to your beast's Strength (Athletics) check.
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
Immediately after your beast hits a creature with a melee attack on your turn, you can expend one Command
die and then have your beast try to grapple the target as a bonus action (see the Player’s Handbook for rules
on grappling). Add the Command die to your beast's Strength (Athletics) check.
