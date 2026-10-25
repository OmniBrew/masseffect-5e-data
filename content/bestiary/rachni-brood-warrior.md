---
name: Rachni Brood Warrior
image: https://vignette.wikia.nocookie.net/masseffect/images/e/e5/Rachni_Brood_Warrior.PNG/revision/latest/scale-to-width-down/700?cb=20100824160815
type: organic
unit: rachni
alignment: u
profBonus: 2
ac: 15
hp:
  dieCount: 12
  dieType: 10
abilityScores:
  str: 19
  dex: 12
  con: 17
  int: 7
  wis: 15
  cha: 7
savingThrows:
  - con
  - wis
senses:
  blindsight: 4
size: large
skills:
  - perception
speed:
  walk: 30
entries:
  features:
    - uses: 3
      perDay: true
      id: barrier
      name: Barrier
      text: As an action or bonus action, the rachni brood warrior gains 5 barrier ticks. When the rachni brood warrior is dealt damage, remove one barrier tick and reduce the damage by 1d8.
    - mod: wis
      ref: power
      list:
        - id: stasis
          perDay: 3
        - id: warp
          perDay: 5
      id: innate-powercasting
      name: Innate Powercasting
      text: "The rachni brood warrior's innate powercasting ability is Wisdom (power save DC 12, +4 to hit with power attacks). It can innately cast the following powers:"
    - name: Grappler
      text: The rachni brood warrior has advantage on attack rolls against any creature grappled by it.
      id: grappler
  actions:
    - attack: ranged
      proficient: true
      range: 50
      mod: dex
      damage:
        - dieCount: 2
          dieType: 6
          mod: false
          type: acid
        - dieCount: 2
          dieType: 6
          mod: false
          type: necrotic
      target: one
      id: acid-spit
      name: Acid Spit
      hit: " This damage bypasses shields"
    - attack: melee
      proficient: true
      range: 10
      mod: str
      damage:
        - dieCount: 2
          dieType: 10
          mod: true
          type: piercing
        - dieCount: 1
          dieType: 10
          mod: false
          type: acid
      target: one
      id: impale
      name: Impale
    - name: Multiattack
      text: The brood warrior makes two Impale attacks or attempts to grapple a creature and makes an Impale attack.
      id: multiattack
cr: "04000"
---
