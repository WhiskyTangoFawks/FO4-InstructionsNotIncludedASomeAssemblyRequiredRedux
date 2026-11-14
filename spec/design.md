# Design

The patterns behind the placements and the numbers. The plugin source holds both.

## Distribution

Rarity follows the setting ([principles](principles.md), The world is plausible).

- Raider pieces come from the raiders who wear them, and T-45 and T-51 pieces lie scattered across the Commonwealth, most where the military or a faction would have kept them. A place that held a full frame holds one or two pieces.
- X-01 exists as one set, scattered piece by piece.
- T-60 comes only from the Brotherhood of Steel, and X-02 from the Enclave, which America Rising 2 adds.
- Where a vanilla frame stood, a supply cache stands: chems, weapons, ammo and explosives.
- A power armor spawn that remains is the raider or T-45 suit its enemies would wear, and does not return when its cell resets. A boss that spawns already in power armor is unchanged.
- A showpiece suit is standard T-51 at 1% health, with a display lining.

## Tiers

The suits fall into tiers by who built them, and a tier decides what a repair takes.

| Tier | Suits | Repair |
|---|---|---|
| Non-military | Raider | No perk |
| Pre-war military | T-45, T-51 | Armorer |
| Advanced | T-60, X-02, Hellfire | Armorer and Science |
| Unique | X-01 | Armorer and Science; one set exists |

A suit a raider rebuilt, such as Nuka-World's Raider Overboss T-51, repairs as raider work does.

## Niches

Each suit is the best choice for something and pays for it elsewhere ([principles](principles.md), Every suit has a niche), and its lore decides which ([principles](principles.md), The world is plausible). A niche spans more than resistances: movement and reload speed, repair perks and materials, the mods a suit accepts, its linings, and fuel economy.

| Suit | Best at | Pays with |
|---|---|---|
| Raider | Repairs with no perk | The weakest protection, and few mods |
| T-45 | Decent protection that is easy to keep repaired | The least protection of the military suits |
| T-51 | The best protection, and the widest high-tech mods, the jetpack among them | The costliest repairs, in material and perks |
| T-60 | Versatility: the best fuel economy, radiation protection | Less protection than T-51, and Science to repair |
| X-02 | The Enclave's suit, as T-60 is the Brotherhood's: T-60's versatility for a player who sides with the Enclave | Numbers near T-60's, and Science to repair |
| X-01 | A testbed that takes almost any mod, with far more health than T-51 | Less armor than T-51, and one set to find |
| Hellfire | Hazardous environments: the most health and radiation resistance of any suit | Less armor than T-51 and X-01 |

## Fuel

Fuel economy is a strength a suit can have, never a cost. A suit that drains fusion cores faster than vanilla is unusable in a modlist where cores are scarce, such as one with Lunar Fallout Overhaul. T-60's pieces drain cores more slowly, and the advanced suits' and X-01's top linings slow the drain a little.

## Linings

A lining tier adds to the armor it fits. The top lining adds the armor's signature enchantment, borrowed from a vanilla or DLC enchantment: T-45 its own battery drain, T-51 explosives resistance, T-60 Automatron energy damage, and the X-01 battery drain for X-01, X-02 and Hellfire.

## Damage formula

Power armor protects its wearer through the game's damage formula. Vanilla's formula reduces a hit by at most about 70 to 80% whatever the resistance, so power armor's resistances barely change what the wearer takes, and the wearer dies long before the suit is damaged. The module lowers that floor, by the damage factor and armor reduction exponent settings, so resistance decides protection, and each suit's resistances serve its niche. The settings are global: they change the damage every armor and every actor takes. The alternatives rejected are in [references](references.md).

The module also changes the power drain settings.
