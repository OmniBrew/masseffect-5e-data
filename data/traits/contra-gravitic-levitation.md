---
species:
  - hanar
mechanics:
  - type: speed
    speed: walk
    distance: 30
    note: If contra-gravitic levitation device is functional, ignore difficult terrain. If not functional, walking speed becomes 0.
  - type: fall-damage
    reduce:
      dieCount: 4
      dieType: 6
    note: if contra-gravitic levitation device is functional
  - type: condition-immunity
    value: prone
    note: if contra-gravitic levitation device is functional
---
