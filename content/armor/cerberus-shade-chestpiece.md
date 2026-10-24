---
name: Cerberus Shade Chestpiece
coverage: piece
slot: chest
armorType: medium
cost: 31300
manufacturer: cerberus-skunkworks
image: https://vignette.wikia.nocookie.net/masseffect/images/6/67/Cerberus_shade.jpg/revision/latest/scale-to-width-down/700?cb=20130308134524
tags:
  - shields
  - shield_regen
  - set_bonus
andromeda: false
set: cerberus-shade
rarity: spectre
flavor: Cerberus Shade armor is worn by Phantoms who need to be prepared for a wide variety of threats. Its capacitors give modest boosts to shields and shield regeneration time. Many small improvements increase the performance of biotic amps and omni-tools, heat management and kinetic coils for ranged weapons, and synthetic muscle assistors for melee capability.
mechanics:
  - type: me:shields
    capacity:
      type: flat
      value: 10
    regen:
      type: flat
      value: 10
  - type: me:thermal-clip-capacity
    value: 6
  - type: me:medi-gel-capacity
    value: 2
---
- 10 shields (regen 10).
