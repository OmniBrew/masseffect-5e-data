# Mass Effect 5e content

The rules content for Mass Effect 5e: classes, species, powers, gear, the bestiary, the
player's manual and more. One markdown file per record, checked automatically on every pull
request.

> **The live site doesn't read this repo yet.** n7.world still uses the old data at
> [queryluke/masseffect-5e-data](https://github.com/queryluke/masseffect-5e-data) (data.n7.world),
> which is frozen. Edits made here appear on the new site, which is being built in
> [OmniBrew/omnibrew](https://github.com/OmniBrew/omnibrew).

- [How to edit](#how-to-edit)
- [The file format](#the-file-format)
- [Content types, with an example of each](#content-types)
- [Checking your changes](#checking-your-changes)
- [Pull requests](#pull-requests)

## How to edit

**In the browser (no setup):** open the file on GitHub, click the pencil icon, make the change,
then choose **Create a new branch … and start a pull request**. The checks run on their own; see
[Pull requests](#pull-requests).

**On your computer:** clone the repo, create a branch, edit with any text editor (VS Code shows
YAML mistakes as you type), then push and open a pull request. To run the checks yourself first,
see [Checking your changes](#checking-your-changes).

Finding a record: every record is `content/<type>/<id>.md`. The id is the file name, and it is
what other records use to point at it (`klass: adept`, `weaponId: m-3-predator`). **Don't rename
files** unless you also update every record that points at them; the checks will list any you miss.

## The file format

```
content/<type>/<id>.md    one record per file (the folder is the content type)
content/navigation/       tables of contents for the manual (manual.yml) and the guides (guide.yml)
content/site/about.yml    the About page's team list
messages/en.yml           text used by the site itself (buttons, headings, page intros)
images/                   images the content links to (served from data.n7.world today)
OGL.md                    the Open Game License that covers the 5e rules text
```

Each record is a markdown file with YAML **front-matter** (the fields, between two `---` lines)
and a markdown **body** (the description):

```md
---
name: Search
type: action
---
When you take the Search action, you devote your attention to finding something.
```

YAML tips:
- Indent with two spaces, never tabs. A list item starts with `- `.
- Put text in quotes if it starts with a special character (`*`, `-`, `:`, `#`, `{`, `[`, `@`, `` ` ``)
  or holds `: ` or ` #`: `text: "#1 fan"`.
- Leave a field out rather than writing `false`, `null` or an empty value for "none". The checks
  report `image: null` and `set: false` as errors. (`andromeda: false` is fine: it's a yes/no field.)
- Long text can go on one line; for several paragraphs use `|-` and indent the lines:
  ```yaml
  text: |-
    First paragraph.

    Second paragraph.
  ```

### Prose: markdown plus a few components

Bodies and text fields (`shortDesc`, `text`, `notes`…) are markdown. A few **components** cover
what plain markdown can't: distances that switch between feet and meters, condition links and so
on. They are written in [MDC](https://content.nuxt.com/docs/files/markdown) syntax, not HTML or Vue
tags:

| Write | Shows | Notes |
|---|---|---|
| `:distance{length="30"}` | 12 meters / 30 feet | Always in **feet**. Add `adj` (12-meter), `abbr` (12m), `num-only` (12), `large` (miles), `tiny` (inches), `override="extra {metric}"` |
| `:weight{amount="55"}` | 25 kilograms / 55 pounds | Always in **pounds**; same options as distance |
| `:condition{id="primed" sub="fire"}` | primed: fire | `id` must be a file in `content/conditions/`; `label="…"` replaces the text |
| `:change-badge{type="new"}` | a "new" badge | In manual headings; `type="change"` for changed rules |
| `:icon{name="ic:baseline-filter-center-focus"}` | an icon | Any [Iconify](https://icones.js.org) icon |
| `::note` … `::` | a call-out box | GM advice, examples, optional rules |
| `::figure{max-width="300"}` … `::` | a framed image | Wrap a markdown image |
| `::source-reference{source="basic" pages="39"}` then `::` | "text adapted from …" | Sources: `srd`, `basic`, `races`, `wiki` (for `wiki`, `pages` is the article name) |
| `::edge-list{type="commands"}` then `::` | every edge of that type | `type` is an edge family |

Inline components (one colon) need a space or a line start before them: write
`range 60/[:distance{length="100" abbr}]` (square brackets) when they follow other characters, or
they show up as plain text. Block components (two colons) sit on their own lines, closed by a line
with just `::`:

```md
::note
Because thermal clips are so easily attainable, GMs might not track them at all.
::
```

`{{ damage }}`, `{{ dc }}` and similar in a mechanic's text are filled in by the character sheet.

### Mechanics

Most records have a `mechanics:` list: the rules the character sheet applies (ability score
increases, resistances, actions, shields…). Each entry has a `type`. Core 5e types have plain
names (`asi`, `resistance`, `skill`); Mass Effect types start with `me:` (`me:shields`,
`me:barrier`, `me:grenade-capacity`). The full lists, with the fields each one takes, are in the
engine: [core](https://github.com/OmniBrew/omnibrew/blob/main/packages/engine/schemas/mechanics/core.ts)
and [Mass Effect](https://github.com/OmniBrew/omnibrew/blob/main/apps/me5e/game/mechanics.ts).
Copying a mechanic from a similar record is usually the quickest start; the checks tell you if a
field is wrong or missing.

## Content types

Each example is a real record, sometimes shortened (`# …`).

<details><summary><b>actions</b>: actions anyone can take in combat</summary>

```md
---
name: Search
type: action        # action, bonus_action or reaction
---
When you take the Search action, you devote your attention to finding something.
```
</details>

<details><summary><b>armor</b>: body armor (a suit) and armor pieces (head, chest, arms, legs)</summary>

```md
---
name: Andromeda Elite Helmet
coverage: piece     # piece (needs a slot) or suit
slot: head          # head, chest, arms or legs
armorType: light    # light, medium or heavy
cost: 62050
manufacturer: andromeda-initiative
rarity: rare
tags:
  - ac
  - shields
set: initiative     # optional: a set-bonuses id
flavor: This special-issue Andromeda Initiative helmet is custom designed for explorers…
mechanics:
  - type: ac
    bonus:
      type: flat
      value: 2
  - type: me:shields
    capacity:
      type: flat
      value: 5
---
- +2 AC.
```
</details>

<details><summary><b>attributions</b>: credits for artwork</summary>

```md
---
title: Prothean
path: https://data.n7.world/images/species/prothean.png
attribution: Prothean by JTickner
source: https://data.n7.world/images/species/prothean.png
---
```
</details>

<details><summary><b>backgrounds</b></summary>

```md
---
name: Urchin
startingCredits: 1000
mechanics:
  - type: tool
    value: thieves-tools
  - type: skill
    value: stealth
---
__Skill Proficiencies__. Sleight of Hand, Stealth
```
</details>

<details><summary><b>bestiary</b>: NPCs and creatures</summary>

```md
---
name: Geth Trooper
type: synthetic       # organic, synthetic, synorg or organic_or_synthetic
unit: geth
alignment: ln
size: medium
cr: "02000"
profBonus: 2
ac: 13
hp:
  dieCount: 16
  dieType: 8
abilityScores: { str: 12, dex: 14, con: 11, int: 12, wis: 8, cha: 8 }
speed:
  walk: 30
irv:                  # immunities, resistances, vulnerabilities
  conImm: [poisoned]
  damImm: [poison, psychic]
  vul: [lightning]
entries:
  actions:
    - id: geth-pulse-rifle
      ref: weapon
      weaponId: geth-pulse-rifle
      proficient: true
    - id: multiattack
      name: Multiattack
      text: The geth trooper makes two Geth Pulse Rifle attacks.
---
```
</details>

<details><summary><b>changelog</b>: release notes</summary>

```md
---
title: v0.4.1 - Minor changes
description: Minor adjustments to Mass Effect 5e version 0.4.0
date: 2017-01-09
---
* Starting credits reduced.
```
</details>

<details><summary><b>character-progression</b>: XP and proficiency bonus by level (one file per level)</summary>

```md
---
level: 1
xp: 0
profBonus: 2
---
```
</details>

<details><summary><b>class-features</b></summary>

```md
---
name: Indomitable (2)
klass: soldier
level: 13
subclass: gladiator   # only for subclass features
mechanics: []         # optional
---
At 13th level, you can use Indomitable twice between long rests.
```
</details>

<details><summary><b>classes</b></summary>

```md
---
name: Experiment
hitDie: 12
primaryAbility: [con]
profs:
  armor: { has: [light], text: Light Armor }
  weapon:
    has: [heavy_pistol, melee]
    choices: { items: [assault_rifle, shotgun], count: 1 }
    text: Heavy Pistols, Melee and choose one between Assault Rifles and Shotguns
  skill:
    choices: { items: [acrobatics, athletics, insight], count: 3 }
    text: Choose three from …
  saving-throw: { has: [con, int], text: Constitution }
startingEquipment:
  - choices: { items: [omni-blade, monomolecular-blade, riot-shield], count: 1 }
    text: (a) Monomolecular Blade (b) Omni-Blade or (c) Riot Shield
progression:
  subclass: [1, 2, 6, 10, 14]
  abi: [4, 8, 12, 16, 19]
  # columns: the class table's other columns (powers known, slots…)
---
```
</details>

<details><summary><b>conditions</b></summary>

```md
---
name: Incapacitated
---
* An incapacitated creature can't take actions or reactions.
```
</details>

<details><summary><b>edges</b>: choices a feature offers (subgrounds, maneuvers, primers…)</summary>

```md
---
name: Cook
type: subgrounds      # the edge family
mechanics:
  - type: tool
    value: cooks-utensils
---
```
</details>

<details><summary><b>feats</b></summary>

```md
---
name: Savage Attacker
note: Reroll damage dice for melee weapon attacks
mechanics: []
---
Player's Handbook, p. 169
```
</details>

<details><summary><b>gear</b></summary>

```md
---
name: Disguise Kit
gearType: tool        # ammo, device, grenade, heavy_weapon, medi_gel, omni_gel, omni_tool_program, shield or tool
rarity: common
cost: 2500
weight: 3
---
A pouch of cosmetics, dyes, and a micro-fabricator.
```
</details>

<details><summary><b>guide</b> and <b>manual</b>: pages of the guides and the player's manual</summary>

```md
---
title: Monster Types
---
There are only three monster types: __Organic__, __Synthetic__, and __Synth-organic__.
```

A new page also needs an entry in `content/navigation/manual.yml` (or `guide.yml`), or the site
never links to it:

```yaml
chapters:
  - id: equipment
    title: manual.equipment    # a key in messages/en.yml
    sections:
      - id: armor              # the page's file name
        is_new: false
        is_change: true
```
</details>

<details><summary><b>mods</b>: weapon and armor mods</summary>

```md
---
name: Power Magnifier
modType: weapon       # weapon or armor
placement: body
availability: [heavy_pistol, smg]
rarity: uncommon
cost: 12000
tags: [extra_damage]
flavor: Generator designed to enhance the effectiveness of tech or biotic attacks.
---
+1 on power damage rolls while holding this weapon.
```
</details>

<details><summary><b>npc-stats</b>: NPC statistics by challenge rating</summary>

```md
---
cr: "0"
normalized: 1
profBonus: 2
ac: 12
hp: 3
attack: 2
damage: 1
dc: 9
save: 1
xp: 10
---
```
</details>

<details><summary><b>powers</b></summary>

The first `casting` entry is the whole power; each later one is the power cast one level higher,
and lists only what changes.

```md
---
name: Charge
level: 0
powerType: biotic     # biotic, combat or tech
classes: [vanguard]
tags: [damage, movement]
version: 1
casting:
  - castingTime: { length: 1, unit: action }
    duration: { length: 0, unit: instant }
    concentration: false
    range: { short: 40 }
    dc: { save: dex }
    damage:
      - { dieCount: 1, dieType: 10, type: force }
    detonates: true
  - damage:
      - dieCount: 2   # 2d10 when cast one level higher
advancements:
  - id: area-charge
    name: Area Charge
    text: Each creature within :distance{length="10"} of the target must make the Dexterity saving throw.
    casting:
      - range: { aoe: { type: sphere, size: 10 } }
---
Choose a creature or object within range… and becomes :condition{id="prone"}.
```
</details>

<details><summary><b>set-bonuses</b>: armor set bonuses</summary>

```md
---
name: Heleus
max: 2
bonuses:
  - threshold: 2
    text: +3 AC
    mechanics:
      - type: ac
        bonus: { type: flat, value: 3 }
---
```
</details>

<details><summary><b>ship-upgrades</b></summary>

```md
---
name: Heavy Ship Armor I
cost: "300000"
prerequisite: "-"
system: "-"
---
+1 AC
```
</details>

<details><summary><b>skills</b></summary>

```md
---
name: Athletics
link: str             # the ability the skill uses
---
Your Strength (Athletics) check covers difficult situations you encounter while climbing…
```
</details>

<details><summary><b>species</b>, <b>subspecies</b> and <b>traits</b></summary>

```md
---
name: Asari
galaxy: milky_way
group: primary
subspecies: lifestage
mechanics:
  - type: asi
    ability: wis
    amount: 1
  - type: speed
    speed: walk
    distance: 30
size: Asari have builds incredibly similar to female humans. Your size is Medium.
# …
---
```

A variant or subspecies points at its parent: `species: vorcha` with `type: subspecies` or
`type: variant`. A trait lists the species that have it:

```md
---
name: Amphibious
species: [hanar, salarian, lystheni]
mechanics: []
---
Can breathe both air and water.
```
</details>

<details><summary><b>subclasses</b></summary>

```md
---
name: Beast Master
klass: tracker
author: Helios
---
```
</details>

<details><summary><b>tool-profs</b></summary>

```md
---
name: Starship System (Weapons)
type: starship        # artisan or starship; leave out for other tools
---
Represents your ability to target and attack moving objects through space…
```
</details>

<details><summary><b>vehicles</b></summary>

```md
---
name: ET3
type: transport
subtype: land
size: large
ac: 16
hp: 150
sp: 0
speed: 4
crew: { min: 1, max: 8 }
cargo: 2
range: { distance: 500, units: km }
systems:
  - type: Helm
    crew: 1
---
The ET3 is a civilian vehicle.
```
</details>

<details><summary><b>weapon-properties</b></summary>

```md
---
name: Heat
is_new: true
takesValue: true      # optional: weapons must then give it a value ({ id: heat, value: 9 })
---
The number of times a weapon can be fired before it must be reloaded.
```
</details>

<details><summary><b>weapons</b></summary>

```md
---
name: M-8 Avenger
weaponType: assault_rifle   # assault_rifle, heavy_pistol, melee, shotgun, smg or sniper_rifle
rarity: common
cost: 7500
manufacturer: elkoss-combine
weight: 7
damage: { dieCount: 1, dieType: 8, type: piercing }
range: { short: 60, long: 180 }
properties:
  - id: burst-fire
  - id: two-handed
  - id: heat
    value: 9
slots: 2
---
```
</details>

<details><summary><b>messages/en.yml</b>: the site's own text</summary>

Grouped by page or topic. `{level}` placeholders are filled in by the site, and `a | b` gives
the singular and plural forms:

```yaml
homepage:
  title: Mass Effect + D&D 5th Edition
abi_feature:
  at_level: When you reach {level}, | When you reach {level}, and again at {and_list} level,
```
</details>

## Checking your changes

Every pull request runs the checks (the **Validate content** workflow) and shows a red ✗ with
the problems if anything is wrong: a misspelled field, an id that doesn't exist, a mechanic with
a missing value, a component MDC can't read. Click **Details** next to the check to read them.

To run the same checks on your computer, you need [Node.js 24](https://nodejs.org) and the
engine repo next to this one:

```sh
git clone https://github.com/OmniBrew/omnibrew.git
cd omnibrew
corepack pnpm install --ignore-scripts
corepack pnpm validate:me5e --content ../masseffect-5e-data
```

Use the path of your checkout of this repo after `--content`. Add `--format md --out report.md`
for a full report; `--fail-on none` lists everything without failing.

## Pull requests

1. Make your change on a branch (the GitHub editor creates one for you).
2. Open a pull request against `master` and say what changed and why.
3. Wait for the **Validate content** check to pass. Fix anything it reports by pushing more commits
   to the same branch.
4. Another editor reviews it. Rules changes (not typos) should be discussed on Discord first.
5. A maintainer merges it.

Content is English only for now; translations will come later as separate files that follow the
English ones.
