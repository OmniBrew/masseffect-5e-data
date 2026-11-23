---
name: Rally
mechanics:
  - type: bonus-action
    resource:
      reset: short
      id: command-dice
      max:
        type: flat
        value: 4
    shortDesc: On your turn, you can use a bonus action and expend one Command die to bolster the resolve of one of your companions. When you do so, choose a friendly creature who can see or hear you. That creature gains temporary hit points equal to the Command die roll + your Charisma modifier.
    damage:
      - dieCount: 1
        dieType:
          type: progressive
          limit: tracker
          value:
            3: 8
            10: 10
            14: 12
        mod: cha
        type: temp
type: commands
---
On your turn, you can use a bonus action and expend one Command die to bolster the resolve of one of your companions.
When you do so, choose a friendly creature who can see or hear you. That creature gains temporary hit points equal to
the Command die roll + your Charisma modifier.
