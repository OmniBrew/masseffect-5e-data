---
name: Geth Trooper
image: https://vignette.wikia.nocookie.net/masseffect/images/c/cf/ME3_Geth_Trooper.png/revision/latest/scale-to-width-down/238?cb=20120315171310
type: synthetic
unit: geth
alignment: ln
profBonus: 2
ac: 13
hp:
  dieCount: 16
  dieType: 8
abilityScores:
  str: 12
  dex: 14
  con: 11
  int: 12
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
      id: weapon-strike
      name: Weapon Strike
    - ref: weapon
      proficient: true
      id: geth-pulse-rifle
      weaponId: geth-pulse-rifle
    - name: Multiattack
      text: The geth trooper makes two Geth Pulse Rifle attacks.
      id: multiattack
cr: "02000"
---
