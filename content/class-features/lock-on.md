---
name: Lock On
level: 15
klass: soldier
subclass: legionnaire
mechanics:
  - type: other
    shortDesc: "Using Hold Your Ground or attacking with an SMG: +1 to hit and +1d4 damage on all your attacks this round."
    toggle:
      id: lock-on
      whenOn:
        - type: attack-augment
          augmentTypes:
            - hit
          bonus:
            type: flat
            value: 1
        - type: attack-augment
          augmentTypes:
            - damage
          addDamage:
            - dieCount: 1
              dieType: 4
---
Your nerves have become more steeled when holding your ground against a potential horde, allowing you to focus your
aim better against the victims of your wrath.

At 15th level, whenever you're using Hold Your Ground or attacking with an SMG, all of your attacks this round
will gain a +1 to hit and +1d4 to damage rolls.
