---
name: Brute
image: https://vignette.wikia.nocookie.net/masseffect/images/9/90/ME3_Brute.png/revision/latest/scale-to-width-down/700?cb=20120320023753
type: synorg
unit: reaper
alignment: le
profBonus: 4
ac: 18
hp:
  dieCount: 13
  dieType: 10
abilityScores:
  str: 20
  dex: 12
  con: 18
  int: 9
  wis: 6
  cha: 12
irv:
  res:
    - bludgeoning
    - piercing
    - slashing
savingThrows:
  - str
  - con
senses:
  darkvision: 30
size: large
skills:
  - athletics
speed:
  walk: 40
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 5
          dieType: 12
          mod: true
          type: bludgeoning
      target: one
      id: clobber
      name: Clobber
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 3
          dieType: 8
          mod: true
          type: bludgeoning
      target: one
      id: smash
      name: Smash
    - name: Multiattack
      text: The brute makes two Smash attacks or two Clobber attacks.
      id: multiattack
  features:
    - name: Blood Frenzy
      text: The brute has advantage on melee attack rolls against any creature that doesn't have all its hit points.
      id: blood-frenzy
    - name: Brutal Charge
      text: If the brute moves at least :distance{length="15"} straight toward a target and then hits it with a smash attack on the same turn, the target takes an extra 7 (2d6) damage. If the target is a creature, it must succeed on a DC 17 Strength saving throw or be knocked prone.
      id: brutal-charge
cr: "10000"
---
