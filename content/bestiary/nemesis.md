---
name: Nemesis
image: https://vignette.wikia.nocookie.net/masseffect/images/a/aa/ME3_Cerberus_Nemesis.png/revision/latest/scale-to-width-down/338?cb=20120314005634
type: organic
unit: cerberus
alignment: ne
profBonus: 3
ac: 16
hp:
  dieCount: 15
  dieType: 8
abilityScores:
  str: 8
  dex: 20
  con: 11
  int: 16
  wis: 13
  cha: 14
savingThrows:
  - dex
senses:
  darkvision: 60
size: medium
skills:
  - perception
  - stealth
  - survival
speed:
  walk: 30
entries:
  actions:
    - ref: weapon
      proficient: true
      id: m-98-widow
      weaponId: m-98-widow
  features:
    - name: Pack Tactics
      text: The nemesis has advantage on an attack roll against a creature if at least one of the nemesis's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
    - name: Self-Destruct
      text: When the nemesis dies, it explodes. Each creature within :distance{length="10"} of it must make a DC 15 Dexterity saving throw, taking 33 (6d10) thunder damage on a failed save, or half as much damage on a successful one.
      id: self-destruct
    - name: Shadow Cloak
      text: While in dim light or darkness, the nemesis can take the Hide action as a bonus action.
      id: shadow-cloak
    - name: Surprise Attack
      text: If the nemesis surprises a creature and hits it with an attack during the first round of combat, the target takes an extra 10 (3d6) damage from the attack.
      id: surprise-attack
cr: "06000"
shields:
  capacity: 20
  regen: 10
---
