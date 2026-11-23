---
name: Shock Cavalry
level: 3
klass: tracker
subclass: outrider
mechanics:
  - type: other
    name: Shock Cavalry
    dc:
      base: 8
      proficient: true
      mod: wis
      save: wis
    shortDesc: 'You or your beast hit a creature after moving at least :distance{length="20"}, from within :distance{length="15"} of it: it makes a {{ dc }} Wisdom saving throw or is :condition{id="frightened"} for 1 minute (it retries at the end of each of its turns).'
---
Disrupting the frontlines is your best tactic.

If you or your beast hit a creature with an attack after moving at least :distance{length="20"}, and the one
hitting the target is within :distance{length="15"} of the target, that creature must then make a Wisdom saving
throw against your Powercasting saving throw or become frightened for 1 minute. The creature can retry the saving
throw at the end of each of his turns, ending the effect on a success.
