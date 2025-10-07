# Root

### **Resources**
* **OTA Extractor:** [otaripper](https://github.com/syedinsaf/otaripper/releases)

1.  Download the Full OTA zip corresponding to your current OxygenOS version from the ROM Archive.

2.  Use the OTA Extractor (`otaripper`) to extract the `init_boot.img` files from the `ota.zip`.
    ```
    otaripper ota.zip --partitions init_boot
    ```

3.  Copy the extracted `init_boot.img` to your device's internal storage.

4.  Download and install the latest manager APK from [KernelSU Next](https://github.com/KernelSU-Next/KernelSU-Next).

5.  Open KernelSU Next app, tap **Install** button in the top right, and select the `init_boot.img` to begin patching.

6.  A patched file named `kernelsu_next_patched_{date}_{time}.img` will be created in your device's `Downloads` folder. Copy this file back to your PC.

7.  Boot your device into Fastboot mode and connect it to your PC.

8.  In your terminal, run the following commands to flash the patched image:

    ```
    fastboot flash init_boot kernelsu_next_patched_{date}_{time}.img
    ```

9.  If the flashing is successful, reboot your device:

    ```
    fastboot continue
    ```