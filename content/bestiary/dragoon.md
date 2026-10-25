---
name: Dragoon
image: https://vignette.wikia.nocookie.net/masseffect/images/0/01/Cerberus_dragoon_smash.png/revision/latest?cb=20121013090412
type: organic
unit: cerberus
alignment: ne
profBonus: 3
ac: 16
hp:
  dieCount: 20
  dieType: 8
abilityScores:
  str: 12
  dex: 18
  con: 13
  int: 14
  wis: 12
  cha: 13
savingThrows:
  - dex
size: medium
skills:
  - acrobatics
speed:
  walk: 35
entries:
  actions:
    - ref: weapon
      proficient: true
      id: omni-whip
      weaponId: omni-whip
    - ref: weapon
      proficient: true
      id: m-25-hornet
      weaponId: m-25-hornet
    - name: Multiattack
      text: The dragoon makes three Omni-whip attacks
      id: multiattack
  features:
    - name: Aggressive
      text: As a bonus action, the dragoon can move up to its speed toward a hostile creature that it can see.
      id: aggressive
cr: "05000"
---
