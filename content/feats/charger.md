---
name: Charger
mechanics:
  - type: bonus-action
    shortDesc: After you take the Dash action, make a melee attack or shove. With > :distance{length="10" abbr} movement in a straight line, +5 to damage roll or push :distance{length="10" abbr} away.
  - type: attack-augment
    ask: After a Dash of more than :distance{length="10"} in a straight line?
    attackLimit:
      type: melee
    augmentTypes:
      - damage
    bonus:
      type: flat
      value: 5
note: Make a melee attack or shove after the Dash action
---
Player's Handbook, p. 165
