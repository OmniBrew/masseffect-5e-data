---
name: Combat Engineer
image: https://vignette.wikia.nocookie.net/masseffect/images/5/54/ME3_Cerberus_Combat_Engineer.png/revision/latest/scale-to-width-down/214?cb=20120322145158
type: organic
unit: cerberus
alignment: nn
profBonus: 2
ac: 14
hp:
  dieCount: 14
  dieType: 8
abilityScores:
  str: 11
  dex: 16
  con: 12
  int: 16
  wis: 13
  cha: 16
size: medium
skills:
  - electronics
speed:
  walk: 30
entries:
  actions:
    - ref: weapon
      proficient: true
      id: m-5-phalanx
      weaponId: m-5-phalanx
    - name: Multiattack
      text: The combat engineer makes two M-5 Phalanx attacks.
      id: multiattack
    - name: Repair
      text: The combat engineer uses its action to repair a friendly, synthetic target within :distance{length="5"} for 1d8 hit points.
      id: repair
  features:
    - name: Deploy Turret
      text: The combat engineer is equipped with 1 Turret (see Bestiary). As an action, the combat engineer can deploy the Turret on a level surface within :distance{length="5"}. The Turret is controlled by the combat engineer and takes its turn at the end of the combat engineer's turn. The combat engineer can use an action to stow the Turret, placing it at another location with a subsequent action.
      id: deploy-turret
cr: "03000"
shields:
  capacity: 20
  regen: 10
---
