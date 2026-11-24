---
name: Supply Pylon
level: 18
klass: engineer
subclass: medic
mechanics:
  - type: other
    resource:
      reset: long
    name: Supply Pylon
    range:
      short: 10
    dc:
      base: 8
      proficient: true
      mod: int
      save: dex
    damage:
      - dieCount: 4
        dieType: 8
        type: bludgeoning
    shortDesc: Call a supply pylon to a point within :distance{length="10"}; it lands at the start of your next turn. A creature in that spot makes a {{ dc }} Dexterity saving throw with advantage, or takes {{ roll }} and is knocked :condition{id="prone"}. It holds 5 resources you choose (restock with 5 omni-gel).
---
By 18th level, you can call in a :distance{length="5"} tall by :distance{length="2"} wide supply pylon to a location within :distance{length="10"}. At the start of your next turn, the pylon arrives. If any creature is
standing in the targeted location, the creature must make a Dexterity saving throw with advantage.
On a failed save, a creature takes 4d8 bludgeoning damage and is knocked prone.

The pylon contains 5 resources from the following list, which you choose when you call the pylon:

* 1 heavy weapon ammo charges
* 10 thermal clips
* A battery capable to quickly recharging your Omni-tool, recovering 5 tech points
* A stim pack capable of staving off biotic fatigue, recovering 5 levels worth of power slots
* 4 enhanced medi-gel
* 2 Mk II Frag grenades
* 2 Mk II Lift Grenades
* 2 Mk IV Flashbang
* 2 Mk IV Smoke grenades

Once the pylon has landed, friendly creatures (including you) within melee range of the pylon can use their action to collect
one of the resources you chose.

Once you use this feature, you cannot use it again until you finish a long rest and restock the pylon with 5 omni-gel.
