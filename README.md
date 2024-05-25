# Attack Shark x3 / Kysona M600 fixes

## Disclaimer: <u>**I have no affiliation with either Attack Shark or Kysona**</u>, I am simply someone who bought the X3 mouse and would want to share information about it.

Hello! I've created this repo to share my knowledge about the Attack Shark X3 mouse.  
Please be aware there are risks of bricking your mouse when attempting any firmware upgrades.  
You will <u>definitely</u> brick your mouse if you apply the firmware update on your V2 or newer X3 mouse.

**Note: This repo serves as a mirror for the Kysona M600 mouse files in case the official download sources are down.**

## Table of contents

- [How to check/update if you have a V1, V1.1 or V2 variant](#how-to-check-if-you-have-a-v1-v11-or-v2-variant)
- [Firmware files usage guide](#firmware-files-usage-guide)
- [Mods etc](#mods-etc)
- [References](#references)

## How to check if you have a V1, V1.1 or V2 variant

### Instructions

First check if the Windows mouse software works.

1. Download and install `Attack_SharkX3Mouse.exe`. Check if your mouse is detected and change the click debounce time to 4ms.

   - If this does not work, you have V1 and should upgrade to V1.1 first with `1._M600_Upgrade_Tool.zip`.
     - Once that is done, continue to step 2.
   - If this works, continue to step 2.

2. Hold `caps lock` while moving the mouse left and right.
   - If your mouse cursor stops moving while holding `caps lock`, you have a V1 or V1.1. Apply the fix with these 2 files:
     - `M600-20231013-_driver_for_receiver.zip`
     - `M600_20231013-_driver_for_M600_Mouse.zip`
   - If your mouse is still working during this movement, do not apply any firmware upgrade. You have a V2 variant.
     - **WARNING!** You will brick your device if you apply the firmware upgrades.

Once you follow these instructions you will finish with a <u>fixed V1.1</u>, or an already working <u>V2</u> (or newer).

If you have a V2 variant, you did not need to upgrade any firmware files. That is normal.

Here is the motherboard difference V1 on the left, V2 on the right:  
<img style='max-height: 400px' src='./img/v1v2diff.png'></img>

## Firmware files usage guide

There are 4 files that come from the Kysona blog post. (See [references](#references))  
These firmware files only apply to the earlier V1 models manufactured before September 2023.

| Filename                                   | File Type        | Compatibility           | Usage                                                                                                                  |
| ------------------------------------------ | ---------------- | ----------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| `1._M600_Upgrade_Tool.zip`                 | Firmware         | <u>**V1 Only**</u>      | Fixes jittery mouse sensor tracking <u>(and upgrades to V1.1)</u>                                                      |
| `Attack_SharkX3Mouse.exe`                  | Windows Software | V1, V2 and likely newer | Main mouse software which allows ajusting the mouse debounce time to as low as 4ms (lower is better)                   |
| `M600-20231013-_driver_for_receiver.zip`   | Firmware         | <u>**V1.1 Only**</u>    | Fixes mouse freezing when holding `caps lock` (Must be used alongside with `M600_20231013-_driver_for_M600_Mouse.zip`) |
| `M600_20231013-_driver_for_M600_Mouse.zip` | Firmware         | <u>**V1.1 Only**</u>    | Fixes mouse freezing when holding `caps lock` (Must be used alongside with `M600-20231013-_driver_for_receiver.zip`)   |

See [instructions](#instructions) to know how to use these files.

## Mods etc

I lowered the weight to only <u>44g</u> by cutting the bottom shell and by installing a smaller battery.  
See pictures of my modded X3 mouse in [mod_showcase](./mod_showcase/README.md).

### WARNING: Battery mod

This mouse does not have any power circuit protection.  
If you accidentally invert the positive and negative polarities, your mouse's board is done for.  
I learned about this the hard way `:(`

## References:

https://shop.kysona.com/blogs/news/upgrade-kysona-m600-drive-to-enable-debounce-time-adjustment  
https://shop.kysona.com/blogs/news/troubleshooting-bricked-kysona-m600-mice-two-essential-tools-for-recovery

If you have any questions or comments to add, feel free to do so in this [post](https://github.com/SLAzurin/attack-shark-x3-fix/issues/2)
