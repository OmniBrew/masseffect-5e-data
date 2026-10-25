---
name: Thorian Controller
image: https://vignette.wikia.nocookie.net/masseffect/images/e/ee/Test_subject_hyperres.png/revision/latest/scale-to-width-down/180?cb=20131218143230
type: organic
unit: thorian
alignment: le
profBonus: 2
ac: 14
hp:
  dieCount: 8
  dieType: 8
abilityScores:
  str: 14
  dex: 11
  con: 15
  int: 14
  wis: 12
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
      text: The creeper regurgitates acid in a 4-meter cone. A creature within the code must succeed on a DC 15 Dexterity saving throw or take 14 (4d6) acid damage.
  features:
    - name: Creeper Resemblance
      text: The controller resembles a Thorian creeper. A creature that can see the controller can discern its true nature with a successful DC 15 Intelligence (Science) or Intelligence (Investigation) check.
      id: creeper-resemblance
    - name: Hive Mind Overseer
      text: The controller gains a +1 bonus to its attack and damage rolls, ability checks, and saving throws for each creature within :distance{length="60"} of it that has the Hive Mind feature. This bonus cannot exceed +5.
      id: hive-mind-overseer
    - name: Indoctrination
      text: Unless a thorian controller is incapacitated, it is a source of indoctrination to all creatures within :distance{length="250"} of it. See the indoctrination condition.
      id: indoctrination
cr: "00500"
---
These creatures act as the eyes, ears, and mouth of the Thorian, issuing its commands while also 
informing on its enemies.
