---
name: Experiment
primaryAbility:
  - con
hitDie: 12
profs:
  armor:
    has:
      - light
    text: Light Armor
  weapon:
    has:
      - heavy_pistol
      - melee
    choices:
      items:
        - assault_rifle
        - shotgun
      count: 1
    text: Heavy Pistols, Melee and choose one between Assault Rifles and Shotguns
  skill:
    choices:
      items:
        - acrobatics
        - athletics
        - insight
        - medicine
        - perception
        - science
        - survival
      count: 3
    text: Choose three from Athletics, Acrobatics, Survival, Science, Medicine, Perception, or Insight.
  saving-throw:
    has:
      - con
      - int
    text: Constitution
startingEquipment:
  - choices:
      items:
        - omni-blade
        - monomolecular-blade
        - riot-shield
      count: 1
    text: (a) Monomolecular Blade (b) Omni-Blade or (c) Riot Shield
  - choices:
      items:
        - m-3-predator
      count: 1
    text: M-3 Predator
  - choices:
      items:
        - stock-light-armor
      count: 1
    text: Light Stock Armor
progression:
  subclass:
    - 1
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
homebrew: true
author: Spagheddy
snippet: You have been granted abilities that some would consider unnatural uses of biology or tech.
---
As an experiment, you have been granted abilities that some would consider unnatural uses of biology or tech. However,
taking advantage of these abilities heavily taxes your body and might end up being your downfall. You're the one to
decide how far to push these scars.
