---
name: Radiation Poisoning
level: 6
klass: adept
subclass: nuclear
mechanics:
  - type: power-augment
    damageTypes:
      - radiant
    merge:
      primes: radiant
---
At 6th level, your powers that deal Radiant damage also force your opponent to make a save against your Power Save DC
or be :condition{id="primed" sub="radiant"}.
