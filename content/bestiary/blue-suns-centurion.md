---
name: Blue Suns Centurion
image: https://vignette.wikia.nocookie.net/masseffect/images/2/22/Blue_Suns_Centurion.png/revision/latest/scale-to-width-down/348?cb=20100621022434
type: organic
unit: blue_suns
alignment: nn
profBonus: 2
ac: 14
hp:
  dieCount: 10
  dieType: 8
abilityScores:
  str: 12
  dex: 15
  con: 13
  int: 11
  wis: 12
  cha: 12
savingThrows:
  - str
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
      text: As a bonus action, the centurion can activate its Tech Armor. It immediately gains 20 temporary hit points. While the centurion has at least 1 of these temporary hit points remaining, it has +2 AC.
    - name: Disruptor Ammo
      text: "When the centurion hits with its M-27 Scimitar, if the target is primed, the target detonates. Otherwise, the target becomes primed: lightning until the end of the centurion's next turn."
      id: disruptor-ammo
    - name: Shotgun Marksman
      text: The centurion gains a +4 bonus to ranged weapon attacks with shotguns if the target is within normal range.
      id: shotgun-marksman
  actions:
    - ref: weapon
      proficient: true
      id: m-27-scimitar
      weaponId: m-27-scimitar
  reactions:
    - name: Tech Armor
      text: As a reaction to taking damage, the centurion can activate its tech armor.
      id: tech-armor
cr: "03000"
shields:
  capacity: 15
  regen: 5
---
