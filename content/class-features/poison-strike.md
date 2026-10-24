---
name: Poison Strike
level: 10
klass: vanguard
subclass: cabal
mechanics:
  - type: augment
    value:
      model: vanguard
      id: venom-training
      limit:
        - natural-weapon
    merge:
      value:
        damage:
          dieCount: 2
        html: |-
          When you take the Attack Action to use your Venom Gauntlets, you can teleport up to :distance{length="15"}
             before every attack you make.

          If you attack two different targets with each of the attacks provided by your
             Attack action, you can make a third attack against another different target.
        notes:
          - Can be used for Two-Weapon Fighting
          - Teleport :distance{length="15"}
---
At 10th level, when you take the Attack Action to use your Venom Gauntlets, you can teleport up to :distance{length="15"}
before every attack you make. If you attack two different targets with each of the attacks provided by your
Attack action, you can make a third attack against another different target.

The damage of your Venom Gauntlets increases to 2d8 poison damage.
