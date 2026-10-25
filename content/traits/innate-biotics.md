---
name: Innate Biotics
species:
  - asari
  - ardat-yakshi
mechanics:
  - type: model-choice
    label: Choose two cantrips
    model: powers
    options: true
    limits:
      - attr: type
        value:
          - biotic
      - attr: level
        value:
          - 0
    selections: 2
    hide: true
    append:
      provider:
        model: species
        id: asari
      mod: wis
  - type: model-choice
    label: Choose one 1st level power
    model: powers
    options: true
    limits:
      - attr: type
        value:
          - biotic
      - attr: level
        value:
          - 1
    hide: true
    append:
      castAt: 1
      alwaysCastable: true
      provider:
        model: species
        id: asari
      mod: wis
      resource:
        id: innate-biotics
        label: "@ 1st Level / long rest"
---
You learn two biotic cantrips of your choice. In addition, choose one 1st-level biotic power of your choice.
You learn that power and can cast it at 1st-level level. Once you cast it, you must finish a long rest before you can
cast it again. Wisdom is your powercasting modifier for these powers.
