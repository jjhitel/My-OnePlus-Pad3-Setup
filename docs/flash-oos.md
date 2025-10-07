# Flash OxygenOS

This section is for manually flashing a full OxygenOS package. Your bootloader must be unlocked.

### **Resources**
* **OOS Flasher:** [Flasher Template for OPD2415](https://github.com/jjhitel/My-OnePlus-Pad3-Setup/raw/refs/heads/main/OPD2415_OOS%20Flasher_v1.1.zip)
* **ROM Archive:** [Official OnePlus ROMs (China)](https://yun.daxiaamu.com/OnePlus_Roms/%E4%B8%80%E5%8A%A0OnePlus%20Pad%202%20Pro/)
* **OTA Extractor:** [otaripper](https://github.com/syedinsaf/otaripper/releases)

### **Flashing Steps**

1.  Download the OOS Flasher Template and extract it.

2.  Download the required Full OTA file from the ROM Archive.

3.  Use the OTA Extractor (`otaripper`) to extract all `.img` files from the `ota.zip`.
    ```
    otaripper -p path/to/ota.zip -o path/to/output_dir
    ```

4.  Place the extracted image files into the `OOS_FILES_HERE` folder within the extracted Flasher Template directory.

5.  **(Optional for Pad 2 Pro)** To fix a stylus malfunction when installing OxygenOS on Pad 2 Pro, you can replace the ODM image.

    * Extract `odm.img` from a ColorOS firmware.

    * Place it inside the `COS_FILES_HERE` folder. You will be able to select the ODM when running the flasher script.

    * Relocking the bootloader is still possible even after replacing it, but it may cause issues with OTA updates.

> **Note:**
> If you plan to root, you can skip this and use the `fix-odm-oplus-pad2pro` module instead.

> **Note2:**
> Recently, I purchased a new Pad 3 in addition to my existing Pad 2 Pro, and I've noticed more compatibility issues that aren't easily recognized in the same OOS environment. It appears that replacing more files within the ODM is necessary, so I recommend simply replacing the odm.img file.


6.  Boot your device into Fastboot mode (`Volume Down + Power`) and connect it to your PC.

7.  Run `OOS_Flasher.bat` script and follow the on-screen instructions.