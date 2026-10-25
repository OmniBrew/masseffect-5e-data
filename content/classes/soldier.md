---
name: Soldier
primaryAbility:
  - dex
  - str
hitDie: 10
profs:
  armor:
    has:
      - light
      - medium
      - heavy
    text: Light Armor, Medium Armor, Heavy Armor
  weapon:
    has:
      - assault_rifle
      - heavy_pistol
      - melee
      - shotgun
      - smg
      - sniper_rifle
    text: Assault Rifles, Heavy Pistols, Melee, Shotguns, SMGs, Sniper Rifles
  tool:
    text: None
  skill:
    choices:
      items:
        - acrobatics
        - athletics
        - history
        - intimidation
        - medicine
        - perception
        - persuasion
        - stealth
        - survival
        - vehicle-handling
      count: 3
    text: Choose three from Acrobatics, Athletics, History, Intimidation, Medicine, Perception, Persuasion, Stealth, Survival, Vehicle Handling
  saving-throw:
    has:
      - str
      - dex
    text: Strength, Dexterity
startingEquipment:
  - choices:
      items:
        - m-3-predator
        - m-4-shuriken
        - m-8-avenger
        - m-92-mantis
        - m-23-katana
      count: 1
    text: (a) M-3 Predator or (b) M-4 Shuriken or (c) M-8 Avenger or (d) M-92 Mantis or (e) M-23 Katana
  - choices:
      items:
        - omni-blade
        - omni-hammer
      count: 1
    text: (a) Omni-Blade or (b) Omni-Hammer
  - has:
      - stock-light-armor
      - stock-medium-armor
      - stock-heavy-armor
    text: (a) Stock Light Armor or (b) Stock Medium Armor or (c) Stock Heavy Armor
progression:
  subclass:
    - 3
    - 7
    - 10
    - 15
    - 18
  abi:
    - 4
    - 6
    - 8
    - 12
    - 14
    - 16
    - 19
  columns:
    - label: features
    - label: combat_powers
      values:
        - 3
        - 3
        - 3
        - 4
        - 4
        - 4
        - 4
        - 5
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
        - 8
snippet: Soldiers are pure combat specialists effective at taking down enemies with gunfire.
---
The Soldier is a tough warrior, able to deal with a range of combat situations. The Soldier gets improved health and has the widest selection of weapons. No one is tougher or more effective at taking down enemies with gunfire.
