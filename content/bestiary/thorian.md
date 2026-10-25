---
name: Thorian
image: https://vignette.wikia.nocookie.net/masseffect/images/8/8a/Thorian_charbox.png/revision/latest/scale-to-width-down/700?cb=20140409103930
type: organic
unit: thorian
alignment: le
profBonus: 2
ac: 19
hp:
  dieCount: 40
  dieType: 12
abilityScores:
  str: 15
  dex: 13
  con: 20
  int: 25
  wis: 26
  cha: 17
irv:
  conImm:
    - prone
    - lifted
  vul:
    - fire
size: huge
speed:
  walk: 0
entries:
  features:
    - name: Indoctrination
      text: Unless a thorian controller is incapacitated, it is a source of indoctrination to all creatures within 1[:distance{length="0"}] of it. See the indoctrination condition.
      id: indoctrination
    - name: Root Structure
      text: One a thorian reaches maturity, it's roots grow at a rate of :distance{length="5" num-only} to :distance{length="10"} per year. Over time, these roots create vast tunnel systems and caverns that act as the thorian's lair.
      id: root-structure
    - name: Neural Nodes
      text: The thorian has 4 + 1d4 neural nodes located along its root structure, spread throughout its lair. At start of its turn, the thorian gains 2d12 points for each remaining neural node. Each node has AC 10 and 30 (6d6 + 10) hit points.
      id: neural-nodes
  actions:
    - name: Indoctrinate
      text: The thorian targets one creature within :distance{length="300"} of it that it or one of its controllers, thralls, or creepers can see. That creature must make a DC 17 Wisdom saving throw or suffer a level of indoctrination.
      id: indoctrinate
    - name: Summon Thrall
      text: The thorian summons a thrall to its aid. It arrives on initiative count 20 somewhere along the thorian's root structure.
      id: summon-thrall
cr: "17000"
---
### Lair Actions
On initiative count 20 (losing initiative ties), the thorian takes a lair action to cause one of the 
following effects; it can't use the same effect two rounds in a row:

- The thorian sprouts 1d12 + 3 thorian spawn. These spawn can appear in an unoccupied space within 
:distance{length="5"} of any part of the thorian's root structure. The spawn take their turn at 
the end of the thorian's turn.
- The thorian summons 1d8 + 4 thorian creepers. These creepers can appear in an unoccupied space 
within :distance{length="5"} of any part of the thorian's root structure. The creepers take 
their turn at the end of the thorian's turn.
- The thorian summons 1d4 thorian controllers. These controllers can appear in an unoccupied space 
within :distance{length="5"} of any part of the thorian's root structure. The controllers take 
their turn at the end of the thorian's turn.
