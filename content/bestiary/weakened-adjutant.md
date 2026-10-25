---
name: Weakened Adjutant
image: https://vignette.wikia.nocookie.net/masseffect/images/4/46/EPP_-_adjutant_1.png/revision/latest/scale-to-width-down/640?cb=20121202170742
type: synorg
unit: cerberus
alignment: le
profBonus: 2
ac: 14
hp:
  dieCount: 10
  dieType: 10
abilityScores:
  str: 10
  dex: 16
  con: 10
  int: 8
  wis: 10
  cha: 8
size: large
speed:
  walk: 25
entries:
  actions:
    - attack: ranged
      proficient: true
      range: 50
      mod: dex
      damage:
        - dieCount: 1
          dieType: 10
          mod: true
          type: piercing
      target: one
      id: arm-cannon
      name: Arm Cannon
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 8
          mod: true
          type: bludgeoning
      target: one
      id: bash
      name: Bash
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 6
          mod: true
          type: piercing
        - dieCount: 3
          dieType: 6
          mod: true
          type: necrotic
      target: one organic creature that is grappled by the weakened adjutant, incapacitated, or restrained
      id: reaper-infection
      name: Reaper Infection
      hit: The target's hit point maximum is reduced by an amount equal to the necrotic damage taken
    - name: Multiattack
      text: The adjutant makes two Arm Cannon attacks.
      id: multiattack
  features:
    - name: Grappler
      text: The weakened adjutant has advantage on attack rolls against any creature grappled by it.
      id: grappler
cr: "02000"
---
