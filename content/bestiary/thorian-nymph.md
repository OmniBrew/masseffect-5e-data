---
name: Thorian Nymph
image: https://vignette.wikia.nocookie.net/elderscrolls/images/c/c3/Chaurus_3D.png/revision/latest/scale-to-width-down/700?cb=20120612155204
type: organic
unit: thorian
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 5
  dieType: 6
abilityScores:
  str: 11
  dex: 13
  con: 11
  int: 13
  wis: 11
  cha: 2
size: small
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
          dieType: 4
          mod: true
          type: piercing
      target: one
      id: bite
      name: Bite
    - attack: ranged
      proficient: true
      range: 25
      mod: dex
      damage:
        - dieCount: 2
          dieType: 6
          mod: true
          type: necrotic
      target: one
      id: acid-spit
      name: Acid Spit
    - uses: 1
      perDay: true
      id: release-spores
      name: Release Spores
      text: The nymph releases spores in a :distance{length="10" adj}-radius sphere lasting until the end of its next turn. A creature that enters the area for the first time on a turn or starts its turn there takes 3 (1d6) psychic damage and must make a DC 13 Wisdom saving throw. On a failed save, a creature becomes paralyzed until the start of its next turn.
cr: "00500"
---
In its juvenile stage, the Thorian becomes mobile and sneaks aboard unknowing ships to spread across 
the galaxy.
