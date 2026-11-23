---
name: Peak Performance
level: 18
klass: engineer
subclass: biohacker
mechanics:
  - type: other
    shortDesc: "Attacking with Intelligence: attack twice when you take the Attack action."
    toggle:
      id: peak-performance
      whenOn:
        - type: extra-attack
          value: 2
  - type: asi
    ability: con
    amount: 2
---
At 18th level, your Constitution score increases by 2, and it's cap also increases by 2. When you take the attack
action that would use your Intelligence for the attack and damage roll, you can attack twice.
