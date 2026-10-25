---
name: Kath Hound
image: https://vignette.wikia.nocookie.net/swtor/images/5/5c/Khound.png/revision/latest/scale-to-width-down/476?cb=20150207213717
type: organic
unit: alien
alignment: u
profBonus: 2
ac: 12
hp:
  dieCount: 2
  dieType: 6
abilityScores:
  str: 14
  dex: 13
  con: 14
  int: 2
  wis: 12
  cha: 5
size: medium
skills:
  - perception
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
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 2
          dieType: 8
          mod: true
          type: piercing
      target: one
      id: maul
      name: Maul
      miss: Hit or miss, if the target is a creature, it must succeed on a DC 12 Dexterity saving throw or be knocked prone and is grappled. A creature takes half damage on a successful saving throw
  features:
    - name: Keen Hearing and Smell
      text: The kath hound has advantage on Wisdom (Perception) checks that rely on hearing or smell.
      id: keen-hearing-and-smell
    - name: Pack Tactics
      text: The kath hound has advantage on an attack roll against a creature if at least one of the kath hound's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
    - name: Grappler
      text: The kath hound has advantage on attack rolls against any creature grappled by it.
      id: grappler
cr: "00250"
---
