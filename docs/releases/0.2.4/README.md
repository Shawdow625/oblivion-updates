# Oblivion 0.2.4 — Windows friends beta

Download the reviewed installer from:

https://shawdow625.github.io/oblivion-updates/releases/0.2.4/Oblivion_0.2.4_x64-setup.exe

Compare its SHA-256 with SHA256SUMS.txt before running it. In PowerShell: Get-FileHash -Algorithm SHA256 .\Oblivion_0.2.4_x64-setup.exe

Close Oblivion and Minecraft before installation. Preserve your existing installation and data; do not uninstall or delete instances. After installation, check Settings → About for 0.2.4.

The .exe.sig is the detached Tauri updater signature. Tauri verifies publisher signatures and the announced version for future in-app updates. This is separate from Windows Authenticode publisher signing; this installer is not Authenticode-signed.

The updater feed is intentionally inactive until a newer approved version is ready. Genuine automatic update/install/restart, clean-install acceptance and interrupted-upgrade acceptance remain unverified.

This is an early Windows beta. Local verification did not install it or change existing launcher or Minecraft data.
