---
name: Sniper
mechanics:
  - type: other
    shortDesc: 'No hostile creature within :distance{length="30"}: +2 to damage rolls with a sniper rifle.'
    toggle:
      id: FS_sniper
      whenOn:
        - type: attack-augment
          attackLimit:
            model: weapon
            modelTypes:
              - sniper_rifle
          augmentTypes:
            - damage
          bonus:
            type: flat
            value: 2
type: fighting-styles
---
If no hostile creature is within :distance{length="30"} of you, gain +2 to damage rolls on attacks made with a sniper rifle.
