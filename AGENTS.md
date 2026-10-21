# Instructions for Codex / coding agents

Read `README.md`, `docs/PROJECT_STATUS.md`, and `docs/CODEX_CONTINUATION_PROMPT.md` first. Audit actual sources; previous plans are not proof of an implemented feature.

- Preserve existing working standalone OptiFine 1.8.9, versions, worlds, profiles and settings.
- Never implicitly delete, replace or synchronize user mods across loaders. Separate instance for each version/loader.
- Microsoft Premium OAuth only; securely encrypt stored sessions. Never log/store plaintext credentials.
- MoonHUD needs an actual compiled, valid, tested adapter to be considered supported.
- Forge 1.8.9, OptiFine standalone, and Fabric each need a compatible in-game integration; do not pretend Forge mods work in standalone OptiFine.
- Verify JavaScript, PowerShell and ForgeGradle builds; test launching and mods discovery on target Windows.
- Publish no runtime folders, secrets, downloaded mods/JARs, user logs or backup data.
- Original MoonClient dark-violet design, compact Play button, Moon Orbit loading indicator, custom scrollbars.
- Keep changes atomic with concise tests and honest status.
