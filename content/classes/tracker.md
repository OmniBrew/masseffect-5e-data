---
name: Tracker
primaryAbility:
  - str
  - dex
hitDie: 10
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
        - melee
        - shotgun
        - sniper_rifle
      count: 2
    text: Heavy Pistols, and choose 2 from Melee, Sniper Rifles, and Shotguns
  tool:
    has:
      - cooks-utensils
    text: Cook's Utensils
  skill:
    choices:
      items:
        - acrobatics
        - athletics
        - deception
        - intimidation
        - medicine
        - perception
        - persuasion
        - sleight-of-hand
        - stealth
        - survival
        - vehicle-handling
      count: 3
    text: Choose three from Acrobatics, Athletics, Deception, Intimidation, Medicine, Perception, Persuasion, Science, Sleight of Hand, Stealth, Survival, and Vehicle Handling
  saving-throw:
    has:
      - str
      - dex
    text: Strength, Dexterity
startingEquipment:
  - choices:
      items:
        - monomolecular-blade
        - omni-blade
        - omni-claws
      count: 1
    text: (a) Monomolecular Blade (b) Omni-Blade or (c) Omni-Claws
  - choices:
      items:
        - m-3-predator
        - m-92-mantis
        - m-27-scimitar
      count: 1
    text: (a) M-3 Predator or (b) M-92 Mantis or (c) M-27 Scimitar
  - choices:
      items:
        - stock-light-armor
        - stock-medium-armor
      count: 1
    text: (a) Light Stock Armor or (b) Medium Stock Armor
  - text: Cook's Utensils
progression:
  subclass:
    - 3
    - 7
    - 10
    - 14
  abi:
    - 4
    - 8
    - 12
    - 16
    - 19
homebrew: true
author: Helios
snippet: Trackers are expert hunters that use animal companions and have an affinity for surviving in the harshest of environments.
---
While infiltrators may excel at taking down high priority sapient targets, Trackers are experts at finding all sorts of
other prey. Be it footprints, remains of their food, scratches or markings on trees or whatever else, they are
relentless when it comes to finding whatever beast, or man, it is they are pursuing.
