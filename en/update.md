# Updating drivers

## Files/Tools Needed

Modified TWRP:

| File Name                                       | Android version |
|-------------------------------------------------|-----------------|
| [twrp-3.7.1_12-vayu.img](https://github.com/woa-venus/POCOX3Pro-Guides/raw/main/Files/twrp-3.7.1_12-vayu.img) | Android 12/12.1/13/14 |
| [twrp-3.7.0_11-vayu.img](https://github.com/woa-venus/POCOX3Pro-Guides/raw/main/Files/twrp-3.7.0_11-vayu.img) | Android 11 |

- [Drivers](https://github.com/woa-venus/Xiaomi11-Releases/releases/latest)

- [UEFI image](https://github.com/woa-venus/Xiaomi11-Releases/releases/latest)

### Boot into TWRP
>
> If your recovery has been replaced by the stock recovery, flash it again using

```cmd
fastboot boot path\to\moddedtwrp.img 
```

#### Execute the msc script
>
> If it asks you to run it once again, do so

```cmd
adb shell msc
```

### Diskpart

```cmd
diskpart
```

#### Select the Windows volume of the phone
>
> Use `list volume` to find it, replace "$" with the actual number of **WINVENUS**

```diskpart
select volume $
```

#### Assign the letter X

```diskpart
assign letter x
```

#### Exit diskpart

```diskpart
exit
```

### Installing drivers
>
> [!Note]
> This process will take +- 20 minutes. Do not worry, this is normal.

- Unpack the driver archive, then open the `OfflineUpdater.cmd` file

> If it asks you to enter a letter, enter the drive letter of **WINVENUS** (which should be **X**), then press enter

### Reboot your device
>
> Make sure to also change the UEFI image in Android, otherwise you may face a "blue screen of death" (BSoD) when booting Windows later.

```cmd
adb reboot
```

## Finished
