---
name: Rally Point
species:
  - exaltation-anointed
mechanics:
  - type: other
    shortDesc: "Speed reduced to 0 at the start of your turn: +proficiency to the DC of your next Burst Fire this turn."
    toggle:
      id: rally-point
      whenOn:
        - type: attack-augment
          attackLimit:
            model: weapon
            special: bf
          augmentTypes:
            - dc
          bonus:
            type: proficiency
---
At the start of your turn, you may reduce your speed to 0 to increase the DC of
the next Burst Fire action you take this turn by your proficiency bonus.
