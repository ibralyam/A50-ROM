# Release Template

Use one release per ROM version.

- Tag: `lineageos-23.2` (name in lowercase, then the version)
- Title: `LineageOS 23.2 (Android 16) for Galaxy A50`
- Assets: the zip, and `SHA256SUMS.txt`
- Keep the KernelSU Manager APK as a separate asset.

## Release body

```
ROM NAME VERSION (Android XX) for Galaxy A50 (a505f)
Repacker: @Ibralyam
Build date: YYYY-MM-DD
Date published: YYYY-MM-DD

Downloads
ROM | TWRP | KernelSU Manager

Features
- ...
- Mint Kernel Beta (build 1413) with KernelSU (legacy)
- MultiDisabler v3.1 by Ian Macdonald
- Auto security patch shim for kernel compatibility
- System Resizer included

Known issues
- ...

Flashing guide
1. Boot to TWRP.
2. Wipe Dalvik, System, Vendor, Cache and Data. Do not wipe internal storage.
3. Flash the zip from storage. Do not use ADB sideload.
4. Wait until it says "All done".
5. No manager icon? Install KernelSU.apk from /storage/emulated/0/Download/

SHA-256
<paste the value here>

Notes
- ...

Source
Vendor, GSI, Kernel, KernelSU Manager, MultiDisabler, System Resizer
Details: SOURCES.md
```

## Checklist before you publish

- Zip name has no spaces.
- SHA-256 matches `SHA256SUMS.txt`.
- The ROM table in README.md and ROMS.md has the new row.
- CHANGELOG.md has the new line.
