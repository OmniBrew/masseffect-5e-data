---
name: Singularity
version: 1
level: 3
powerType: biotic
classes:
  - adept
tags:
  - control
casting:
  - castingTime:
      length: 1
      unit: action
    dc:
      base: 8
      proficient: true
      save: str
    conditions:
      - lifted
    duration:
      length: 1
      unit: minute
    concentration: true
    range:
      short: 90
      aoe:
        type: sphere
        size: 10
    detonates: false
  - range:
      aoe:
        size: 20
  - range:
      aoe:
        size: 30
advancements:
  - id: heavy-singularity
    name: Heavy Singularity
    text: Creatures have disadvantage when making the Strength saving throw or Strength (Athletics) check.
    casting: []
  - id: damage
    name: Damage
    text: Any creature within singularity's radius is primed (necrotic) and takes 1d8 necrotic damage at the end of each of your turns.
    casting:
      - damage:
          - dieCount: 1
            dieType: 8
            type: necrotic
        primes: necrotic
---
Create a negative mass effect field in a :distance{length="10" adj} sphere at a target location within range. Each creature or object within the
sphere's radius must succeed on a Strength saving throw or becomes lifted. Only Medium or smaller creature and objects
are affected. Any creature or object that enters the sphere for the first time or ends its turn there must succeed on a
Strength (Athletics) check or they are drawn into the sphere and become lifted. Creatures with at least 1 shield point
have advantage on the Strength saving throw or Strength (Athletics) check.

__At Higher Levels__: When you cast this power using a power slot of 4th level or higher, increase the size of the sphere
by :distance{length="10"} per power slot above the 3rd.
