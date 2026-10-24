---
name: Abomination
image: https://vignette.wikia.nocookie.net/masseffect/images/8/8e/AbominationME3.jpg/revision/latest/scale-to-width-down/316?cb=20121201211954
type: synorg
unit: reaper
alignment: le
profBonus: 2
ac: 11
hp:
  dieCount: 4
  dieType: 8
abilityScores:
  str: 13
  dex: 8
  con: 14
  int: 3
  wis: 6
  cha: 5
savingThrows:
  - wis
senses:
  darkvision: 30
size: medium
speed:
  walk: 30
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      target: one
      id: grapple
      name: Grapple
      hit: The creature is grappled (escape DC 11). At the start of the abomination's next turn, it uses Post-Mortem Explosion
  features:
    - name: Aggressive
      text: As a bonus action, the abomination can move up to its speed toward a hostile creature that it can see.
      id: aggressive
    - name: Post-Mortem Explosion
      text: When the abomination dies, it explodes in a burst of necrotic energy. Each creature within :distance{length="5"} of it must succeed on a DC 14 Dexterity saving throw, taking 28 (8d6) necrotic damage on a failed save, or half as much damage on a successful one. A creature that is grappled by the abomination automatically fails its saving throw.
      id: post-mortem-explosion
cr: "01000"
---
