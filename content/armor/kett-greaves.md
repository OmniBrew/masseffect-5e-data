---
name: Kett Greaves
coverage: piece
slot: legs
armorType: heavy
cost: 30400
manufacturer: kett
image: https://vignette.wikia.nocookie.net/masseffect/images/0/08/MEA_Kett_Unity_Legs.png/revision/latest/scale-to-width-down/350?cb=20180510050500
tags:
  - movement
  - set_bonus
andromeda: true
set: kett
rarity: rare
flavor: Although this hardsuit's basic materials-ceramic armor plating and kinetic padding-are Initiative standard, kett biotech permeates the overall design and feeds directly into the user's nervous system. Kett armor enhances combat prowess through chemical regulation and stimulation.
mechanics:
  - type: me:thermal-clip-capacity
    value: 2
  - type: me:grenade-capacity
    value: 2
  - type: speed-bonus
    value:
      - walk
    bonus:
      type: flat
      value: 10
---
- Increase walking speed by :distance{length="10"}.
