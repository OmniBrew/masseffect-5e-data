---
name: Twice as Bright
species:
  - salarian
mechanics:
  - type: skill-choice
    options: true
    selections: 2
  - type: tool-choice
    profType: tool
    options: true
    selections: 2
  - type: skill-check
    effect:
      type: die-bonus
      note: add a d4 to the roll
    valueLookup:
      model: traits
      id: twice-as-bright
      limit:
        - skill
        - tool
---
You gain proficiency in two skills of your choice and two tools or kits of your choice.  

Whenever you make an ability check with one of the chosen skills or tools from
Twice as Bright, roll a d4, and add the number rolled to the check’s total.
