---
name: Combat Blink
level: 6
klass: adept
subclass: fury
mechanics:
  - type: augment
    value:
      model: adept
      id: furycasting
    merge:
      moreInfo:
        additional:
          - model: class-features
            id: combat-blink
---
At 6th level, when you Furycast a power, your movement speed increases by :distance{length="15"}, and this
extra movement does not provoke attacks of opportunity.
