---
traits:
  - id: amphibious
    name: Amphibious
    text: The {{ name }} can breathe both air and water.
  - id: bioluminescence
    name: Bioluminescence
    text: The {{ name }} can shed dim light in a :distance{length="30" adj} radius.
  - id: contra-gravitic-levitation
    name: Contra-Gravitic Levitation
    text: When the {{ name }} suffers a critical hit, roll a d20. On a roll of 1 or 2, its contra-gravitic levitation device fails and its walking speed becomes 0. It can use its action to make a DC 15 Intelligence (Engineering) check to repair the device.
  - id: tentacles
    name: Tentacles
    text: The target must succeed on a DC {{ dc }} Strength saving throw or be :condition{id="grappled"}. The {{ name }} can have up to six targets grappled at once
  - id: secrete-toxin
    name: Secrete Toxin
    text: One creature grappled by the {{ name }} must make a DC {{ dc }} Constitution saving throw or be :condition{id="poisoned"} for 1 hour.
---
