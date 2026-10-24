---
name: Engineer
primaryAbility:
  - int
hitDie: 8
profs:
  armor:
    has:
      - light
      - medium
    text: Light Armor, Medium Armor
  weapon:
    has:
      - heavy_pistol
    choices:
      items:
        - assault_rifle
        - melee
        - smg
      count: 1
    text: Heavy Pistols and choose one from Assault Rifles, Melee, or SMGs
  tool:
    choices:
      items:
        - armorsmiths-workbench
        - tailors-tools
        - tinkers-tools
        - weaponsmiths-workbench
      count: 1
    text: Choose 1 from Armorsmith's Workbench, Tailor's Tools, Tinker's Tools, and Weaponsmith's Workbench
  skill:
    choices:
      items:
        - athletics
        - electronics
        - engineering
        - history
        - investigation
        - medicine
        - science
        - vehicle-handling
      count: 3
    text: Choose three from Athletics, Electronics, Engineering, History, Investigation, Medicine, Science, and Vehicle Handling
  saving-throw:
    has:
      - con
      - int
    text: Constitution, Intelligence
startingEquipment:
  - choices:
      items:
        - m-3-predator
        - m-4-shuriken
        - m-8-avenger
      count: 1
    text: (a) M-3 Predator or (b) M-4 Shuriken or (c) M-8 Avenger
  - choices:
      items:
        - omni-blade
        - omni-taser
        - omni-torch
      count: 1
    text: (a) Omni-Blade or (b) Omni-Taser or (c) Omni-Torch
  - choices:
      items:
        - stock-light-armor
        - stock-medium-armor
      count: 1
    text: (a) Stock Light Armor or (b) Stock Medium Armor
progression:
  subclass:
    - 2
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
    - label: tech_points
      values:
        - 2
        - 4
        - 5
        - 7
        - 11
        - 13
        - 15
        - 17
        - 20
        - 23
        - 26
        - 26
        - 30
        - 30
        - 34
        - 34
        - 39
        - 42
        - 45
        - 50
    - label: tech_point_limit
      values:
        - 1
        - 1
        - 1
        - 1
        - 2
        - 2
        - 2
        - 2
        - 3
        - 3
        - 3
        - 3
        - 4
        - 4
        - 4
        - 4
        - 5
        - 5
        - 6
        - 6
snippet: Engineers are tech specialists, the only class able to employ combat drones on the battlefield.
---
The Engineer is a tech specialist, able to quickly and easily manipulate the environment with specific talents, and repair or modify technical equipment. Gameplay focus is on shaping the battlefield during combat, healing the party, and debuffing enemies (disabling weapons and lowering shields).
