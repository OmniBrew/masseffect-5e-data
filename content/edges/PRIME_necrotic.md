---
name: Necrotic
type: primers
mechanics:
  - type: me:primer-detonation
    levels:
      - 1
      - 5
      - 11
      - 17
    tiers:
      - damage:
          - dieCount: 1
            dieType: 12
            type: necrotic
        dc:
          base: 13
          save: con
        shortDesc: Detonated creature suffers {{ damage }} damage and must succeed on a DC 13 Constitution saving throw or
          becomes <me-condition id="stunned" /> until the end of its next turn.
      - damage:
          - dieCount: 2
      - damage:
          - dieCount: 3
      - damage:
          - dieCount: 4
---
When a creature that is primed: necrotic detonates, it suffers 1d12 necrotic damage and must succeed on a
DC 13 Constitution saving throw or becomes <me-condition id="stunned" /> until the end of its next turn.
