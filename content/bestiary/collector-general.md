---
name: Collector General
image: https://vignette.wikia.nocookie.net/masseffect/images/3/3c/Collectors_Leader_Character_Shot.png/revision/latest/scale-to-width-down/350?cb=20091119091650
type: organic
unit: collector
alignment: le
profBonus: 4
ac: 16
hp:
  dieCount: 25
  dieType: 10
abilityScores:
  str: 10
  dex: 12
  con: 12
  int: 14
  wis: 18
  cha: 16
irv:
  conImm:
    - charmed
senses:
  darkvision: 30
size: large
skills:
  - history
  - perception
  - science
  - persuasion
  - deception
speed:
  walk: 30
entries:
  features:
    - mod: wis
      casterLevel: "12"
      ref: power
      list:
        - dark-channel
        - pull
        - reave
        - shockwave
        - singularity
      id: powercasting
      name: Powercasting
      text: "The collector general is a 12th-level powercaster. Its powercasting ability is Wisdom (power save DC 16, +8 to hit with powers). The collector general has the following powers:"
    - name: Barrier
      text: The collector general has 20 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 3
          dieType: 8
          mod: true
          type: bludgeoning
      target: one
      id: bash
      name: Bash
  legendary:
    actions:
      - cost: 2
        id: assume-control
        name: Assume Control
        text: The harbinger targets a friendly collector that is not incapacitated. The target creature becomes possessed and gains the benefits listed on its monster sheet. The harbinger can only assume control of one creature at a time. While it is assuming control, its speed becomes 0, attacking creatures have advantage, it automatically fails Strength and Dexterity saving throws, and it cannot cast any powers. If the harbinger is incapacitated, assume control ends. The harbinger can use its bonus action to end assume control. As a result, the targeted creature loses all benefits including any temporary hit points and barrier ticks.
      - cost: 1
        id: bash-attack
        name: Bash Attack
        text: The collector general makes one bash attack.
      - cost: 3
        id: cast-a-power
        name: Cast a Power
        text: The collector general casts a power from its list of prepared powers, using a power slot as normal.
    text: The collector general can take 3 legendary actions, choosing from the options below. Only one legendary action can be used at a time and only at the end of another creature's turn. The collector general regains spent legendary actions at the start of its turn.
cr: "11000"
---
