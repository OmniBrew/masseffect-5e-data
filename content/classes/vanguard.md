---
name: Vanguard
primaryAbility:
  - str
  - wis
hitDie: 12
profs:
  armor:
    has:
      - light
      - medium
    text: Light Armor, Medium Armor
  weapon:
    has:
      - heavy_pistol
      - melee
    choices:
      items:
        - shotgun
        - smg
      count: 1
    text: Heavy Pistols, Melee and choose either Shotguns or SMGs
  tool:
    text: None
  skill:
    choices:
      items:
        - acrobatics
        - athletics
        - deception
        - insight
        - intimidation
        - performance
        - persuasion
        - sleight-of-hand
        - survival
      count: 3
    text: Choose three from Acrobatics, Athletics, Deception, Insight, Intimidation, Performance, Persuasion, Sleight of Hand, and Survival
  saving-throw:
    has:
      - str
      - wis
    text: Strength, Wisdom
startingEquipment:
  - choices:
      items:
        - m-3-predator
        - m-4-shuriken
        - m-23-katana
      count: 1
    text: (a) M-3 Predator or (b) M-4 Shuriken or (c) M-23 Katana
  - choices:
      items:
        - omni-blade
        - omni-hammer
        - monomolecular-blade
        - riot-shield
      count: 1
    text: (a) Omni-Blade or (b) Omni-Hammer or (c) Monomolecular Blade or (d) Riot Shield
  - choices:
      items:
        - stock-light-armor
        - stock-medium-armor
      count: 1
    text: (a) Stock Light Armor or (b) Stock Medium Armor
progression:
  subclass:
    - 3
    - 6
    - 10
    - 14
    - 18
  abi:
    - 4
    - 8
    - 12
    - 16
    - 19
  columns:
    - label: features
    - label: barrier_uses
      values:
        - 2
        - 2
        - 3
        - 3
        - 3
        - 4
        - 4
        - 4
        - 4
        - 4
        - 4
        - 5
        - 5
        - 5
        - 5
        - 5
        - 6
        - 6
        - 6
        - 6
    - label: barrier_ticks
      values:
        - 3
        - 3
        - 3
        - 4
        - 4
        - 4
        - 5
        - 5
        - 5
        - 6
        - 6
        - 6
        - 7
        - 7
        - 7
        - 8
        - 8
        - 9
        - 9
        - 10
    - label: cantrips
      values:
        - 4
        - 4
        - 4
        - 5
        - 5
        - 5
        - 5
        - 5
        - 5
        - 6
        - 6
        - 6
        - 6
        - 6
        - 6
        - 6
        - 6
        - 6
        - 6
        - 6
    - label: powers_known
      values:
        - 0
        - 2
        - 3
        - 3
        - 4
        - 4
        - 5
        - 5
        - 6
        - 6
        - 6
        - 7
        - 8
        - 8
        - 9
        - 9
        - 10
        - 10
        - 11
        - 11
    - label: power_slots_by_power_level
      values:
        - - 0
          - 2
          - 3
          - 4
          - 6
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
          - 7
        - - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 2
          - 2
          - 3
          - 3
          - 4
          - 4
          - 5
          - 5
          - 6
          - 6
          - 6
          - 6
        - - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 0
          - 1
          - 1
          - 2
          - 2
snippet: Vanguards have a high-risk high-reward combat style, using biotics and melee strikes.
---
Vanguards are feared for their high-risk high-reward combat style, closing quickly on enemies and destroying them at close range with weapons and biotic abilities. They are outfitted with L5n implants, enabling them to perform a biotic charge that strikes the opponent with incredible force while closing distance.
