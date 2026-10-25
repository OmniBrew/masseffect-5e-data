---
name: Rachni Queen
image: https://vignette.wikia.nocookie.net/masseffect/images/3/38/Noveria_rachni_queen.png/revision/latest/scale-to-width-down/700?cb=20090919061419
type: organic
unit: rachni
alignment: ln
profBonus: 6
ac: 21
hp:
  dieCount: 22
  dieType: 20
abilityScores:
  str: 25
  dex: 10
  con: 18
  int: 22
  wis: 25
  cha: 18
irv:
  conImm:
    - charmed
savingThrows:
  - wis
  - con
  - str
senses:
  blindsight: 30
size: gargantuan
skills:
  - perception
  - history
speed:
  walk: 15
entries:
  actions:
    - attack: melee
      proficient: true
      range: 10
      mod: str
      damage:
        - dieCount: 3
          dieType: 12
          mod: true
          type: piercing
      target: one
      id: bite
      name: Bite
    - attack: melee
      proficient: true
      range: 20
      mod: str
      damage:
        - dieCount: 4
          dieType: 10
          mod: true
          type: piercing
      target: one
      id: impale
      name: Impale
    - name: Multiattack
      text: The rachni queen makes one bite attack and two impale attacks.
      id: multiattack
cr: "18000"
---
### Lair Actions
On initiative count 20 (losing initiative ties), the rachni queen takes a lair action to cause one
of the following effects; it can't use the same effect two rounds in a row:

- The rachni queen summons 1d10 + 3 rachni workers. These arrive at the beginning of the queen's
next turn and take their turn on the queen's initiative.
- The rachni queen summons 1d6 + 1 rachni soldiers. These arrive at the beginning of the queen's next
turn and take their turn on the queen's initiative.
- The rachni queen summons one rachni brood warrior. It arrives at the beginning of the queen's next
turn and takes its turn on the queen's initiative.
