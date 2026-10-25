---
name: Ravager
image: https://vignette.wikia.nocookie.net/masseffect/images/7/7b/ME3_Ravager.png/revision/latest/scale-to-width-down/350?cb=20120319195950
type: synorg
unit: reaper
alignment: le
profBonus: 3
ac: 12
hp:
  dieCount: 20
  dieType: 10
abilityScores:
  str: 16
  dex: 14
  con: 10
  int: 8
  wis: 11
  cha: 11
irv:
  conImm:
    - charmed
senses:
  darkvision: 30
size: large
speed:
  walk: 30
entries:
  actions:
    - recharge:
        - "5"
        - "6"
      id: acid-splash
      name: Acid Splash
      text: The ravager spits acid in a :distance{length="15" adj} cube. Each creature in the area must make a DC 15 Dexterity saving throw, taking 27 (6d8) acid damage on a failed save, or half as much damage on a successful one.
    - attack: ranged
      proficient: true
      range: 150
      mod: dex
      damage:
        - dieCount: 3
          dieType: 10
          mod: true
          type: piercing
        - dieCount: 3
          dieType: 6
          mod: true
          type: acid
      target: one
      id: twin-artillery-cannons
      name: Twin Artillery Cannons
    - name: Multiattack
      text: The ravager makes two twin artillery cannon attacks.
      id: multiattack
  features:
    - name: Egg Sacs
      text: If the ravager takes piercing or slashing damage that is not from the result of a critical hit one of its egg sacs explodes, releasing 1d10 swarmers.
      id: egg-sacs
cr: "06000"
---
