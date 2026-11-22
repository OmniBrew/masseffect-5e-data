---
name: Mountains
mechanics:
  - type: speed-bonus
    value:
      - climb
    ifExists:
      bonus:
        type: flat
        value: 10
    else:
      bonus:
        type: speed
        value: walk
type: tracker-affinity
---
You gain a climbing speed equal to your walking speed. If you already have a climbing speed, increase it by :distance{length="10"}.
