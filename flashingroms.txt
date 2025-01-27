# How to Flash

## Required Files
1. **If MIUI 12 is installed:**
   - Download the required file from [this link](https://t.me/selenetr/15272).

2. **If MIUI 13 or higher is installed:**
   - Download the required file from [this link](https://t.me/selenetr/4962).

3. **Additional Files:**
   - **Recovery ROM** for the MIUI version you are currently on.
   - **boot.img** from the MIUI version you are currently on.
   - **ROM zip** for the version you are trying to flash.

---

## Custom Recovery Installation Instructions
1. Flash the custom recovery:
   ```
   fastboot flash boot CUSTOMRECOVERYNAMEFILENAME.img
   ```

2. Reboot into recovery:
   ```
   fastboot reboot recovery
   ```

3. Flash the **boot.img** from your stock MIUI ROM to the boot partition.

4. Flash CUSTOMRECOVERYNAMEFILENAME.img to the ramdisk partition. 

*Alternatively, you can use the "Install Current Recovery" option available in your custom recovery.*

5. Reboot to recovery:
   ```
   fastboot reboot recovery
   ```

---

## Flashing Steps
1. **Format data** using the custom recovery.
2. Flash the **Recovery ROM** for your current MIUI version.
   - **Note:** Doing this might replace your custom recovery with MIUI recovery, so you might need to re-flash the custom recovery (repeat **Custom Recovery Installation Instructions** above).
3. Flash the **Custom ROM** of your choice.
4. Reboot to system if you want to boot into the ROM, or reboot to recovery for flashing GApps.
5. Format Data.
6. Flash GApps.
7. Reboot to system.

---

## Warning
- If your device has an **FTS screen type**, flash this kernel before proceeding: [FTS Kernel Link](https://t.me/fukiamimir/243).

---
