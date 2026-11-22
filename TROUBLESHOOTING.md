# Troubleshooting

## Error: nothing was written yet

A check failed early. Your phone is unchanged. Read the message on screen, then try again.
If it happens again, download the zip again and compare the SHA-256 value.

## Error after the writing started

Do not reboot to system. Flash the zip again.
If it fails again, send me the recovery log.

## Read-only file system at the BiTGApps step

The system image is read only. Wipe System in TWRP (Wipe, Advanced Wipe, System), then flash again.

## Bootloop

Boot to TWRP. Format Data, then flash again.
Do not wipe internal storage, or you lose the zip.

## No KernelSU Manager icon

Install `KernelSU.apk` from `/storage/emulated/0/Download/`.

## Stuck on the logo for a long time

The first boot can take up to 10 minutes. Wait. If it is still stuck, boot to TWRP and flash again.

## The flash looks frozen

The screen shows a message every 15 seconds on some zips. Wait until you see "All done".

## Fingerprint does not work

This is a known A50 limit on AOSP ROMs. Use a PIN, pattern or password.

## Google apps are missing

Some ROMs already include them. Some zips add BiTGApps. Check [ROMS.md](ROMS.md).
RestlessOS has no Google apps by design.

## How to get the recovery log

In TWRP, tap Advanced, then Copy Log. The file is saved as `recovery.log`.
Send it to https://t.me/ibralyam.
