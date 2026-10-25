---
name: Blood Pack Pyro
image: https://vignette.wikia.nocookie.net/masseffect/images/e/ec/Blood_Pack_Pyro.png/revision/latest/scale-to-width-down/348?cb=20100621053224
type: organic
unit: blood_pack
alignment: ce
profBonus: 2
ac: 11
hp:
  dieCount: 6
  dieType: 8
abilityScores:
  str: 13
  dex: 11
  con: 13
  int: 4
  wis: 4
  cha: 6
irv:
  res:
    - poison
size: medium
speed:
  walk: 35
entries:
  actions:
    - attack: melee
      proficient: true
      range: 5
      mod: str
      damage:
        - dieCount: 1
          dieType: 6
          mod: true
          type: slashing
      target: one
      id: claws
      name: Claws
    - name: M-451 Firestorm
      text: Creatures within a :distance{length="15" adj} cone must make a DC 13 Dexterity saving throw. On a failed save, a creature takes 14 (4d6) fire damage, or half as much damage on a successful one.
      id: m-451-firestorm
  features:
    - name: Aggressive
      text: As a bonus action, the pyro can move up to its speed toward a hostile creature that it can see.
      id: aggressive
    - name: Regeneration
      text: The pyro regains 4 hit points at the start of its turn. If the pyro takes fire damage, this trait doesn't function at the start of the pyro's next turn. The pyro dies only if it starts its turn with 0 hit points and doesn't regenerate.
      id: regeneration
  reactions:
    - name: Fortification
      text: As a reaction to being hit by an attack the pyro can see, it gains a +5 bonus to its AC until the start of its next turn (including against the triggering attack).
      id: fortification
cr: "01000"
---
