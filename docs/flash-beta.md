# Flash Beta (Android 16)

This is a guide for those who were not approved for the beta and cannot wait the remaining few weeks.

Currently, only the ColorOS 16.0.0.206 package for the OnePlus Pad 2 Pro has been leaked. (Source: Coolapk)

Beta packages cannot be installed via a typical local installation without root.

## Steps

1.  First, downgrade to version [15.0.1.701](https://yun.daxiaamu.com/OnePlus_Roms/%E4%B8%80%E5%8A%A0OnePlus%20Pad%202%20Pro/ColorOS%20OPD2413_15.0.1.701(CN01)%20A.36/).

2.  Download the two zip files from this [link](https://mega.nz/folder/gMFxxKwD#guo6b2ZEH-pwX1hmPALPFQ) to your device.

3.  Root your device by patching `init_boot.img` with Magisk Alpha. Install [Tricky Store](https://github.com/5ec1cff/TrickyStore) (v1.4.0 or higher), [ReZygisk](https://github.com/PerformanC/ReZygisk), and [LSPosed](https://github.com/JingMatrix/LSPosed) modules.

4.  After rebooting, add `com.oplus.ota` to the target apps in Tricky Store. Find and install LuckyTool v1.3.2 beta apk from their [community](https://luckyzyx.gitlab.io/LuckyTool_Doc/en/link.html), activate it, and reboot.

5.  Open LuckyTool and, in the OTA app options, enable all three checkboxes at the bottom. With this setup, go to the OTA app for a local update.

6.  If you receive an '801' update notification, clear the OTA app's data and disconnect from the internet. Then, go to the local update menu and select the 500MB zip file you downloaded earlier.

7.  Restore the original image in the Magisk app, then return to the OTA app to begin the installation.

8.  When the installation is complete, **do not reboot**. Go back to the Magisk app, install Magisk to the inactive slot, and then reboot. If your device still shows version 701 after rebooting, patch the inactive slot one more time and reboot again.

9.  Once completed, you will be updated to the 801SP version required for beta participation. You can now repeat the process to install the 3GB Android 16 package.

> **Note:**
> Due to the limitations of this test version, Fastboot will be disabled. However, you can access `fastbootd` with the command below, downgrade only the bootloader ([abl.img](https://mega.nz/file/RINhnJzC#xe6ymfwAMm2_lTnIaWWPmuHhsDHmgzxNDXy4xR__Dls)) to enable Fastboot.
> ```sh
> adb reboot fastboot
> fastboot flash --slot=all abl abl.img
> ```