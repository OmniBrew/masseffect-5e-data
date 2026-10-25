---
name: Eclipse Heavy
image: https://vignette.wikia.nocookie.net/masseffect/images/4/4d/Eclipse_Heavy.png/revision/latest?cb=20100624034136
type: organic
unit: eclipse
alignment: nn
profBonus: 2
ac: 13
hp:
  dieCount: 17
  dieType: 8
abilityScores:
  str: 12
  dex: 14
  con: 11
  int: 13
  wis: 12
  cha: 10
size: medium
skills:
  - perception
speed:
  walk: 30
entries:
  actions:
    - name: ML-77 Missile Launcher
      text: Choose a creature within :distance{length="150"} that you can see and fire a missile at it. Each creature within a :distance{length="10" adj} cube of the target, including the target, must make a DC 14 Dexterity saving throw. On a failed save a creature takes 39 (6d12) thunder damage or half as much on a successful one.
      id: ml-77-missile-launcher
cr: "04000"
shields:
  capacity: 5
  regen: 5
---
