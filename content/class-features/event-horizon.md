---
name: Event Horizon
level: 14
klass: vanguard
subclass: void-fist
mechanics:
  - type: other
    shortDesc: "Wearing no armor: add your Charisma modifier to all your saving throws."
    toggle:
      id: event-horizon
      whenOn:
        - type: saving-throw
          value:
            - str
            - dex
            - con
            - int
            - wis
            - cha
          effect:
            type: bonus
            bonus:
              type: mod
              value: cha
---
At 14th level, your biotics emanate in a field around you. The terrain in a :distance{length="15" adj} radius
around you is considered difficult terrain to your enemies. In addition, while you do not
have any armor, you add your Charisma modifier to all of your saving throws.
