# Oblivion 0.2.5 — Windows friends beta candidate

Fixes a startup crash when an optional runtime-information file could not be saved. That diagnostic failure now produces a warning instead of aborting application setup.

Existing launcher features, companion, seven cosmetic packs, themes and HUD settings are retained. Application identity, user-data locations, updater verification key and HTTPS hosting endpoint are unchanged.

This candidate requires separate installation-and-launch acceptance before distribution. The corrected development build passed Home, Library, Settings, About and normal close/relaunch checks; that does not substitute for testing this exact installer.

Automatic updates remain inactive. A manual patch installation may be needed for the previously published 0.2.4, which crashes on the tested PC. Genuine automatic updating, clean-machine WebView prerequisites and interrupted-installation recovery remain unverified.

Windows x64 only. The Tauri updater signature is separate from Windows Authenticode publisher signing; this candidate is not Authenticode-signed.
