---
name: Blood Pack Trooper
image: https://vignette.wikia.nocookie.net/masseffect/images/8/80/ME2_blood_pack_trooper.png/revision/latest/scale-to-width-down/305?cb=20140516115803
type: organic
unit: blood_pack
alignment: ce
profBonus: 2
ac: 11
hp:
  dieCount: 8
  dieType: 8
abilityScores:
  str: 11
  dex: 12
  con: 11
  int: 4
  wis: 4
  cha: 6
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
    - ref: weapon
      proficient: true
      id: m-3-predator
      weaponId: m-3-predator
    - ref: weapon
      proficient: true
      id: m-8-avenger
      weaponId: m-8-avenger
  features:
    - name: Aggressive
      text: As a bonus action, the trooper can move up to its speed toward a hostile creature that it can see.
      id: aggressive
    - name: Regeneration
      text: The trooper regains 4 hit points at the start of its turn. If the trooper takes fire damage, this trait doesn't function at the start of the trooper's next turn. The trooper dies only if it starts its turn with 0 hit points and doesn't regenerate.
      id: regeneration
  reactions:
    - name: Fortification
      text: As a reaction to being hit by an attack the trooper can see, it gains a +5 bonus to its AC until the start of its next turn (including against the triggering attack).
      id: fortification
cr: "00250"
---
