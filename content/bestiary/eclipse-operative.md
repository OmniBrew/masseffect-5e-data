---
name: Eclipse Operative
image: https://vignette.wikia.nocookie.net/masseffect/images/9/92/Eclipse_Operative.png/revision/latest?cb=20100704072730
type: organic
unit: eclipse
alignment: nn
profBonus: 2
ac: 15
hp:
  dieCount: 9
  dieType: 8
abilityScores:
  str: 11
  dex: 14
  con: 13
  int: 16
  wis: 14
  cha: 12
savingThrows:
  - int
size: medium
skills:
  - electronics
speed:
  walk: 30
entries:
  features:
    - uses: 1
      perDay: true
      id: tech-armor
      name: Tech Armor
      text: As a bonus action, the operative can activate its Tech Armor. It immediately gains 10 temporary hit points. While the operative has at least 1 of these temporary hit points remaining, it has +2 AC.
    - mod: int
      list:
        - id: incinerate
          perDay: 5
          level: 2
      id: innate-powercasting
      name: Innate Powercasting
      text: "The eclipse operative's innate powercasting ability is Intelligence (power save DC 13, +5 to hit with power attacks). It can innately cast the following powers:"
  actions:
    - ref: weapon
      proficient: true
      id: m-9-tempest
      weaponId: m-9-tempest
    - uses: 2
      perDay: true
      id: summon-combat-drone
      name: Summon Combat Drone
      text: The operative summons a Combat Drone.
    - name: Repair
      text: The operative uses its action to repair a friendly, synthetic target within :distance{length="5"} for 1d8 hit points.
      id: repair
  reactions:
    - name: Tech Armor
      text: As a reaction to taking damage, the operative can activate its tech armor.
      id: tech-armor
cr: "03000"
shields:
  capacity: 10
  regen: 10
---
