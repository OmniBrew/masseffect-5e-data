---
name: Apex Processor
mechanics:
  - type: saving-throw
    value: int
  - type: saving-throw
    value: cha
  - type: saving-throw
    value: str
  - type: saving-throw
    value: dex
  - type: saving-throw
    value: con
  - type: saving-throw
    value: wis
  - type: other
    name: Apex Processor
    damage:
      - type: hp
        mod: con
        bonus:
          type: flat
          value: 5
    shortDesc: "At the start of each of your turns, while you have at least 1 hit point and are below half your maximum: regain {{ roll }}."
type: apex-augments
---
You gain proficiency in all saving throws. You regenerate hit points equal to 5 + your constitution
modifier each turn as long as you are below half your max hit points and still have at least one hit point.
