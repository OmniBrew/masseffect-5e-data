---
name: Contra-Gravitic Levitation
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
When not in water, you use a contra-gravitic levitation pack to move. It provides a
walking speed of 12 meters and you hover 1 meter from the ground, providing the following benefits:
- You are immune to becoming prone
- You reduce falling damage by 4d6
- You ignore any penalties caused by difficult terrain.

However, when you suffer a critical hit, you must roll a d20. On a 1 or a 2, the device malfunctions and you fall
to the ground. Your walking speed becomes 0 and you are considered prone. You or another creature can use
an Action to repair the pack with a successful DC 15 Intelligence (Engineering) check.
