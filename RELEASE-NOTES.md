[Download Penguin 1.9.63 for Windows](https://github.com/penguinmodowner/penguin/releases/download/v1.9.63/Penguin-Lunar-1.9.63.zip) · Requires Lunar Fabric 1.21.11 and Fabric API. Java is included.

### Mining layer repeat

In **K → Mining → Gen Mining → Cycle**, enable **Move up and repeat**. Start already flying using the server's flight ability, aim at the first generator and press your configured cycle key. Penguin finishes four blocks, rises one block, then repeats at the next layer until no unfinished block is ahead.

- Off by default; existing one-layer behavior remains when disabled.
- Uses the selected Prismarine or Legendary completion pattern.
- F8 or manual input cancels it. Blocked ascent, lost flight, changed worlds or interrupted movement stop the run.
- The completion alert plays once at the end. Existing background mining and verification pause/resume remain available.

### Nametags and saved settings

- **Visuals → Nametags → Display → Show player nametags** hides labels independently of tracer lines. J remains the master overlay toggle.
- Overlay positioning now follows the actual rendered view, including zoom.
- Fixes the settings migration that could make the local 1.9.61 build fall back to old friend/preferences data. Existing saves and exported profiles are preserved; the new layer setting starts off.

### Updating

Extract the entire Windows ZIP into a new folder, close any chest/inventory, open the new **Penguin.exe**, select your game and click **Update Penguin**. Compatible versions update without restarting Minecraft. Active automation stops during updating; saved settings remain. Use the same version in games sharing settings. Versions 1.9.47 or earlier and failed initializations require a Minecraft restart. Companion mods are not updated by loading Penguin.

### Validation and source

**895 tests passed, one skipped, no failures or errors.** The live update to 1.9.63 succeeded and the layer-repeat behavior was confirmed in game. Tests cover repeated layers, empty-layer completion, cancellation, blocked/lost flight, verification pauses and settings/profile migration.

[Application source and tests](https://github.com/penguinmodowner/penguin/releases/download/v1.9.63/Penguin-Lunar-1.9.63-Source.zip) are attached separately; GitHub's automatic Source code downloads contain the documentation repository. **SHA256SUMS.txt** covers both ZIPs. Personal settings, friend lists and game logs are not bundled.
