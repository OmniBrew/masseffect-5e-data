---
name: The Free Hand
mechanics:
  - type: other
    shortDesc: "Holding no more than one light, non-two-handed weapon: +2 to hit with ranged power attacks."
    toggle:
      id: FS_the-free-hand
      whenOn:
        - type: attack-augment
          attackLimit:
            model: power
            type: ranged
          augmentTypes:
            - hit
          bonus:
            type: flat
            value: 2
type: fighting-styles
---
When holding no more than one light, non-two-handed weapon, you gain a +2 bonus to hit with ranged power attacks.
