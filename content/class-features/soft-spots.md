---
name: Soft Spots
level: 10
klass: soldier
subclass: migrant-marine
mechanics:
  - type: other
    shortDesc: "Against an enemy marked with Tactical Sweep: + your Intelligence modifier (minimum +1) to damage."
    toggle:
      id: soft-spots
      whenOn:
        - type: attack-augment
          augmentTypes:
            - damage
          bonus:
            type: mod
            value: int
            min: 1
---
At 10th level, enemies that you scan with Tactical Sweep take extra damage when hit by one of your attacks. Whenever
your attacks hit against an enemy you marked with Tactical Sweep, you deal bonus damage equal to your Intelligence Modifier (minimum +1)
