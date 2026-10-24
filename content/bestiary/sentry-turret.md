---
name: Sentry Turret
image: https://vignette.wikia.nocookie.net/masseffect/images/f/f8/ME3_Sentry_Turret.png/revision/latest/scale-to-width-down/100?cb=20180206214039
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 14
hp:
  dieCount: 22
  dieType: 6
abilityScores:
  str: 10
  dex: 10
  con: 10
  int: 10
  wis: 10
  cha: 10
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  vul:
    - lightning
size: small
speed:
  walk: 0
entries:
  features:
    - mod: int
      list:
        - id: flamethrower
          perDay: 3
      id: innate-powercasting
      name: Innate Powercasting
      text: "The sentry turret's innate powercasting ability is Intelligence (power save DC 10, +2 to hit with power attacks). It can innately cast the following powers:"
    - name: Stationary
      text: The sentry turret automatically fails Strength and Dexterity saving throws and skill checks.
      id: stationary
  actions:
    - attack: ranged
      proficient: true
      range: 150
      mod: dex
      damage:
        - dieCount: 2
          dieType: 6
          mod: true
          type: piercing
        - dieCount: 2
          dieType: 6
          mod: true
          type: radiant
      target: one
      id: mass-accelerator-machinegun
      name: Mass Accelerator Machinegun
      hit: " The sentry turret can make a burst fire attack instead"
cr: "01000"
---
