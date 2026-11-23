---
name: Acceleration
level: 3
klass: explorer
subclass: path-of-the-voidhopper
mechanics:
  - type: other
    shortDesc: "Moved at least half your speed this turn: +1 AC."
    toggle:
      id: acceleration
      whenOn:
        - type: ac
          bonus:
            type: flat
            value: 1
  - type: speed-bonus
    value:
      - walk
    bonus:
      type: speed
      value: walk
      multiplier: 0.5
---
At 3rd level, your focus is on positioning and distraction rather than standing your ground. Your movement speed
increases by half. If you move half or more of your movement in a turn, you gain a bonus +1 to AC, as your
quick feet make you unpredictable to your enemies.
