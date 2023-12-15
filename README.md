# Attack Shark x3 / Kysona M600 fixes

Hello! I've created this repo to share my knowledge about the Attack Shark X3 mouse. I have no affiliation with either Attack Shark or Kysona, I am simply someone who bought the X3 mouse and would want to share information about it. Please be aware there are risks of bricking your mouse when attempting any firmware upgrades.

A more detailed explanation about these firmware files will follow up once I have more time. 

## Firmware warning
If your mouse has been manufactured after September 2023, or if your mouse motherboard is the V2 board, you do not need to perform any of these steps.  
Only install the mouse software `2._M600_Driver_V1.1.zip` and set your Key Response Time to 4MS.  
```diff
- Your mouse can brick if you install these firmware packages onto a V2 Attack Shark x3.
```

You can find out if your board is a V2 board if you can still move your mouse while holding `caps lock` without updating any firmware files.

Run the updaters in this order:

1. 1._M600_Upgrade_Tool.zip
2. 2._M600_Driver_V1.1.zip
3. M600-20231013-_driver_for_receiver.zip
4. M600_20231013-_driver_for_M600_Mouse.zip

## Mods warning

### Battery mod
This mouse does not have any battery circuit protection.  
If you accidentally invert the positive and negative polarities, your mouse's board is done for.  
