---
name: Geth Stalker
image: https://vignette.wikia.nocookie.net/masseffect/images/e/ec/ME_geth_stalker.png/revision/latest/scale-to-width-down/350?cb=20130517141111
type: synthetic
unit: geth
alignment: ln
profBonus: 2
ac: 14
hp:
  dieCount: 18
  dieType: 8
abilityScores:
  str: 8
  dex: 16
  con: 8
  int: 12
  wis: 14
  cha: 5
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  vul:
    - lightning
savingThrows:
  - dex
senses:
  darkvision: 30
  infrared-vision: 30
size: medium
skills:
  - perception
speed:
  walk: 40
entries:
  features:
    - mod: int
      list:
        - id: sabotage
          perDay: at_will
      id: innate-powercasting
      name: Innate Powercasting
      text: "The geth stalker's innate powercasting ability is Intelligence (power save DC 11, +3 to hit with power attacks). It can innately cast the following powers:"
    - name: Assassination
      text: Once per turn, the geth stalker can deal an extra 7 (2d6) damage to one creature it hits with an attack if it has advantage on the attack roll. The attack must be made with a melee or ranged weapon.
      id: assassination
    - name: Avoidance
      text: If the geth stalker subjected to an effect that allows it to make a saving throw to take only half damage, it instead takes no damage if it succeeds on the saving throw, and only half damage if it fails.
      id: avoidance
    - name: Leap
      text: The geth stalker can leap up to one half its speed.
      id: leap
    - name: Spider Climb
      text: The geth stalker can climb difficult surfaces, including upside down on ceilings, without needing to make an ability check.
      id: spider-climb
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 8
          mod: true
          type: slashing
      target: one
      id: claw
      name: Claw
    - attack: ranged
      proficient: true
      range: 150
      mod: dex
      damage:
        - dieCount: 3
          dieType: 6
          mod: true
          type: radiant
      target: one
      id: eye-cannon
      name: Eye Cannon
cr: "03000"
shields:
  capacity: 5
  regen: 5
---
