---
name: Ride On!
level: 3
klass: tracker
subclass: outrider
mechanics:
  - type: other
    name: Ride On!
    damage:
      - dieCount:
          type: progressive
          limit: tracker
          value:
            3: 1
            7: 2
            14: 3
        dieType: 8
    shortDesc: "While mounted: once per turn, a hit by you or by your beast deals {{ roll }} extra damage."
  - name: Ride On! (mounted)
    type: other
    shortDesc: "Mounted: add your Charisma modifier to initiative."
    toggle:
      id: ride-on-mounted
      whenOn:
        - type: initiative
          effect:
            type: bonus
            bonus:
              type: mod
              value: cha
---
You and your beast are of one mind, and perfectly adjusted to each others strengths, weaknesses, and weights. Starting
at 3rd level, you gain the ability to mount creatures that are the same size as you. If the Beast casts a power that
moves it, such as Charge, while its tracker is mounted atop him, the Tracker is moved with it to its new location
without being dismounted.

While mounted, you gain the following benefits:

- You may add your Charisma to your initiative checks.
- When you use a bonus action to order your beast to take the Dash action, you may still command your beast to attack.
- Both you and your beast's attack deal an additional 1d8 damage when hitting an attack. This damage occurs once per turn,
per creature. The damage increases to 2d8 at level 7, and 3d8 at level 14.
