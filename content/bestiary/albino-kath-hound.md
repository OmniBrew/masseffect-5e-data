---
name: Albino Kath Hound
image: https://vignette.wikia.nocookie.net/starwars/images/e/e2/Kathhound.jpg/revision/latest/scale-to-width-down/439?cb=20091106175830
type: organic
unit: alien
alignment: u
profBonus: 2
ac: 16
hp:
  dieCount: 5
  dieType: 10
abilityScores:
  str: 16
  dex: 13
  con: 16
  int: 10
  wis: 16
  cha: 6
senses:
  blindsight: 30
size: large
skills:
  - perception
speed:
  walk: 40
entries:
  features:
    - mod: wis
      ref: power
      list:
        - id: throw
          perDay: at_will
        - id: warp
          perDay: 3
      id: innate-powercasting
      name: Innate Powercasting
      text: "The albino kath hound's innate powercasting ability is Wisdom (power save DC 13, +5 to hit with power attacks). It can innately cast the following powers:"
    - name: Barrier
      text: The albino kath hound has 5 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Keen Hearing and Smell
      text: The kath hound has advantage on Wisdom (Perception) checks that rely on hearing or smell.
      id: keen-hearing-and-smell
    - name: Pack Tactics
      text: The kath hound has advantage on an attack roll against a creature if at least one of the kath hound's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
    - name: Grappler
      text: The kath hound has advantage on attack rolls against any creature grappled by it.
      id: grappler
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
      miss: Hit or miss, if the target is a creature, it must succeed on a DC 12 Dexterity saving throw or be knocked prone and is grappled. A creature takes half damage on a successful saving throw
cr: "01000"
---
