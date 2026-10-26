# Penguin 1.9.28-preview.4 — shift-click clues and optional textures

Download **[Penguin-Lunar-1.9.28-preview.4.zip](https://github.com/eksimpkins/penguin/releases/download/v1.9.28-preview.4/Penguin-Lunar-1.9.28-preview.4.zip)** for Windows x64. Extract the entire ZIP and keep Penguin.exe, app and runtime together. Java is included. Requires Lunar Fabric 1.21.11 and Fabric API.

This is a **prerelease**. Restart Minecraft before loading it, and use the same Penguin build in game windows sharing settings.

## Clue scroll transfers

- **Dump clues** and **Collect matching** now use a normal shift-click per scroll stack. Items move between the chest and inventory without the previous pickup-and-place cursor sequence.
- Compatible stacks can merge. Transfers account for ping even with the delay set to 0.05 seconds. Exact server rollbacks receive up to two slower retries; unexpected inventory changes stop further clicks.
- Completed and unrecognized scrolls remain protected. Collection uses the reference in hotbar slot 1, with Exact/Similar matching. Lapis and redstone stay separate; matching deepslate variants can group together.
- Sort clues still rearranges items within the chest. The shift-click change applies to Dump and Collect.

## Prepare Lunar

- **MrMexican 1.3.2** is optional and unchecked by default. **Include CosmicTextures 1.2** is available alongside it, also unchecked by default. Both download the exact reviewed official releases.
- MrMexican setup backs up and removes old CosmicUtilities, CosmicPings and Penguin copies from the selected profile. CosmicTextures is kept/installed when included and removed when omitted. Lunar's other mods are preserved.
- Including CosmicTextures disables MrMexican's overlapping texture packs and its automatic Ground Zero/Prison Break pack switching. MrMexican automatic updates, automatic Papa Ping and Peaceful Mining are disabled by setup.
- Fully close Minecraft and Lunar, including its tray icon, before reviewing/installing companion changes. Updating Penguin alone does not change installed companions. Backups are stored under the profile's `penguin-mod-backups` folder.

Other preview additions include the white-concrete Vault preset, dynamic friend gangs and Raid Watch with an optional local Discord-bot relay. See the bundled README for setup and limits. No live Discord notification was sent during development.

## Validation and source

**564 automated tests passed across 61 suites; one filesystem-link test was skipped.** The packaged application files match the build. Shift-click transfers, the two-mod texture combination and other new preview features still need in-game testing. The user's initial MrMexican check looked good; that does not validate every feature.

The attached **Penguin-Lunar-1.9.28-preview.4-Source.zip** contains Penguin source and tests. Its `SOURCE-BUILD.txt` explains the optional mod fixtures needed by integration tests. GitHub's automatic Source code downloads contain this documentation repository. **SHA256SUMS.txt** covers both release ZIPs.

Companion mods retain their authorship and licenses; Penguin's MIT license applies to Penguin code. See `THIRD-PARTY-NOTICES.txt`. Static review is not a guarantee of safety. Manually creating a `/papa` group can still authenticate your Minecraft identity with its external service.
