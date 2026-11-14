[Download Penguin 1.9.65 for Windows](https://github.com/penguinmodowner/penguin/releases/download/v1.9.65/Penguin-Lunar-1.9.65.zip) · Requires Lunar Fabric 1.21.11 and Fabric API. Java is included.

### Automatic pickaxe absorption

In **K → Mining → Gen Mining → Cycle**, enable **Auto absorb full pickaxe**. It starts OFF for new and existing setups until you enable it. An already-saved selection from 1.9.64 is kept.

- During a running mining cycle, the server's **Your pickaxe is full of energy!** warning stops mining immediately.
- Penguin takes an **Absorber** from your inventory and applies it to the held pickaxe using the normal drag-and-drop inventory action.
- Keep **one inventory slot empty** for extracted energy.
- Mining resumes on the same block and layer only after the server confirms lower energy, one consumed absorber, and an empty cursor after storing any remainder.
- Missing absorbers, unexpected inventory changes, or an unconfirmed extraction stop the cycle. Check your inventory before restarting. Inventory clicks are not blindly retried.
- Works with the existing one-layer and **Move up and repeat** cycles. It does not automate extraction during ordinary manual mining.

### Adjustable pause

**Pause before absorbing** is directly under the absorber switch. Choose **0–10 seconds**, with a **1-second default**. Mining stays stopped during the pause, before any inventory click. The pause saves with your preferences and settings profiles. Manual input or F8 still cancels the cycle.

### Updating

Extract the entire Windows ZIP into a new folder, close any chest/inventory, open **Penguin.exe**, select your game and click **Update Penguin**. Compatible versions update without restarting Minecraft. Running automation stops during the update; saved settings remain. Use the same version in games sharing settings. Versions 1.9.47 or earlier and failed initializations require a Minecraft restart. Companion mods are unchanged by this update.

### Validation and source

**914 tests passed, one skipped, no failures or errors.** The live update preserved settings, and both automatic absorption and the adjustable pause were confirmed in game by the tester. Regression checks cover delayed server responses, interruption, pause timing, and existing settings/profile migration.

[Application source and tests](https://github.com/penguinmodowner/penguin/releases/download/v1.9.65/Penguin-Lunar-1.9.65-Source.zip) are attached separately. GitHub's automatic Source code downloads contain the documentation repository. **SHA256SUMS.txt** covers both ZIPs. Personal settings, friend lists and game logs are not bundled.
