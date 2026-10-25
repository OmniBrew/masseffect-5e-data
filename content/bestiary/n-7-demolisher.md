---
name: N7 Demolisher
image: https://vignette.wikia.nocookie.net/masseffect/images/0/04/N7_Demolisher_Engineer_MP.png/revision/latest/scale-to-width-down/250?cb=20120717151043
type: organic
unit: n_7
alignment: ln
profBonus: 3
ac: 15
hp:
  dieCount: 15
  dieType: 8
abilityScores:
  str: 13
  dex: 16
  con: 14
  int: 13
  wis: 13
  cha: 14
savingThrows:
  - con
  - dex
size: medium
skills:
  - vehicle-handling
  - engineering
  - survival
speed:
  walk: 30
entries:
  features:
    - list:
        - id: arc-grenade
          mark: iii
          uses: 3
        - id: homing-grenade
          mark: i
          uses: 3
      id: grenades
      name: Grenades
      text: The N7 demolisher has the following grenades equipped. It can use a grenade as an action.
    - name: N7 Training
      text: The N7 demolisher has advantage on its first attack roll each turn.
      id: n7-training
  actions:
    - ref: weapon
      proficient: true
      id: n-7-eagle
      weaponId: n-7-eagle
    - ref: weapon
      proficient: true
      id: n-7-hurricane
      weaponId: n-7-hurricane
    - uses: 1
      perDay: true
      id: deploy-shield-pylon
      name: Deploy Shield Pylon
      text: The N7 demolisher deploys a Shield Pylon to an unoccupied space within :distance{length="5"}. The pylon has AC 10, 25 hit points and provides half cover. At the end of the N7 demolisher's turn, any friendly creature within :distance{length="10"} of the pylon gains 2 shield points. Shield points gained this way cannot exceed the creatures maximum shield points.
    - name: Multiattack
      text: The N7 demolisher makes three weapon attacks or two weapon attacks and uses one grenade.
      id: multiattack
    - name: Repair
      text: The N7 demolisher uses its action to repair a friendly, synthetic target within :distance{length="5"} for 2d8 hit points.
      id: repair
cr: "05000"
shields:
  capacity: 20
  regen: 10
---
