# My device is bricked!

## Unlocked Bootloader
If you still have access to Fastboot, you can fix it by following the instructions in [flash-oos](docs/flash-oos.md).

If the partition table is corrupted, download the EDL package below, extract `super_meta.01000100.raw` (for Pad 3) or `super_meta.10100111.raw` (for Pad 2 Pro), rename it to `super.img`, and run `fastboot wipe-super super.img`.

## Locked Bootloader
If your device is bricked with a locked bootloader, you will need to flash firmware in EDL (Emergency Download) mode.

- OnePlus Pad 3 [15.0.1.306](https://dfs-serverauto-in.allawnofs.com/dfs/25/05/12/ec3fb9a938c3462abe962c37a179d92b.zip)
- OnePlus Pad 2 Pro [15.0.1.601](https://dfs-serverauto-in.allawnofs.com/dfs/25/08/05/5c568cdb9436442796dac8f2d0eae4ac.zip)

OnePlus does not make the tool available to the general public, so you will have to contact a third-party repair service and pay a expensive fee.

However, there is a free alternative called [OP_Flash_Tool](https://github.com/z4g7298d6b/OP_Flash_Tool). I plan to test this on my spare device in the coming weeks.

If you can send your device to OnePlus service center, do so.
