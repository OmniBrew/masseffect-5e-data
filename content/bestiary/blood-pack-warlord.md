---
name: Blood Pack Warlord
image: https://vignette.wikia.nocookie.net/masseffect/images/b/b6/ME3_Krogan_Warlord_Sentinel.png/revision/latest/scale-to-width-down/240?cb=20130227103010
type: organic
unit: blood_pack
alignment: ce
profBonus: 3
ac: 18
hp:
  dieCount: 8
  dieType: 8
abilityScores:
  str: 18
  dex: 15
  con: 22
  int: 11
  wis: 14
  cha: 12
irv:
  res:
    - necrotic
savingThrows:
  - con
  - str
size: medium
skills:
  - athletics
speed:
  walk: 25
entries:
  features:
    - uses: 1
      perDay: true
      id: tech-armor
      name: Tech Armor
      text: As a bonus action, the warlord can activate its Tech Armor. It immediately gains 30 temporary hit points. While the warlord has at least 1 of these temporary hit points remaining, it has +2 AC and resistance to bludgeoning, piercing, and slashing damage.
    - recharge: short
      id: rage
      name: Rage
      text: If the warlord begins its turn with less than half of its hit points, it enters into a rage for 1 minute. While in a rage, all melee weapon attacks deal 5 additional bludgeoning damage.
    - recharge:
        - "5"
        - "6"
      id: biotic-hammer
      name: Biotic Hammer
      text: Before making an attack with its Krogan Warhammer, the warlord can charge the weapon with biotic force. On a hit, the attack deals an additional 9 (2d8) force damage and detonates the target if it was primed.
    - recharge:
        - "5"
        - "6"
      id: electrical-hammer
      name: Electrical Hammer
      text: Before making an attack with its Krogan Warhammer, the warlord can charge the weapon with electricity. On a hit, the attack deals an additional 7 (2d6) lightning damage and the target must succeed on a DC 15 Constitution saving throw or become stunned until the end of its next turn.
    - name: Aggressive
      text: As a bonus action, the warlord can move up to its speed toward a hostile creature that it can see.
      id: aggressive
  actions:
    - ref: weapon
      proficient: true
      id: krogan-warhammer
      weaponId: krogan-warhammer
    - ref: weapon
      proficient: true
      id: m-300-claymore
      weaponId: m-300-claymore
cr: "05000"
---
