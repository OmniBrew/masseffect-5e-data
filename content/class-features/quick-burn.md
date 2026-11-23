---
name: Quick Burn
level: 10
klass: soldier
subclass: armiger
mechanics:
  - type: bonus-action
    name: Quick Burn
    shortDesc: Spend fuel to cast Havoc Strike as a bonus action. The number of Fuel spent is equal to the number of damage dice that Havoc Strike deals
    resource:
      reset: short
      id: armiger-fuel
      max:
        type: resource
        value: armiger-fuel
        useMax: true
---
At 10th level, you can spend fuel to cast Havoc Strike as a bonus action. The number of Fuel spent is equal to the number of damage dice that Havoc Strike deals
