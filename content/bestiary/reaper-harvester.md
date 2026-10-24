---
name: Reaper Harvester
image: https://vignette.wikia.nocookie.net/masseffect/images/a/ae/ME3_Harvester.png/revision/latest/scale-to-width-down/350?cb=20120320013110
type: synorg
unit: reaper
alignment: le
profBonus: 6
ac: 20
hp:
  dieCount: 27
  dieType: 12
abilityScores:
  str: 27
  dex: 10
  con: 25
  int: 11
  wis: 12
  cha: 16
irv:
  res:
    - bludgeoning
    - piercing
    - slashing
savingThrows:
  - con
  - wis
senses:
  darkvision: 30
size: huge
skills:
  - perception
speed:
  walk: 40
  burrow: 40
  fly: 65
entries:
  legendary:
    actions:
      - cost: 1
        id: detect
        name: Detect
        text: The reaper harvester makes a Wisdom (Perception) check.
      - cost: 2
        id: harvester-cannon-attack
        name: Harvester Cannon Attack
        text: The reaper harvester makes a harvester cannon attack.
      - cost: 3
        id: spawn-husks
        name: Spawn Husks
        text: The reaper harvester releases 1d10 Husks from its body.
    text: The reaper harvester can take 3 legendary actions, choosing from the options below. Only one legendary action can be used at a time and only at the end of another creature's turn. The reaper harvester regains spent legendary actions at the start of its turn.
  actions:
    - name: Multiattack
      text: The reaper harvester makes two harvester cannon attacks.
      id: multiattack
    - name: Harvester Cannon
      text: The reaper harvester targets a location within :distance{length="90"}. Each creature within a :distance{length="15"} radius must make a DC 19 Dexterity saving throw. On a failed save a creature takes 3d10 force and 3d10 thunder damage, or half as much damage on a successful one.
      id: harvester-cannon
cr: "20000"
---
