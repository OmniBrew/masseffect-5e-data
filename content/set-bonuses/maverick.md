---
bonuses:
  - threshold: 2
    text: Roll one additional weapon damage die when determining the extra damage for a critical hit with a weapon attack.
    mechanics:
      - type: attack-augment
        attackLimit:
          model: weapon
        augmentTypes:
          - damage
        addCritDie: 1
  - threshold: 4
    text: Your weapon attacks score a critical hit on a roll of 18–20.
    mechanics:
      - type: attack-augment
        attackLimit:
          model: weapon
        augmentTypes:
          - hit
        crit: 18
max: 4
---
