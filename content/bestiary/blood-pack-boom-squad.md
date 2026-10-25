---
name: Blood Pack Boom-Squad
image: https://vignette.wikia.nocookie.net/masseffect/images/0/05/Blood_Pack_Boom-Squad.png/revision/latest/scale-to-width-down/388?cb=20100621053021
type: organic
unit: blood_pack
alignment: ce
profBonus: 2
ac: 11
hp:
  dieCount: 4
  dieType: 8
abilityScores:
  str: 12
  dex: 13
  con: 9
  int: 2
  wis: 4
  cha: 4
irv:
  res:
    - poison
size: medium
speed:
  walk: 40
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 6
          mod: true
          type: slashing
      target: one
      id: claws
      name: Claws
    - name: ML-77 Missile Launcher
      text: Choose a creature within :distance{length="150"} that you can see and fire a missile at it. Each creature within a :distance{length="10" adj} cube of the target, including the target, must make a DC 14 Dexterity saving throw. On a failed save a creature takes 39 (6d12) thunder damage or half as much on a successful one.
      id: ml-77-missile-launcher
  features:
    - name: Regeneration
      text: The vorcha regains 4 hit points at the start of its turn. If the vorcha takes fire damage, this trait doesn't function at the start of the vorcha's next turn. The vorcha dies only if it starts its turn with 0 hit points and doesn't regenerate.
      id: regeneration
cr: "03000"
shields:
  capacity: 5
  regen: 0
---
