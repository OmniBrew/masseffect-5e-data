---
name: N7 Paladin
image: https://vignette.wikia.nocookie.net/masseffect/images/8/83/N7_Paladin_Sentinel_MP.png/revision/latest/scale-to-width-down/250?cb=20120717151128
type: organic
unit: n_7
alignment: ln
profBonus: 3
ac: 16
hp:
  dieCount: 17
  dieType: 8
abilityScores:
  str: 14
  dex: 12
  con: 16
  int: 13
  wis: 16
  cha: 13
savingThrows:
  - con
size: medium
skills:
  - survival
speed:
  walk: 30
entries:
  features:
    - uses: 1
      perDay: true
      id: barrier
      name: Barrier
      text: As an action or bonus action, the N7 paladin gains 5 barrier ticks. When the N7 paladin is dealt damage, remove one barrier tick and reduce the damage by 1d8.
    - uses: 1
      perDay: true
      id: omni-shield
      name: Omni-Shield
      text: 'As a bonus action, the N7 Paladin deploys its omni-shield, lasting 1 minute. While the shield is deployed, the N7 Paladin gains +2 AC and can make a melee weapon attack with the shield: +5 to hit, :distance{length="5"} reach, 1d12 bludgeoning damage.'
    - uses: 1
      perDay: true
      id: variant--fire-shield
      name: "Variant: Fire-Shield"
      text: Gain all the benefits of Omni-Shield. In addition, targets hit by the Fire-Shield take 3d10 fire damage. This damage detonates primed targets, but the N7 Paladin is immune to any detonating effects.
    - uses: 1
      perDay: true
      id: variant--cryo-shield
      name: "Variant: Cryo-Shield"
      text: Gain all the benefits of Omni-Shield. In addition, a creature hit by the Cryo-Shield take 1d8 cold damage and must succeed on a DC 13 Strength saving throw or become Frozen until the end its next turn.
    - mod: wis
      list:
        - id: incinerate
          perDay: at_will
        - id: energy-drain
          perDay: 3
        - id: snap-freeze
          perDay: 3
          level: 4
      id: innate-powercasting
      name: Innate Powercasting
      text: "The N7 paladin's innate powercasting ability is Wisdom (power save DC 14, +6 to hit with power attacks). It can innately cast the following powers:"
    - name: N7 Training
      text: The N7 Paladin has advantage on its first attack roll each turn.
      id: n7-training
  actions:
    - ref: weapon
      proficient: true
      id: n-7-hurricane
      weaponId: n-7-hurricane
    - name: Multiattack
      text: The N7 Paladin makes two N7 Hurricane attacks.
      id: multiattack
cr: "07000"
shields:
  capacity: 20
  regen: 10
---
