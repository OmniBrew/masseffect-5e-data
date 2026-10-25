---
name: Blood Trail
level: 13
klass: infiltrator
subclass: stalker
mechanics:
  - type: attack-augment
    ask: Did the target take damage since the end of your last turn?
    attackLimit:
      model: weapon
      type: ranged
    augmentTypes:
      - hit
    bonus:
      type: flat
      value: 2
    addDamage:
      - dieCount: 1
        dieType: 8
---
When a creature is freshly wounded, you can almost taste the the meal of a fresh kill, pushing you to bring the
prey down as soon as possible.

At 13th level, you gain +2 to hit and +1d8 to damage rolls on all ranged weapon attacks on any creatures
that have already taken any damage between the end of your last turn and the start of this turn.
