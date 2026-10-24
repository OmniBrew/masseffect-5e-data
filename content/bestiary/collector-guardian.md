---
name: Collector Guardian
image: https://vignette.wikia.nocookie.net/masseffect/images/c/ce/Collector_Guardian.png/revision/latest/scale-to-width-down/350?cb=20100623060233
type: organic
unit: collector
alignment: le
profBonus: 2
ac: 16
hp:
  dieCount: 10
  dieType: 8
abilityScores:
  str: 16
  dex: 15
  con: 16
  int: 8
  wis: 8
  cha: 9
savingThrows:
  - con
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
          dieType: 8
          mod: true
          type: bludgeoning
      target: one
      id: weapon-bash
      name: Weapon Bash
    - ref: weapon
      proficient: true
      id: collector-assault-rifle
      weaponId: collector-assault-rifle
    - uses: 1
      perDay: true
      id: hex-shield
      name: Hex Shield
      text: As a bonus action, the collector guardian generates a :distance{length="5"} tall and wide, hexagon-shaped shield with 5AC and 50 shield points which offers full-cover.
    - name: Multiattack
      text: The collector guardian makes two Collector Assault Rifle attacks.
      id: multiattack
  features:
    - name: Barrier
      text: The collector guardian has 2 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Possessed Collector
      text: When the collector guardian is possessed by a harbinger it gains temporary hit points equal to its total hit points and 6 barrier ticks. While it has barrier ticks it also gains resistance to bludgeoning, piercing, and slashing damage.
      id: possessed-collector
    - name: Warp Ammo
      text: Successful ranged attacks on a target with an active barrier will strip away 2 barrier ticks and reduce the damage reduction by half. Warp ammo can detonate primed targets.
      id: warp-ammo
cr: "04000"
---
