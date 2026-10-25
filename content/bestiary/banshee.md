---
name: Banshee
image: https://vignette.wikia.nocookie.net/masseffect/images/e/eb/ME3_Banshee.png/revision/latest/scale-to-width-down/548?cb=20120319210941
type: synorg
unit: reaper
alignment: le
profBonus: 5
ac: 16
hp:
  dieCount: 30
  dieType: 10
abilityScores:
  str: 11
  dex: 16
  con: 11
  int: 12
  wis: 20
  cha: 18
savingThrows:
  - dex
  - wis
senses:
  darkvision: 30
size: large
speed:
  walk: 15
entries:
  features:
    - uses: 3
      perDay: true
      id: barrier
      name: Barrier
      text: As an action or bonus action, the banshee gains 20 barrier ticks. When the banshee is dealt damage, remove one barrier tick and reduce the damage by 1d8.
    - mod: wis
      list:
        - id: charge
          perDay: at_will
        - id: nova
          perDay: at_will
        - id: warp
          perDay: 6
          level: 4
      id: innate-powercasting
      name: Innate Powercasting
      text: "The banshee's innate powercasting ability is Wisdom (power save DC 18, +10 to hit with power attacks). It can innately cast the following powers:"
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 3
          dieType: 8
          mod: true
          type: piercing
      target: one
      id: impale
      name: Impale
    - recharge:
        - "5"
        - "6"
      id: wail
      name: Wail
      text: The banshee lets out a wail. Each creature within :distance{length="150"} that can hear the wail must make DC 17 Wisdom saving throw. On a failed save a creature is frightened for 1 minute.
  legendary:
    actions:
      - cost: 3
        id: cast-a-power
        name: Cast a Power
        text: The banshee casts a power from its list of prepared powers, using a power slot as normal.
      - cost: 1
        id: impale-attack
        name: Impale Attack
        text: The banshee uses its imaple attack.
      - cost: 2
        id: wail-attack
        name: Wail Attack
        text: The banshee uses its wail.
    text: The banshee can take 3 legendary actions, choosing from the options below. Only one legendary action can be used at a time and only at the end of another creature's turn. The banshee regains spent legendary actions at the start of its turn.
  reactions:
    - name: Teleporting Dodge
      text: In response to making a Dexterity saving throw, the banshee can use its reaction to teleport up to :distance{length="10"} away. If it is still within the affected area, it has advantage on the saving throw.
      id: teleporting-dodge
cr: "13000"
---
