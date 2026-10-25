---
name: Blue Suns Legate
image: https://vignette.wikia.nocookie.net/masseffect/images/8/8c/Blue_Suns_Commander.png/revision/latest/scale-to-width-down/369?cb=20100626053904
type: organic
unit: blue_suns
alignment: nn
profBonus: 3
ac: 16
hp:
  dieCount: 20
  dieType: 8
abilityScores:
  str: 13
  dex: 16
  con: 14
  int: 15
  wis: 12
  cha: 14
savingThrows:
  - con
  - wis
size: medium
skills:
  - survival
  - perception
  - athletics
speed:
  walk: 30
entries:
  features:
    - uses: 1
      perDay: true
      id: tech-armor
      name: Tech Armor
      text: As a bonus action, the legate can activate its Tech Armor. It immediately gains 30 temporary hit points. While the legate has at least 1 of these temporary hit points remaining, it has +2 AC and resistance to bludgeoning, piercing, and slashing damage.
    - recharge: short
      id: leadership
      name: Leadership
      text: For 1 minute, the legate can utter a special command or warning whenever a non-hostile creature that it can see within :distance{length="30"} of it makes an attack roll or a saving throw. The creature can add a d4 to its roll provided it can hear and understand the legate. A creature can benefit from only one Leadership die at a time. This effect ends if the legate is incapacitated.
    - mod: int
      ref: power
      list:
        - id: target-painting
          perDay: 3
      id: innate-powercasting
      name: Innate Powercasting
      text: "The blue suns legate's innate powercasting ability is Intelligence (power save DC 13, +5 to hit with power attacks). It can innately cast the following powers:"
    - name: Incendiary Ammo
      text: "When the centurion hits with its M-76 Revenant or M-300 Claymore, the target takes an additional 1d4 fire damage and becomes primed: fire until the end of the legate's next turn."
      id: incendiary-ammo
  actions:
    - ref: weapon
      proficient: true
      id: m-76-revenant
      weaponId: m-76-revenant
    - ref: weapon
      proficient: true
      id: m-300-claymore
      weaponId: m-300-claymore
    - name: Multiattack
      text: The legate makes 2 attacks with its M-76 Revenant or M-300 Claymore.
      id: multiattack
  reactions:
    - name: Tech Armor
      text: As a reaction to taking damage, the legate can activate its tech armor.
      id: tech-armor
cr: "05000"
shields:
  capacity: 20
  regen: 10
---
