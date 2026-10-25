---
name: Dark Sphere
level: 3
version: 1
powerType: biotic
tags:
  - damage
classes:
  - adept
casting:
  - castingTime:
      length: 1
      unit: action
    dc:
      save: con
    damage:
      - dieCount: 6
        dieType: 8
        type: necrotic
    duration:
      length: 1
      unit: minute
    concentration: true
    range:
      short: 0
      aoe:
        type: sphere
        size: 10
    detonates: true
    primes: necrotic
  - damage:
      - dieCount: 8
  - damage:
      - dieCount: 10
advancements:
  - id: control
    name: Control
    text: Before the sphere moves, you may change its direction and speed. Its speed becomes :distance{length="10"}, :distance{length="15"}, or :distance{length="20"}.
    casting: []
  - id: amplify
    name: Amplify
    text: Add 1d8 to the detonation damage for each :distance{length="10"} the sphere travels.
    casting: []
---
Launch a slow-moving, :distance{length="10" adj} wide sphere of dark energy in a straight line. It moves :distance{length="10"} at the end of each of your turns.
A creature caught in the sphere's path becomes :condition{id="primed" sub="necrotic"} until the end of its next turn and
must make a Constitution saving throw. On a failed save, a creature takes necrotic damage equal to 6d8, or half as much on a successful one.

At the start of your turn, if the sphere has traveled :distance{length="60"}, it detonates and the power ends. Each creature within
a :distance{length="15" adj} radius must make a Constitution saving throw. On a failed save a creature takes necrotic damage equal to
6d8 or half as much damage on a successful one. This damage detonates any primed targets.

You can use an action to detonate the sphere before it travels :distance{length="60"}. If you lose concentration while casting the power,
it does not detonate.

__At Higher Levels__: When you cast this power using a power slot of 4th level or higher, the damage increases by 2d8
for each slot level above 3rd.
