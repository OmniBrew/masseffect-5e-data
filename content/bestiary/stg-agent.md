---
name: Salarian STG Agent
image: https://vignette.wikia.nocookie.net/masseffect/images/7/7c/STG_busybodies.png/revision/latest/scale-to-width-down/640?cb=20141208193957
type: organic
unit: archetype
alignment: ln
profBonus: 2
ac: 16
hp:
  dieCount: 12
  dieType: 8
abilityScores:
  str: 10
  dex: 16
  con: 11
  int: 15
  wis: 14
  cha: 12
savingThrows:
  - int
size: medium
skills:
  - stealth
  - survival
speed:
  walk: 30
entries:
  features:
    - mod: int
      ref: power
      list:
        - id: decoy
          perDay: 3
        - id: overload
          perDay: 5
          level: 2
      id: innate-powercasting
      name: Innate Powercasting
      text: "The salarian stg agent's innate powercasting ability is Intelligence (power save DC 12, +4 to hit with power attacks). It can innately cast the following powers:"
    - list:
        - id: flashbang-grenade
          mark: iii
          uses: 2
      id: grenades
      name: Grenades
      text: The salarian stg agent has the following grenades equipped. It can use a grenade as an action.
    - name: Surprise Attack
      text: If the agent surprises a creature and hits it with an attack during the first round of combat, the target takes an extra 10 (3d6) damage from the attack.
      id: surprise-attack
  actions:
    - ref: weapon
      proficient: true
      id: scorpion
      weaponId: scorpion
    - name: Multiattack
      text: The agent makes 2 attacks with its Scorpion.
      id: multiattack
    - name: Explosive Decoy
      text: As an action, the agent detonates its active Decoy. Each creature within :distance{length="10"} of the decoy must make a Dexterity saving throw. On a failed save, a creature takes 3d6 thunder damage or half as much on a successful one.
      id: explosive-decoy
cr: "03000"
shields:
  capacity: 10
  regen: 5
---
