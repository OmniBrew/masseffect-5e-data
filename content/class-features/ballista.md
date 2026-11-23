---
name: Ballista
level: 18
klass: engineer
subclass: bowman
mechanics:
  - type: augment
    value:
      model: engineer
      id: omni-bow
      limit:
        - powers
    merge:
      merge:
        damage:
          - {}
          - bonus:
              type: proficiency
            label: Engineer's Efficiency element
---
At 18th level, your Bowshot now adds your proficiency modifier to their damage, in the form of the
elemental effect of your Engineer's Efficiency power.
