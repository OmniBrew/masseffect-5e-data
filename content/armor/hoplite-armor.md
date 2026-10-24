---
name: Hoplite Armor
coverage: suit
armorType: light
cost: 80750
manufacturer: ceberus-skunkworks
tags:
  - shields
  - shield_regen
  - ac
andromeda: false
rarity: uncommon
flavor: With additional research into kinetic barrier devices, Cerberus Skunkworks created the Hoplite Armor. As light and simple as their popular Freedom Armor with a shield generator around the waist, giving it an appearance of ancient Greek hoplites.
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
- +2 AC.
