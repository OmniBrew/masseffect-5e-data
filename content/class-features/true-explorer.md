---
name: True Explorer
level: 20
klass: explorer
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
    append:
      klass: explorer
  - type: model-choice
    label: Choose a Combat Cantrip
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
          - combat
    append:
      klass: explorer
  - type: reaction
    name: True Explorer
    shortDesc: "When you detonate a primed target: prime it again with the same type."
---
Your abilities have reached their peak, and the galaxy is ripe for your exploring. You double the number of cantrips
you select every short rest with The Right Cantrip for the Job.

In addition, whenever you detonate a primed target, you can use your reaction to reprime the target in the same kind
of priming it had before you detonated it.
