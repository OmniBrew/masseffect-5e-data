---
name: Horned Kath Hound
image: https://vignette.wikia.nocookie.net/starwars/images/5/5b/HornedKathhound.jpg/revision/latest/scale-to-width-down/448?cb=20091107052416
type: organic
unit: alien
alignment: u
profBonus: 2
ac: 14
hp:
  dieCount: 5
  dieType: 8
abilityScores:
  str: 16
  dex: 15
  con: 16
  int: 5
  wis: 14
  cha: 6
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
        - dieCount: 3
          dieType: 4
          mod: true
          type: piercing
      target: one
      id: gore
      name: Gore
      hit: " If the target is a creature, it must succeed on a DC 14 Strength saving throw or be knocked prone"
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
      miss: Hit or miss, if the target is a creature, it must succeed on a DC 12 Dexterity saving throw or be knocked prone and is grappled. A creature takes half damage on a successful saving throw.
    - name: Howl
      text: Each other kath hound within :distance{length="60"} that is not incapacitated gains +2 Dexterity and +1 Wisdom for 1 minute. Kath hounds can only benefit from one Howl at a time.
      id: howl
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
cr: "01000"
---
