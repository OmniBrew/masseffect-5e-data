---
name: Soft Spots
level: 10
klass: soldier
subclass: migrant-marine
mechanics:
  - type: attack-augment
    ask: Is the target marked by your Tactical Sweep?
    augmentTypes:
      - damage
    bonus:
      type: mod
      value: int
      min: 1
---
At 10th level, enemies that you scan with Tactical Sweep take extra damage when hit by one of your attacks. Whenever
your attacks hit against an enemy you marked with Tactical Sweep, you deal bonus damage equal to your Intelligence Modifier (minimum +1)
