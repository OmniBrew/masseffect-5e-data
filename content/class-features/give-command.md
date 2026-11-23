---
name: Give Command
level: 3
klass: tracker
subclass: beast-master
mechanics:
  - type: other
    name: Command Dice
    damage:
      - dieCount: 1
        dieType:
          type: progressive
          limit: tracker
          value:
            3: 8
            10: 10
            14: 12
        label: Command Die
    resource:
      id: command-dice
      reset: short
      max:
        type: flat
        value: 4
    shortDesc: Spend one on a Command you know.
  - type: model-choice
    options: true
    model: commands
---
As a commander of man and beast, you are able to give orders to not only your beast, but also your allies.

Starting at 3rd level, you gain 4 Command Dice, which are d8s. Choose 3 Commands from the options below. You learn
these Commands, and you can use them if the described trigger occurs during combat.

If a command requires a saving throw from the target, the DC is 8 + your proficiency bonus + your Intelligence modifier
(Synthetic Only) or your Charisma modifier (Organic).

You regain all Command dice at the end of a short rest.

::edge-list{type="commands"}
::
