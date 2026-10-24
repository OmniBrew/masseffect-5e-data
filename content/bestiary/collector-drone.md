---
name: Collector Drone
image: https://vignette.wikia.nocookie.net/masseffect/images/a/a3/Collector.png/revision/latest/scale-to-width-down/331?cb=20100130000709
type: organic
unit: collector
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 7
  dieType: 8
abilityScores:
  str: 10
  dex: 10
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
        - dieCount: 1
          dieType: 6
          mod: true
          type: bludgeoning
      target: one
      id: weapon-bash
      name: Weapon Bash
    - ref: weapon
      proficient: true
      id: collector-assault-rifle
      weaponId: collector-assault-rifle
  features:
    - name: Barrier
      text: The collector drone has 0 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Possessed Collector
      text: When the collector drone is possessed by a harbinger it gains temporary hit points equal to its total hit points and 4 barrier ticks. While it has barrier ticks it also gains resistance to bludgeoning, piercing, and slashing damage.
      id: possessed-collector
cr: "01000"
---
