---
name: Varren Alpha
image: https://vignette.wikia.nocookie.net/masseffect/images/6/63/Codex_ME_-_Varren.png/revision/latest/scale-to-width-down/200?cb=20140820063614
type: organic
unit: alien
alignment: u
profBonus: 2
ac: 14
hp:
  dieCount: 5
  dieType: 10
abilityScores:
  str: 17
  dex: 15
  con: 15
  int: 3
  wis: 12
  cha: 7
size: large
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
          dieType: 6
          mod: true
          type: piercing
      target: one
      id: bite
      name: Bite
      hit: " If the target is a creature, it must succeed on a DC 14 Strength saving throw or be knocked prone"
  features:
    - name: Keen Hearing and Smell
      text: The varren alpha has advantage on Wisdom (Perception) checks that rely on hearing or smell.
      id: keen-hearing-and-smell
    - name: Pack Tactics
      text: The varren alpha has advantage on an attack roll against a creature if at least one of the varren alpha's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
cr: "01000"
---
