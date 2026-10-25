---
name: Tactical Scan
version: 1
level: 0
powerType: combat
classes:
  - infiltrator
  - soldier
  - tracker
  - explorer
tags:
  - debuff
casting:
  - castingTime:
      length: 1
      unit: action
    duration:
      length: 1
      unit: minute
    concentration: false
    range:
      short: 90
    detonates: false
advancements:
  - id: area-scan
    name: Area Scan
    text: Scan a :distance{length="15" adj} cube. Each creature within the cube must make the Charisma (Deception) check against your Wisdom (Insight). This feature only affects a single target, but you can choose one creature from the ones that failed the contested check.
    casting:
      - range:
          aoe:
            size: 15
            type: cube
  - id: telegraphed-attacks
    name: Telegraphed Attacks
    text: Your HUD alerts you when the creature is about to attack. It has disadvantage on ranged and melee attacks against you and you have advantage on any saving throws caused by powers and abilities of the creature.
    casting: []
---
Spend your action scanning a creature you can see, studying its movement and revealing weaknesses.
Make a Wisdom (Insight) check, contested by the target's Charisma (Deception) check. On a success, you have advantage on
attack rolls against the target and you score a critical hit on a roll of 19 or 20.

This benefit lasts 1 minute or until you successfully use this feature against a different target.
