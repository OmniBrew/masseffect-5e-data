---
name: Harvester
image: https://vignette.wikia.nocookie.net/masseffect/images/9/92/ME2_Harvester.jpg/revision/latest/scale-to-width-down/200?cb=20100210004033
type: organic
unit: alien
alignment: u
profBonus: 6
ac: 16
hp:
  dieCount: 26
  dieType: 12
abilityScores:
  str: 26
  dex: 14
  con: 24
  int: 16
  wis: 15
  cha: 16
irv:
  conImm:
    - poisoned
  damImm:
    - poison
savingThrows:
  - str
  - con
  - wis
size: huge
skills:
  - perception
speed:
  walk: 60
  fly: 90
entries:
  actions:
    - attack: melee
      proficient: true
      range: 10
      mod: str
      damage:
        - dieCount: 2
          dieType: 6
          mod: true
          type: piercing
      target: one
      id: stomp
      name: Stomp
    - name: Multiattack
      text: "The harvester can use its Frightful Presence. It then makes three attacks: one with its acid spit and two with its stomp."
      id: multiattack
    - name: Acid Spit
      text: The harvester targets a :distance{length="15" adj} radius  within :distance{length="150"} and launches a glob of acid that coats the area.  Each creature within the area must succeed on a DC 19 Dexterity saving throw,  taking 44 (8d10) acid damage on a failed save, or half as much on a successful one.  Until the end of the harvester's next turn, each creature that enters the area or  ends its turn there must also make the saving throw.
      id: acid-spit
  legendary:
    actions:
      - cost: 1
        id: detect
        name: Detect
        text: The harvester makes a Wisdom (Perception) check.
      - cost: 1
        id: stomp-attack
        name: Stomp Attack
        text: The harvester makes a stomp attack.
      - cost: 2
        id: trample-attack
        name: Trample Attack
        text: The harvester moves :distance{length="30"} in a straight line, moving over Large or smaller creatures in its path. Each creature caught in its path must succeed on a DC 19 Dexterity saving throw or take 15 (2d6 + 8) piercing damage and be knocked :condition{id="prone"}. The harvester cannot move through a Huge or larger creature.
    text: The harvester can take 3 legendary actions, choosing from the options below. Only one legendary action can be used at a time and only at the end of another creature's turn. The harvester regains spent legendary actions at the start of its turn.
  features:
    - name: Frightful Presence
      text: Each creature of the harvester's choice that is within :distance{length="150"} of the harvester and aware of it must succeed on a DC 19 Wisdom saving throw or become :condition{id="frightened"} for 1 minute. A creature can repeat the saving throw at the end of each of its turns, ending the effect on itself on a success. If a creature's saving throw is successful or the effect ends for it, the creature is immune to the harvester's Frightful Presence for the next 24 hours.
      id: frightful-presence
    - name: Drop Klixen
      text: If the harvester is within a region that contains Klixen, it  begins the fight by dropping 1d10 Klixen in a :distance{length="15" adj} by :distance{length="50" adj} area.
      id: drop-klixen
cr: "19000"
---
