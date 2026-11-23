---
name: True Devotion
level: 17
klass: infiltrator
subclass: devotee-of-the-old-ways
mechanics:
  - type: other
    name: True Devotion
    shortDesc: "During a long rest, attune to either Kalahira, Arashu, or Amonkira. You cannot attune to a single god twice in a row: you need to change the god you are attuned to during your long rests."
    toggle:
      id: devotee-true-devotion
      whenOn:
        - type: resource
          id: devotee-true-devotion-resource
          method: add
          value:
            type: flat
            value: 1
      options:
        - id: devotee-true-devotion-kalahira
          name: Kalahira
          whenOn:
            - type: other
              name: Kalahira Devotion
              damage:
                - dieCount: 1
                  dieType: 4
                  mod: wis
                  type: shields
              shortDesc: 'An enemy within :distance{length="50"} dies: regain {{ roll }} points (temporary hit points until your next short rest if your shields are full).'
        - id: devotee-true-devotion-arashu
          name: Arashu
          whenOn:
            - type: ac
              bonus:
                type: mod
                value: wis
        - id: devotee-true-devotion-amonkira
          name: Amonkira
          whenOn:
            - type: global-note
              subType: action
              value: Amonkira Devotion
              moreInfo:
                model: class-features
                id: true-devotion
    resource:
      id: devotee-true-devotion-resource
---
At 17th level, you are truly devoted to your gods. Choose one god to attune per Long Rest. Each god provides you
one of these major benefits:

__Kalahira__: When an enemy within :distance{length="50"} of you dies, you regain 1d4 + Wisdom modifier shield points.
If your shields are already full, you instead gain that many Temporary Hit Points that last until your next short rest.

__Arashu__: You add your Wisdom bonus to your AC.

__Amonkira__: When you roll an attack with advantage, you may reroll one of the die once.

You cannot attune to a single god twice in a row: you need to change the god you are attuned to during your long rests.
