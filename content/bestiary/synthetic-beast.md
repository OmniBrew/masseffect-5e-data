---
name: Synthetic Beast
type: synthetic
unit: tracker
alignment: u
profBonus: 2
ac: 12
acNote: 10 + Dex, plus the armor chosen with Custom Armor
hp:
  dieCount: 1
  dieType: 8
abilityScores:
  str: 14
  dex: 14
  con: 14
  int: 12
  wis: 10
  cha: 3
irv:
  vul:
    - lightning
  imm:
    - poison
    - psychic
  conImm:
    - poisoned
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
          dieType: 6
          mod: true
          type: bludgeoning
      target: one
      id: maul
      name: Maul
  features:
    - name: Custom Armor
      text: Rather than wearing armor, the Synthetic beast has an armor type of choice. (See Geth for rules on this.) Medium and Heavy armor do not have their strength requirements. The Synthetic beast has an amount of mod slots equal to the Tracker's PB.
      id: custom-armor
    - name: Custom Frame
      text: Due to their inherent customization, you may choose 1 Training Regimen from the list. It may not have a level requirement, and you must fulfill all other requirements as usual.
cr: "00125"
shields:
  capacity: 10
author: Helios
---
