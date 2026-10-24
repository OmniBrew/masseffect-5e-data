---
name: Rampart Mech
image: https://vignette.wikia.nocookie.net/masseffect/images/6/60/ME3-Rampart-Mech.png/revision/latest/scale-to-width-down/287?cb=20121128090615
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 15
hp:
  dieCount: 15
  dieType: 8
abilityScores:
  str: 16
  dex: 15
  con: 8
  int: 16
  wis: 11
  cha: 8
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  vul:
    - lightning
size: medium
speed:
  walk: 30
entries:
  features:
    - uses: 1
      perDay: true
      id: hex-shield
      name: Hex Shield
      text: As a bonus action, the rampart mech generates a :distance{length="5"} tall and wide, hexagon-shaped shield with 5AC and 50 shield points which offers full-cover.
    - uses: 1
      perDay: true
      id: tactical-cloak
      name: Tactical Cloak
      text: As a bonus action, the rampart mech activates its tactical cloak, becoming invisible for 1 minute. When the rampart mech makes a melee or ranged attack or uses a tech or combat power, tactical cloak ends.
    - name: Aggressive
      text: As a bonus action, the rampart mech can move up to its speed toward a hostile creature that it can see.
      id: aggressive
    - name: Post-Mortem Vent
      text: When the rampart mech dies, it vents excess heat from its weapon and armor in a :distance{length="5"} radius until the start of its next turn. Each creature that enters the radius for the first time or ends its turn there takes 18 (4d8) radiant damage.
      id: post-mortem-vent
  actions:
    - ref: weapon
      proficient: true
      id: omni-blade
      weaponId: omni-blade
    - ref: weapon
      proficient: true
      id: m-23-katana
      weaponId: m-23-katana
    - name: Multiattack
      text: The rampart mech makes two omni-blade attacks.
      id: multiattack
cr: "02000"
---
