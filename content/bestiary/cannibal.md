---
name: Cannibal
image: https://vignette.wikia.nocookie.net/masseffect/images/1/1b/ME3_Cannibal.png/revision/latest/scale-to-width-down/339?cb=20120320020900
type: synorg
unit: reaper
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 16
  dieType: 8
abilityScores:
  str: 13
  dex: 10
  con: 10
  int: 8
  wis: 5
  cha: 3
senses:
  darkvision: 30
size: medium
speed:
  walk: 25
entries:
  features:
    - list:
        - id: frag-grenade
          mark: iii
          uses: 2
      id: grenades
      name: Grenades
      text: The cannibal has the following grenades equipped. It can use a grenade as an action.
    - name: Pack Tactics
      text: The cannibal has advantage on an attack roll against a creature if at least one of the cannibal's allies is within :distance{length="5"} of the creature and the ally isn't incapacitated.
      id: pack-tactics
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
    - uses: 1
      perDay: true
      id: cannibalize
      name: Cannibalize
      text: The cannibal spends its action consuming a creature with 0 hit points within :distance{length="5"}. At the start of its next turn it gains 5 AC and 1d8 hit points and the consumed creature (including all of its weapons, armor, and items) is completely dissolved. If the creature is a player character, it dies. Cannibals prefer to use their cannibalize action over any other.
    - name: Multiattack
      text: The cannibal makes 2 Arm Cannon attacks.
      id: multiattack
cr: "02000"
---
