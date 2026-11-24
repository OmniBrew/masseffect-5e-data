---
name: Feinting Attack
mechanics:
  - type: bonus-action
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: You can expend one Command die and use a bonus action on your turn to command an ally to feint, choosing one creature within :distance{length="5"} of the ally as their target. Your ally has advantage on its next attack roll against that creature this turn. If that attack hits, add the Command die to the attack’s damage roll.
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
You can expend one Command die and use a bonus action on your turn to command an ally to feint, choosing one creature
within :distance{length="5"} of the ally as their target. Your ally has advantage on its next attack roll
against that creature this turn. If that attack hits, add the Command die to the attack’s damage roll.
