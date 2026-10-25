---
name: Sniper
mechanics:
  - type: attack-augment
    ask: No hostile creature within :distance{length="30"}?
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
