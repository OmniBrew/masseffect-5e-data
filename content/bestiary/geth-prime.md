---
name: Geth Prime
image: https://vignette.wikia.nocookie.net/masseffect/images/c/c9/ME3_Geth_Prime.png/revision/latest/scale-to-width-down/229?cb=20120403192110
type: synthetic
unit: geth
alignment: ln
profBonus: 4
ac: 18
hp:
  dieCount: 20
  dieType: 10
abilityScores:
  str: 16
  dex: 18
  con: 16
  int: 14
  wis: 10
  cha: 10
irv:
  conImm:
    - poisoned
  damImm:
    - poison
    - psychic
savingThrows:
  - con
  - int
size: large
skills:
  - electronics
speed:
  walk: 30
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 10
          mod: true
          type: bludgeoning
      target: one
      id: weapon-bash
      name: Weapon Bash
    - ref: weapon
      proficient: true
      id: geth-pulse-rifle
      weaponId: geth-pulse-rifle
    - uses: 3
      perDay: true
      id: summon-combat-drone
      name: Summon Combat Drone
      text: The geth prime summons a Combat Drone. It can only have 1 Combat Drone active at a time.
    - uses: 1
      perDay: true
      id: summon-geth-turret
      name: Summon Geth Turret
      text: The geth prime summons a Geth Turret.
    - name: Multiattack
      text: The geth prime makes two Geth Pulse Rifle attacks.
      id: multiattack
    - name: Radar Jamming
      text: The geth prime releases an emp burst that temporarily disables targeting systems. Each hostile creature within a :distance{length="30"} radius has disadvantage on ranged weapon attack rolls until the start of the geth prime's next turn.
      id: radar-jamming
  legendary:
    actions:
      - cost: 2
        id: activate-radar-jamming
        name: Activate Radar Jamming
        text: The geth prime activates its radar jamming.
      - cost: 1
        id: geth-pulse-rifle-attack
        name: Geth Pulse Rifle Attack
        text: The geth prime makes a Geth Pulse Rifle attack.
      - cost: 3
        id: summon-turret-or-drone
        name: Summon Turret or Drone
        text: The geth prime uses its Summon Drone or Summon Geth Turret action.
    text: The geth prime can take 3 legendary actions, choosing from the options below. Only one legendary action can be used at a time and only at the end of another creature's turn. The geth prime regains spent legendary actions at the start of its turn.
cr: "09000"
shields:
  capacity: 30
  regen: 10
---
