---
name: Praetorian
image: https://vignette.wikia.nocookie.net/masseffect/images/0/09/PraetorianME3.jpg/revision/latest/scale-to-width-down/700?cb=20121201212320
type: synorg
unit: collector
alignment: le
profBonus: 4
ac: 20
hp:
  dieCount: 13
  dieType: 10
abilityScores:
  str: 20
  dex: 19
  con: 21
  int: 11
  wis: 14
  cha: 10
irv:
  conImm:
    - charmed
    - grappled
    - paralyzed
    - poisoned
  res:
    - force
    - necrotic
savingThrows:
  - dex
  - con
  - str
senses:
  darkvision: 30
size: large
skills:
  - acrobatics
  - athletics
  - perception
speed:
  walk: 30
  fly: 30
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 6
          dieType: 10
          mod: true
          type: piercing
      target: one
      id: claw
      name: Claw
    - recharge:
        - "5"
        - "6"
      id: pounce
      name: Pounce
      text: The praetorian pounces to a location within :distance{length="35"} and makes a claw attack.
    - recharge:
        - "5"
        - "6"
      id: twin-particle-beams
      name: Twin Particle Beams
      text: The praetorian shoots particle beams in a :distance{length="30" adj} line that is :distance{length="10"} wide originating from itself. Each creature within the area must make a DC 18 Dexterity saving throw. On a failed save a creature takes 54 (12d8) radiant damage or half as much on a successful one.
  features:
    - name: Barrier
      text: The praetorian has 10 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Possessed Praetorian
      text: When the praetorian is possessed by a harbinger it gains 10 barrier ticks and while it has barrier ticks it also gains resistance to bludgeoning, piercing, and slashing damage. It can use its action to launch 2 missiles at a single or different target creatures within 60m. Each target must make a DC 18 Dexterity saving throw. On a failed save a target takes 33 (6d10) thunder damage, or half as much on a successful one. Once the praetorian fires its missiles, it cannot do so again.
      id: possessed-praetorian
  reactions:
    - name: Negation Barrier
      text: When targeted by a biotic power or tech power, the praetorian can use its reaction to gain 2 barrier ticks and gain resistance to force, necrotic, cold, lightning, and fire damage until the start of its next turn.
      id: negation-barrier
cr: "12000"
---
