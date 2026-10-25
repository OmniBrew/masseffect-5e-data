---
name: Titan Armor
coverage: suit
armorType: heavy
cost: 87550
manufacturer: rosenkov-materials
image: https://vignette.wikia.nocookie.net/masseffect/images/5/5f/Heavy-human-Titan.png/revision/latest/scale-to-width-down/160?cb=20100209161744
tags:
  - shields
  - shield_regen
  - ac
andromeda: false
rarity: uncommon
flavor: Titan armor was created by Rosenkov Materials as an upgrade to their other lines of heavy armor.
mechanics:
  - type: me:shields
    capacity:
      type: flat
      value: 20
    regen:
      type: flat
      value: 5
  - type: me:thermal-clip-capacity
    value: 10
  - type: me:medi-gel-capacity
    value: 4
  - type: me:grenade-capacity
    value: 2
  - type: ac
    bonus:
      type: flat
      value: 2
---
- 20 shields (regen 5).
- +2 AC
