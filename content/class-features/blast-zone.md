---
name: Blast Zone
level: 10
klass: adept
subclass: fury
mechanics:
  - type: immunity
    id: detonations
    label: Detonations you trigger
  - type: reaction
    name: Blast Zone
    shortDesc: Add your Wisdom modifier to a detonation you triggered with a power you Furycast.
  - type: augment
    value:
      model: adept
      id: furycasting
    merge:
      moreInfo:
        additional:
          - {}
          - model: class-features
            id: blast-zone
---
At 10th level, you are immune to the effects of detonations you trigger. In addition, you may spend your reaction to
add your Wisdom modifier to a detonation you triggered via a power you Furycast.
