---
name: Brute Beast
type: organic
unit: tracker
alignment: u
profBonus: 2
ac: 11
hp:
  dieCount: 1
  dieType: 10
abilityScores:
  str: 16
  dex: 10
  con: 16
  int: 2
  wis: 11
  cha: 7
size: medium
speed:
  walk: 30
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 10
          mod: true
          type: bludgeoning
      target: one
      id: gore
      name: Gore
  features:
    - name: Charge
      text: If this creature moves at least 8m before making an attack with its Gore, it deals an additional 2d6 damage.
      id: charge
    - name: Powerful Build
      text: The Brute counts as 1 size larger when determining push, lift and carryweight.
      id: powerful-build
cr: "00125"
shields:
  capacity: 5
  regen: 5
author: Helios
---
