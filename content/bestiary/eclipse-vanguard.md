---
name: Eclipse Vanguard
image: https://vignette.wikia.nocookie.net/masseffect/images/4/45/Eclipse_Vanguard.png/revision/latest?cb=20100624033844
type: organic
unit: eclipse
alignment: nn
profBonus: 2
ac: 14
hp:
  dieCount: 9
  dieType: 8
abilityScores:
  str: 13
  dex: 13
  con: 14
  int: 14
  wis: 15
  cha: 13
size: medium
speed:
  walk: 30
entries:
  features:
    - uses: 3
      perDay: true
      id: barrier
      name: Barrier
      text: As an action or bonus action, the eclipse vanguard gains 6 barrier ticks. When the eclipse vanguard is dealt damage, remove one barrier tick and reduce the damage by 1d8.
    - uses: 1
      perDay: true
      id: tech-armor
      name: Tech Armor
      text: As a bonus action, the vanguard can activate its Tech Armor. It immediately gains 10 temporary hit points. While the vanguard has at least 1 of these temporary hit points remaining, it has +2 AC.
    - mod: wis
      casterLevel: "6"
      list:
        - shockwave
        - warp
      id: powercasting
      name: Powercasting
      text: "The eclipse vanguard is a 6th-level powercaster. Its powercasting ability is Wisdom (power save DC 12, +4 to hit with powers). The eclipse vanguard has the following powers:"
  actions:
    - ref: weapon
      proficient: true
      id: m-27-scimitar
      weaponId: m-27-scimitar
    - name: Multiattack
      text: The vanguard makes 2 M-27 Scimitar attacks.
      id: multiattack
  reactions:
    - name: Tech Armor
      text: As a reaction to taking damage, the operative can activate its tech armor.
      id: tech-armor
cr: "03000"
---
