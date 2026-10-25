---
name: Swarmer
image: https://vignette.wikia.nocookie.net/masseffect/images/8/82/ME3_Swarmer.png/revision/latest/scale-to-width-down/350?cb=20120319204747
type: synorg
unit: reaper
alignment: le
profBonus: 2
ac: 10
hp:
  dieCount: 3
  dieType: 4
abilityScores:
  str: 4
  dex: 12
  con: 8
  int: 4
  wis: 4
  cha: 4
irv:
  conImm:
    - charmed
savingThrows:
  - dex
senses:
  darkvision: 30
size: tiny
speed:
  walk: 35
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: dex
      damage:
        - dieCount: 1
          dieType: 6
          mod: true
          type: acid
      target: one
      id: suicide-attack
      name: Suicide Attack
      hit: On a hit, the swarmer explodes (its hit points immediately become 0 after resolving the attack)
  features:
    - name: Aggressive
      text: As a bonus action, the swarmer can move up to its speed toward a hostile creature that it can see.
      id: aggressive
cr: "00125"
---
