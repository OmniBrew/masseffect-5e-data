---
name: Oculus
image: https://vignette.wikia.nocookie.net/masseffect/images/e/ed/Oculus_Combat.png/revision/latest?cb=20100731075649&format=original
type: synthetic
unit: reaper
alignment: le
profBonus: 4
ac: 17
hp:
  dieCount: 22
  dieType: 10
abilityScores:
  str: 12
  dex: 16
  con: 15
  int: 13
  wis: 9
  cha: 10
irv:
  conImm:
    - blinded
    - deafened
    - frightened
    - lifted
    - paralyzed
    - poisoned
    - prone
  damImm:
    - poison
savingThrows:
  - dex
  - con
senses:
  infrared-vision: 30
size: large
skills:
  - perception
speed:
  fly: 60
entries:
  actions:
    - attack: melee
      proficient: true
      range: 25
      mod: str
      damage:
        - dieCount: 4
          dieType: 6
          mod: true
          type: bludgeoning
      target: one
      id: crush
      name: Crush
    - name: Particle Beam
      text: The oculus fires a persistent particle beam that is :distance{length="60"} long and :distance{length="5"} wide that lasts until the start of the oculus's next turn. While firing the beam, the oculus's speed becomes 0. Each creature that is within the beam's path or that moves into the beam's path for the first time on its turn must make a DC 16 Constitution saving throw. On a failed save, a creature takes 66 (12d10) radiant damage, or half as much on a successful save.
      id: particle-beam
cr: "11000"
---
