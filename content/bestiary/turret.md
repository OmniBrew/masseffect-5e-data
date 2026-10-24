---
name: Turret
image: https://vignette.wikia.nocookie.net/masseffect/images/0/0c/ME3_Cerberus_Turret.png/revision/latest/scale-to-width-down/350?cb=20120322141943
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 12
hp:
  dieCount: 10
  dieType: 6
abilityScores:
  str: 1
  dex: 1
  con: 8
  int: 10
  wis: 6
  cha: 1
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  res:
    - bludgeoning
  vul:
    - lightning
size: small
speed:
  walk: 0
entries:
  actions:
    - attack: ranged
      proficient: true
      range: 150
      mod: int
      damage:
        - dieCount: 2
          dieType: 6
          mod: true
          type: piercing
        - dieCount: 2
          dieType: 6
          mod: true
          type: radiant
      target: one
      id: mass-accelerator-machinegun
      name: Mass Accelerator Machinegun
      hit: " The turret can make a burst fire attack instead"
  features:
    - name: Stationary
      text: The turret automatically fails Strength and Dexterity saving throws and skill checks.
      id: stationary
cr: "01000"
shields:
  capacity: 10
  regen: 0
---
