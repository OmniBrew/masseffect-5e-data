---
name: Repair Drone
image: https://vignette.wikia.nocookie.net/masseffect/images/2/21/Maintenance_Drone.png/revision/latest/scale-to-width-down/350?cb=20100909024927
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 11
hp:
  dieCount: 5
  dieType: 6
abilityScores:
  str: 8
  dex: 12
  con: 10
  int: 11
  wis: 11
  cha: 6
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
  fly: 35
entries:
  features:
    - mod: int
      ref: power
      list:
        - id: first-aid
          perDay: 3
      id: innate-powercasting
      name: Innate Powercasting
      text: "The repair drone's innate powercasting ability is Intelligence (power save DC 10, +2 to hit with power attacks). It can innately cast the following powers:"
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 4
          mod: true
          type: lightning
      target: one
      id: defibrillators
      name: Defibrillators
    - recharge: short
      id: stabalize
      name: Stabilize
      text: The repair drone can stabilize a friendly creature within :distance{length="5"}.
cr: "00125"
shields:
  capacity: 5
  regen: 5
---
