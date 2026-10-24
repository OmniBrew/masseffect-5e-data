---
name: Geth Armature
image: https://vignette.wikia.nocookie.net/masseffect/images/a/a9/ArmatureLanding.png/revision/latest/scale-to-width-down/350?cb=20090125024722
type: synthetic
unit: geth
alignment: ln
profBonus: 5
ac: 15
hp:
  dieCount: 10
  dieType: 12
abilityScores:
  str: 22
  dex: 10
  con: 25
  int: 18
  wis: 6
  cha: 8
irv:
  conImm:
    - charmed
    - deafened
    - frightened
    - frozen
    - grappled
    - invisible
    - lifted
    - paralyzed
    - poisoned
    - restrained
    - stunned
  damImm:
    - poison
    - psychic
  res:
    - bludgeoning
    - piercing
    - slashing
  vul:
    - lightning
savingThrows:
  - int
senses:
  darkvision: 30
  infrared-vision: 30
size: huge
skills:
  - perception
speed:
  walk: 15
entries:
  features:
    - uses: 3
      perDay: true
      id: repair-protocol
      name: Repair Protocol
      text: If the geth armature starts its turn with 0 shield points, it activates its repair protocol, collapsing into a compact shell. Until the start of its next turn, its speed becomes :distance{length="0" override="0 {metric}"} and it can take no Actions, but it is immune to all damage. At the start of its next turn, it regains 50 shields points.
  actions:
    - attack: ranged
      proficient: true
      range: 300
      mod: dex
      damage:
        - dieCount: 3
          dieType: 12
          mod: true
          type: piercing
        - dieCount: 3
          dieType: 12
          mod: true
          type: radiant
      target: one
      id: mass-accelerator-machinegun
      name: Mass Accelerator Machinegun
      hit: " The geth armature can make a burst fire attack instead"
    - recharge:
        - "6"
      id: siege-pulse
      name: Siege Pulse
      text: The geth armature releases a burst of electrostatic energy that disrupts armor biofeedback. Each creature within a :distance{length="15"} radius must make a DC 18 Constitution saving throw. On a failed save, a creature wearing armor looses 1d4 to their Strength and Dexterity ability scores. This loss ends if the armor is repaired, removed, or replaced.
    - name: Siege Cannon
      text: The geth armature targets a creature within :distance{length="150"} and launches a homing projectile. The target must make a DC 18 Dexterity saving throw. On a failed save, the target takes 55 (10d10) radiant damage, or half as much on a successful one.
      id: siege-cannon
cr: "15000"
shields:
  capacity: 100
  regen: 0
---
