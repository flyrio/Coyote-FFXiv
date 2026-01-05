# AGENTS.md

- Project type: Dalamud plugin (FFXIV CN).
- Entry point: `Coyote-FFXiv/Plugin.cs`.
- UI files: `Coyote-FFXiv/Windows`, helpers in `Coyote-FFXiv/Utils`.
- Build: `dotnet build Coyote-FFXiv/Coyote-FFXiv.csproj -c Release` (requires Dalamud.CN.NET.SDK 14.0.1, .NET 10 SDK, and the local ECommons.dll reference).
- Config files live in the Dalamud plugin config dir: `chatTriggerRules.json`, `hpTriggerRules.json`, `BuffTriggerConfig.json`.
- When editing fire logic, keep the request JSON shape: `strength`, `time`, `override`, `pulseId`.
