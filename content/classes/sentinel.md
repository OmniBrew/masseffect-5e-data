---
name: Sentinel
primaryAbility:
  - wis
  - int
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
      - heavy_pistol
    choices:
      items:
        - assault_rifle
        - melee
        - shotgun
        - smg
      count: 2
    text: Heavy Pistols and choose two from Assault Rifles, Melee, Shotguns, and SMGs
  tool:
    text: None
  skill:
    choices:
      items:
        - athletics
        - engineering
        - insight
        - intimidation
        - medicine
        - persuasion
        - science
        - survival
      count: 3
    text: Choose three from Athletics, Engineering, Insight, Intimidation, Medicine, Persuasion, Science, and Survival
  saving-throw:
    has:
      - cha
      - con
    text: Charisma, Constitution
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
        - omni-hammer
        - monomolecular-blade
        - riot-shield
      count: 1
    text: (a) Omni-Blade or (b) Omni-Hammer or (c) Monomolecular Blade or (d) Riot Shield
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
        - 6
        - 7
        - 7
        - 8
        - 8
    - label: cantrips
      values:
        - 2
        - 2
        - 2
        - 3
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
        - 4
        - 4
        - 4
        - 4
    - label: powers_known
      values:
        - 2
        - 3
        - 4
        - 5
        - 6
        - 7
        - 8
        - 9
        - 10
        - 10
        - 11
        - 11
        - 12
        - 12
        - 13
        - 13
        - 14
        - 14
        - 15
        - 15
    - label: power_slots
      values:
        - 1
        - 2
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
        - 3
        - 3
        - 4
        - 4
        - 4
        - 4
    - label: power_level
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
        - 3
        - 3
        - 3
        - 3
        - 3
        - 3
        - 3
        - 3
snippet: Sentinels are unique, bringing both tech and biotic abilities to the battlefield.
---
The Sentinel is able to combine tech and biotics to manipulate the environment, disable and track enemies, or defend
the party. In addition to complete weapons training, Sentinels are equipped with an advanced shield that makes taking
cover much less necessary and rushing their enemies much more productive.
