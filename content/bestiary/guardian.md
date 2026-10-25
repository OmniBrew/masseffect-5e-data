---
name: Guardian
image: https://vignette.wikia.nocookie.net/masseffect/images/3/3f/ME3_Cerberus_Guardian.png/revision/latest/scale-to-width-down/350?cb=20120321201359
type: organic
unit: cerberus
alignment: nn
profBonus: 3
ac: 18
hp:
  dieCount: 20
  dieType: 8
abilityScores:
  str: 16
  dex: 12
  con: 15
  int: 11
  wis: 10
  cha: 12
savingThrows:
  - str
size: medium
speed:
  walk: 15
entries:
  actions:
    - ref: weapon
      proficient: true
      id: stun-baton
      weaponId: stun-baton
    - ref: weapon
      proficient: true
      id: m-358-talon
      weaponId: m-358-talon
    - name: Multiattack
      text: The guardian makes two M-358 Talon attacks.
      id: multiattack
  features:
    - name: Heavy Shield
      text: While the guardian has their Heavy Shield equipped, it gains +2 AC and has resistance bludgeoning, piercing, and slashing damage.
      id: heavy-shield
cr: "05000"
---
