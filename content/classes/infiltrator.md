---
name: Infiltrator
primaryAbility:
  - dex
  - int
hitDie: 8
profs:
  armor:
    has:
      - light
    text: Light Armor
  weapon:
    has:
      - heavy_pistol
    choices:
      items:
        - assault_rifle
        - melee
        - smg
        - sniper_rifle
      count: 2
    text: Heavy Pistols and choose two from Assault Rifles, Melee, SMGs, and Sniper Rifles
  tool:
    choices:
      items:
        - hacking-tools
        - thieves-tools
      count: 1
    text: Choose 1 from Hacking Tools or Thieves' Tools
  skill:
    choices:
      items:
        - athletics
        - acrobatics
        - deception
        - electronics
        - history
        - insight
        - investigation
        - perception
        - persuasion
        - sleight-of-hand
        - stealth
        - vehicle-handling
      count: 3
    text: Choose three from Athletics, Acrobatics, Deception, Electronics, History, Insight, Investigation, Perception, Persuasion, Sleight of Hand, Stealth, and Vehicle Handling
  saving-throw:
    has:
      - dex
      - int
    text: Dexterity, Intelligence
startingEquipment:
  - choices:
      items:
        - m-3-predator
        - m-4-shuriken
        - m-92-mantis
      count: 1
    text: (a) M-3 Predator or (b) M-4 Shuriken or (c) M-92 Mantis
  - choices:
      items:
        - omni-blade
        - omni-taser
        - monomolecular-blade
      count: 1
    text: (a) Omni-Blade or (b) Omni-Taser or (c) Monomolecular Blade
  - has:
      - stock-light-armor
    text: Stock Light Armor
progression:
  subclass:
    - 3
    - 9
    - 13
    - 17
  abi:
    - 4
    - 8
    - 10
    - 12
    - 16
    - 19
  columns:
    - label: sneak_attack_damage
      values:
        - 1d6
        - 1d6
        - 2d6
        - 2d6
        - 3d6
        - 3d6
        - 4d6
        - 4d6
        - 5d6
        - 5d6
        - 6d6
        - 6d6
        - 7d6
        - 7d6
        - 8d6
        - 8d6
        - 9d6
        - 9d6
        - 10d6
        - 10d6
    - label: features
    - label: tactical_cloak_uses
      values:
        - 2
        - 2
        - 2
        - 2
        - 2
        - 3
        - 3
        - 3
        - 3
        - 3
        - 4
        - 4
        - 4
        - 4
        - 4
        - 4
        - 4
        - 5
        - 5
        - 5
    - label: combat_powers
      values:
        - 0
        - 1
        - 1
        - 1
        - 1
        - 2
        - 2
        - 2
        - 2
        - 2
        - 3
        - 3
        - 3
        - 3
        - 3
        - 4
        - 4
        - 4
        - 4
        - 4
    - label: tech_points
      values:
        - 2
        - 2
        - 3
        - 4
        - 6
        - 6
        - 7
        - 7
        - 11
        - 11
        - 13
        - 13
        - 15
        - 15
        - 17
        - 17
        - 20
        - 20
        - 23
        - 25
    - label: tech_point_limit
      values:
        - 1
        - 1
        - 1
        - 1
        - 1
        - 1
        - 1
        - 1
        - 2
        - 2
        - 2
        - 2
        - 2
        - 2
        - 2
        - 2
        - 3
        - 3
        - 3
        - 3
snippet: Infiltrators are tech and combat specialists with the unique ability to cloak themselves.
---
The Infiltrator is a tech-savvy warrior, able to win battles by quickly disabling and killing enemies. These soldiers focus on unlocking alternate routes, gaining access to good equipment, and obtaining an advantageous position over enemies in combat.
