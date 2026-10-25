---
name: Blue Suns Legionnaire
image: https://vignette.wikia.nocookie.net/masseffect/images/9/94/Blue_Suns_Legionnaire.png/revision/latest/scale-to-width-down/369?cb=20100626080854
type: organic
unit: blue_suns
alignment: nn
profBonus: 2
ac: 12
hp:
  dieCount: 3
  dieType: 8
abilityScores:
  str: 12
  dex: 14
  con: 13
  int: 9
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
      text: As a bonus action, the legionnaire can activate its Tech Armor. It immediately gains 10 temporary hit points. While the legionnaire has at least 1 of these temporary hit points remaining, it has +2 AC.
    - list:
        - id: inferno-grenade
          mark: iii
          uses: 2
      id: grenades
      name: Grenades
      text: The blue suns legionnaire has the following grenades equipped. It can use a grenade as an action.
    - name: Disruptor Ammo
      text: "When the legionnaire hits with its M-15 Vindicator, if the target is primed, the target detonates. Otherwise, the target becomes primed: lightning until the end of the legionnaire's next turn."
      id: disruptor-ammo
  actions:
    - ref: weapon
      proficient: true
      id: m-15-vindicator
      weaponId: m-15-vindicator
  reactions:
    - name: Tech Armor
      text: As a reaction to taking damage, the legionnaire can activate its tech armor.
      id: tech-armor
cr: "00500"
shields:
  capacity: 5
  regen: 5
---
