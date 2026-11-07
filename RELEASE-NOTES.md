Download **[Penguin-Lunar-1.9.56.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.56/Penguin-Lunar-1.9.56.zip)** for Windows x64. Extract the entire ZIP and keep `Penguin.exe`, `app` and `runtime` together. Java is included. Requires **Lunar Fabric 1.21.11 and Fabric API**.

**Existing settings are preserved.** Features start OFF only on a first installation with no saved Penguin settings. The new PvE target mode starts OFF for everyone until enabled.

## PvE Aim Assist

In **K → Combat → Aim Assist**, enable **PvE enemies instead of players** to aim at recognized CosmicPrisons normal, elite and blood bandits, werewolves and escapees.

- Player and PvE targeting are separate modes. Listed players, friends, guards, wardens, enforcers, unrelated NPCs and floating labels stay excluded in PvE mode.
- Existing smoothing, aim height, range, maximum angle, visibility and held-weapon choices remain. The naked/target-sword filter applies only to player targeting.
- Enable **Aim Assist** and **Left Clicker**, then physically hold left-click to activate assistance. This changes aim selection; it does not add attack reach or prevent manual attacks on other entities.
- NPC detection uses the body's own label and matching identity instead of a fixed generated account suffix. Ordinary ore-name labels need additional NPC evidence.

## Clue buttons in player vaults

With **Clue Scrolls** enabled, opening **`/pv` or `/pv <number>`** shows compact **Pull all clues / Dump all clues** buttons at the bottom of the open vault. They transfer recognized clues between that vault and your inventory, following the existing **Include completed** switch. The large number panels remain hidden in vaults, and the vault selector itself has no transfer buttons.

Includes the fix for a crash when closing a vault with no focused button. Normal chest controls remain on the left with quantity counts above the chest, following Minecraft GUI Scale.

## Updating

Extract the new ZIP into its own folder, close any chest/inventory, open the new **Penguin.exe**, select your game and click **Update Penguin**. Keep Minecraft visible while resources reload. Compatible loaded versions update without restarting Minecraft; active automation stops and saved settings remain. Update each running game separately and use the same Penguin version in games sharing settings.

**Coming from 1.9.47 or earlier, or a failed initialization? Restart Minecraft once** before loading. Companion mod changes also require a restart. Do not overwrite the running version's folder. This release does not install or update Guard Lab or other companions automatically.

## Checks and source

**839 automated tests: 838 passed, 1 skipped, no failures or errors.** The packaged files match the tested build. A live update from **1.9.55 to 1.9.56** succeeded without restarting Lunar and preserved settings. The vault fix was confirmed in game. Enemy recognition tests include a captured Elite Bandit identity; the newly added blood-bandit and werewolf variants still need live confirmation.

**[Penguin-Lunar-1.9.56-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.56/Penguin-Lunar-1.9.56-Source.zip)** contains the full application source and tests. `SOURCE-BUILD.txt` explains separately obtained test fixtures, and `HOT-UPDATES.md` documents runtime replacement. GitHub's automatic Source code downloads contain the documentation repository. **SHA256SUMS.txt** covers both ZIPs. Third-party mods retain their original authorship and licenses.
