---
name: Electrical Conduits
rarity: rare
modType: weapon
cost: 15000
tags:
  - augmentation
placement: ammo
availability:
  - assault_rifle
  - heavy_pistol
  - smg
  - shotgun
  - sniper_rifle
flavor: Augment the weapons firing system to arc lightning.
mechanics:
  - type: me:weapon-augment
    shortRangeMax: 30
    longRangeMax: 60
  - type: adjust-weapon-props
    remove:
      - burst-fire
      - double-tap
    add:
      - arc
---
The weapon loses the Burst Fire and Double Tap properties and gains the Arc property. If its range is
farther than :distance{length="30" num-only}/[:distance{length="60"}], its range becomes
:distance{length="30" num-only}/[:distance{length="60"}].
