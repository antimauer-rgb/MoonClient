# MoonClient development status (2026-10-22)

## Confirmed locally by the user
- Standalone **OptiFine 1.8.9** is working. Do not overwrite its installed version.
- Minecraft 1.8.9 and Forge can start with Java 8 and Microsoft Premium authentication.
- A Forge log listed 3 active JARs from launcher (including moonclient-hud.jar and Xaero's mods), but FML only found its 3 built-in mods. Check the actual game directory and mod discovery.
- RSHIFT MoonHUD currently does **not** work reliably.
- Earlier npm install with `@xmcl` package version failed with `EUNSUPPORTEDPROTOCOL workspace:^*`.

## Next tasks
1. Sync current Windows source tree, not outdated generated ZIP; audit code and tests.
2. Add simple version names and choice of Vanilla/Forge/Fabric where supported: 1.8.9 Vanilla, 1.8.9 OptiFine, 1.8.9 Forge, 26.2 Vanilla, 26.2 Fabric.
3. Per-profile persistent game directories, mods, config, options.txt, resourcepacks and saves; safe one-time migration from `mods` and `mods-1.8.9`, no implicit deleting.
4. Modrinth browser only for loader-supporting Forge/Fabric profiles; correct downloads and dependencies.
5. Build functioning Forge MoonHUD with ~30 real features, polished MoonClient click-GUI, HUD editor and RSHIFT. Standalone OptiFine requires its own LaunchWrapper adapter; Fabric separate adapter.
6. Add repair/reinstall/version cleanup commands with explicit confirmation, backups and no account/worlds deletion.
7. Verify UI including compact Play and launch animation tied to actual progress.

## Repository state
This GitHub repository was previously empty except README and .gitignore. Current authoritative app files are on user's computer: `C:\Users\toNy\Desktop\projekt\MoonClient`. The GitHub integration cannot read that local directory directly. Source import must be run locally using provided secure PowerShell uploader.

## Boundaries
MoonClient is distinct from Hone Optimizer (amber system optimization app). Do not conflate them.
