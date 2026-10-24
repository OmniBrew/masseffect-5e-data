---
name: Gladiator Armor
coverage: suit
armorType: heavy
cost: 42500
manufacturer: elkoss-combine
image: https://vignette.wikia.nocookie.net/masseffect/images/5/54/Heavy-human-Gladiator.png/revision/latest/scale-to-width-down/160?cb=20100209161008
tags:
  - shields
  - ac
andromeda: false
rarity: uncommon
flavor: Elkoss Combine's Gladiator Armor is a simple upgrade to most heavy armor.
mechanics:
  - type: me:shields
    capacity:
      type: flat
      value: 10
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
      value: 1
---
- 10 shields (regen 5).
- +1 AC
