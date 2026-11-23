---
name: Momentum
level: 5
klass: explorer
subclass: path-of-the-voidhopper
mechanics:
  - type: other
    shortDesc: "Moved at least half your speed this turn: attack twice when you take the Attack action."
    toggle:
      id: momentum
      whenOn:
        - type: extra-attack
          value: 2
---
At 5th level, you can attack twice instead of once when you take the attack action, but only if you moved half or
more of your movement during your turn.
