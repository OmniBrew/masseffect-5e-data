---
name: Primal Processor
mechanics:
  - type: saving-throw
    value: int
  - type: saving-throw
    value: cha
  - type: resistance
    value: psychic
  - type: other
    name: Primal Processor
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
        type: psychic
    shortDesc: A creature that deals you psychic damage takes {{ roll }}.
type: primal-augments
---
You gain proficiency in Intelligence and Charisma Saving throws, and you become resistant to Psychic damage.
Any creature who causes you Psychic damage takes Psychic damage equal to one roll of your Exploit die.
