---
name: Power from Pain
level: 3
klass: soldier
subclass: incubus
mechanics:
  - type: other
    damage:
      - dieCount:
          type: progressive
          limit: soldier
          value:
            3: 1
            7: 2
            10: 3
            15: 4
            18: 5
        dieType: 6
---
Your greatest strength lies in inflicting pain on others. Especially enemies that are already wounded are prime targets
for your agonizing strikes.

Starting at 3rd level, once per turn when you hit a creature below their maximum hit points, you deal bonus damage
equal to 1d6 damage of the same type as your weapon’s. This damage scales to 2d6 at level 7, 3d6 at
level 10, 4d6 at level 15, and 5d6 at level 18.
