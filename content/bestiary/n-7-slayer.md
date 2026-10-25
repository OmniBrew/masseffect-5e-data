---
name: N7 Slayer
image: https://vignette.wikia.nocookie.net/masseffect/images/9/97/N7_Slayer_Vanguard_MP.png/revision/latest/scale-to-width-down/250?cb=20120717151234
type: organic
unit: n_7
alignment: ln
profBonus: 3
ac: 14
hp:
  dieCount: 14
  dieType: 8
abilityScores:
  str: 16
  dex: 14
  con: 13
  int: 13
  wis: 14
  cha: 12
savingThrows:
  - str
  - dex
size: medium
skills:
  - acrobatics
  - survival
speed:
  walk: 40
entries:
  features:
    - uses: 2
      perDay: true
      id: barrier
      name: Barrier
      text: As an action or bonus action, the N7 slayer gains 5 barrier ticks. When the N7 slayer is dealt damage, remove one barrier tick and reduce the damage by 1d8.
    - mod: wis
      casterLevel: 9
      ref: power
      list:
        - charge
        - phase-disruptor
        - biotic-slash
      id: powercasting
      name: Powercasting
      text: "The N7 slayer is a 9th-level powercaster. Its powercasting ability is Wisdom (power save DC 13, +5 to hit with powers). The N7 slayer has the following powers:"
    - name: Aggressive
      text: As a bonus action, the N7 Slayer can move up to its speed toward a hostile creature that it can see.
      id: aggressive
    - name: Avoidance
      text: If the N7 Slayer is subjected to an effect that allows it to make a saving throw to take only half damage, it instead takes no damage if it succeeds on the saving throw, and only half damage if it fails.
      id: avoidance
    - name: N7 Training
      text: The N7 Slayer has advantage on its first attack roll each turn.
      id: n7-training
  actions:
    - ref: weapon
      proficient: true
      id: monomolecular-blade
      weaponId: monomolecular-blade
    - ref: weapon
      proficient: true
      id: n-7-piranha
      weaponId: n-7-piranha
    - name: Multiattack
      text: The N7 Slayer makes three monomolecular blade attacks or two N7 Piranha attacks.
      id: multiattack
  reactions:
    - name: Parry and Counter
      text: The N7 Slayer adds 3 to its AC against one melee that would hit it. To do so, it must be able to see the target and be wielding a melee weapon. If the attack misses, the N7 Slayer can make one melee attack against the attacker if it is within its reach.
      id: parry-and-counter
cr: "05000"
shields:
  capacity: 15
  regen: 5
---
