# Penguin for Lunar

**Penguin 1.9.56** adds a PvE Aim Assist mode for CosmicPrisons enemies and compact clue-transfer buttons in player vaults, including the vault-close crash fix. Live updates, remembered terrain, Legendary mining and the existing features remain included.

**[Download Penguin 1.9.56 for Windows](https://github.com/penguinmodowner/penguin/releases/download/v1.9.56/Penguin-Lunar-1.9.56.zip)** · **[Release notes and downloads](https://github.com/penguinmodowner/penguin/releases/tag/v1.9.56)**

Requires **Windows x64, Lunar Client, Minecraft 1.21.11 with Fabric, and Fabric API**. Java is included in the download. Existing Penguin preferences are preserved.

## Get started

1. Extract the **entire ZIP**. Keep `Penguin.exe`, `app` and `runtime` together.
2. First time only: fully close Minecraft and Lunar, including Lunar's tray icon. Open `Penguin.exe` and choose **Prepare Lunar** to enable Lunar's attach setting. Optional companion mods start unchecked.
3. Launch Lunar **Fabric 1.21.11** and wait for Minecraft's main menu.
4. Select the game in Penguin and choose **Load Penguin**. Keep Minecraft visible while resources reload. If you have several games open, select the intended one explicitly.
5. Press **K** in a world, or use **Open menu** in the launcher. **Start** explains the controls and links to common tasks.

For later sessions, start at step 3. **Upgrading from 1.9.47 or earlier requires one Minecraft restart.** For compatible newer runtimes, extract the new ZIP into its own folder, close any chest/inventory, and use **Update Penguin** in that new launcher. Keep Minecraft visible during the reload. Update each game separately and keep the same version in games sharing settings. Opening Penguin alone does not change Lunar settings; Prepare Lunar does. Do not also install a Penguin JAR in the mods folder.

## First-time settings

All Penguin features and tracer lines start **OFF** only when this game folder has **no saved Penguin settings**. Curated colors, ranges, speeds and volumes are ready for the features you choose to enable. Child preferences are separate from the module's OFF switch. Friends, gangs, private shortcuts, clue selections and relay details are not bundled.

**Updating never applies this preset to an existing setup.** Current shared settings and older settings files keep their saved switches, tuning, lists and keys. Loading displays a local **Penguin mod — press K for settings** message once you join a world; it uses your rebound menu key if different and is not sent to the server.

## Find your features

| Tab | What's inside |
| --- | --- |
| **Start** | Quick guide, friends, profiles, menu size and shortcut help |
| **Mining** | Gen Mining and Block Tracers, as separate modules |
| **Combat** | Left Clicker, Right Clicker and Aim Assist |
| **Visuals** | Nametags, Friend Overlay, Guards, Stone View, No Debuff, Constant FOV, Clear Distance Fog and Waypoint Groups |
| **Bandits** | Escapee Radar highlights, direction and alerts |
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

**Gen Mining → Cycle:** choose a key, aim at the first unfinished center block and start. Penguin mines four blocks, turns after the first three, then stops, with a completion alert if enabled. It can continue while tabbed out; input directed at that game or F8 cancels it. Verify, Sell, Alerts and the optional Escape-menu actions have their own sections.

Choose **Crude ore → Prismarine / Legendary** in Gen Mining. Legendary uses **Glowstone at 50**, **Nether Bricks at 25**, **Nether Quartz Ore at 10**, and **Netherrack when finished**. Prismarine uses Sea Lantern, Dark Prismarine, Prismarine Bricks and Prismarine respectively. The choice controls cycle completion, 90-degree turns, Escape actions and stage alerts. Only the finished stage advances a generator. Each stage alert has its own switch and volume, and the new 25/10 alerts start off.

**Block Tracers:** search block names or IDs, add them to one shared list and choose a color for each type. Outlines and tracer lines toggle independently. Trace all matches or the closest of each type. Only loaded chunks are searched. The top-left Block Tracers status banner has been removed.

Presets add or remove their blocks while preserving unrelated selections: **Ground Zero** includes yellow wool, blue-highlighted black concrete and red-highlighted raw gold blocks; **Vault** uses white concrete. The block inspector identifies what the server sends to your client, including blocks beneath entity decorations.

## Friends, gangs and waypoints

**Friends** has individual ON/OFF switches and a shortcut to friend colors and nametags. ON applies friend visuals and excludes that player from Aim Assist; OFF treats them as a regular player.

**Auto-add from gangs** watches exact gang names. Recognized live tags or a complete `/g info <gang>` / `/g who <gang>` roster add members to your saved Friends list. Saved friends remain after they leave a gang or you stop watching it. Individual OFF switches stay respected. Use OFF to exclude someone: removing them can let an enabled gang watch add them again.

**Visuals → Waypoint Groups** shows or hides the members of one Lunar group, such as `vaults`, without changing other groups. Lunar's Waypoints mod must be on. Lunar saves these visibility changes, even after Stop Penguin.

## Clue scrolls

Enable **Clue Scrolls** and open a storage chest. Enter MrMexican category numbers such as `4, 12, 17`, then **Take** from the chest or **Put** into it. Spaces and ranges work too. No reference scroll is needed. **From chest** fills the number list without moving anything.

The **CHEST CLUES** panel above the chest lists the quantity of each numbered clue in the chest, sorted by quantity (highest first), with clue number breaking ties. It updates as contents change and combines tiers, materials and stacked quantities, independently of your transfer filters. It excludes player inventory, completed rewards and unnumbered items. Both panels follow **Minecraft's GUI Scale**. The counts above match the chest width and grow vertically before paging. The full clue controls sit on the left with roomy Take/Put and bulk-action rows, the full ore selector and the Include completed switch. Narrow windows stack controls in the left margin. Short windows use the right margin for counts when needed. Use the arrow buttons for long lists. Item tooltips render above these panels. Counts use compatible **MrMexican 1.3.2** and its customized category numbers.

**Player vaults hide the large panels automatically.** This covers `/pv` and `/pv <number>` for any vault number, including MrMexican's selector and page changes. Once a vault is open, compact **Pull all clues / Dump all clues** buttons at the bottom transfer recognized clues between that vault and your inventory. They follow **Include completed** from the normal chest panel. The selector has no transfer buttons, and number shortcuts stay inactive in vaults. Normal chest tools return after leaving the vault. The vault-close crash is fixed.

Click **x** on the clue tools panel to hide the tools and counts for this chest opening. Reopening a chest restores them automatically; saved settings and the enabled switch stay unchanged. Take/Put shortcuts are inactive while hidden.

For ore-mining clues, use **Ore** in the panel. It starts at **Choose ore…**, so mining clues stay put until one material is selected. **Redstone**, for example, accepts redstone tasks across tiers and required amounts while leaving lapis, iron and gold alone. Normal/deepslate forms share a material; selected category numbers still apply. **Any ore** opts into mixed materials. Non-ore tasks are unaffected. Material choices are **Iron, Lapis, Redstone, Gold, Diamond, Emerald**, in that order; **Choose ore…** and **Any ore** are separate controls below them. Saved selections for removed materials return to **Choose ore…**.

**Take all / Dump all** ignore the number and ore filters and move only recognized clue scrolls. **Include completed** starts OFF and applies to these two bulk buttons. Number-based Take/Put always skip completed rewards. Bulk actions work without MrMexican; number matching requires compatible **MrMexican 1.3.2** and respects its customized numbers.

Set separate **Take / Put** keyboard shortcuts in **K → Clues → Clue Scrolls → Controls**. Both start unbound. They use the panel's selected numbers and ore, act only in an open chest, and do not fire while typing, choosing ore or holding the shortcut down.

All four actions send normal shift-clicks in one batch without added per-item delay. Server processing can still affect timing. Leave the inventory alone until the result appears; Penguin checks for corrections and does not automatically retry. **More tools** and the older sorting/reference interface have been removed. Remove standalone ClueSort and avoid running two inventory automation tools together.

Assign **Toggle Clue Scrolls** in **K → Clues → Clue Scrolls → Controls**. It starts unbound and works in gameplay or an open chest, even while Clue Scrolls is off. Disabling stops transfers and hides both panels; re-enabling restores them in the same chest. It ignores typing, modifier combinations and held-key repeats.

## Escapee Radar

Enable **K → Bandits → Escapee Radar** for loaded Escapee NPC outlines, a nearest-target label/direction arrow and an **ESCAPEE!** banner. Range, color, highlights, direction, banner and tracer line are separate controls. The feature and tracer line start OFF; the direction arrow is independent of the line and of J. It never moves your camera or extends the server's entity tracking. Live Escapee detection is still awaiting confirmation; automated tests cannot confirm the server's exact label layout.

Block presets preserve your tracer-line choice. Existing users keep their saved choices, including the older combined Escapee direction/line preference.

## Remembered terrain and Elite Bandits

For farther terrain, fully close Minecraft and Lunar, then open **Prepare Lunar** and select **Bobby — remember terrain you've visited**. Review and install into the intended Fabric 1.21.11 profile. Bobby works independently of MrMexican and starts unchecked. Relaunch, set Minecraft's video render distance to around **16 chunks**, and explore. Previously visited terrain stays visible farther away; unseen terrain and live distant entities are not supplied. Existing Bobby settings and cache are kept. New installs get multiple-world matching and a seven-day unused-region expiry. Penguin block tools use live chunks only.

For Elite Bandits, enable **K → Visuals → Nametags → Display → Include elite bandits**. It starts off and shares the normal nametag/tracer settings and **J** toggle. NPC labels are recognized without hardcoding generated account suffixes; floating text decorations are excluded. This nametag option is separate from the PvE Aim Assist mode below.

**Clear Distance Fog** is available under Visuals, off by default. It removes the distance fade for already-loaded terrain while keeping environmental fog.

## Aim Assist: players or PvE

Under **K → Combat → Aim Assist**, turn on **PvE enemies instead of players** to target recognized normal, elite and blood bandits, werewolves and escapees. It starts OFF; turning it off restores player targeting. Listed players, friends, guards, wardens, enforcers, unrelated NPCs and floating text decorations stay excluded from PvE targeting.

Enable **Aim Assist** and **Left Clicker**, then physically hold left-click. The existing smoothing, range, angle, aim height, visibility and held-weapon settings still apply. The naked/target-sword filter applies only to player mode. The feature changes aim selection, not manual attacks or reach. Generated NPC account suffixes are not hardcoded. Blood-bandit and werewolf label variants have automated coverage but still need live confirmation.

## Guards

Enable **K → Visuals → Guards** for separate guard, cell guard, enforcer and warden nametags/tracers. Choose type colors, visible types, range and style. Guards start OFF on existing installs. **Follow J toggle** starts ON: J hides and restores enabled Guards together with player/friend overlays. Turn it off for independent operation, or assign a separate guard shortcut. These overlays label loaded NPCs and distance; they do not estimate a guard's detection area.

## Settings and alerts

Preferences save automatically and sync between games sharing a settings folder. Use the same Penguin version in those games. Running cycles and menu navigation remain local.

**Profiles → Export file** saves a shareable settings file. Friends and gangs are excluded unless selected. To import, copy a file into the profiles folder, Refresh, inspect it and Apply profile. Penguin backs up current settings and leaves automatic actions off until enabled. Raid Watch connection settings are local and are not exported.

Message Alerts work independently of Gen Mining. Mining Alerts links to the same sounds available under Gen Mining. Raid Watch can monitor a cell and optionally write to an existing local PenguinTracker Discord-bot relay; it does not create the bot or require its token. A local relay write does not confirm Discord delivery.

## Optional companion setup

Prepare Lunar offers **MrMexican 1.3.2**, optional **CosmicTextures 1.2**, and **Bobby 5.2.11.1+mc1.21.11**, all initially unchecked. Bobby can be selected independently; choosing it alone preserves the other mods and their settings. Penguin works without them. Fully close Minecraft and Lunar before selecting a profile, reviewing changes and installing companions.

MrMexican setup backs up superseded CosmicUtilities, CosmicPings and old Penguin mod copies. CosmicTextures is kept or installed only when included in this setup; unrelated Lunar mods remain. Backups go into the profile's `penguin-mod-backups` folder. Updating Penguin alone does not replace companion mods.

Official downloads are pinned by hash. Setup disables MrMexican's automatic updater, automatic Papa Ping and Peaceful Mining; including CosmicTextures also disables its overlapping texture packs. Manually using `/papa` → Create still contacts its external authentication service. Do not share that service's relay token. Third-party mods retain their own authorship and licenses; see [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

## Stop, update and source

**Stop Penguin** disables its runtime features while Minecraft stays open. **Update Penguin** replaces a compatible runtime with the version from the new launcher folder. Updates stop running automation and preserve settings. Do not overwrite the active version's folder. A pre-1.9.48 runtime, an incompatible runtime or a previous initialization failure requires a Minecraft restart. Companion changes take effect on the next game launch.

The bundled `README.txt` contains more detailed instructions. **839 automated tests: 838 passed, 1 skipped, no failures or errors.** A live update from 1.9.55 to 1.9.56 succeeded in the same Lunar process and preserved settings. The vault-transfer fix was confirmed in game. New PvE target variants still need live confirmation. Live Escapee recognition, final gang-friend behavior and Raid Watch relay validation remain pending. The terrain cache and vaults-only waypoint control were previously confirmed in Lunar.

Developers: download **[Penguin-Lunar-1.9.56-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.56/Penguin-Lunar-1.9.56-Source.zip)** for the application source and tests. Its `SOURCE-BUILD.txt` explains optional test fixtures. GitHub's automatic **Source code** downloads contain this documentation repository. **[SHA256SUMS.txt](https://github.com/penguinmodowner/penguin/releases/download/v1.9.56/SHA256SUMS.txt)** covers both release ZIPs. [Penguin's MIT license](LICENSE) applies to Penguin code only.
