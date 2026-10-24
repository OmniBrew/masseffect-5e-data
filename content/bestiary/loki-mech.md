---
name: LOKI Mech
image: https://vignette.wikia.nocookie.net/masseffect/images/c/c0/ME2_Loki_Mech.png/revision/latest?cb=20120917060158
type: synthetic
unit: mech
alignment: nn
profBonus: 2
ac: 10
hp:
  dieCount: 5
  dieType: 8
abilityScores:
  str: 10
  dex: 12
  con: 11
  int: 8
  wis: 6
  cha: 5
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
  vul:
    - lightning
senses:
  infrared-vision: 30
size: medium
skills:
  - perception
speed:
  walk: 25
entries:
  features:
    - mod: int
      list:
        - id: shocking-grasp
          perDay: 5
      id: innate-powercasting
      name: Innate Powercasting
      text: "The loki mech's innate powercasting ability is Intelligence (power save DC 9, +1 to hit with power attacks). It can innately cast the following powers:"
    - name: Chatter (variant)
      text: The LOKI mech can be programmed with pre-recorded phrases, which it utters occasionally during combat. Each hostile creature that hears the phrase must pass a Wisdom saving throw. On a failure, a creature becomes unnerved by the phrase and can only target the LOKI mech when making attack rolls or using damaging powers. On a success, a creature is unaffected and is immune to the LOKI mech's Chatter. The DC of the saving throw is dependant on the phrase, but cannot be higher than 12.
      id: chatter--variant-
    - name: Limited Tactics
      text: The LOKI mech is incapable of complex combat tactics. It never seeks cover and cannot take the Hide, Dodge, Help, or Disengage actions.
      id: limited-tactics
    - name: Post-mortem Explosion
      text: When the LOKI mech is reduced to 0 hit points, it self-destructs. Each creature within a :distance{length="5" adj}-radius sphere must succeed on a DC 10 Dexterity saving throw or take 5 (2d4) thunder damage.
      id: post-mortem-explosion
  actions:
    - ref: weapon
      proficient: true
      id: m-4-shuriken
      weaponId: m-4-shuriken
    - ref: weapon
      proficient: true
      id: m-3-predator
      weaponId: m-3-predator
cr: "00125"
---
