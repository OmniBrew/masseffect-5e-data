---
name: Seeker Plague
image: https://vignette.wikia.nocookie.net/masseffect/images/9/9f/SwarmME3_Plague.jpg/revision/latest/scale-to-width-down/350?cb=20121201212536
type: organic
unit: collector
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 4
  dieType: 6
abilityScores:
  str: 4
  dex: 12
  con: 10
  int: 10
  wis: 8
  cha: 6
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
        - dieCount: 1
          dieType: 4
          mod: true
          type: necrotic
      target: one
      id: plague-sting
      name: Plague Sting
      hit: The target must succeed on DC 13 Constitution saving throw or has disadvantage on its next attack roll
  features:
    - name: Barrier
      text: The seeker plague has 1 barrier tick. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
cr: "00250"
---
