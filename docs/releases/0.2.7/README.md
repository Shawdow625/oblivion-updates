# Oblivion 0.2.7 Windows v2 candidate

Installer: Oblivion_0.2.7_x64-setup.exe

SHA-256: 676c9537e6b99b2a4dd7697986c4b758d735cbdd3d235dc27941fdafafa4f493

At preparation time native automatic-update/clean-install/recovery acceptance is pending. Later qualification/distribution requires a separate owner decision. Published bytes are immutable.

# Oblivion Windows v2 — installation and update instructions

**Release-review draft: neither candidate is approved for friends distribution yet.** Follow these steps only for an expressly approved installation in the named disposable test VM. Ordinary users should wait for the owner's final release link.

1. Download the exact owner-approved version from `https://shawdow625.github.io/oblivion-updates/releases/0.2.7/`, together with its README/checksums. Run `Get-FileHash -Algorithm SHA256 -LiteralPath '<installer>'` in PowerShell and compare every hexadecimal character with the owner's reviewed hash. Stop on any mismatch.
2. Close Minecraft and the launcher normally. Before any upgrade, back up the stopped launcher data plus every separately selected instance folder. Retain previous backups; never delete `.minecraft`, worlds or launcher data as an installer workaround.
3. Run the reviewed **Oblivion** Windows x64 installer normally as the intended Windows user. Keep the existing directory during an authorized upgrade. The real production identifier is `com.oblivion.client`; **Oblivion Updater Lab** installers are outside this channel.
4. Current candidates have a Tauri Ed25519 updater signature, separately verified against the owner's permanent key and exact version. Windows Authenticode signing remains absent; Windows may show unknown-publisher/SmartScreen warnings or block execution. Do not disable protections or bypass policy. Stop and contact the owner if Windows blocks the reviewed installer.
5. Open the installed application, confirm the approved About version, Home/Library/Settings rendering, correct settings and instance locations, then quit and relaunch normally. Do not sign into personal accounts or launch Minecraft during the synthetic updater trial.
6. Corrected 0.2.7/0.2.8 builds check the **beta/v2** channel automatically at startup. Review the available version, notes and download size; use **Later** to defer or **Check for Updates** in About to review again. An unavailable feed is not a successful up-to-date check.
7. Close Minecraft and click **Update & Restart**. Observe genuine download progress, signature verification, native installer handoff and automatic relaunch. Confirm the new About and executable version. Do not manually start the successor installer or restart the application to turn a failed automatic update into a pass.
8. If an update fails, preserve the error, timestamp, installed version and data. Do not repeatedly run installers, uninstall/reset data, force a downgrade or restore over a newer schema. Recovery needs the owner's separately reviewed instructions.

Windows defaults: `%LOCALAPPDATA%\Oblivion\oblivion.exe`, `%APPDATA%\com.oblivion.client`, and local/WebView data under `%LOCALAPPDATA%\com.oblivion.client`. External instance storage must also be included in backups. Account encryption may bind recovery to the same Windows login; copying a profile is not a verified account migration.

Existing 0.2.4/0.2.5 clients keep the original inactive `beta/latest.json` endpoint and do not discover this v2 feed through it. Their first automatic-update compatibility remains unverified; use an explicitly approved corrected baseline rather than expecting a successor to repair old code before handoff. Published historical bytes remain immutable.

GitHub Pages installers, signatures, notes and manifests are publicly readable and may remain cached after deletion. Never include personal data, secrets, private signing material or confidential assets. macOS remains a separate future release requiring native Apple Silicon and Intel qualification.
