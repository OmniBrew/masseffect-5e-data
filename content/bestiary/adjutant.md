---
name: Adjutant
image: https://vignette.wikia.nocookie.net/masseffect/images/9/98/ME3_adjutant.png/revision/latest/scale-to-width-down/700?cb=20121128185320
type: synorg
unit: cerberus
alignment: le
profBonus: 3
ac: 18
hp:
  dieCount: 15
  dieType: 10
abilityScores:
  str: 15
  dex: 18
  con: 16
  int: 10
  wis: 12
  cha: 8
savingThrows:
  - dex
senses:
  darkvision: 30
size: large
speed:
  walk: 30
entries:
  features:
    - mod: wis
      ref: power
      list:
        - id: singularity
          perDay: 3
      id: innate-powercasting
      name: Innate Powercasting
      text: "The adjutant's innate powercasting ability is Wisdom (power save DC 12, +4 to hit with power attacks). It can innately cast the following powers:"
    - name: Barrier
      text: The adjutant has 6 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Grappler
      text: The adjutant has advantage on attack rolls against any creature grappled by it.
      id: grappler
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
      target: one organic creature that is grappled by the adjutant, incapacitated, or restrained
      id: reaper-infection
      name: Reaper Infection
      hit: The target's hit point maximum is reduced by an amount equal to the necrotic damage taken
    - name: Multiattack
      text: The adjutant makes two Arm Cannon attacks.
      id: multiattack
cr: "06000"
---
