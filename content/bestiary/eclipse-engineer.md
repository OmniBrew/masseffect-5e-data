---
name: Eclipse Engineer
image: https://vignette.wikia.nocookie.net/masseffect/images/2/25/Eclipse_Engineer.png/revision/latest?cb=20100625014624
type: organic
unit: eclipse
alignment: nn
profBonus: 2
ac: 14
hp:
  dieCount: 10
  dieType: 8
abilityScores:
  str: 11
  dex: 13
  con: 12
  int: 14
  wis: 13
  cha: 10
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
      text: As a bonus action, the engineer can activate its Tech Armor. It immediately gains 10 temporary hit points. While the engineer has at least 1 of these temporary hit points remaining, it has +2 AC.
    - mod: int
      ref: power
      list:
        - id: incinerate
          perDay: 3
          level: 2
      id: innate-powercasting
      name: Innate Powercasting
      text: "The eclipse engineer's innate powercasting ability is Intelligence (power save DC 12, +4 to hit with power attacks). It can innately cast the following powers:"
  actions:
    - ref: weapon
      proficient: true
      id: m-6-carnifex
      weaponId: m-6-carnifex
    - uses: 1
      perDay: true
      id: summon-combat-drone
      name: Summon Combat Drone
      text: The engineer summons a Combat Drone.
    - name: Repair
      text: The engineer uses its action to repair a friendly, synthetic target within :distance{length="5"} for 1d8 hit points.
      id: repair
  reactions:
    - name: Tech Armor
      text: As a reaction to taking damage, the engineer can activate its tech armor.
      id: tech-armor
cr: "02000"
shields:
  capacity: 10
  regen: 5
---
