---
name: Hologram
level: 3
klass: soldier
subclass: holo-operative
mechanics:
  - type: bonus-action
    name: Hologram
    shortDesc: Create a hologram of yourself within :distance{length="15"} (AC {{ 14 + profBonus }}, 1 hit point, immune to conditions and priming). It moves :distance{length="25"} on your turn (no action). Your attacks and aimed combat powers can come from its position, as lightning damage.
  - type: reaction
    name: Hologram Opportunity Attack
    shortDesc: "A creature moves through your hologram's threatened area: a melee attack from the hologram."
    attack:
      type: melee
      proficient: true
      bonus:
        type: modComparison
        value:
          - str
          - dex
    range:
      short: 5
    damage:
      - dieCount: 1
        dieType: 6
        type: lightning
        bonus:
          type: modComparison
          value:
            - str
            - dex
---
At 3rd level, you can create a lifelike hologram of yourself within :distance{length="15"} of your current
location as a bonus action. The hologram stays active until you dismiss it (no action required), it is hit or you try
and create another hologram. On your turn, you can command your hologram to move :distance{length="25"} in any
direction (no action required). If your hologram is more than :distance{length="25"} from you at the end
of your turn, it is automatically dismissed.

The hologram has an AC of 14+Your Proficiency Modifier, has 1 hit point, and is immune to all
conditions and priming. If it has to make a saving throw, it uses your modifiers for that saving throw.

- When you take the attack action on your turn, or cast a Combat Power that necessitates you aim or target
an area, you can make your attacks or draw that area from your hologram's position: the damage of the
attack turns to Lightning.

- When a creature moves through the Hologram's threatened area (all adjacent squares to it), you can use your reaction
to make an opportunity attack against the target. This attack deals 1d6+your strength or dexterity modifier Lightning
damage, and is considered a melee attack.
