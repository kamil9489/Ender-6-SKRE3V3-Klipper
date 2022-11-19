# Ender-6-SKRE3V3-Klipper
<b> Configs for changing mainboard in Ender 6 to SKR E3 V3 with klipper. </b>

I use BiquH2 as direct drive + Y endstop relocation for more print space (https://www.thingiverse.com/thing:5222477)




<b>For klipper install you can follow this guide: https://3dprintbeginner.com/how-to-install-klipper-on-creality-ender-6/ </b>

I recommend MainsailOS. Use desuuuu repo if you want stock screen working, use kiauh if you want clean klipper with aftermarket screen working (or android tablet with kliperscreen)

There are few options:

SKRE3V3-BLTouch-dgus  -  This is for desuuuu fork of klipper to get stock screen working + BLTouch (connect it to the motherboard instead of z endstop plug)

SKRE3V3-dgus  -  This is for desuuuu fork of klipper to get stock screen working with klipper

SKRE3V3  -  Ender 6 with SKRE3V3

SKRE3V3-BLTouch  -  Ender 6 with SKRE3V3 and BLTouch






<b>Few tips to motherboard replace:</b>
1. Just plug everything similar to old mobo. 
2. Parts cooling fan should go to FAN0 port
3. SDCard plug dont fit, hide it.
4. Switch X and Y motor cable (Ender 6 is CoreYX machine, no CoreXY)

<b>After replacing configs set again:</b>
1. Raspberry Pi/mcu serial adress:
- connect with Putty to Raspberry Pi
- ls /dev/serial/by-id/*
- replace your serial id with existing one in printer.cfg on [mcu] section
2. Pid tuning: https://all3dp.com/2/klipper-pid-tune-tuning-3d-printer/
3. Z offset (if you have BLTouch): https://www.youtube.com/watch?v=vduYl9Rw5iI
4. Esteps (rotation distance on [extruder] section)
- You can use rotation distance calculator to change marlin value to klipper value: https://3dprintbeginner.com/rotation-distance-calculator/

Test autohome, fan behaviour, print test cube.



Happy printing
