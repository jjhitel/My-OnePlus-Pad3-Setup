# My device is bricked!

## Unlocked Bootloader
If your bootloader is still unlocked, you should also have access to Fastboot.
If so, you can fix it by following the instructions in [flash-oos](docs/flash-oos.md).

If the partition table is corrupted, obtain and flash `super.img`. It may not completely solve the problem, but it will still allow you to use the device.

## Locked Bootloader
If your device is bricked with a locked bootloader, you will need to flash firmware in EDL (Emergency Download) mode.

[OPD2415GDPR_11_15.0.1.306EX01_2025050821380000.zip](https://dfs-serverauto-in.allawnofs.com/dfs/25/05/12/ec3fb9a938c3462abe962c37a179d92b.zip)

OnePlus does not make the tool available to the general public, so you will have to contact a third-party repair service and pay a fee.

However, as of now, the EDL server has been offline for months, making recovery impossible.

If you can send your device to OnePlus, do so; otherwise, you will have to wait.
