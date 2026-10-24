---
name: Come Get Me
mechanics:
  - type: asi
    ability: cha
    amount: 1
  - type: action
    resource:
      reset: short
    range:
      short: 0
      aoe:
        type: sphere
        size: 20
    dc:
      base: 8
      proficient: true
      mod: cha
      save: wis
    shortDesc: Each creature of your choice within :distance{length="20" abbr} must succeed on a DC {{ dc }} WIS saving throw or suffer disadvantage on attack rolls against creatures other than you until it makes an attack against you.
new: true
note: Draw the enemy fire.
---
Conventional wisdom in combat is to avoid being targeted. You prefer an alternate school of thought, keeping enemies
focused on you and off of your less stalwart allies.

Increase your Charisma score by 1, to a maximum of 20.

As an action, you can make a feint to draw enemy attention. This feint may be a war cry, a loud insult, or a different
distraction. All enemies within :distance{length="20"} must make a Wisdom saving throw (DC 8 + your proficiency bonus + your Charisma modifier).
On a successful saving throw, a target is unaffected and is immune to this effect for the next 24 hours. On a failed
saving throw, an enemy has disadvantage on attacking any creature except you for the next minute, or until
they make an attack against you. You may use this ability once per short or long rest.
