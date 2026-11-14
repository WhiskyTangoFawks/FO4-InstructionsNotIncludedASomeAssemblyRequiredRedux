# Architecture

## Modules

| Module | Owns | Masters beyond the game and its DLCs |
|---|---|---|
| `SomeAssemblyRequired.esp` | Distribution: every power armor placement and spawn, and the sets it swaps. | |
| `SomeAssemblyRequired_SWAP.ini` | The leveled vanilla sets that other mods place, swapped through Base Object Swapper. | |
| `SomeAssemblyRequired - LBPAC.esp` | The LBPAC module: armor stats, linings, repair recipes, the damage formula, and the loading screens and terminals that describe the armor. | `SomeAssemblyRequired.esp`, SuperAlloys, Raider Power Armor Chop-Shop, the Creation Club X-02 and Hellfire |
| `Scripts/PowerArmorExoPAWorkbenchPerkScript` | The player's repair tokens, at a power armor workbench. | |
| `RaiderPAChopShop.esp` | Replaces Raider Power Armor Chop-Shop's plugin of the same name. | |
| `CoAPowerArmor.esp` | Replaces Children of Atom Power Armor's plugin of the same name, and fits its armor into South of the Sea and Ashlands. | South of the Sea, Ashlands |
| `Ashlands - UseVanillaRaiderPA.esp` | Ashlands' power armor, set to the vanilla raider armor. | Ashlands |
| `SotS - UseVanillaRaiderPA.esp` | South of the Sea's power armor, set to the vanilla raider armor. | South of the Sea |

A module needs its masters. The distribution also needs SuperAlloys, which it does not master: a showpiece suit's display lining is replaced through SuperAlloys' linings.

## Rules

- Distribution and balance are separate plugins, so the distribution stands without the LBPAC module. The LBPAC module masters the distribution, never the reverse.
- A replacing plugin takes the other author's file name, so the game loads it in place of the author's.
- A change to another mod's power armor is a plugin named for that mod.
- The mod loads before any mod with previs, so the previs mods win the cells it edits.
- A repair's perk requirement is a component its recipe asks for, so the workbench shows it as a material. The workbench script gives the player a token for each Armorer and Science rank they hold while they use the station, and each token yields its component. A power armor workbench carries the script on its furniture, so a mod that adds a new kind of power armor workbench needs a patch that adds it.
