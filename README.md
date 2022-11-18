# Ender-6-SKRE3V3-Klipper
Configs for changing mainboard in Ender 6 to SKR E3 V3 with klipper


There are few options:

SKRE3V3-BLTouch-dgus  -  This is for desuuuu fork of klipper to get stock screen working with klipper and BLTouch (connect it to the motherboard instead of z endstop plug)

SKRE3V3-dgus  -  This is for desuuuu fork of klipper to get stock screen working with klipper

SKRE3V3  -  Ender 6 with SKRE3V3

SKRE3V3-BLTouch  -  Ender 6 with SKRE3V3 and BLTouch






Few tips to motherboard replace:
1. Just plug everything similar to old mobo. 
2. Parts cooling fan should go to FAN0 port
3. SDCard plug dont fit, hide it.

After replacing configs set again:
1. Raspberry Pi/mcu serial adress:
- connect with Putty to Raspberry Pi
- ls /dev/serial/by-id/*
- replace your serial id with existing one in printer.cfg on [mcu] section
2. Pid tuning: https://all3dp.com/2/klipper-pid-tune-tuning-3d-printer/
3. Z offset (if you have BLTouch): https://www.youtube.com/watch?v=vduYl9Rw5iI

Test autohome, fan behaviour



Happy printing
