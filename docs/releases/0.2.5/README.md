# Oblivion 0.2.5 — Windows beta candidate

This is a locally staged candidate. Installation, publication and distribution require separate approval after artifact review.

Planned download location, currently unpublished:

https://shawdow625.github.io/oblivion-updates/releases/0.2.5/Oblivion_0.2.5_x64-setup.exe

Before any approved installation, compare the installer SHA-256 with SHA256SUMS.txt:

```powershell
Get-FileHash -Algorithm SHA256 .\Oblivion_0.2.5_x64-setup.exe
```

Close Oblivion and Minecraft. Preserve the existing installation and launcher data; do not uninstall, delete instances or reset profiles. After an approved installation, verify Settings → About reports 0.2.5 and test normal launch/relaunch before sharing it.

The .exe.sig is the detached Tauri updater signature, bound to version 0.2.5. It is separate from Windows Authenticode publisher signing. This installer is not Authenticode-signed.

The production update feed remains inactive. Do not upload or activate a candidate manifest. Manual patch installation may be necessary because the tested 0.2.4 application crashes during startup.
