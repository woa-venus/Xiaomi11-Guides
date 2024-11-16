# Uninstall Windows and revert your Mi 11 to stock

## Why is this needed?

If you want to uninstall Windows, this is used instead of deleting partitions manually to avoid human error + writing a whole dedicated guide to just uninstalling.

If you want to relock your bootloader you'll need your partition table to be stock.

### Files/Tools Needed

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)

Modified TWRP:

| File Name                                       | Android version |
|-------------------------------------------------|-----------------|
| [twrp-3.7.0_12-venus.img](https://github.com/woa-venus/Xiaomi11-Guides/raw/main/Files/twrp-3.7.0_12-venus.img) | Android 12/12.1/13/14 |
| [twrp-3.7.0_11-venus.img](https://github.com/woa-venus/Xiaomi11-Guides/raw/main/Files/twrp-3.7.0_11-venus.img) | Android 11 |

## Flash and boot modified recovery

```cmd
fastboot boot path\to\moddedtwrp.img
```

### Execute the restore script

```cmd
adb shell restore
```

#### Finished
