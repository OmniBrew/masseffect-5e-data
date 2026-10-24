---
name: Collector Captain
image: https://vignette.wikia.nocookie.net/masseffect/images/8/8f/Collector_CapME3.jpg/revision/latest/scale-to-width-down/335?cb=20121201212047
type: organic
unit: collector
alignment: le
profBonus: 3
ac: 16
hp:
  dieCount: 19
  dieType: 8
abilityScores:
  str: 15
  dex: 18
  con: 14
  int: 11
  wis: 14
  cha: 14
savingThrows:
  - dex
  - con
senses:
  darkvision: 30
size: medium
skills:
  - athletics
  - science
  - survival
speed:
  walk: 30
  fly: 15
entries:
  actions:
    - ref: weapon
      proficient: true
      id: collector-assault-rifle
      weaponId: collector-assault-rifle
    - recharge: short
      id: leadership
      name: Leadership
      text: For 1 minute, the collector captain can utter a special command or warning whenever a non-hostile creature that it can see within :distance{length="30"} of it makes an attack roll or a saving throw. The creature can add a d4 to its role provided it can hear and understand the collector captain. A creature can benefit from only one Leadership die at a time. This effect ends if the collector captain is incapacitated.
    - recharge:
        - "5"
        - "6"
      id: summon-seeker-swarm
      name: Summon Seeker Swarm
      text: The collector captain summons 1d4 seeker swarms at an unoccupied space it can see within :distance{length="30"}.
    - name: Multiattack
      text: The collector captain makes two Collector Assault Rifle attacks.
      id: multiattack
  features:
    - name: Barrier
      text: The collector captain has 6 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Pack Tactics
      text: The collector captain has advantage on an attack roll against a creature if at least one of the collector captain's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
    - name: Possessed Captain
      text: When the captain is possessed by a harbinger it gains temporary hit points equal to its total hit points and 8 barrier ticks. While it has barrier ticks it also gains resistance to bludgeoning, piercing, and slashing damage. Instead of summoning a seeker swarm, it summons a seeker plague.
      id: possessed-captain
cr: "07000"
---
