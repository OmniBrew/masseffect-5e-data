---
name: Blood Pack Warrior
image: https://vignette.wikia.nocookie.net/masseffect/images/e/e8/Blood_Pack_Warrior.png/revision/latest/scale-to-width-down/352?cb=20100621023223
type: organic
unit: blood_pack
alignment: ce
profBonus: 2
ac: 16
hp:
  dieCount: 8
  dieType: 8
abilityScores:
  str: 16
  dex: 13
  con: 17
  int: 7
  wis: 12
  cha: 10
irv:
  res:
    - necrotic
savingThrows:
  - con
size: medium
speed:
  walk: 30
entries:
  actions:
    - ref: weapon
      proficient: true
      id: m-27-scimitar
      weaponId: m-27-scimitar
  features:
    - name: Aggressive
      text: As a bonus action, the warrior can move up to its speed toward a hostile creature that it can see.
      id: aggressive
    - name: Shotgun Specialist
      text: The warrior has advantage on shotgun weapon attacks against targets within the normal range of the shotgun.
      id: shotgun-specialist
    - name: Regeneration
      text: The warrior regains 4 hit points at the start of its turn. If the warrior takes fire damage, this trait doesn't function at the start of the warrior's next turn. The warrior dies only if it starts its turn with 0 hit points and doesn't regenerate.
      id: regeneration
    - name: Incendiary Ammo
      text: "When the warrior hits with its M-27 Scimitar, the target takes an additional 1d4 fire damage and becomes primed: fire until the end of the warrior's next turn."
      id: incendiary-ammo
cr: "03000"
---
