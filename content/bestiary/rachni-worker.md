---
name: Rachni Worker
image: https://vignette.wikia.nocookie.net/masseffect/images/e/e0/Rachni_Worker.png/revision/latest?cb=20100824223955
type: organic
unit: rachni
alignment: u
profBonus: 2
ac: 13
hp:
  dieCount: 2
  dieType: 6
abilityScores:
  str: 8
  dex: 10
  con: 12
  int: 1
  wis: 7
  cha: 3
savingThrows:
  - wis
senses:
  blindsight: 10
size: small
speed:
  walk: 35
entries:
  actions:
    - recharge:
        - "4"
        - "6"
      id: acid-splash
      name: Acid Splash
      text: The rachni worker spits acid at one target within :distance{length="30"} or two targets within :distance{length="30"} if both targets are within :distance{length="5"} of each other. A target must succeed on a DC 13 Dexterity saving throw or take 3 (1d6) acid damage.
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 6
          mod: true
          type: piercing
      target: one
      id: bite
      name: Bite
cr: "00125"
---
