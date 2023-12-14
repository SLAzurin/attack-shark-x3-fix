# Attack Shark x3 / Kysona M600 fixes

## Firmware warning
If your mouse has been manufactured after September 2023, or if your mouse motherboard is the V2 board, you do not need to perform any of these steps.  
Only install the mouse software `2._M600_Driver_V1.1.zip` and set your Key Response Time to 4MS.  
```diff
- Your mouse can brick if you install these firmware packages onto a V2 Attack Shark x3.
```

Run the updaters in this order:

1. 1._M600_Upgrade_Tool.zip
2. 2._M600_Driver_V1.1.zip
3. M600-20231013-_driver_for_receiver.zip
4. M600_20231013-_driver_for_M600_Mouse.zip

## Mods warning

### Battery mod
This mouse does not have any battery circuit protection.  
If you accidentally invert the positive and negative polarities, your mouse's board is done for.  
