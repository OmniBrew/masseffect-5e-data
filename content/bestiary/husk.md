---
name: Husk
image: https://vignette.wikia.nocookie.net/masseffect/images/2/27/ME3_Husk.png/revision/latest/scale-to-width-down/350?cb=20120320012912
type: synorg
unit: reaper
alignment: le
profBonus: 2
ac: 11
hp:
  dieCount: 1
  dieType: 8
abilityScores:
  str: 13
  dex: 8
  con: 14
  int: 3
  wis: 6
  cha: 5
savingThrows:
  - wis
senses:
  darkvision: 30
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
          type: slashing
      target: one
      id: swipe
      name: Swipe
      hit: " A creature that is grappled by the husk takes 11 (3d6) necrotic damage at the start of each of the husk's turns"
  features:
    - name: Aggressive
      text: As a bonus action, the husk can move up to its speed toward a hostile creature that it can see.
      id: aggressive
cr: "00500"
---
