# Dragon Riders - AGOT-Inspired System

A comprehensive dragon system mod for Crusader Kings III, inspired by the AGOT mod's mechanics.

## Overview

This mod adds a complete dragon taming, breeding, and combat system to CK3. Dragons are represented through a hybrid artifact + trait system, with character variables tracking bond strength, combat experience, and dragon stats.

## Key Features

### Valyrian Blood System
- **4-level bloodline** that dilutes over generations (Pure → Strong → Faint → Trace)
- Blood dilution can be toggled via game rules
- Successfully bonding with a dragon restores blood to Pure level
- Affects taming success chance and egg hatching ability

### Dragon Bonding
- **Bond Levels** (3 tiers): Novice → Bonded → Legendary
- Bond deepens through events and the "Deepen Bond" decision
- Stronger bonds mean better dragon obedience and combat effectiveness

### Dragon Training
- **Combat Training** (4 tiers): Untrained → Tested → Veteran → Legendary
- Improves through actual combat participation
- Affects knight effectiveness and provides prowess bonuses

### Egg Hatching (Two Methods)
1. **Simple Hatching** - For characters with Strong Valyrian Blood
   - Time-based with success/failure chance
   - Failed eggs may turn to stone

2. **Hatching Ceremony** - For stone eggs or weak/no blood
   - Complex ritual requiring piety, gold, and learning
   - Can potentially revive stone eggs

### Cradle Bonding
- Place eggs in infant's cradle for strongest possible bond
- Dragon and child grow up together
- Nearly guaranteed hatching success

### Dragon Mourning
- **Permanent Mourning** (default): Losing your dragon means you can NEVER bond again
- Alternative game rules for temporary mourning or no restriction
- Severe stress and stat penalties during mourning

### Dragon Combat
- Challenge rival dragon riders to deadly duels
- Combat success based on dragon training, bond level, and prowess
- Outcomes range from victory to death (configurable via game rules)

### Dragon Naming
- Name your dragon from preset Valyrian names
- Choose from fantasy name alternatives
- Name based on dragon's appearance/color

## Game Rules

Configure these when starting a new game:

| Rule | Options | Default |
|------|---------|---------|
| Blood Requirement | Required / Bonus / Not Required | Required |
| Blood Dilution | Dilutes / Stable | Dilutes |
| Dragon Mourning | Permanent / Temporary / None | Permanent |
| Combat Lethality | Lethal / Moderate / Safe | Lethal |
| Egg Hatching | Easy / Moderate / Hard | Moderate |
| Dragon Ownership | Single / Multiple | Single |

## Installation

1. Download and extract to: `Documents/Paradox Interactive/Crusader Kings III/mod/dragon_mod/`
2. Copy `descriptor.mod` to `Documents/Paradox Interactive/Crusader Kings III/mod/` and rename to `dragon_mod.mod`
3. Edit the copy to uncomment the `path = "mod/dragon_mod"` line
4. Enable in CK3 launcher

## File Structure

```
dragon_mod/
├── descriptor.mod
├── common/
│   ├── artifacts/          # Dragon and egg artifacts
│   ├── character_modifiers/# Temporary modifiers
│   ├── decisions/          # Player decisions
│   ├── game_rules/         # Customization options
│   ├── on_action/          # Automatic event triggers
│   ├── scripted_effects/   # Reusable actions
│   ├── scripted_triggers/  # Reusable conditions
│   └── traits/             # Character traits
├── events/
│   ├── dragon_taming_events.txt
│   ├── dragon_hatching_events.txt
│   ├── dragon_bond_events.txt
│   ├── dragon_naming_events.txt
│   ├── dragon_death_events.txt
│   └── dragon_combat_events.txt
└── localization/english/   # All text strings
```

## How to Play

### Getting Started
1. Use **Ruler Designer** to add "Pure Valyrian Blood" trait
2. OR play normally and find/steal dragon eggs
3. Hatch eggs or claim wild dragons

### Taming a Dragon
1. Have Valyrian Blood (or play without the requirement)
2. Find an unbonded dragon
3. Use "Claim a Dragon" decision
4. Survive the attempt (based on bloodline, prowess, and luck)

### Hatching Eggs
- **Strong Blood**: Use "Hatch Dragon Egg" decision
- **Weak/No Blood**: Use "Dragon Egg Hatching Ceremony" (expensive)
- **For Children**: Use "Cradle Egg for Child" decision

### Strengthening Your Bond
- Use "Deepen Dragon Bond" decision periodically
- Go flying with "Go Flying" decision
- Random events will occasionally offer bond improvements

### Combat
- Challenge rivals with "Challenge to Dragon Duel" decision
- Must be at war or have rivalry
- **WARNING**: Duels are often fatal!

## Tips

- **Preserve your bloodline**: Marry others with Valyrian Blood
- **Don't rush combat**: Dragon duels are extremely dangerous
- **Cradle eggs for heirs**: Cradle bonds are the strongest
- **Multiple eggs**: You can own many eggs, but only ride one dragon at a time

## Known Limitations

- Dragons use the artifact system (no 3D models)
- Combat is event-based (no animated battles)
- Dragon AI is limited

## Compatibility

- **Base Game**: Full support
- **Royal Court DLC**: Enhanced features
- **Other Mods**: May conflict with fantasy/dragon mods

## Version History

- **1.0.0** - Initial release
  - Complete trait system
  - Dragon artifacts
  - Taming, hatching, bonding events
  - Combat system
  - Full localization

## Credits

Inspired by the A Game of Thrones mod's dragon mechanics.

---

*Fire and Blood!*
