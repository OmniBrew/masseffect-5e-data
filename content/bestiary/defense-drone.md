---
name: Defense Drone
image: https://vignette.wikia.nocookie.net/masseffect/images/e/e0/Info_Drone.png/revision/latest/scale-to-width-down/531?cb=20100908213419
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 14
hp:
  dieCount: 6
  dieType: 6
abilityScores:
  str: 15
  dex: 10
  con: 14
  int: 12
  wis: 10
  cha: 7
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
  fly: 30
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 8
          mod: true
          type: bludgeoning
      target: one
      id: bash
      name: Bash
  reactions:
    - name: Guard
      text: When a creature the defense drone can see attacks a target other than itself that is within :distance{length="5"} of it, it can use its reaction to impose disadvantage on the attack roll.
      id: guard
cr: "00500"
shields:
  capacity: 5
  regen: 5
---
