---
name: Seeker Swarm
image: https://vignette.wikia.nocookie.net/masseffect/images/8/8f/SwarmME3.jpg/revision/latest/scale-to-width-down/350?cb=20121201212516
type: organic
unit: collector
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 4
  dieType: 6
abilityScores:
  str: 2
  dex: 10
  con: 8
  int: 10
  wis: 8
  cha: 5
savingThrows:
  - dex
size: small
speed:
  fly: 30
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: dex
      damage:
        - dieCount: 1
          dieType: 4
          mod: true
          type: poison
      target: one
      id: sting
      name: Sting
cr: "00125"
---
