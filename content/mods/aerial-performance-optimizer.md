---
name: Aerial Performance Optimizer
rarity: rare
modType: armor
cost: 40000
manufacturer: elanus-risk-control-services
tags:
  - special
placement: chest
availability:
  - light
  - medium
  - heavy
flavor: Enhance your jet pack or jump jet armor modification with an advanced aerial lubricant and stabilizer.
mechanics:
  - type: other
    shortDesc: "Hovering (jump jets) or flying (jetpack): +2 to all attack and damage rolls."
    toggle:
      id: aerial-performance-optimizer
      whenOn:
        - type: attack-augment
          augmentTypes:
            - hit
            - damage
          bonus:
            type: flat
            value: 2
---
Requires a Jump Jet or Jetpack mod also be installed. When you are hovering (via Jump Jets) or flying (via Jetpack), you have a +2 bonus to all attack and damage rolls.
