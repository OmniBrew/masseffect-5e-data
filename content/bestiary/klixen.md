---
name: Klixen
image: https://vignette.wikia.nocookie.net/masseffect/images/2/2f/ME2_Klixen.PNG/revision/latest/scale-to-width-down/350?cb=20100703065034
type: organic
unit: alien
alignment: u
profBonus: 2
ac: 14
hp:
  dieCount: 5
  dieType: 8
abilityScores:
  str: 12
  dex: 14
  con: 12
  int: 5
  wis: 10
  cha: 7
irv:
  conImm:
    - poisoned
  damImm:
    - fire
    - poison
  vul:
    - cold
size: medium
speed:
  walk: 30
entries:
  actions:
    - recharge:
        - "6"
      id: fire-breath
      name: Fire Breath
      text: The klixen exhales a 6-meter cone of fire. Each creature in that area must make a DC 14 Dexterity saving throw, taking 10 (3d6) fire damage on a failed save, or half as much damage on a successful one.
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 4
          mod: true
          type: piercing
        - dieCount: 1
          dieType: 4
          mod: true
          type: fire
      target: one
      id: pincer
      name: Pincer
  features:
    - name: Death Burst
      text: When the klixen dies, it explodes in a burst of lava. Each creature within :distance{length="5"} of it must make a DC 14 Dexterity saving throw, taking 10 (3d6) fire damage on a failed save, or half as much damage on a successful one.
      id: death-burst
    - name: Heated Body
      text: A creature that touches the klixen or hits it with a melee attack while within :distance{length="5"} of it takes 3 (1d6) fire damage.
      id: heated-body
cr: "01000"
---
