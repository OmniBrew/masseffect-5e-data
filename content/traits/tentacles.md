---
name: Tentacles
species:
  - hanar
mechanics:
  - type: natural-weapon
    replacesUnarmedStrike: true
    value:
      damageModOverride: noMod
      name: Tentacles
      type: natural-melee
      range:
        short: 5
      damage:
        dieCount: 1
        dieType: 8
        type: poison
      notes:
        - On a hit, DC {{ 8 + profBonus + conMod }} or poisoned for 1 minute
        - +1 to attack roll and DC for each additional tentacle used
      moreInfo:
        model: traits
        id: tentacles
---
You have six tentacles instead of arms that can grip tightly but can't lift anything heavier than a few kilograms.
You can only wield weapons with the _light_ property.

In addition, your tentacles are natural weapons, which you can use to make unarmed strikes. When you attack
with multiple tentacles simultaneously, gain a +1 bonus to the attack roll for each additional tentacle used.

When you hit with your tentacles, you deal 1d8 poison damage and the target must succeed on a
Constitution saving throw or become poisoned for one minute. The DC of this saving throw is equal to
10 + your proficiency bonus + the number of tentacles used on this attack.
