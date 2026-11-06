# Penguin 1.9.52 — live updates, clue panels and Legendary mining

Download **[Penguin-Lunar-1.9.52.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.52/Penguin-Lunar-1.9.52.zip)** for Windows x64. Extract the entire ZIP and keep `Penguin.exe`, `app` and `runtime` together. Java is included. Requires **Lunar Fabric 1.21.11 and Fabric API**.

**Existing settings are preserved.** All features start OFF only on a first installation with no saved Penguin settings.

## Updating Penguin

- **Coming from 1.9.47 or earlier? Restart Minecraft once**, then load 1.9.52 from its new launcher. Older builds cannot retire their loaded code safely.
- With a compatible update-capable version already loaded, extract the new download into its own folder, close any chest or inventory, select the correct game and click **Update Penguin**. Keep Minecraft visible during the resource reload. Do not overwrite the running version's folder.
- Updating stops active automation and preserves your saved switches, colors, tuning, friends and shortcuts. Start a mining cycle again yourself when ready. Each running game updates separately.
- This includes the HUD registration fix for repeated updates. The corrected update path was tested from **1.9.50 to 1.9.51 in the same Lunar game process**, without restarting Minecraft.
- Companion mods and incompatible future changes still need a game restart. A game that reports an earlier initialization failure also needs a restart before retrying.

## Clue panels that fit the chest

- **CHEST CLUES sits above the chest and CLUE TOOLS below it.** Item tooltips render above the panels so the clue name remains readable.
- Both panels follow **Minecraft's GUI Scale** and match the chest width. Counts use more vertical rows before paging. Short windows use available outer margins when needed.
- Counts remain sorted by **quantity, highest first**, with clue number breaking ties. Take/Put, the six-material ore filter, Take all / Dump all, Include completed and configurable shortcuts remain available.
- Both panels stay hidden in **`/pv` and `/pv <number>` for any vault number**, including MrMexican's vault selector and numbered pages. They return for a regular chest. This also prevents clue shortcuts from operating through the vault overlay.
- The **x** button still hides both panels only for the current chest opening.

## Legendary crude ore

Choose **Crude ore → Legendary** in Gen Mining. The existing Prismarine option remains available and keeps its default for existing setups.

| Remaining | Prismarine | Legendary |
| --- | --- | --- |
| 50 | Sea Lantern | Glowstone |
| 25 | Dark Prismarine | Nether Bricks |
| 10 | Prismarine Bricks | Nether Quartz Ore |
| Finished | Prismarine | Netherrack |

The selected pattern applies to the **four-block mining cycle, smooth 90-degree turns, Escape-menu actions and mining alerts**. Only the finished block triggers the next turn. The intermediate stages do not finish a generator. Alerts for 50, 25, 10 and finished have separate switches and volumes, with the newer 25/10 alerts off by default.

## Retained features and checks

Escapee Radar, Elite Bandit nametags, Bobby remembered terrain, guard overlays, friends/gangs, waypoint groups and the earlier clue tools remain included. Prepare Lunar still offers optional MrMexican 1.3.2, CosmicTextures 1.2 and Bobby 5.2.11.1+mc1.21.11, initially unchecked. Updating Penguin alone does not replace those companion mods.

**821 automated tests passed, 1 skipped, no failures or errors.** Coverage includes GUI-scale layout, vault commands and transitions, Legendary stages and the four-block cycle, settings preservation, runtime replacement and the real Fabric HUD registry. The final 1.9.52 GUI/vault behavior and a full Legendary cycle still await an in-game check. Live Escapee label recognition remains unconfirmed.

**[Penguin-Lunar-1.9.52-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.52/Penguin-Lunar-1.9.52-Source.zip)** contains the full application source and tests, with `SOURCE-BUILD.txt` for the separately obtained test fixtures and `HOT-UPDATES.md` for the update architecture. GitHub's automatic Source code downloads contain the documentation repository. **SHA256SUMS.txt** covers both ZIPs. Third-party mods retain their authorship and licenses.
