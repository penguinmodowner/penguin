# Penguin for Lunar

**Penguin 1.9.37** adds a simpler clue-scroll panel with category numbers, ore selection and Take/Put shortcuts, plus configurable guard nametags and tracers.

**[Download Penguin 1.9.37 for Windows](https://github.com/penguinmodowner/penguin/releases/download/v1.9.37/Penguin-Lunar-1.9.37.zip)** · **[Release notes and downloads](https://github.com/penguinmodowner/penguin/releases/tag/v1.9.37)**

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
| **Visuals** | Nametags, Friend Overlay, Guards, Stone View, No Debuff, Constant FOV and Waypoint Groups |
| **Clues** | Clue Scrolls guide and Take/Put shortcut controls |
| **Alerts** | Message Alerts, Mining Alerts and Raid Watch |
| **All** | Every feature; search also searches every category |

Select a feature to open its settings. Switches turn things on or off; buttons open pages or perform their named action. Gen Mining has separate controls instead of one master switch. Closing the menu keeps features running and remembers your page and scroll position for that game session.

**Settings** has three pages: **Display** for menu size, **Controls** for configurable keys, and **Help** for setup and shortcuts.

## Everyday controls

| Key | Action |
| --- | --- |
| **K** | Open Penguin |
| **J** | Toggle player/friend overlays and enabled, linked guard overlays |
| **O / P** | Toggle block outlines / block tracer lines |
| **U** | Toggle Stone View |
| **F8** | Stop clickers, passive turning and the mining cycle |
| **Esc** | Go back or close a menu |

Left Clicker defaults to **]**, Right Clicker to **F7**. Mining-cycle, waypoint-group and separate guard keys start **Unbound**; choose them in Settings → Controls. Clickers require focused gameplay: enable one, then release and hold its mouse button.

## Mining and blocks

**Gen Mining → Cycle:** choose a key, aim at the first unfinished center block and start. Penguin mines four blocks, turns after the first three, then stops with its completion alert. It can continue while tabbed out; input directed at that game or F8 cancels it. Verify, Sell, Alerts and the optional Escape-menu actions have their own sections.

**Block Tracers:** search block names or IDs, add them to one shared list and choose a color for each type. Outlines and tracer lines toggle independently. Trace all matches or the closest of each type. Only loaded chunks are searched. The top-left Block Tracers status banner has been removed.

Presets add or remove their blocks while preserving unrelated selections: **Ground Zero** includes yellow wool, blue-highlighted black concrete and red-highlighted raw gold blocks; **Vault** uses white concrete. The block inspector identifies what the server sends to your client, including blocks beneath entity decorations.

## Friends, gangs and waypoints

**Friends** has individual ON/OFF switches and a shortcut to friend colors and nametags. ON applies friend visuals and excludes that player from Aim Assist; OFF treats them as a regular player.

**Auto-add from gangs** watches exact gang names. Recognized live tags or a complete `/g info <gang>` / `/g who <gang>` roster add members to your saved Friends list. Saved friends remain after they leave a gang or you stop watching it. Individual OFF switches stay respected. Use OFF to exclude someone: removing them can let an enabled gang watch add them again.

**Visuals → Waypoint Groups** shows or hides the members of one Lunar group, such as `vaults`, without changing other groups. Lunar's Waypoints mod must be on. Lunar saves these visibility changes, even after Stop Penguin.

## Clue scrolls

Enable **Clue Scrolls** and open a storage chest. Enter MrMexican category numbers such as `4, 12, 17`, then **Take** from the chest or **Put** into it. Spaces and ranges work too. No reference scroll is needed. **From chest** fills the number list without moving anything.

For ore-mining clues, use **Ore** in the panel. It starts at **Choose ore…**, so mining clues stay put until one material is selected. **Redstone**, for example, accepts redstone tasks across tiers and required amounts while leaving lapis, iron and gold alone. Normal/deepslate forms share a material; selected category numbers still apply. **Any ore** opts into mixed materials. Non-ore tasks are unaffected.

**Take all / Dump all** ignore the number and ore filters and move only recognized clue scrolls. **Include completed** starts OFF and applies to these two bulk buttons. Number-based Take/Put always skip completed rewards. Bulk actions work without MrMexican; number matching requires compatible **MrMexican 1.3.2** and respects its customized numbers.

Set separate **Take / Put** keyboard shortcuts in **K → Clues → Clue Scrolls → Controls**. Both start unbound. They use the panel's selected numbers and ore, act only in an open chest, and do not fire while typing, choosing ore or holding the shortcut down.

All four actions send normal shift-clicks in one batch without added per-item delay. Server processing can still affect timing. Leave the inventory alone until the result appears; Penguin checks for corrections and does not automatically retry. The panel expands from **Clue tools** on narrow windows. **More tools** and the older sorting/reference interface have been removed. Remove standalone ClueSort and avoid running two inventory automation tools together.

## Guards

Enable **K → Visuals → Guards** for separate guard, cell guard, enforcer and warden nametags/tracers. Choose type colors, visible types, range and style. Guards start OFF on existing installs. **Follow J toggle** starts ON: J hides and restores enabled Guards together with player/friend overlays. Turn it off for independent operation, or assign a separate guard shortcut. These overlays label loaded NPCs and distance; they do not estimate a guard's detection area.

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

The bundled `README.txt` contains more detailed feature instructions. This release passed **723 automated tests, with one skipped**. The latest clue panel and shortcuts, default guard link to J and removed status banner still need final in-game checks. Earlier menu and vaults-only waypoint checks passed. Final gang friend-list/nametag confirmation and live Raid Watch relay validation remain pending.

Developers: download **[Penguin-Lunar-1.9.37-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.37/Penguin-Lunar-1.9.37-Source.zip)** for the application source and tests. Its `SOURCE-BUILD.txt` explains optional test fixtures. GitHub's automatic **Source code** downloads contain this documentation repository. **[SHA256SUMS.txt](https://github.com/penguinmodowner/penguin/releases/download/v1.9.37/SHA256SUMS.txt)** covers both release ZIPs. [Penguin's MIT license](LICENSE) applies to Penguin code only.
