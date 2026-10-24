---
name: Pyjak
image: https://static.wikia.nocookie.net/masseffect/images/7/7a/338px-Spacemonkey.jpg
type: organic
unit: alien
alignment: u
profBonus: 2
ac: 12
hp:
  dieCount: 1
  dieType: 6
abilityScores:
  str: 8
  dex: 14
  con: 11
  int: 8
  wis: 12
  cha: 6
size: small
speed:
  walk: 30
  climb: 15
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 4
          mod: true
          type: piercing
      target: one
      id: bite
      name: Bite
  features:
    - name: Pack Tactics
      text: The pyjak has advantage on an attack roll against a creature if at least one of the pyjak's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
cr: "00000"
---
