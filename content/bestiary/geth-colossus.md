---
name: Geth Colossus
image: https://vignette.wikia.nocookie.net/masseffect/images/6/64/Geth_Colossus_01.jpg/revision/latest/scale-to-width-down/350?cb=20080922231050
type: synthetic
unit: geth
alignment: ln
profBonus: 7
ac: 17
hp:
  dieCount: 9
  dieType: 20
abilityScores:
  str: 28
  dex: 8
  con: 28
  int: 20
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
size: gargantuan
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
      text: If the geth colossus starts its turn with 0 shield points, it activates its repair protocol, collapsing into a compact shell. Until the start of its next turn, its speed becomes :distance{length="0" override="0 {metric}"} and it can take no Actions, but it is immune to all damage. At the start of its next turn, it regains 50 shields points.
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
      hit: " The geth colossus can make a burst fire attack instead"
    - recharge:
        - "6"
      id: siege-pulse
      name: Siege Pulse
      text: The geth colossus releases a burst of electrostatic energy that disrupts armor biofeedback. Each creature within a :distance{length="15"} radius must make a DC 20 Constitution saving throw. On a failed save, a creature wearing armor looses 1d4 to their Strength and Dexterity ability scores. This loss ends if the armor is repaired, removed, or replaced.
    - name: Siege Cannon
      text: The geth colossus targets a creature within :distance{length="150"} and launches a homing projectile. The target must make a DC 20 Dexterity saving throw. On a failed save, the target takes 55 (10d10) radiant damage, or half as much on a successful one.
      id: siege-cannon
  legendary:
    actions:
      - cost: 1
        id: mass-accelerator-machinegun-attack
        name: Mass Accelerator Machinegun Attack
        text: The geth colossus makes a Mass Accelerator Machinegun attack.
      - cost: 1
        id: siege-cannon-attack
        name: Siege Cannon Attack
        text: The geth colossus makes a Siege Cannon attack.
      - cost: 2
        id: siege-pulse-attack
        name: Siege Pulse Attack
        text: The geth colossus uses its Siege Pulse
    text: The geth colossus can take 3 legendary actions, choosing from the options below. Only one legendary action can be used at a time and only at the end of another creature's turn. The geth colossus regains spent legendary actions at the start of its turn.
cr: "21000"
shields:
  capacity: 100
  regen: 0
---
