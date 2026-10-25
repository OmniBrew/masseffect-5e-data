---
name: Thorian Creeper
image: https://vignette.wikia.nocookie.net/masseffect/images/e/e5/Thorian_Creeper.png/revision/latest/scale-to-width-down/424?cb=20140614190322
type: organic
unit: thorian
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 4
  dieType: 8
abilityScores:
  str: 13
  dex: 11
  con: 15
  int: 2
  wis: 2
  cha: 2
irv:
  vul:
    - bludgeoning
    - force
size: medium
speed:
  walk: 30
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 2
          dieType: 4
          mod: true
          type: slashing
      target: one
      id: slash
      name: Slash
    - recharge:
        - "4"
        - "6"
      id: acid-vomit
      name: Acid Vomit
      text: The creeper regurgitates acid in a 4-meter cone. A creature within the cone must succeed on a DC 15 Dexterity saving throw or take 7 (2d6) acid damage.
  features:
    - name: Hive Mind
      text: If the creeper is within :distance{length="60"} of a Thorian Controller, it gains +1 to attack and damage rolls, ability checks, and saving throws.
      id: hive-mind
cr: "00250"
---
