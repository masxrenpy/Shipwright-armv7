# Changelog – Android 32-bit (armv7) beta

## v9.2.3-armv7-beta.2
- The app keeps `oot.o2r` when updating (no need to extract the ROM again); the files that ship inside the APK are refreshed on every new build.
- "Fix Vanishing Paths" now defaults to **No Vanish** on Android.
- Crash and bug-report logs in `SOH/logs/`: `device-info.txt`, `exit-reasons.txt` (Android 11+), `java-crash.txt`, `native-crash.txt`. Diagnostic files above 1 MB are removed at startup.
- Clearer message while the ROM is being extracted.
- New FAQ (`docs/ARMV7_BETA.md`) and an issue form for bug reports.

## v9.2.3-armv7-beta.1
- First public beta: `armeabi-v7a` build with the NEON audio mixer fix, automatic ROM detection in `SOH`, a more robust file picker and a rendering fix for PowerVR GPUs.
