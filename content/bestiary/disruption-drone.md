---
name: Disruption Drone
image: https://vignette.wikia.nocookie.net/masseffect/images/b/b6/ME3_disruption_drone.png/revision/latest/scale-to-width-down/350?cb=20130308125421
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 8
hp:
  dieCount: 4
  dieType: 6
abilityScores:
  str: 8
  dex: 14
  con: 8
  int: 8
  wis: 8
  cha: 8
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
  fly: 40
entries:
  features:
    - name: Post-mortem explosion
      text: When the disruption drone drops to 0 hit points it explodes. Each creature within a :distance{length="5"} radius must make a DC 13 Dexterity saving throw. On a failed save, a creature takes 13 (2d12) thunder damage, or half as much on a successful one.
      id: post-mortem-explosion
  actions:
    - name: Kamikaze Attack
      text: The disruption drone can use its action to immediately reduce its hit points to 0.
      id: kamikaze-attack
cr: "00125"
---
