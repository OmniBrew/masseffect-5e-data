---
name: Kett Chosen
image: https://vignette.wikia.nocookie.net/masseffect/images/f/fd/MEA_Enemy_Chosen.png/revision/latest?cb=20170705200934
type: organic
unit: kett
alignment: le
profBonus: 2
ac: 15
hp:
  dieCount: 10
  dieType: 8
abilityScores:
  str: 14
  dex: 13
  con: 14
  int: 10
  wis: 8
  cha: 7
savingThrows:
  - dex
size: medium
speed:
  walk: 30
entries:
  features:
    - list:
        - id: frag-grenade
          mark: iii
          uses: 2
      id: grenades
      name: Grenades
      text: The kett chosen has the following grenades equipped. It can use a grenade as an action.
  actions:
    - ref: weapon
      proficient: true
      id: zalkin
      weaponId: zalkin
cr: "01000"
---
