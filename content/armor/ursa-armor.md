---
name: Ursa Armor
coverage: suit
armorType: medium
cost: 84150
manufacturer: hahne-kedar
image: https://vignette.wikia.nocookie.net/masseffect/images/9/95/Medium-human-Ursa.png/revision/latest/scale-to-width-down/160?cb=20100209162744
tags:
  - shields
  - shield_regen
  - ac
andromeda: false
rarity: uncommon
flavor: Hahne-Kedar's Urse armor is known for its "think hide", and is a moderate update over stock armor.
mechanics:
  - type: me:shields
    capacity:
      type: flat
      value: 20
    regen:
      type: flat
      value: 10
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
- 20 shields (regen 10).
- +2 AC
