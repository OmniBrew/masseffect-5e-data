---
name: Musician
primaryAbility:
  - cha
hitDie: 6
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
        - melee
        - shotgun
        - sniper_rifle
        - smg
      count: 2
    text: Heavy Pistols, and choose one from Melee, SMGs, Sniper Rifles, and Shotguns
  skill:
    has:
      - performance
    choices:
      items:
        - acrobatics
        - athletics
        - deception
        - electronics
        - engineering
        - history
        - intimidation
        - persuasion
        - science
        - sleight-of-hand
        - vehicle-handling
      count: 3
    text: Performance and choose three from Acrobatics, Athletics, Deception, Electronics, Engineering, History, Intimidation, Persuasion, Science, Sleight of Hand, and Vehicle Handling
  saving-throw:
    has:
      - cha
      - wis
    text: Charisma, Wisdom
startingEquipment:
  - choices:
      items:
        - omni-blade
        - omni-hammer
        - riot-shield
      count: 1
    text: (a) Omni-Blade (b) Omni-Hammer or (c) Riot Shield
  - choices:
      items:
        - m-3-predator
        - m-92-mantis
        - m-23-katana
        - m-4-shuriken
      count: 1
    text: (a) M-3 Predator or (b) M-92 Mantis or (c) M-23 Katana or (d) M-4 Shuriken
  - choices:
      items:
        - stock-light-armor
      count: 1
    text: Light Stock Armor
progression:
  subclass:
    - 3
    - 7
    - 11
    - 17
    - 20
  abi:
    - 4
    - 8
    - 12
    - 16
    - 19
homebrew: true
author: Spagheddy
snippet: Musicians are beings who dedicate their lives to inspiring others.
---
As old as stories themselves, Musicians are beings who dedicate their lives to inspiring others. Their outlooks vary:
cult leaders, entertainers, even war criers. It matters not. All that matters is that they listen to the music
of the spheres... and through them, others can hear whispers of it.
