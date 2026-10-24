---
name: Cerberus Nightmare Boots
coverage: piece
slot: legs
armorType: light
cost: 21950
manufacturer: cerberus-skunkworks
image: https://vignette.wikia.nocookie.net/masseffect/images/5/5d/Cerberus_Shade_Female.png/revision/latest?cb=20160619125819
tags:
  - movement
  - set_bonus
andromeda: false
set: cerberus-nightmare
rarity: spectre
flavor: Nightmare armor is worn by Cerberus Phantoms expecting long-range conflicts. Powerful capacitors deliver punishing energy to the Phantom's weapons, and circulating coolant in its gloves allows for more shots before a given thermal clip overheats. The remaining energy focuses on shield strength and regeneration time to help survivability.
mechanics:
  - type: speed-bonus
    value:
      - walk
    bonus:
      type: flat
      value: 15
  - type: me:thermal-clip-capacity
    value: 2
  - type: me:grenade-capacity
    value: 2
---
- Walking speed increased by :distance{length="15"}.
