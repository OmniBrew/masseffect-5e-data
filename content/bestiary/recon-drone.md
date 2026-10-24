---
name: Recon Drone
image: https://vignette.wikia.nocookie.net/masseffect/images/2/29/Geth_Recon_Drone_ME2.png/revision/latest/scale-to-width-down/350?cb=20100627032507
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 13
hp:
  dieCount: 4
  dieType: 6
abilityScores:
  str: 10
  dex: 16
  con: 8
  int: 11
  wis: 12
  cha: 5
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  vul:
    - lightning
senses:
  infrared-vision: 30
size: small
skills:
  - perception
  - stealth
speed:
  fly: 40
entries:
  features:
    - uses: 3
      perDay: true
      id: tactical-cloak
      name: Tactical Cloak
      text: As a bonus action, the recon drone activates its tactical cloak, becoming invisible for 1 minute. When the recon drone makes a melee or ranged attack or uses a tech or combat power, tactical cloak ends.
  actions:
    - attack: ranged
      proficient: true
      range: 150
      mod: dex
      damage:
        - dieCount: 1
          dieType: 4
          mod: true
          type: radiant
      target: one
      id: pulse-rifle
      name: Pulse Rifle
cr: "00125"
shields:
  capacity: 5
  regen: 5
---
