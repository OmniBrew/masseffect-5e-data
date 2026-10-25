---
name: Tactical Focus Range
level: 7
klass: sentinel
subclass: bastion
mechanics:
  - type: augment
    value:
      model: tactical-focus
      id: bastion-tactics
      limit:
        - bonus-action
        - reaction
    merge:
      range:
        aoe:
          size: 20
---
At 7th level, your tactical focus increases to :distance{length="20"} per side.
