---
name: Scion
image: https://vignette.wikia.nocookie.net/masseffect/images/d/da/ScionME3.jpg/revision/latest/scale-to-width-down/350?cb=20121201212433
type: synorg
unit: reaper
alignment: le
profBonus: 4
ac: 18
hp:
  dieCount: 7
  dieType: 8
abilityScores:
  str: 18
  dex: 11
  con: 16
  int: 6
  wis: 6
  cha: 5
irv:
  res:
    - bludgeoning
    - piercing
    - slashing
savingThrows:
  - con
senses:
  darkvision: 30
size: medium
speed:
  walk: 25
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 8
          mod: true
          type: bludgeoning
      target: one
      id: bash
      name: Bash
    - recharge:
        - "4"
        - "6"
      id: salvo
      name: Salvo
      text: The scion targets three locations within :distance{length="90"} and launches an explosive blast to each. The locations can be the same or different. Each creature within a :distance{length="15"} radius of a target location must make a DC 16 Dexterity saving throw. On a failed save a creature takes 15 (3d10) thunder damage or half as much on a successful one.
cr: "09000"
---
