---
name: N7 Shadow
image: https://vignette.wikia.nocookie.net/masseffect/images/0/08/N7_Shadow_Infiltrator_MP.png/revision/latest/scale-to-width-down/250?cb=20120717151201
type: organic
unit: n_7
alignment: ln
profBonus: 3
ac: 15
hp:
  dieCount: 11
  dieType: 8
abilityScores:
  str: 12
  dex: 18
  con: 14
  int: 16
  wis: 11
  cha: 12
savingThrows:
  - dex
size: medium
skills:
  - acrobatics
  - survival
speed:
  walk: 35
entries:
  features:
    - uses: 3
      perDay: true
      id: tactical-cloak
      name: Tactical Cloak
      text: As a bonus action, the N7 Shadow activates its tactical cloak, becoming invisible for 1 minute. When the N7 Shadow makes a melee or ranged attack or uses a tech or combat power, tactical cloak ends.
    - mod: int
      ref: power
      list:
        - id: electric-slash
          perDay: 4
          level: 3
      id: innate-powercasting
      name: Innate Powercasting
      text: "The N7 shadow's innate powercasting ability is Intelligence (power save DC 14, +6 to hit with power attacks). It can innately cast the following powers:"
    - name: Assassinate
      text: During its first turn, the N7 Shadow has advantage on attack rolls against any creature that hasn't taken a turn. Any hit the N7 Shadow scores against a surprised creature is a critical hit.
      id: assassinate
    - name: Evasion
      text: If the N7 Shadow is subjected to an effect that allows it to make a Dexterity saving throw to take only half damage, the N7 Shadow instead takes no damage if it succeeds on the saving throw, and only half damage if it fails.
      id: evasion
    - name: N7 Training
      text: The N7 Shadow has advantage on its first attack roll each turn.
      id: n7-training
    - name: Sneak Attack
      text: Once per turn, the N7 Shadow deals an extra 14 (4d6) damage when it hits a target with a weapon attack and has advantage on the attack roll, or when the target is within :distance{length="5"} of an ally of the N7 Shadow that isn't incapacitated and the N7 Shadow doesn't have disadvantage on the attack roll.
      id: sneak-attack
  actions:
    - ref: weapon
      proficient: true
      id: monomolecular-blade
      weaponId: monomolecular-blade
    - ref: weapon
      proficient: true
      id: m-97-viper
      weaponId: m-97-viper
    - name: Multiattack
      text: The N7 Shadow makes three monomolecular blade attacks.
      id: multiattack
cr: "07000"
shields:
  capacity: 20
  regen: 10
---
