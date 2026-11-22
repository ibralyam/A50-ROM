# Install Guide

For the Samsung Galaxy A50 (SM-A505F, a50dd) only.

## Before you start

- The bootloader must be unlocked.
- You need TWRP. TWRP v3 is recommended.
- Battery must be above 50 percent.
- Back up your data.
- Keep the zip on the SD card, or send it to the phone with MTP after you wipe.
  Do not wipe internal storage, or the zip will be gone.

## Check your download

```
sha256sum Name.zip
```

The value must match the one in the release notes.

## Install

1. Boot to TWRP.
2. Tap Wipe, then Advanced Wipe.
3. Select Dalvik, System, Vendor, Cache and Data. Swipe to wipe.
   Do not select internal storage.
4. Go back, tap Install, and pick the zip.
5. Swipe to flash. Do not use ADB sideload.
6. Wait. The screen shows progress messages. The flash takes several minutes.
7. When you see "All done", tap Reboot, then System.
8. The first boot can take up to 10 minutes.

## After the first boot

- No KernelSU Manager icon? Install `KernelSU.apk` from `/storage/emulated/0/Download/`.
- Fingerprint does not work. Set a PIN, pattern or password.
- Some ROMs need Google setup. Some have the setup wizard skipped. See [ROMS.md](ROMS.md).

## Update to a newer build

Flash the new zip the same way. Wipe Data if the ROM or its Android version changed.
Always back up first.

## What the installer checks

- Every image is verified before anything is written.
- If a check fails before the vendor step, your phone is unchanged.
- If a write fails, the installer tries busybox `dd`, then `cat`.

## Help

Send your `recovery.log` to https://t.me/ibralyam.
In TWRP, tap Advanced, then Copy Log.
