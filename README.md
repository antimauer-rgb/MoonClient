# MoonClient

MoonClient is a custom **Minecraft Java Edition** launcher built with **Electron, Node.js, Tailwind CSS**, and a Minecraft runtime. It includes Microsoft Premium login, a standalone OptiFine 1.8.9 profile, and work-in-progress Forge/Fabric support with an in-game MoonHUD (RSHIFT).

**Development status:** The user's Windows project is newer than this remote repository. Full application sources must be synced from their local folder before treating this repository as the source of truth. The user confirmed that standalone OptiFine 1.8.9 currently works locally; don't overwrite that installation.

## Roadmap
- Stable version profiles: `1.8.9 Vanilla`, `1.8.9 OptiFine`, `1.8.9 Forge`, `26.2 Vanilla`, `26.2 Fabric`.
- Isolated instance directories with persistent mods, `options.txt`, resource packs, and saves per profile.
- Mod browser only for Forge/Fabric.
- Lunar-inspired, original purple/cyan MoonHUD GUI with RSHIFT, 30+ functioning features, and in-game HUD editor; adapters per loader/version.
- Safe version repair, reinstall, and cache cleanup with backups and explicit confirmation.

## Design
Dark Violet premium visual system, Minecraft night-world art, small Play button, Moon Orbit launch animation, custom purple scrollbars. No fake statuses or nonfunctional placeholder controls.

## Setup
Once the actual sources are uploaded, review `package.json` and the lockfile before `npm install`. Earlier `@xmcl` versions failed on `workspace:^*`. Follow the accompanying [project status](docs/PROJECT_STATUS.md) and [agent instructions](AGENTS.md).

## Security
The repository is **public**. Never upload `%APPDATA%\.moonclient`, accounts, Microsoft tokens, OptiFine or other downloaded third-party JARs, worlds, local runtime files, or logs. The `.gitignore` is intentionally strict.
