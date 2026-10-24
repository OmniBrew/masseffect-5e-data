---
name: Yahg
image: https://vignette.wikia.nocookie.net/masseffect/images/3/34/ME3_Yahg.png/revision/latest/scale-to-width-down/230?cb=20120322212821
type: organic
unit: alien
alignment: ce
profBonus: 3
ac: 17
hp:
  dieCount: 21
  dieType: 10
abilityScores:
  str: 18
  dex: 12
  con: 15
  int: 18
  wis: 16
  cha: 10
irv:
  res:
    - poison
savingThrows:
  - str
  - dex
  - wis
  - int
senses:
  blindsight: 10
size: large
skills:
  - acrobatics
  - athletics
  - deception
  - insight
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
          dieType: 10
          mod: true
          type: piercing
      target: one
      id: bite
      name: Bite
    - attack: melee
      proficient: true
      range: 10
      mod: str
      damage:
        - dieCount: 2
          dieType: 8
          mod: true
          type: slashing
      target: one
      id: claw
      name: Claw
    - name: Multiattack
      text: "The yahg makes three attacks: one with its bite and two with its claws."
      id: multiattack
  features:
    - name: Assassinate
      text: During its first turn, the yahg has advantage on attack rolls against any creature that hasn't taken a turn. Any hit the yahg scores against a surprised creature is a critical hit.
      id: assassinate
    - name: Avoidance
      text: If the yahg subjected to an effect that allows it to make a saving throw to take only half damage, it instead takes no damage if it succeeds on the saving throw, and only half damage if it fails.
      id: avoidance
    - name: Sneak Attack
      text: The yahg  deals an extra 13 (4d6) damage when it hits a target with a weapon attack and has advantage on the attack roll, or when the target is within :distance{length="5"} of an ally of the yahg that isn't incapacitated and the yahg doesn't have disadvantage on the attack roll.
      id: sneak-attack
cr: "08000"
---
