---
name: Varren
image: https://vignette.wikia.nocookie.net/masseffect/images/f/f5/Varren.png/revision/latest?cb=20100220175817
type: organic
unit: alien
alignment: u
profBonus: 2
ac: 13
hp:
  dieCount: 2
  dieType: 8
abilityScores:
  str: 12
  dex: 15
  con: 12
  int: 3
  wis: 12
  cha: 6
size: medium
skills:
  - perception
  - stealth
speed:
  walk: 40
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 2
          dieType: 4
          mod: true
          type: piercing
      target: one
      id: bite
      name: Bite
      hit: " If the target is a creature, it must succeed on a DC 13 Strength saving throw or be knocked prone"
  features:
    - name: Keen Hearing and Smell
      text: The varren has advantage on Wisdom (Perception) checks that rely on hearing or smell.
      id: keen-hearing-and-smell
    - name: Pack Tactics
      text: The varren has advantage on an attack roll against a creature if at least one of the varren's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
cr: "00250"
---
