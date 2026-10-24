---
name: Fly
version: 1
level: 2
powerType: biotic
classes:
  - adept
  - sentinel
  - vanguard
  - explorer
tags:
  - movement
casting:
  - castingTime:
      length: 1
      unit: action
    duration:
      length: 10
      unit: minute
    concentration: true
    range:
      short: 0
    detonates: false
advancements:
  - id: speed
    name: Speed
    text: You may cast fly as a bonus action. Increase the flying speed to :distance{length="90"}
    casting:
      - altCasting:
          - length: 1
            unit: bonus_action
  - id: extended-cast
    name: Extended Cast
    text: The duration of fly becomes 30 minutes.
    casting:
      - duration:
          length: 30
---
Create a negative mass effect field around yourself allowing you to move freely through the air. During the duration of
this power, you gain a flying speed of :distance{length="60"}. When the power ends if you are still aloft, you fall to the ground.
