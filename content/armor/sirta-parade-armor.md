---
name: Sirta Parade Armor
coverage: suit
armorType: light
cost: 38675
manufacturer: ariake-technologies
tags:
  - ability_skill_bonus
andromeda: false
rarity: uncommon
flavor: Glossy armor that shines in the light, designed to look good as its first function.
mechanics:
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
  - type: skill-check
    value:
      - persuasion
      - performance
    effect:
      type: advantage
---
- Advantage on Persuasion and Performance checks.
