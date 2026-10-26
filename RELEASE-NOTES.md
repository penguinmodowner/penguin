# Penguin 1.9.28-preview.5 — clue-scroll fixes and inventory cleanup

Download **[Penguin-Lunar-1.9.28-preview.5.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.28-preview.5/Penguin-Lunar-1.9.28-preview.5.zip)** for Windows x64. Extract the entire ZIP and keep Penguin.exe, app and runtime together. Java is included. Requires Lunar Fabric 1.21.11 and Fabric API.

This is a **prerelease**. Restart Minecraft before loading it, and use the same Penguin build in game windows sharing settings.

## Fixed clue eligibility

- **Dump clues** and **Collect matching** now recognize the combined **“COMPLETE! Right-click to claim rewards!”** footer from the reported Elite and Uncommon scrolls. Completed rewards stay out of transfers even when an older task remains or strikethrough formatting is missing.
- Completed checkmarks after bullets or task text are protected. Wrapped lines cannot make completed or unknown tasks appear unfinished again; valid unfinished wrapped tasks retain their full requirements.
- Unfinished **Lose, Join, Attack, Discover, Level up, Fail, Reveal and Receive** tasks are now recognized, fixing skipped valid scrolls.

## Collect matching cleanup

- After collection finishes successfully, a matching unfinished scroll stack in **hotbar slot 2** moves into the **first free upper-inventory slot**. The reference in **slot 1** remains in place.
- If the upper inventory is full, slot 2 stays put. Completed scrolls, unrelated items and nonmatching stacks are not moved. Stopping collection cancels this final move too.

## Included from preview 4

- Dump and Collect shift-click one scroll stack at a time, support compatible merging and pace transfers for connection lag. Exact server rollbacks get up to two slower retries; unexpected inventory changes stop further clicks. Sort clues still rearranges items within the chest.
- **Prepare Lunar:** optional **MrMexican 1.3.2** and **Include CosmicTextures 1.2** are both unchecked by default. Setup downloads the pinned official releases, backs up superseded Cosmic/Penguin copies and preserves unrelated Lunar mods. Including Textures disables MrMexican's overlapping texture packs and automatic Ground Zero/Prison Break pack switching. MrMexican automatic updates, automatic Papa Ping and Peaceful Mining are disabled by setup.
- Fully close Minecraft and Lunar, including its tray icon, before installing companion changes. Updating Penguin alone does not update companions. Backups are stored under the profile's `penguin-mod-backups` folder.
- The white-concrete Vault preset, dynamic friend gangs and Raid Watch with an optional local Discord-bot relay remain included. See the bundled README for setup and limits. No live Discord notification was sent during development.

## Validation and source

**601 automated tests passed across 63 suites; one filesystem-link test was skipped.** New regression checks cover the reported completed tooltips, missing task verbs, wrapped tasks, transfer selection and the final hotbar move. The user confirmed the clue-scroll update works after loading preview 5. This does not validate every inventory edge case, companion combination or other preview feature.

The attached **Penguin-Lunar-1.9.28-preview.5-Source.zip** contains Penguin source and tests. Its `SOURCE-BUILD.txt` explains the optional mod fixtures needed by integration tests. GitHub's automatic Source code downloads contain this documentation repository. **SHA256SUMS.txt** covers both release ZIPs.

Companion mods retain their authorship and licenses; Penguin's MIT license applies to Penguin code. See `THIRD-PARTY-NOTICES.txt`. Static review is not a guarantee of safety. Manually creating a `/papa` group can still authenticate your Minecraft identity with its external service.
