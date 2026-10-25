---
name: Chemical Drone
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 17
hp:
  dieCount: 5
  dieType: 6
abilityScores:
  str: 14
  dex: 10
  con: 14
  int: 12
  wis: 10
  cha: 7
irv:
  conImm:
    - poisoned
  damImm:
    - acid
size: tiny
speed:
  walk: 12
entries:
  features:
    - mod: int
      list:
        - id: noxious-gas
          perDay: 1
        - id: fuel-spill
          perDay: 1
      id: innate-powercasting
      name: Innate Powercasting
      text: The chemical drone's innate powercasting ability is Intelligence (power save DC 10, +2 to hit with power attacks). Three times per day, it can innately cast noxious gas or fuel spill.
  actions:
    - ref: weapon
      proficient: true
      weaponId: omni-torch
cr: "00500"
shields:
  capacity: 5
  regen: 5
author: Helios
---
