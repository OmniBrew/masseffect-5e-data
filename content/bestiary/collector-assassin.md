---
name: Collector Assassin
image: https://vignette.wikia.nocookie.net/masseffect/images/6/69/Collector_Assassin.png/revision/latest/scale-to-width-down/350?cb=20100623060453
type: organic
unit: collector
alignment: le
profBonus: 2
ac: 14
hp:
  dieCount: 10
  dieType: 8
abilityScores:
  str: 10
  dex: 18
  con: 10
  int: 8
  wis: 8
  cha: 8
savingThrows:
  - dex
senses:
  darkvision: 30
size: medium
skills:
  - athletics
speed:
  walk: 30
  fly: 15
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 2
          dieType: 6
          mod: true
          type: slashing
      target: one
      id: claw
      name: Claw
    - ref: weapon
      proficient: true
      id: particle-rifle
      weaponId: particle-rifle
    - name: Multiattack
      text: The collector assassin makes two Particle Rifle attacks.
      id: multiattack
  features:
    - name: Barrier
      text: The collector assassin has 4 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Possessed Collector
      text: When the collector assassin is possessed by a harbinger it gains temporary hit points equal to its total hit points and 6 barrier ticks. While it has barrier ticks it also gains resistance to bludgeoning, piercing, and slashing damage.
      id: possessed-collector
cr: "03000"
---
