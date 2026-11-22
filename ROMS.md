# ROM List

All ROMs are repacked for the Galaxy A50 (a505f). Dates are year, month, day.

| ROM | Version | Android | Built | Published | Project no. |
| --- | --- | --- | --- | --- | --- |
| LineageOS | 23.2 | 16 | 2026-11-01 | 2026-11-08 | 1 |
| RisingOS | 6.3 | 15 | 2026-11-06 | 2026-11-10 | 2 |
| RestlessOS | 16.0 | 16 | 2026-11-11 | 2026-11-12 | 3 |
| AxionOS | 2.9 | 16 | 2026-11-12 | 2026-11-12 | 4 |
| InfinityX | 3.12 | 16 | 2026-11-13 | 2026-11-13 | 5 |
| crDroid | 12.12 | 16 | 2026-11-13 | 2026-11-14 | 6 |
| PixelOS | 16.2 | 16 | 2026-11-14 | 2026-11-15 | 7 |
| DerpFest | 16.2 | 16 | 2026-11-15 | 2026-11-15 | 8 |
| Project Sakura | 16.3 | 16 | 2026-11-16 | 2026-11-16 | 9 |
| Evolution X | 11.4 | 16 | 2026-11-17 | 2026-11-18 | 10 |

## Shared by every zip

- Mint Kernel Beta (build 1413) with KernelSU (legacy)
- MultiDisabler v3.1 by Ian Macdonald
- Auto security patch shim for kernel compatibility
- System Resizer
- Flash from storage. Do not use ADB sideload.

## LineageOS 23.2

- Android 16. GSI based. Gapps build.
- Variants: EROFS and EXT4.
- Google TTS crash fix (experimental).
- KernelSU Manager is copied to `/data/app`.
- Known issues: fingerprint, ultrawide camera, macro camera.
- Note: this is the first project.

## RisingOS 6.3

- Android 15.
- RisingOS Settings. Gapps build with BiTGApps ROAR (A15).
- KernelSU Manager is copied to `/data/app`.
- Known issues: fingerprint, ultrawide camera, macro camera.
- Note: better to use TWRP v3.

## RestlessOS 16.0

- Android 16. GrapheneOS-based GSI.
- Known issues:
  - Fingerprint, ultrawide camera, macro camera.
  - No verified boot.
  - No Auditor.
  - USB protection does not work.
  - hardened_malloc is replaced by Scudo, and more.
- Notes:
  - This is not as secure as real GrapheneOS.
  - Not recommended for daily use.
  - Better to use TWRP v3.

## AxionOS 2.9

- Android 16. Gapps build with BiTGApps Core (A16).
- If `dd` fails, the installer tries busybox `dd`, then `cat`.
- KernelSU Manager is copied to `/data/app`.
- Known issues: fingerprint, ultrawide camera, macro camera.
- Note: better to use TWRP v3.

## InfinityX 3.12

- Android 16. Infinity Suite and Gapps build with BiTGApps Core (A16).
- If `dd` fails, the installer tries busybox `dd`, then `cat`.
- The setup wizard is already skipped.
- Known issues: fingerprint, ultrawide camera, macro camera.
- Note: better to use TWRP v3.

## crDroid 12.12

- Android 16. crDroid Settings and Gapps build with BiTGApps Core (A16).
- If `dd` fails, the installer tries busybox `dd`, then `cat`.
- Known issues: fingerprint, ultrawide camera, macro camera.
- Note: better to use TWRP v3.

## PixelOS 16.2

- Android 16.
- If `dd` fails, the installer tries busybox `dd`, then `cat`.
- Known issues: vibration, ultrawide camera, macro camera.
- Note: better to use TWRP v3.

## DerpFest 16.2

- Android 16. DerpFest Settings. Gapps build, already built in.
- If `dd` fails, the installer tries busybox `dd`, then `cat`.
- Known issues: vibration, ultrawide camera, macro camera.
- Note: better to use TWRP v3.

## Project Sakura 16.3

- Android 16. Sakura Settings. Gapps build with BiTGApps Core.
- If `dd` fails, the installer tries busybox `dd`, then `cat`.
- Known issues: vibration, ultrawide camera, macro camera.
- Note: better to use TWRP v3.

## Evolution X 11.4

- Android 16. Evolver. Gapps build, already built in.
- If `dd` fails, the installer tries busybox `dd`, then `cat`.
- Known issues: vibration, ultrawide camera, macro camera.
- Note: better to use TWRP v3.
