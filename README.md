# OnePlus Pad 3 / OnePlus Pad 2 Pro Guide

A collection of instructions and resources for OnePlus Pad 3 (OPD2415) aka OnePlus Pad 2 Pro (OPD2413).

---

## **Environment**

* Tested On [OxygenOS 15.0.1.701](https://community.oneplus.com/thread/1924865591823302663)

---

## **Game Assistant**

Game Assistant app is not pre-installed on OnePlus Pad 3.

1.  Install [Games by HeyTap](https://play.google.com/store/apps/details?id=com.oplus.games) from Google Play Store.

> **Note:** The global variant of Games app is missing "Championship Mode," which includes Touch Boost. If you need this, install the [ColorOS variant](https://www.apkmirror.com/apk/heytap/oneplus-games-3) (with the green icon) instead.

---

## **Unlock Bootloader**

> **⚠️ Important FRP Warning**
> It has been reported that OnePlus devices on recent OOS updates (like `.701` for Pad 3) have FRP (Factory Reset Protection) issues. **You must sign out of your Google account from the device before proceeding to avoid being locked out.**

### **Install Drivers, ADB & Fastboot**

* [Nexus Tools](https://github.com/corbindavenport/nexus-tools)

1.  **Enable Developer Options:** Go to `Settings > About device > Version` and tap the `Version number` multiple times until you see a confirmation message.

2.  **Enable OEM Unlocking:** Go to `Settings > System & update > Developer Options` and turn on `OEM unlocking`.

3.  **Boot into Fastboot Mode:** Power off your device. Then, press and hold the `Volume Down + Power` keys simultaneously to boot into Fastboot mode.

4.  **Connect to PC:** Connect your device to your computer via USB.

5.  **Unlock Command:** Open a terminal or command prompt and enter the following command:

    <code>fastboot flashing unlock</code>

6.  **Confirm on Device:** Use the Volume and Power keys on your device to select `UNLOCK THE BOOTLOADER` and confirm.

---

## **Flashing OxygenOS**

This section is for manually flashing a full OxygenOS package. Your bootloader must be unlocked.

### **Resources**
* **OOS Flasher:** [Flasher Template for OPD2415](https://github.com/jjhitel/My-OnePlus-Pad3-Setup/raw/refs/heads/main/OPD2415_OOS%20Flasher_v1.0.zip)
* **ROM Archive:** [Official OnePlus ROMs (China)](https://yun.daxiaamu.com/OnePlus_Roms/%E4%B8%80%E5%8A%A0OnePlus%20Pad%202%20Pro/)
* **Payload Extractor:** [payload-dumper-go](https://github.com/ssut/payload-dumper-go)

### **Flashing Steps**

1.  Download the OOS Flasher Template and extract it.

2.  Download the required Full OTA file from the ROM Archive.

3.  Use the OTA Extractor (`payload-dumper-go`) to extract all `.img` files from the `payload.bin`.

4.  Place the extracted image files into the `OOS_FILES_HERE` folder within the extracted Flasher Template directory.

5.  **(Optional for Pad 2 Pro)** To fix a stylus malfunction when installing OxygenOS on Pad 2 Pro, you can replace the ODM image.

    * Extract `odm.img` from a ColorOS firmware.

    * Place it inside the `COS_FILES_HERE` folder. You will be able to select the ODM when running the flasher script.

    * Relocking the bootloader is still possible even after replacing it, but it may cause issues with OTA updates.

    * *Note: If you plan to root, you can skip this and use the `fix-odm-oplus-pad2pro` module instead.*

6.  Boot your device into Fastboot mode (`Volume Down + Power`) and connect it to your PC.

7.  Run `OOS_Flasher.bat` script and follow the on-screen instructions.

---

## **Root**

1.  Download the Full OTA zip corresponding to your current OxygenOS version from the ROM Archive.

2.  Use `payload-dumper-go` to extract the `init_boot.img` file.

3.  Copy the extracted `init_boot.img` to your device's internal storage.

4.  Download and install the latest manager APK from [KernelSU Next](https://github.com/KernelSU-Next/KernelSU-Next).

5.  Open KernelSU Next app, tap **Install** button in the top right, and select the `init_boot.img` to begin patching.

6.  A patched file named `kernelsu_next_patched_{date}_{time}.img` will be created in your device's `Downloads` folder. Copy this file back to your PC.

7.  Boot your device into Fastboot mode and connect it to your PC.

8.  In your terminal, run the following commands to flash the patched image:

    ```fastboot flash init_boot kernelsu_next_patched_{date}_{time}.img```
    
9.  If the flashing is successful, reboot your device:

    ```fastboot continue```

---

## **[Magisk/KernelSU Modules I use](./MODULES.md)**
