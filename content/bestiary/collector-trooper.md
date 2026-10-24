---
name: Collector Trooper
image: https://vignette.wikia.nocookie.net/masseffect/images/d/d3/Collector_TrooperME3.jpg/revision/latest/scale-to-width-down/350?cb=20121201212208
type: organic
unit: collector
alignment: le
profBonus: 2
ac: 15
hp:
  dieCount: 14
  dieType: 8
abilityScores:
  str: 13
  dex: 14
  con: 12
  int: 11
  wis: 12
  cha: 8
savingThrows:
  - dex
senses:
  darkvision: 30
size: medium
skills:
  - athletics
speed:
  walk: 30
  fly: 15
entries:
  features:
    - list:
        - id: frag-grenade
          mark: iii
          uses: 2
      id: grenades
      name: Grenades
      text: The collector trooper has the following grenades equipped. It can use a grenade as an action.
    - name: Barrier
      text: The collector trooper has 2 barrier ticks. When it is dealt damage, remove one barrier tick and reduce the damage by 1d8.
      id: barrier
    - name: Possessed Collector
      text: When the collector trooper is possessed by a harbinger it gains temporary hit points equal to its total hit points and 6 barrier ticks. While it has barrier ticks it also gains resistance to bludgeoning, piercing, and slashing damage.
      id: possessed-collector
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 2
          dieType: 6
          mod: true
          type: slashing
      target: one
      id: claw
      name: Claw
    - ref: weapon
      proficient: true
      id: collector-smg
      weaponId: collector-smg
    - attack: ranged
      proficient: true
      range: 25
      mod: dex
      target: one
      id: collector-web
      name: Collector Web
      hit: The target is restrained by organic webbing. As an action, the restrained target  can make a DC 14 Strength check, bursting the webbing on a success. The webbing  can also be attacked and destroyed (AC 10; hp 5; vulnerability to fire damage;  immunity to bludgeoning, poison, and psychic damage).
cr: "03000"
---
