---
name: Rosenkov Reflex Armor
coverage: piece
slot: chest
armorType: heavy
cost: 20400
manufacturer: rosenkov-materials
image: https://vignette.wikia.nocookie.net/masseffect/images/7/7f/ME3_rosenkov_materials_chest.png/revision/latest/scale-to-width-down/100?cb=20120310234640
tags:
  - special
andromeda: false
rarity: rare
flavor: Sturdy armor that gathers real-time battle telemetry and and onboard combat computer that can help a combatant move faster than they can think.
mechanics:
  - type: me:shields
    capacity:
      type: flat
      value: 5
    regen:
      type: flat
      value: 5
  - type: me:thermal-clip-capacity
    value: 6
  - type: me:medi-gel-capacity
    value: 2
  - type: other
    shortDesc: You may take 2 reactions this turn.
    resource:
      reset: short
---
- Once per short rest, you may take 2 reactions within a single turn.
