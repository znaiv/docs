# <a id="title0">Contents</a>

---

[Read before installation](#title1)  
[Prepare everything before installation](#title2)  
[First time installation (Clean Flash)](#title3)  
[Update to a newer build of the same AlphaDroid version](#title4)  

---

# <a id="title1">Read before installation:</a>

1. Read through the instructions at least once before actually following them, so as to avoid any problems due to any missed steps!
2. Make sure your computer has ***adb*** and ***fastboot***.
3. AlphaDroid is provided as-is with no warranty. You are installing this at your own risk!
--- 

# <a id="title2">Prepare everything before installation:</a>

1. Download ROM
   - [Download](https://sourceforge.net/projects/alphadroid-project/files/sunny/3.1/AlphaDroid-15.1-20250225-gapps-sunny-v3.1.zip/download)
2. Download ROM Recovery
   - [Download](https://sourceforge.net/projects/alphadroid-project/files/sunny/3.1/AlphaDroid-15.1-20250225-recovery.zip/download)
3. Download 14.0.9.0 Firmware
    - [Download](https://drive.google.com/file/d/1y_V2SgRkpRSYnc1IhHqvfu4l5QELqgQ0/view)

--- 

# <a id="title3">First time installation (Clean Flash)</a>

1. Boot to bootloader
2. Run fastboot update
    - Ignore fastboot: error: could not load ’system.img’: No such file or directory
    ```
    fastboot update AlphaDroid-15.1-*-recovery.zip
    ```
3. Reboot to recovery
4. Format data with the rom recovery.
5. Click apply for update.
6. Run adb sideload

```
adb sideload AlphaDroid-15.1-*.zip
```

7. Reboot to system

## (Optional) Firmware 14.0.9.0
**Note:** 
Most devices now uses 14.0.9.0 firmware so you can skip this part if you already flash it.

1. Boot to recovery
2. Click apply for update.
3. Run adb sideload

```
adb sideload <firmware.zip>
```

4. Reboot to recovery
5. Flash [ROM](https://sourceforge.net/projects/alphadroid-project/files/sunny/3.1/AlphaDroid-15.1-20250225-gapps-sunny-v3.1.zip/download)

----

# <a id="title4">Update to a newer build of the same AlphaDroid version</a>

## Dirty Flash:

---

1. Download ROM zip.
    - [ROM](https://sourceforge.net/projects/alphadroid-project/files/sunny/3.1/AlphaDroid-15.1-20250225-gapps-sunny-v3.1.zip/download)
2. Boot to recovery.
3. Click apply for update.
4. Run adb sideload

```
adb sideload AlphaDroid-15.1-*.zip
```
5. Reboot to system.

---

## OTA Flash:

1. Open Settings, navigate to ***System***, then ***Updater***.
2. Click the Refresh Icon in the top right corner.
3. Choose which update you’d like and press ***Download***.
4. When the download completes, click ***Install***. Once the update process has finished, the device will display a ***Reboot*** button, you may need to go into the Updater menu in Settings, ***System*** to see it. This will reboot you into the updated system.

---