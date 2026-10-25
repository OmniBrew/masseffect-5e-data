---
name: Atlas
image: https://vignette.wikia.nocookie.net/masseffect/images/1/16/ME3_Cerberus_Atlas.png/revision/latest/scale-to-width-down/700?cb=20120322140845
type: synthetic
unit: cerberus
alignment: nn
profBonus: 5
ac: 20
hp:
  dieCount: 14
  dieType: 10
abilityScores:
  str: 20
  dex: 10
  con: 20
  int: 18
  wis: 10
  cha: 9
irv:
  conImm:
    - blinded
    - deafened
    - grappled
    - paralyzed
    - poisoned
    - stunned
  damImm:
    - poison
    - psychic
  res:
    - bludgeoning
    - piercing
    - slashing
  vul:
    - lightning
savingThrows:
  - str
  - int
senses:
  darkvision: 30
size: large
speed:
  walk: 15
entries:
  features:
    - list:
        - id: smoke-grenade
          uses: 5
      id: grenades
      name: Grenades
      text: The atlas has the following grenades equipped. It can use a grenade as an action.
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
      id: smash
      name: Smash
    - attack: ranged
      proficient: true
      range: 300
      mod: dex
      damage:
        - dieCount: 5
          dieType: 8
          mod: true
          type: radiant
      target: one
      id: mass-accelerator-cannon
      name: Mass Accelerator Cannon
    - recharge:
        - "5"
        - "6"
      id: rocket-launcher
      name: Rocket Launcher
      text: The atlas targets an area within :distance{length="150"}. Each creature within :distance{length="15"} of the target must make a DC 18 Dexterity saving throw. On a failed save, a creature takes 52 (8d12) thunder damage or half as much damage on a successful one.
  legendary:
    actions:
      - cost: 3
        id: eject
        name: Eject
        text: The pilot of the Atlas ejects, landing in an unoccupied space within :distance{length="100"}. The pilot is an Assault Trooper. The Atlas then self-destructs. Each creature within a :distance{length="15" adj} radius must make a DC 18 Dexterity saving throw. On a failed save, a creature takes 39 (6d12) thunder damage or half as much on a successful one.
      - cost: 1
        id: mass-accelerator-cannon-attack
        name: Mass Accelerator Cannon Attack
        text: The atlas makes a Mass Accelerator Cannon attack.
      - cost: 1
        id: smash-attack
        name: Smash Attack
        text: The atlas makes a Smash attack.
    text: The atlas can take 3 legendary actions, choosing from the options below. Only one legendary action can be used at a time and only at the end of another creature's turn. The atlas regains spent legendary actions at the start of its turn.
cr: "14000"
shields:
  capacity: 50
  regen: 5
---
