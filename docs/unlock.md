# Unlock Bootloader

> **⚠️ Important FRP Warning**
> It has been reported that OnePlus devices on recent OOS updates (like `.701` for Pad 3) have FRP (Factory Reset Protection) issues. **You must sign out of your Google account from the device before proceeding to avoid being locked out.**

### **Install Drivers, ADB & Fastboot**

* [Installer](https://github.com/K3V1991/ADB-and-FastbootPlusPlus)

1.  **Enable Developer Options:** Go to `Settings > About device > Version` and tap the `Version number` multiple times until you see a confirmation message.

2.  **Enable OEM Unlocking:** Go to `Settings > System & update > Developer Options` and turn on `OEM unlocking`.

3.  **Boot into Fastboot Mode:** Power off your device. Then, press and hold the `Volume Down + Power` keys simultaneously to boot into Fastboot mode.

4.  **Connect to PC:** Connect your device to your computer via USB.

5.  **Unlock Command:** Open a terminal or command prompt and enter the following command:

    ```
    fastboot flashing unlock
    ```

6.  **Confirm on Device:** Use the Volume and Power keys on your device to select `UNLOCK THE BOOTLOADER` and confirm.