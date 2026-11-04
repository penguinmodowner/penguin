# Penguin 1.9.43 — remembered terrain and Elite Bandit nametags

Download **[Penguin-Lunar-1.9.43.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.43/Penguin-Lunar-1.9.43.zip)** for Windows x64. Extract the entire ZIP and keep `Penguin.exe`, `app` and `runtime` together. Java is included. Requires **Lunar Fabric 1.21.11 and Fabric API**.

**Restart Minecraft before loading this update.** Existing Penguin settings are preserved. Use the same Penguin version in game windows sharing settings.

## Remembered terrain

**Prepare Lunar now offers Bobby**, independently of MrMexican. Check **Bobby — remember terrain you've visited** to install the same official **5.2.11.1+mc1.21.11** version tested in Lunar. All optional mods start unchecked.

1. Fully close Minecraft and Lunar, including its tray icon.
2. Open Penguin 1.9.43 → **Prepare Lunar**, check **Bobby**, select your Fabric 1.21.11 profile, then **Review selected mods → Install selected mods**.
3. Relaunch Lunar. In Minecraft's video settings, try **16 chunks** render distance, then explore and look back.

Bobby keeps terrain you have already visited visible beyond the server's chunk distance. It does not provide unseen terrain or live distant players/guards. Cached scenery can be outdated until the server sends that area again. Penguin's block tracers, inspector, generator actions and block alerts use live chunks only.

New Bobby installs get multiple-world matching, seven-day unused-region expiry, cached block entities disabled, and a render-distance slider maximum of 32 chunks. The actual video distance stays unchanged. Existing Bobby settings and caches are preserved. Updating Penguin alone does not install Bobby; use Prepare Lunar once. Bobby has its own settings and remains active independently of Stop Penguin.

## Elite Bandit nametags and tracers

Enable **K → Visuals → Nametags → Display → Include elite bandits**. This starts **OFF** and adds recognized Elite Bandit NPC bodies to the normal nametags and tracer lines.

- Follows **J**, the normal tracer switch, range, colors, size, screen-edge and through-block settings.
- Recognizes the NPC's Elite Bandit label instead of hardcoding its generated account suffix; excludes separate floating text decorations.
- Saves and syncs with Penguin settings and exported profiles. Aim Assist targeting stays unchanged.

The existing clue-scroll panel, chest counts, Take/Put shortcuts and six-material ore selector are retained. **Clear Distance Fog** is also available under Visuals, off by default, for terrain already available to the client. Distant-player diagnostic tools and recordings are not included.

## Validation and source

**753 automated tests passed; one filesystem-link test was skipped.** Installer checks covered Bobby alone, all three optional companions together, preserved settings, repeat installation, changed settings after review and rollback when Lunar starts. The setup dialog was visually checked. The exact Bobby release was tested in Lunar and farther terrain was confirmed in game. Elite Bandit identification was checked against a live server sample; the final Elite Bandit overlay still needs an in-game visual check.

**[Penguin-Lunar-1.9.43-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.43/Penguin-Lunar-1.9.43-Source.zip)** contains the application source and tests; `SOURCE-BUILD.txt` explains the three separately obtained test fixtures. GitHub's automatic Source code downloads contain this documentation repository. **SHA256SUMS.txt** covers both release ZIPs. Third-party downloads retain their own authorship and licenses; see the included notices.
