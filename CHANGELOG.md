# Changelog – Android 32-bit (armv7) beta

## v9.2.3-armv7-beta.3
- Fixed the first-launch hang on Android 6-10: after granting the storage permission the setup now continues (no need to close and reopen the app).
- The ROM file picker is gone on Android: the app asks you to copy the ROM to the `SOH` folder and scans it again when you press **Retry**.
- The app is now called "Ship of Harkinian (32-bits)". The game folder is still `SOH`.

## v9.2.3-armv7-beta.2
- The app keeps `oot.o2r` when updating (no need to extract the ROM again); the files that ship inside the APK are refreshed on every new build.
- "Fix Vanishing Paths" now defaults to **No Vanish** on Android.
- Crash and bug-report logs in `SOH/logs/`: `device-info.txt`, `exit-reasons.txt` (Android 11+), `java-crash.txt`, `native-crash.txt`. Diagnostic files above 1 MB are removed at startup.
- Clearer message while the ROM is being extracted.
- New FAQ (`docs/ARMV7_BETA.md`) and an issue form for bug reports.

## v9.2.3-armv7-beta.1
- First public beta: `armeabi-v7a` build with the NEON audio mixer fix, automatic ROM detection in `SOH`, a more robust file picker and a rendering fix for PowerVR GPUs.
