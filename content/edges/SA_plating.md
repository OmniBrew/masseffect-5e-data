---
name: Supercharged Plating
mechanics:
  - type: resistance
    value: lightning
  - type: other
    name: Supercharged Plating
    damage:
      - dieCount: 1
        dieType:
          type: progressive
          limit: experiment
          value:
            1: 4
            5: 6
            9: 8
            13: 10
            17: 12
        type: lightning
        bonus:
          type: level
          value: experiment
    shortDesc: An enemy that hits you in melee takes {{ roll }}.
type: supercharged-augments
---
You become resistant to Lightning damage. Whenever an enemy hits you in melee range, it takes
Lightning damage equal to one roll of your Exploit Die + your Experiment level.
