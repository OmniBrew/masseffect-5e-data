---
name: YMIR Mech
image: https://vignette.wikia.nocookie.net/masseffect/images/5/5f/ME2_YMIR_Mech.png/revision/latest/scale-to-width-down/700?cb=20120419005946
type: synthetic
unit: mech
alignment: nn
profBonus: 4
ac: 18
hp:
  dieCount: 17
  dieType: 10
abilityScores:
  str: 20
  dex: 6
  con: 18
  int: 16
  wis: 8
  cha: 12
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  res:
    - cold
    - bludgeoning
    - piercing
    - slashing
  vul:
    - lightning
savingThrows:
  - str
  - int
senses:
  infrared-vision: 30
size: large
speed:
  walk: 15
entries:
  actions:
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
          dieType: 10
          mod: true
          type: radiant
      target: one
      id: mass-accelerator-machinegun
      name: Mass Accelerator Machinegun
      hit: " The YMIR mech can make a burst fire attack instead"
    - recharge:
        - "5"
        - "6"
      id: rocket-launcher
      name: Rocket Launcher
      text: The YMIR mech targets an area within :distance{length="150"}. Each creature within :distance{length="15"} of the target must make a DC 18 Dexterity saving throw. On a failed save, a creature takes 52 (8d12) thunder damage or half as much damage on a successful one.
  features:
    - name: Post-mortem Explosion
      text: When the YMIR mech is reduced to 0 hit points, it self-destructs. Each creature within a :distance{length="15" adj}-radius sphere must make a DC 15 Dexterity saving throw. On a failed save, a creature takes 22 (4d10) thunder damage or half as much on a successful one.
      id: post-mortem-explosion
cr: "11000"
shields:
  capacity: 50
  regen: 10
---
