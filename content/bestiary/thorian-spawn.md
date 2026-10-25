---
name: Thorian Spawn
image: https://vignette.wikia.nocookie.net/finalfantasy/images/1/15/Sandragora.jpg/revision/latest?cb=20081018141337
type: organic
unit: thorian
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 3
  dieType: 6
abilityScores:
  str: 10
  dex: 13
  con: 9
  int: 11
  wis: 11
  cha: 2
irv:
  conImm:
    - lifted
    - prone
size: small
speed:
  walk: 0
entries:
  actions:
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
      text: The spawn releases spores in a :distance{length="10"}-radius sphere lasting until the end of its next turn. A creature that enters the area for the first time on a turn or starts its turn there takes 3 (1d6) psychic damage and must make a DC 13 Wisdom saving throw. On a failed save, a creature becomes paralyzed until the start of its next turn.
  features:
    - name: Rooted
      text: The spawn in rooted in the ground and cannot be moved. It automatically fails Strength and Dexterity saving throws and skill checks.
      id: rooted
cr: "00250"
---
The beginning of a Thorian's life cycle, these stationary plants feed off nutrients from the mother 
plant while also acting as a last line of defense against intruders.
