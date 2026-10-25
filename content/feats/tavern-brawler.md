---
name: Tavern Brawler
mechanics:
  - type: asi-choice
    limit:
      - str
      - con
  - type: natural-weapon
    replacesUnarmedStrike: true
    value:
      type: natural-melee
      notes: []
      properties: []
      range:
        short: 5
      damage:
        dieCount: 1
        dieType: 4
        type: bludgeoning
  - type: bonus-action
    shortDesc: When you hit a creature with an unarmed strike or an improvised weapon on your turn, you can use a bonus action to attempt to grapple the target.
note: +1 Strength or Constitution, improved improvised weapons
---
Player's Handbook, p. 170
