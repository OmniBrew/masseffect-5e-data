---
name: Blue Suns Pyro
image: https://vignette.wikia.nocookie.net/masseffect/images/c/c2/Blue_Suns_Pyro_2.png/revision/latest/scale-to-width-down/347?cb=20100621035042
type: organic
unit: blue_suns
alignment: nn
profBonus: 2
ac: 13
hp:
  dieCount: 8
  dieType: 8
abilityScores:
  str: 12
  dex: 12
  con: 16
  int: 11
  wis: 12
  cha: 10
size: medium
skills:
  - survival
speed:
  walk: 30
entries:
  features:
    - name: Aggressive
      text: As a bonus action, the pyro can move up to its speed toward a hostile creature that it can see.
      id: aggressive
  actions:
    - name: M-451 Firestorm
      text: Creatures within a :distance{length="15" adj} cone must make a DC 13 Dexterity saving throw. On a failed save, a creature takes 14 (4d6) fire damage, or half as much damage on a successful one.
      id: m-451-firestorm
cr: "01000"
shields:
  capacity: 10
  regen: 0
---
