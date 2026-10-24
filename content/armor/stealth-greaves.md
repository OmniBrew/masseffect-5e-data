---
name: Stealth Greaves
coverage: piece
slot: legs
armorType: light
cost: 14450
manufacturer: sirta-foundation
image: https://vignette.wikia.nocookie.net/masseffect/images/b/bd/ME3_rosenkov_materials_legs.png/revision/latest/scale-to-width-down/100?cb=20120314171643
tags:
  - special
andromeda: false
rarity: uncommon
flavor: Greaves that secrete a highly advanced lubricant in the joints.
mechanics:
  - type: me:thermal-clip-capacity
    value: 2
  - type: me:grenade-capacity
    value: 2
  - type: skill-check
    value:
      - stealth
    effect:
      type: advantage
      note: when this check relies on moving silently
---
- While you wear these greaves, your steps make no sound, regardless of the surface you are moving
across. You also have advantage on Stealth checks that rely on moving silently.
