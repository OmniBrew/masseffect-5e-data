---
name: Blue Suns Heavy
image: https://vignette.wikia.nocookie.net/masseffect/images/e/e0/Blue_Suns_Heavy.png/revision/latest/scale-to-width-down/348?cb=20100621035327
type: organic
unit: blue_suns
alignment: nn
profBonus: 2
ac: 13
hp:
  dieCount: 4
  dieType: 8
abilityScores:
  str: 13
  dex: 12
  con: 14
  int: 11
  wis: 10
  cha: 10
size: medium
skills:
  - survival
speed:
  walk: 30
entries:
  features:
    - uses: 1
      perDay: true
      id: tech-armor
      name: Tech Armor
      text: As a bonus action, the heavy can activate its Tech Armor. It immediately gains 10 temporary hit points. While the heavy has at least 1 of these temporary hit points remaining, it has +2 AC.
  actions:
    - name: ML-77 Missile Launcher
      text: Choose a creature within :distance{length="150"} that you can see and fire a missile at it. Each creature within a :distance{length="10" adj} cube of the target, including the target, must make a DC 14 Dexterity saving throw. On a failed save a creature takes 39 (6d12) thunder damage or half as much on a successful one.
      id: ml-77-missile-launcher
  reactions:
    - name: Tech Armor
      text: As a reaction to taking damage, the heavy can activate its tech armor.
      id: tech-armor
cr: "02000"
shields:
  capacity: 10
  regen: 0
---
