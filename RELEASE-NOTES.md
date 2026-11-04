# Penguin 1.9.47 — first-use defaults and Escapee Radar

Download **[Penguin-Lunar-1.9.47.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.47/Penguin-Lunar-1.9.47.zip)** for Windows x64. Extract the entire ZIP and keep `Penguin.exe`, `app` and `runtime` together. Java is included. Requires **Lunar Fabric 1.21.11 and Fabric API**.

**Restart Minecraft before loading this update. Existing setups are preserved.** Use the same Penguin version in windows sharing settings. Updating Penguin does not install or replace companion mods.

## First use, without resetting existing users

- **All Penguin features start OFF only when the game folder has no saved Penguin settings.** This includes player/friend/guard overlays, Escapee Radar, block tools, clickers, Aim Assist, Gen Mining, auto sell, visual effects, clue tools and independent alerts. Tracer lines also start OFF. Stone View and Raid Watch remain opt-in.
- Colors, ranges, speeds and volumes use the curated preset. Child preferences are ready for when a feature is deliberately enabled. Friends, gangs, personal shortcuts, clue selections and local relay information are not included.
- **Updates preserve saved ON/OFF choices, tuning, friends, gangs and keys.** Both current shared settings and older settings files are recognized. The new preset is not applied to profile imports or existing installations.
- After loading, a local chat message says **“Penguin mod — press K for settings.”** It uses the actual menu key if rebound, waits for a world when loaded at the main menu, and appears once per activation. It is never sent to server chat.
- Block presets keep the current tracer-line preference instead of switching lines on automatically.

## Escapee Radar

Enable **K → Bandits → Escapee Radar** to highlight recognized nearby Escapee NPCs. It has an orange outline, nearest-target distance, a direction/edge arrow and a large **ESCAPEE!** banner when a new target appears. Range, color, highlights, direction, banner and tracer line have separate controls. The optional tracer line starts OFF; the direction arrow remains a separate preference.

Radar is independent of J and only uses living NPCs currently supplied by the server. It does not move the camera or extend server tracking range. Dead entities, ordinary listed players and floating text decorations are excluded; brief unloads do not repeatedly announce the same target.

**Live Escapee recognition still needs confirmation.** The rare targets were killed before a live identity sample could be captured. Automated tests cover classification, selection, notification timing and resets; they do not establish the server's exact live label layout.

## Clue-scroll improvements

- The right-hand **CHEST CLUES** list now sorts by **quantity, highest first**, with clue number breaking ties. Counts include stack quantities. This changes the sidebar order, not chest slots.
- Assign **Toggle Clue Scrolls** under **K → Clues → Clue Scrolls → Controls**. It starts unbound and works during gameplay or an open chest, including when the feature is off. Turning it off stops transfers and hides both panels; turning it back on restores the panels in the same chest.
- Toggle, Take and Put shortcuts avoid typing/modifier conflicts and do not repeat while held. Ore-specific Take/Put, Take all / Dump all and Include completed remain available.

## Retained features and validation

Bobby remembered terrain and Elite Bandit nametags from 1.9.43 remain included. **Prepare Lunar** still offers optional MrMexican 1.3.2, CosmicTextures 1.2 and Bobby 5.2.11.1+mc1.21.11, all unchecked initially. Bobby can be installed independently. Cached terrain does not supply live distant entities. Companion settings remain separate from Penguin's first-use preset.

**782 automated tests passed; 1 skipped; no failures or errors.** Added checks cover first-install defaults, preserving all saved fields during current/legacy upgrades, shared settings, and the queued local welcome message. Earlier 1.9.45 started successfully in Lunar; the final 1.9.47 build and welcome message have not yet been checked in game.

**[Penguin-Lunar-1.9.47-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.47/Penguin-Lunar-1.9.47-Source.zip)** contains the full application source and tests. `SOURCE-BUILD.txt` explains the separately obtained test fixtures. GitHub's automatic Source code downloads contain this documentation repository. **SHA256SUMS.txt** covers both ZIPs. Third-party mods retain their authorship and licenses; see the included notices.
