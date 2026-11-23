---
name: Deep Biotics
level: 3
klass: explorer
subclass: path-of-eezo
mechanics:
  - type: model-choice
    label: Choose a Biotic Cantrip
    model: powers
    options: true
    hide: true
    limits:
      - attr: level
        value:
          - 0
      - attr: classes
        value:
          - explorer
      - attr: powerType
        value:
          - biotic
  - type: power-augment
    powerTypes:
      - biotic
    levels:
      - 0
    dieIncrease: 1
    overflowPerDie: 2
---
At 3rd level, your brain is beginning to attune more finely to the Element Zero in your system. You gain another cantrip
slot that must be occupied by a Biotic Cantrip. When you use a Biotic Cantrip, you bump up the die by one.
A d12 instead gives the power a +2 damage modifier per d12 rolled.
