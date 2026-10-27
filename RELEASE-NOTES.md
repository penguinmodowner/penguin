# Penguin 1.9.28 — a clearer menu and easier setup

**[Download Penguin 1.9.28 for Windows](https://github.com/penguinmodowner/penguin/releases/download/v1.9.28/Penguin-Lunar-1.9.28.zip)**

Requires Windows x64 and Lunar Fabric **1.21.11** with Fabric API. Extract the entire ZIP; Java is included. Existing settings are preserved. **Restart Minecraft before loading this update**, and use the same Penguin version in windows sharing settings.

## A menu that's easier to learn

- A new **Start guide** introduces the controls and links to common tasks.
- Features are organized into **Mining, Combat, Visuals, Clues and Alerts**, with **All** and global search.
- Gen Mining now has **Cycle, Verify, Sell, Alerts and Escape** sections. Block Tracers has **Blocks, Display and Presets**.
- Settings separates **Display, Controls and Help**. Friends, gang watching, profiles and block tools have clearer actions and explanations.
- The menu still remembers your page, search and scroll position when reopened.
- The launcher separates first-time **Prepare → Launch → Load** from everyday game controls. It refreshes the game list automatically and requires an explicit choice when several games are open. Opening it alone no longer edits Lunar settings; **Prepare Lunar** does.

## Clue-scroll fixes

- Completed scrolls are protected from Dump and Collect, including the combined **“COMPLETE! Right-click to claim rewards!”** footer, checkmarks and wrapped task text.
- More unfinished task types are recognized, fixing valid clues being skipped.
- Dump and Collect shift-click one stack at a time, merge compatible stacks and pace transfers for connection lag. Sort remains a separate chest action.
- Collect uses **hotbar slot 1** as its reference. On successful completion, a matching unfinished clue in **slot 2** moves to the first empty upper-inventory slot. Completed, unrelated or nonmatching items are left alone; no move is made if there is no space or collection is cancelled.
- Similar matching groups market-price amounts and normal/deepslate variants of the same ore while keeping lapis and redstone separate.

## Friends, waypoints and blocks

- **Lunar Waypoint Groups:** show or hide only a selected group's waypoints, with an optional configurable key. Other groups and ungrouped waypoints stay unchanged. Lunar saves the visibility changes.
- **Saved gang friends:** recognized members of watched gangs are added permanently to Friends. Leaving a gang or stopping its watch does not remove them. Individual OFF switches stay respected across shared settings.
- Live gang detection now recognizes the server's unquoted team tags as well as supported quoted tags.
- The **Vault** block preset now selects **white concrete**. Ground Zero and individual block colors remain available.

## Companion setup and alerts

Prepare Lunar offers **MrMexican 1.3.2** and optional **CosmicTextures 1.2**, both unchecked by default. It downloads pinned official files, reviews changes before installation, backs up superseded CosmicUtilities/CosmicPings/Penguin copies and preserves unrelated Lunar mods. CosmicTextures is kept or installed when included. The older Utilities port is no longer bundled.

Setup disables MrMexican's updater, automatic Papa Ping and Peaceful Mining. Including CosmicTextures disables overlapping MrMexican texture packs. Fully close Minecraft and Lunar, including its tray icon, before changing companions; loading this Penguin update alone does not replace them.

**Alerts** brings together Message Alerts, Mining Alerts and Raid Watch. Message Alerts remains independent of Gen Mining. Raid Watch supports local cell monitoring and an optional relay to an existing local PenguinTracker Discord bot; no bot token is needed by Penguin.

## Validation and source

**649 automated tests passed; one filesystem-link test was skipped.** In-game checks confirmed the new menu, clue-scroll fixes and vaults-only waypoint toggling. Gang detection passed a read-only check against live tags; the resulting friend-list/nametag behavior still awaits final user confirmation. Live Raid Watch relay delivery and every optional companion combination have not been confirmed.

The attached **Penguin-Lunar-1.9.28-Source.zip** contains the application source and tests, with test-fixture instructions in `SOURCE-BUILD.txt`. GitHub's automatic Source code downloads contain this documentation repository. **SHA256SUMS.txt** covers both release ZIPs.

See `README.txt` for full setup and `THIRD-PARTY-NOTICES.txt` for companion authorship and terms. Penguin's MIT license applies to Penguin code only. Manually creating a `/papa` group can still authenticate your Minecraft identity with its external service.
