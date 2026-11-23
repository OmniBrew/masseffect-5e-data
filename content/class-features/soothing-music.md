---
name: Soothing Music
level: 3
klass: musician
mechanics:
  - type: other
    name: Soothing Music
    shortDesc: When you finish a short rest, you and your allies add one roll of your Inspiration die to the amount of hit points they recovered. If they don't spend hit die during a short rest, they can recover one roll of your Inspiration die + their Constitution modifier hit points.
    damage:
      - dieCount: 1
        dieType:
          type: progressive
          limit: musician
          value:
            1: 6
            5: 8
            10: 10
            15: 12
        type: hp
---
At 3rd level, your allies are soothed or pumped up by the music you play for them during relaxation.

When you finish a short rest, you and your allies add one roll of your Inspiration die to the amount of hit points
they recovered. If they don't spend hit die during a short rest, they can recover one roll of
your Inspiration die + their Constitution modifier hit points.
