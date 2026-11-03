# Penguin 1.9.39 — chest clue counts and quick hide

Download **[Penguin-Lunar-1.9.39.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.39/Penguin-Lunar-1.9.39.zip)** for Windows x64. Extract the entire ZIP and keep `Penguin.exe`, `app` and `runtime` together. Java is included. Requires **Lunar Fabric 1.21.11 and Fabric API**.

**Restart Minecraft before loading this update.** Existing settings are preserved. Use the same Penguin version in game windows sharing settings.

## Chest clue counts

- A new **CHEST CLUES** sidebar on the right of an open chest lists each MrMexican category number and how many scrolls of that number are inside.
- Counts update as the chest changes, combine tiers and ore materials, and count stacked quantities. They exclude your inventory, completed rewards and unnumbered items; your Take/Put filters do not change the counts.
- Long lists can be scrolled or paged with the arrow buttons. Counts require compatible **MrMexican 1.3.2**, including its customized category numbers.

## Hide until the next chest

- Click **x** on the clue tools panel to hide both the tools and counts for the current chest opening.
- Reopening a chest restores them automatically. This does not change the Clue Scrolls switch or saved settings. Take/Put shortcuts are inactive while the panel is hidden.

## Simpler ore choices

- The ore materials are now **Iron, Lapis, Redstone, Gold, Diamond, Emerald**, in that order.
- **Choose ore…** and **Any ore** remain separate controls. Selecting one material accepts different clue tiers and required amounts while keeping other materials out. Normal and deepslate forms share a material; your selected category numbers still apply.
- Saved selections for removed materials return to **Choose ore…**, so ore-mining clues stay put until you pick a supported material.

Number-based Take/Put, configurable shortcuts, Take all / Dump all, and the Include completed switch remain available. Number-based actions always skip completed rewards. **More tools remains removed.**

## Validation and source

**727 automated tests passed; one filesystem-link test was skipped.** The release loaded successfully in Lunar 1.21.11. The new sidebar layout and temporary hide interaction still await a live chest check. The packaged application files were verified against the successful build.

Prepare Lunar continues to offer optional **MrMexican 1.3.2** and **CosmicTextures 1.2**, both unchecked initially. Updating Penguin alone does not replace companion mods. See the bundled README and third-party notices for setup.

**[Penguin-Lunar-1.9.39-Source.zip](https://github.com/penguinmodowner/penguin/releases/download/v1.9.39/Penguin-Lunar-1.9.39-Source.zip)** contains the application source and tests; `SOURCE-BUILD.txt` explains separately obtained test fixtures. GitHub's automatic Source code downloads contain this documentation repository. **SHA256SUMS.txt** covers both release ZIPs.
