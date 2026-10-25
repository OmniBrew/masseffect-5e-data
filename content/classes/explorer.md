---
name: Explorer
primaryAbility:
  - int
  - dex
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
      - melee
    choices:
      items:
        - assault_rifle
        - shotgun
        - smg
        - sniper_rifle
      count: 2
    text: Heavy Pistols, Melee and two of Assault Rifle, Sniper Rifle, Shotgun or SMG
  skill:
    choices:
      items:
        - acrobatics
        - athletics
        - deception
        - electronics
        - engineering
        - history
        - intimidation
        - investigation
        - medicine
        - perception
        - performance
        - persuasion
        - science
        - sleight-of-hand
        - stealth
        - survival
        - vehicle-handling
      count: 4
    text: Choose four of any skills
  saving-throw:
    has:
      - int
      - dex
    text: Intelligence, Dexterity
startingEquipment:
  - choices:
      items:
        - monomolecular-blade
        - omni-blade
        - omni-claws
      count: 1
    text: One common starter weapon of your choice
  - choices:
      items:
        - m-3-predator
        - m-92-mantis
        - m-27-scimitar
      count: 1
    text: One Omni Weapon
  - choices:
      items:
        - stock-light-armor
        - stock-medium-armor
      count: 1
    text: (a) Light Stock Armor or (b) Medium Stock Armor
progression:
  subclass:
    - 3
    - 5
    - 9
    - 15
  abi:
    - 4
    - 6
    - 8
    - 12
    - 16
    - 19
homebrew: true
author: Spagheddy
snippet: Be it unknown tech, thunderous combat or explosive biotics, you can deal with any situation that comes your way.
---
Eager to explore the far reaches of the galaxy, you developed your abilities to the point where you only need your
brains and some gumption to handle any problem. Be it unknown tech, thunderous combat or explosive biotics, you can deal with any situation that comes your way.
