---
name: Phantom
image: https://vignette.wikia.nocookie.net/masseffect/images/4/4d/ME3_Cerberus_Phantom.png/revision/latest/scale-to-width-down/699?cb=20120325214910
type: organic
unit: cerberus
alignment: ne
profBonus: 3
ac: 17
hp:
  dieCount: 20
  dieType: 8
abilityScores:
  str: 16
  dex: 22
  con: 12
  int: 11
  wis: 15
  cha: 15
savingThrows:
  - dex
size: medium
skills:
  - acrobatics
  - electronics
  - perception
  - stealth
speed:
  walk: 40
entries:
  features:
    - uses: 3
      perDay: true
      id: barrier
      name: Barrier
      text: As an action or bonus action, the phantom gains 8 barrier ticks. When the phantom is dealt damage, remove one barrier tick and reduce the damage by 1d8.
    - name: Aggressive
      text: As a bonus action, the phantom can move up to its speed toward a hostile creature that it can see.
      id: aggressive
    - name: Avoidance
      text: If the phantom subjected to an effect that allows it to make a saving throw to take only half damage, it instead takes no damage if it succeeds on the saving throw, and only half damage if it fails.
      id: avoidance
  actions:
    - ref: weapon
      proficient: true
      id: monomolecular-blade
      weaponId: monomolecular-blade
    - attack: ranged
      proficient: true
      range: 10
      mod: dex
      damage:
        - dieCount: 3
          dieType: 10
          mod: true
          type: thunder
      target: one
      id: palm-blaster
      name: Palm Blaster
    - name: Multiattack
      text: The phantom makes three Monomolecular Blade attacks or one Palm Blaster attack and two Monomolecular  Blade (one-handed) attacks.
      id: multiattack
cr: "07000"
---
