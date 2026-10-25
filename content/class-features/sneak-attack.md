---
name: Sneak Attack
level: 1
klass: infiltrator
mechanics:
  - type: other
    damage:
      - dieCount:
          type: progressive
          limit: infiltrator
          value:
            1: 1
            3: 2
            5: 3
            7: 4
            9: 5
            11: 6
            13: 7
            15: 8
            17: 9
            19: 10
        dieType: 6
    progressionColumn:
      label: Sneak Attack Damage
      values:
        - 1d6
        - 1d6
        - 2d6
        - 2d6
        - 3d6
        - 3d6
        - 4d6
        - 4d6
        - 5d6
        - 5d6
        - 6d6
        - 6d6
        - 7d6
        - 7d6
        - 8d6
        - 8d6
        - 9d6
        - 9d6
        - 10d6
        - 10d6
      order: 2
---
Beginning at 1st level, you know how to strike subtly and exploit a foe's distraction. Once per turn, you can
deal an extra 1d6 damage to one creature you hit with an attack if you have advantage on the attack roll. The attack must
be made with a melee or ranged weapon.

You don't need advantage on the attack roll if another enemy of the target is within :distance{length="5"} of it, that enemy isn't incapacitated,
and you don't have disadvantage on the attack roll.

The amount of the extra damage increases as you gain levels in this class, as shown in the Sneak Attack column of the
Infiltrator table.
