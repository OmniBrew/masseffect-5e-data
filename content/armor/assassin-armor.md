---
name: Assassin Armor
coverage: suit
armorType: light
cost: 52700
manufacturer: elkoss-combine
tags:
  - special
andromeda: false
rarity: uncommon
flavor: Elkoss Combine was commissioned by the Salarian Tactics Group to make a set of armor that would allow their agents to remain unseen and unheard.
mechanics:
  - type: action
    resource:
      reset: short
    shortDesc: Become invisible for 1 minute or until you make an attack, cast a power, use a grenade or mine, or fire a heavy weapon.
  - type: me:shields
    capacity:
      type: flat
      value: 5
    regen:
      type: flat
      value: 5
  - type: me:thermal-clip-capacity
    value: 10
  - type: me:medi-gel-capacity
    value: 4
  - type: me:grenade-capacity
    value: 2
---
- As an action, you can activate a tactical cloak, becoming invisible. The cloak lasts 1 minute or
until you make an attack, cast a power, use a grenade or mine, or fire a heavy weapon. You may use
this feature once per short rest.
