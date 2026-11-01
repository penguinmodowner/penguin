# Penguin 1.9.37 — clue tools and guard overlays

Download **[Penguin-Lunar-1.9.37.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.37/Penguin-Lunar-1.9.37.zip)** for Windows x64. Extract the entire ZIP and keep `Penguin.exe`, `app` and `runtime` together. Java is included. Requires **Lunar Fabric 1.21.11 and Fabric API**.

**Restart Minecraft before loading this update.** Existing settings are preserved. Use the same Penguin version in game windows sharing settings.

## New clue-scroll panel

- Enter MrMexican category numbers, then **Take** from the chest or **Put** into it. Custom category numbers, spaces, commas and ranges are supported; no reference scroll is needed.
- **Ore selection is required by default for ore-mining clues.** Pick one material, such as Redstone: different scroll tiers and required amounts match, while lapis, iron and gold stay put. Normal and deepslate forms share a material; your selected category numbers still apply. **Any ore** explicitly allows mixed materials. Other task types are unaffected.
- **Take all** and **Dump all** move recognized clue scrolls regardless of numbers or ore. Their **Include completed** switch starts OFF. Number-based Take/Put always exclude completed rewards.
- Assign separate **Take / Put keyboard shortcuts** in **K → Clues → Clue Scrolls → Controls**. They start unbound and work only in an open chest, without repeating while held or firing while typing or selecting an ore.
- Transfers use normal shift-clicks in one batch with **no added delay between items**. Server processing can still affect visible timing. Transfers stop when the destination fills or an item changes, briefly check for corrections, and do not automatically retry the batch.
- The compact panel replaces the previous reference/sorting interface. **More tools has been removed.** Number matching uses compatible **MrMexican 1.3.2**; Take all / Dump all work without it.

## Guard overlays and cleaner block tracers

- New **Visuals → Guards** section for guard, cell guard, enforcer and warden nametags and tracer lines, with individual type colors, range and style controls.
- Enabled Guards follow **J** by default, together with player/friend overlays. Turn off **Follow J toggle** to keep them independent; a separate configurable guard shortcut is also available.
- Guards start OFF on existing installs. These labels identify loaded NPCs and distance; they do not predict detection areas.
- Removed the **top-left Block Tracers status banner**. Outlines, tracer lines, block lists and presets remain available.

## Setup, validation and source

Prepare Lunar still offers optional **MrMexican 1.3.2** and **CosmicTextures 1.2**, both unchecked initially. Updating Penguin alone does not replace companions. Fully close Minecraft and Lunar before changing companion mods; see the bundled README and third-party notices.

**723 automated tests passed; one filesystem-link test was skipped.** The latest clue panel, shortcuts, J-linked guard overlays and banner removal still need final in-game checks. Earlier menu and waypoint checks do not validate every new transfer edge case.

**[Penguin-Lunar-1.9.37-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.37/Penguin-Lunar-1.9.37-Source.zip)** contains the application source and tests; `SOURCE-BUILD.txt` explains separately obtained test fixtures. GitHub's automatic Source code downloads contain this documentation repository. **SHA256SUMS.txt** covers both release ZIPs.
