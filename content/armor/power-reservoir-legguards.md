---
name: Power Reservoir Legguards
coverage: piece
slot: legs
armorType: medium
cost: 12750
manufacturer: serrice-council
image: https://vignette.wikia.nocookie.net/masseffect/images/7/7e/ME3_serrice_council_legs.png/revision/latest/scale-to-width-down/100?cb=20120314171406
tags:
  - special
andromeda: false
rarity: uncommon
flavor: A set of greaves that have batteries designed to conserve biotic power.
mechanics:
  - type: me:thermal-clip-capacity
    value: 2
  - type: me:grenade-capacity
    value: 2
  - type: reaction
    resource:
      reset: long
    shortDesc: When you have 0 barrier ticks remaining, restore all of your barrier ticks.
---
- As a reaction to having 0 barrier ticks, restore all of your barrier ticks. You may use this
ability once per long rest.
