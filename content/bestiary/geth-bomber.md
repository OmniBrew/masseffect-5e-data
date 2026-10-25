---
name: Geth Bomber
image: https://vignette.wikia.nocookie.net/masseffect/images/0/01/ME3_geth_bomber_AAA.png/revision/latest/scale-to-width-down/700?cb=20130313175937
type: synthetic
unit: geth
alignment: ln
profBonus: 2
ac: 16
hp:
  dieCount: 10
  dieType: 6
abilityScores:
  str: 6
  dex: 18
  con: 6
  int: 14
  wis: 10
  cha: 8
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  vul:
    - lightning
savingThrows:
  - dex
senses:
  darkvision: 60
size: small
skills:
  - perception
speed:
  fly: 30
entries:
  features:
    - mod: int
      ref: power
      list:
        - id: overload
          perDay: at_will
      id: innate-powercasting
      name: Innate Powercasting
      text: "The geth bomber's innate powercasting ability is Intelligence (power save DC 12, +4 to hit with power attacks). It can innately cast the following powers:"
    - list:
        - id: multi-frag-grenade
          mark: ii
          uses: 2
      id: grenades
      name: Grenades
      text: The geth bomber has the following grenades equipped. It can use a grenade as an action.
cr: "02000"
shields:
  capacity: 15
  regen: 5
---
