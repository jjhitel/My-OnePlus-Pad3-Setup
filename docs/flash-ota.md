# Flash OTA

This section is for manually flashing a full OxygenOS package. Your bootloader must be unlocked.

### **Resources**
* **COS Flasher:** [Flasher Template for Pad 2 Pro](https://mega.nz/file/hc91CQLJ#50Veg8rD3tMXoLL6M60GoW6WoaTTvQjtdIJ9BgjkF9k)
* **OOS Flasher:** [Flasher Template for Pad 3](https://mega.nz/file/kJlD2QrT#yzYPmRia8dwsIfaQetgoloNBshgr_jbsiAJ80wryaoo)
* **ROM Archive:** [Official OnePlus ROMs (China)](https://yun.daxiaamu.com/OnePlus_Roms/%E4%B8%80%E5%8A%A0OnePlus%20Pad%202%20Pro/)
* **OTA Extractor:** [otaripper](https://github.com/syedinsaf/otaripper/releases)

### **Flashing Steps**

1.  Download the Flasher Template and extract it.

2.  Download the required Full OTA file from the ROM Archive.

3.  Use the OTA Extractor (`otaripper`) to extract all `.img` files from the `ota.zip`.
    ```
    otaripper -p path/to/ota.zip -o path/to/output_dir
    ```

4.  Place the extracted image files into the `OOS_FILES_HERE`(`COS_FILES_HERE` for COS) folder within the extracted Flasher Template directory.

5.  Boot your device into Fastboot mode (`Volume Down + Power`) and connect it to your PC.

6.  Run `OOS_Flasher.bat` script and follow the on-screen instructions.

### **Cross-Flash**
Thanks to technological advancements, you can now install OxygenOS on Pad 2 Pro or ColorOS on Pad 3 without any stylus or OTA issues! However, the method has changed, so refer to this [guide](./unbrick.md)
