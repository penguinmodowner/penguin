# Penguin for Lunar

**Penguin 1.9.28** brings a clearer menu, a first-use guide and simpler launcher controls, along with clue-scroll fixes, Lunar waypoint-group controls and saved gang friends.

**[Download Penguin 1.9.28 for Windows](https://github.com/penguinmodowner/penguin/releases/download/v1.9.28/Penguin-Lunar-1.9.28.zip)** · **[Release notes and downloads](https://github.com/penguinmodowner/penguin/releases/tag/v1.9.28)**

Requires **Windows x64, Lunar Client, Minecraft 1.21.11 with Fabric, and Fabric API**. Java is included in the download. Existing Penguin preferences are preserved.

## Get started

1. Extract the **entire ZIP**. Keep `Penguin.exe`, `app` and `runtime` together.
2. First time only: fully close Minecraft and Lunar, including Lunar's tray icon. Open `Penguin.exe` and choose **Prepare Lunar** to enable Lunar's attach setting. Optional companion mods start unchecked.
3. Launch Lunar **Fabric 1.21.11** and wait for Minecraft's main menu.
4. Select the game in Penguin and choose **Load Penguin**. Keep Minecraft visible while resources reload. If you have several games open, select the intended one explicitly.
5. Press **K** in a world, or use **Open menu** in the launcher. **Start** explains the controls and links to common tasks.

For later sessions, start at step 3. **Restart Minecraft before loading a newer Penguin version.** Opening Penguin alone does not change Lunar settings; Prepare Lunar does. Do not also install a Penguin JAR in the mods folder.

## Find your features

| Tab | What's inside |
| --- | --- |
| **Start** | Quick guide, friends, profiles, menu size and shortcut help |
| **Mining** | Gen Mining and Block Tracers, as separate modules |
| **Combat** | Left Clicker, Right Clicker and Aim Assist |
| **Visuals** | Nametags, Friend Overlay, Stone View, No Debuff, Constant FOV and Waypoint Groups |
| **Clues** | Clue Scrolls guide, matching and transfer options |
| **Alerts** | Message Alerts, Mining Alerts and Raid Watch |
| **All** | Every feature; search also searches every category |

Select a feature to open its settings. Switches turn things on or off; buttons open pages or perform their named action. Gen Mining has separate controls instead of one master switch. Closing the menu keeps features running and remembers your page and scroll position for that game session.

**Settings** has three pages: **Display** for menu size, **Controls** for configurable keys, and **Help** for setup and shortcuts.

## Everyday controls

| Key | Action |
| --- | --- |
| **K** | Open Penguin |
| **J** | Toggle all player nametags and tracers, including friends |
| **O / P** | Toggle block outlines / block tracer lines |
| **U** | Toggle Stone View |
| **F8** | Stop clickers, passive turning and the mining cycle |
| **Esc** | Go back or close a menu |

Left Clicker defaults to **]**, Right Clicker to **F7**. Mining-cycle and waypoint-group keys start **Unbound**; choose them in Settings → Controls. Clickers require focused gameplay: enable one, then release and hold its mouse button.

## Mining and blocks

**Gen Mining → Cycle:** choose a key, aim at the first unfinished center block and start. Penguin mines four blocks, turns after the first three, then stops with its completion alert. It can continue while tabbed out; input directed at that game or F8 cancels it. Verify, Sell, Alerts and the optional Escape-menu actions have their own sections.

**Block Tracers:** search block names or IDs, add them to one shared list and choose a color for each type. Outlines and tracer lines toggle independently. Trace all matches or the closest of each type. Only loaded chunks are searched.

Presets add or remove their blocks while preserving unrelated selections: **Ground Zero** includes yellow wool, blue-highlighted black concrete and red-highlighted raw gold blocks; **Vault** uses white concrete. The block inspector identifies what the server sends to your client, including blocks beneath entity decorations.

## Friends, gangs and waypoints

**Friends** has individual ON/OFF switches and a shortcut to friend colors and nametags. ON applies friend visuals and excludes that player from Aim Assist; OFF treats them as a regular player.

**Auto-add from gangs** watches exact gang names. Recognized live tags or a complete `/g info <gang>` / `/g who <gang>` roster add members to your saved Friends list. Saved friends remain after they leave a gang or you stop watching it. Individual OFF switches stay respected. Use OFF to exclude someone: removing them can let an enabled gang watch add them again.

**Visuals → Waypoint Groups** shows or hides the members of one Lunar group, such as `vaults`, without changing other groups. Lunar's Waypoints mod must be on. Lunar saves these visibility changes, even after Stop Penguin.

## Clue scrolls

Enable Clue Scrolls and open a storage chest:

- **Sort** organizes recognized clues inside the chest.
- **Collect** uses the clue in **hotbar slot 1** as a reference. Similar matching groups market-price amounts and normal/deepslate forms of the same ore; lapis and redstone remain separate.
- **Dump** stores recognized unfinished inventory clues. Completed and unknown scrolls remain in your inventory.

Collect and Dump shift-click one stack at a time and pace transfers for the connection. After successful collection, a matching unfinished scroll in **hotbar slot 2** moves to the first free upper-inventory slot; the reference stays in slot 1. Remove the old standalone ClueSort and avoid running two inventory automation tools together.

## Settings and alerts

Preferences save automatically and sync between games sharing a settings folder. Use the same Penguin version in those games. Running cycles and menu navigation remain local.

**Profiles → Export file** saves a shareable settings file. Friends and gangs are excluded unless selected. To import, copy a file into the profiles folder, Refresh, inspect it and Apply profile. Penguin backs up current settings and leaves automatic actions off until enabled. Raid Watch connection settings are local and are not exported.

Message Alerts work independently of Gen Mining. Mining Alerts links to the same sounds available under Gen Mining. Raid Watch can monitor a cell and optionally write to an existing local PenguinTracker Discord-bot relay; it does not create the bot or require its token. A local relay write does not confirm Discord delivery.

## Optional companion setup

Prepare Lunar offers **MrMexican 1.3.2** and optional **CosmicTextures 1.2**, both initially unchecked. Penguin works without them. Fully close Minecraft and Lunar before selecting a profile, reviewing changes and installing companions.

MrMexican setup backs up superseded CosmicUtilities, CosmicPings and old Penguin mod copies. CosmicTextures is kept or installed only when included in this setup; unrelated Lunar mods remain. Backups go into the profile's `penguin-mod-backups` folder. Updating Penguin alone does not replace companion mods.

Official downloads are pinned by hash. Setup disables MrMexican's automatic updater, automatic Papa Ping and Peaceful Mining; including CosmicTextures also disables its overlapping texture packs. Manually using `/papa` → Create still contacts its external authentication service. Do not share that service's relay token. Third-party mods retain their own authorship and licenses; see [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

## Stop, update and source

**Stop Penguin** in the launcher disables its runtime features while Minecraft stays open. Loaded Java code remains until Minecraft closes, so restart the game before loading an update. Companion changes also take effect on the next game launch.

The bundled `README.txt` contains more detailed feature instructions. This release passed **649 automated tests, with one skipped**. In-game checks confirmed the new menu, clue-scroll changes and vaults-only waypoint toggling. The gang parser was checked against live server tags; final friend-list/nametag confirmation and live Raid Watch relay validation remain pending.

Developers: download **[Penguin-Lunar-1.9.28-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.28/Penguin-Lunar-1.9.28-Source.zip)** for the application source and tests. Its `SOURCE-BUILD.txt` explains optional test fixtures. GitHub's automatic **Source code** downloads contain this documentation repository. **[SHA256SUMS.txt](https://github.com/penguinmodowner/penguin/releases/download/v1.9.28/SHA256SUMS.txt)** covers both release ZIPs. [Penguin's MIT license](LICENSE) applies to Penguin code only.
