---
name: Geth Turret
image: https://vignette.wikia.nocookie.net/masseffect/images/b/b0/ME3_Geth_Turret.png/revision/latest/scale-to-width-down/350?cb=20120326000908
type: synthetic
unit: geth
alignment: ln
profBonus: 2
ac: 12
hp:
  dieCount: 2
  dieType: 6
abilityScores:
  str: 10
  dex: 10
  con: 10
  int: 10
  wis: 8
  cha: 8
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  vul:
    - lightning
size: small
speed:
  fly: 15
entries:
  actions:
    - attack: ranged
      proficient: true
      range: 50
      mod: dex
      damage:
        - dieCount: 1
          dieType: 10
          mod: true
          type: radiant
      target: one
      id: pulse-cannon
      name: Pulse Cannon
    - recharge:
        - "5"
        - "6"
      id: shield-restore
      name: Shield Restore
      text: The geth turret restores 9 (2d8) shield points to a friendly creature within :distance{length="10"}.
cr: "00250"
shields:
  capacity: 5
  regen: 5
---
