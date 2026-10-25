---
name: High-Caliber Barrel I
rarity: uncommon
modType: weapon
cost: 12000
tags:
  - extra_damage
  - special
placement: barrel
availability:
  - assault_rifle
  - heavy_pistol
  - smg
  - shotgun
  - sniper_rifle
flavor: Superior kinetic coils increase shot penetration and damage.
mechanics:
  - type: attack-augment
    attackLimit:
      model: weapon
    augmentTypes:
      - damage
      - notes
    bonus:
      type: flat
      value: 1
    notes:
      - type: text
        text: Ignore 1/2 cover
---
+1 on damage rolls made with this weapon. Ignores half cover.
