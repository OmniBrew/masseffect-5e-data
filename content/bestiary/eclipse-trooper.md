---
name: Eclipse Trooper
image: https://vignette.wikia.nocookie.net/masseffect/images/9/9e/Eclipse_Trooper.png/revision/latest?cb=20100625014426
type: organic
unit: eclipse
alignment: nn
profBonus: 2
ac: 12
hp:
  dieCount: 4
  dieType: 8
abilityScores:
  str: 11
  dex: 13
  con: 9
  int: 12
  wis: 12
  cha: 10
size: medium
speed:
  walk: 30
entries:
  features:
    - list:
        - id: flashbang-grenade
          mark: iii
          uses: 2
      id: grenades
      name: Grenades
      text: The eclipse trooper has the following grenades equipped. It can use a grenade as an action.
    - name: Pack Tactics
      text: The creature has advantage on an attack roll against a creature if at least one of the creature's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
  actions:
    - ref: weapon
      proficient: true
      id: m-8-avenger
      weaponId: m-8-avenger
cr: "00250"
shields:
  capacity: 5
  regen: 5
---
