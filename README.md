# A50-ROM

Android 15 and 16 custom ROMs for the Samsung Galaxy A50.
Every ROM is one zip. You flash it once in TWRP.

- Device: Samsung Galaxy A50 (SM-A505F, codename a50dd, Exynos 9610)
- Maintainer: ibralyam (@Ibralyam)
- Contact: https://t.me/ibralyam

These are repacks. The ROM teams made the ROMs. I port them to the A50, build the installer, and test the zip.

## Downloads

Go to the Releases page. Each ROM version has its own release.

| ROM | Version | Android | Google apps | Details |
| --- | --- | --- | --- | --- |
| LineageOS | 23.2 | 16 | Gapps build | [ROMS.md](ROMS.md#lineageos-232) |
| RisingOS | 6.3 | 15 | BiTGApps ROAR | [ROMS.md](ROMS.md#risingos-63) |
| RestlessOS | 16.0 | 16 | None | [ROMS.md](ROMS.md#restlessos-160) |
| AxionOS | 2.9 | 16 | BiTGApps Core | [ROMS.md](ROMS.md#axionos-29) |
| InfinityX | 3.12 | 16 | BiTGApps Core | [ROMS.md](ROMS.md#infinityx-312) |
| crDroid | 12.12 | 16 | BiTGApps Core | [ROMS.md](ROMS.md#crdroid-1212) |
| PixelOS | 16.2 | 16 | Built in | [ROMS.md](ROMS.md#pixelos-162) |
| DerpFest | 16.2 | 16 | Built in | [ROMS.md](ROMS.md#derpfest-162) |
| Sakura | 16.3 | 16 | BiTGApps Core | [ROMS.md](ROMS.md#project-sakura-163) |
| Evolution X | 11.4 | 16 | Built in | [ROMS.md](ROMS.md#evolution-x-114) |

"Built in" means the GSI already has Google apps. The zip does not add any.

## What every zip does

The installer runs these steps in order:

1. Checks the payload and every image. Nothing is written yet.
2. Writes the vendor.
3. Runs MultiDisabler.
4. Writes the system (GSI).
5. Installs the Mint KernelSU kernel.
6. Copies the KernelSU Manager APK.
7. Runs the System Resizer.
8. Installs BiTGApps (only on zips that include it).

Newer zips also retry a failed write. If `dd` fails, the installer tries busybox `dd`, then `cat`.

## Common features

- Mint Kernel Beta (build 1413) with KernelSU (legacy)
- MultiDisabler v3.1 by Ian Macdonald. It disables FBE and encryption, vaultkeeperd, and stock recovery restore.
- Auto security patch shim for kernel compatibility
- System Resizer included
- KernelSU Manager APK included

## Quick install

1. Boot to TWRP.
2. Wipe Dalvik, System, Vendor, Cache and Data. Do not wipe internal storage.
3. Flash the zip from storage. Do not use ADB sideload.
4. Wait until you see "All done".
5. Reboot to system. The first boot takes a few minutes.

TWRP v3 is the recommended recovery. Full steps are in [INSTALL.md](INSTALL.md).

## Known issues

These do not work on AOSP ROMs for this phone:

- Fingerprint (FOD)
- Vibration (on some builds)
- Ultrawide camera
- Macro camera

Each ROM has its own list in [ROMS.md](ROMS.md).
The fingerprint tests are in [docs/FINGERPRINT.md](docs/FINGERPRINT.md).

## Documents

| File | What it covers |
| --- | --- |
| [INSTALL.md](INSTALL.md) | Step by step install, update and checks |
| [ROMS.md](ROMS.md) | Every ROM: version, dates, features, issues |
| [TROUBLESHOOTING.md](TROUBLESHOOTING.md) | Errors and fixes |
| [SOURCES.md](SOURCES.md) | Where each part comes from, and credits |
| [CHANGELOG.md](CHANGELOG.md) | Release history |
| [RELEASE_TEMPLATE.md](RELEASE_TEMPLATE.md) | Text for each GitHub release |

## Related

Hybrid TWRP for the A50: https://github.com/ibralyam/TWRP-A50

## Notice

You flash at your own risk. Back up your data first.
Do not redistribute these zips without credit.
