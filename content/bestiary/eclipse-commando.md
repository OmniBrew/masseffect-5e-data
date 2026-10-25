---
name: Eclipse Commando
image: https://vignette.wikia.nocookie.net/masseffect/images/3/3f/Eclipse_Commando.png/revision/latest?cb=20100625014253
type: organic
unit: eclipse
alignment: nn
profBonus: 3
ac: 15
hp:
  dieCount: 16
  dieType: 8
abilityScores:
  str: 15
  dex: 13
  con: 15
  int: 14
  wis: 16
  cha: 14
savingThrows:
  - wis
  - cha
size: medium
speed:
  walk: 30
entries:
  features:
    - uses: 3
      perDay: true
      id: barrier
      name: Barrier
      text: As an action or bonus action, the eclipse commando gains 10 barrier ticks. When the eclipse commando is dealt damage, remove one barrier tick and reduce the damage by 1d8.
    - mod: wis
      casterLevel: "12"
      ref: power
      list:
        - charge
        - warp
      id: powercasting
      name: Powercasting
      text: "The eclipse commando is a 12th-level powercaster. Its powercasting ability is Wisdom (power save DC 14, +6 to hit with powers). The eclipse commando has the following powers:"
    - name: Aggressive
      text: As a bonus action, the commando can move up to its speed toward a hostile creature it can see.
      id: aggressive
  actions:
    - ref: weapon
      proficient: true
      id: m-300-claymore
      weaponId: m-300-claymore
    - recharge: short
      id: leadership
      name: Leadership
      text: For 1 minute, the commando can utter a special command or warning whenever a non-hostile creature that it can see within :distance{length="30"} of it makes an attack roll or a saving throw. The creature can add a d4 to its roll provided it can hear and understand the commando. A creature can benefit from only one Leadership die at a time. This effect ends if the commando is incapacitated.
cr: "05000"
---
