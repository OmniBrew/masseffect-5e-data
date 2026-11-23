---
name: Strike First
level: 2
klass: engineer
subclass: stg
mechanics:
  - type: initiative
    effect:
      type: bonus
      bonus:
        type: mod
        value: int
  - type: other
    shortDesc: "Your first turn of combat (and any surprise round): your power attack rolls have advantage."
    toggle:
      id: strike-first
      whenOn:
        - type: attack-augment
          attackLimit:
            model: power
          augmentTypes:
            - notes
          notes:
            - Advantage (first turn)
---
At 2nd level, you gain a bonus to your initiative rolls equal to your Intelligence modifier. During your first turn,
your attack rolls for powers have advantage. This applies to any surprise round you participate in as well as your first round of each combat.
