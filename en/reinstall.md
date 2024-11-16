# Reinstall Windows on your Mi 11

## Files/Tools Needed

- [ADB & Fastboot](https://developer.android.com/studio/releases/platform-tools)

Modified TWRP:

| File Name                                       | Android version |
|-------------------------------------------------|-----------------|
| [twrp-3.7.0_12-venus.img](https://github.com/woa-venus/Xiaomi11-Guides/raw/main/Files/twrp-3.7.0_12-venus.img) | Android 12/12.1/13/14 |
| [twrp-3.7.0_11-venus.img](https://github.com/woa-venus/Xiaomi11-Guides/raw/main/Files/twrp-3.7.0_11-venus.img) | Android 11 |

### Boot into TWRP

```cmd
fastboot boot path\to\twrp.img
```

#### Formatting the Windows partition

```cmd
adb shell format
```

## [Next step: Reinstalling Windows](/en/3-install.md)
