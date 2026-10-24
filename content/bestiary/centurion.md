---
name: Centurion
image: https://vignette.wikia.nocookie.net/masseffect/images/3/3f/ME3_Cerberus_Centurion.png/revision/latest/scale-to-width-down/417?cb=20120322145316
type: organic
unit: cerberus
alignment: nn
profBonus: 2
ac: 14
hp:
  dieCount: 7
  dieType: 8
abilityScores:
  str: 14
  dex: 14
  con: 16
  int: 11
  wis: 9
  cha: 12
irv:
  res:
    - bludgeoning
    - piercing
    - slashing
senses:
  infrared-vision: 30
size: medium
speed:
  walk: 30
entries:
  features:
    - list:
        - id: frag-grenade
          mark: iii
          uses: 2
        - id: smoke
          mark: grenade
          uses: 2
      id: grenades
      name: Grenades
      text: The centurion has the following grenades equipped. It can use a grenade as an action.
    - name: Aggressive
      text: As a bonus action, the centurion can move up to its speed toward a hostile creature that it can see.
      id: aggressive
  actions:
    - ref: weapon
      proficient: true
      id: stun-baton
      weaponId: stun-baton
    - ref: weapon
      proficient: true
      id: m-96-mattock
      weaponId: m-96-mattock
    - name: Multiattack
      text: The centurion makes two M-96 Mattock attacks or two Stun Baton attacks.
      id: multiattack
cr: "04000"
shields:
  capacity: 10
  regen: 10
---
