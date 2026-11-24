---
name: Injection
level: 9
klass: infiltrator
subclass: poisoner
mechanics:
  - type: bonus-action
    name: Injection
    resource:
      max:
        type: proficiency
    shortDesc: "If you haven't used your Sneak Attack this round, use your Cunning Action to fire a dart of poison at an enemy within :distance{length=\"30\"}: {{ roll }}, and a Toxin if you choose. Targets hit have disadvantage on saving throws against Toxin effects."
    range:
      short: 30
    damage:
      - dieCount:
          type: progressive
          limit: infiltrator
          value:
            1: 1
            3: 2
            5: 3
            7: 4
            9: 5
            11: 6
            13: 7
            15: 8
            17: 9
            19: 10
        dieType: 6
        type: poison
---
At 9th level, instead of striking with your Sneak Attack, you can use your poisons by themselves. If you haven't used
your Sneak Attack this round, you can use your Cunning Action to fire off a dart of poison towards an enemy within
30 feet. This dart deals damage equal to your sneak attack damage, is Poison damage, and applies a Toxin
if you so chose. Targets hit by Injection have disadvantage on any saving throws against Toxin effects.

You can use this feature a number of times equal to your Proficiency bonus per long rest.
