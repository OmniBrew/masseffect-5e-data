---
name: All-Round Beast
type: organic
unit: tracker
alignment: u
profBonus: 2
ac: 14
hp:
  dieCount: 1
  dieType: 8
abilityScores:
  str: 14
  dex: 16
  con: 12
  int: 4
  wis: 12
  cha: 6
size: medium
speed:
  walk: 40
  note: choose :distance{length="40"} swimming or climbing, or :distance{length="20"} of burrowing
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
          type: piercing
      target: one
      id: melee-strike
      name: Melee Strike
  features:
    - name: Biological Versatility
      text: You may choose 1 Unrestricted Training Regimen and add it to your known Regimens. It does not count towards your total known.
      id: biological-versatility
    - name: Keen Senses
      text: The All-Round beast has advantage on Wisdom (Perception) checks that have to do with smelling or hearing.
      id: keen-senses
cr: "00125"
shields:
  capacity: 5
  regen: 5
author: Helios
---
