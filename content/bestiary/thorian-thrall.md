---
name: Thorian Thrall
image: https://vignette.wikia.nocookie.net/masseffect/images/e/eb/Feros_Asari_Clone_and_Thorian.png/revision/latest?cb=20090305015251
type: organic
unit: thorian
alignment: le
profBonus: 2
ac: 13
hp:
  dieCount: 3
  dieType: 8
abilityScores:
  str: 11
  dex: 13
  con: 9
  int: 4
  wis: 5
  cha: 6
size: medium
speed:
  walk: 30
entries:
  actions:
    - ref: weapon
      proficient: true
      id: m-3-predator
      weaponId: m-3-predator
  features:
    - name: Hive Mind
      text: If the creeper is within :distance{length="60"} of a Thorian Controller, it gains +1 to attack and damage rolls, ability checks, and saving throws.
      id: hive-mind
    - name: Enslaved Mind
      text: The thrall loses all levels of indoctrination reverts to its normal self if the controlling Thorian dies.
      id: enslaved-mind
    - name: Random Thrall (variant)
      text: Thralls can be any organic humanoid with an intelligence of 4 or greater. Instead, you may use the stat block of a randomly generated grunt or other organic humanoid from the bestiary.
      id: random-thrall--variant-
cr: "00125"
shields:
  capacity: 5
  regen: 0
---
The poor slaves of the Thorian, they act as the reminder of the dangers of the frontier. Kill the 
Thorian to end their suffering.
