---
name: Cranial Trauma System
rarity: uncommon
modType: weapon
cost: 8000
tags:
  - special
placement: barrel
availability:
  - heavy_pistol
flavor: Increase headshot lethality by balancing barrel calibration so that ammunition pierces bone and explodes in soft tissue.
mechanics:
  - type: attack-augment
    attackLimit:
      model: weapon
    augmentTypes:
      - damage
    addCritDie: 1
---
Roll one additional weapon damage die when determining the extra damage for a critical hit with a ranged attack made with this weapon.
