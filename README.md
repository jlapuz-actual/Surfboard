keyswitch  
---
I mean for this to be a keyboard PCB that you can drop in an [Adafruit Feather](https://www.adafruit.com/product/2829), switches, and diodes.

Layout  
---
[Layout with intended keycaps to use](http://www.keyboard-layout-editor.com/#/gists/e4e8a6f66c2c640a77dbacd3e51fc3d9)  
I wanted a 40% to use with a phone or tablet but with more function and modifier keys that are wider than 1u. In addition I wanted to be able to use keys from a 60% percent at minimum, although limited to DSA, G20, SA R3, and similar sets if contoured keys in the wrong row is a problem  

[Layer 0](http://www.keyboard-layout-editor.com/#/gists/cc1070f71789ace71d15d57b2ea0d759)  
This is default layer  

---
These are the function layers. What I tried to do is put the modified keys on the opposite side of the activating function key. The way I use modifier keys means that I press the modifier key with one hand and type with the other  
[Layer 1](http://www.keyboard-layout-editor.com/#/gists/59b77285f404e8a5413cfdc76923d688)  
Math layer  
[Layer 2](http://www.keyboard-layout-editor.com/#/gists/df4af78e93a107d80d330e3a977cecf1)  
Navigation  
[Layer 3](http://www.keyboard-layout-editor.com/#/gists/67db6d858fd3169d8e3274208c5a3cfd)  
F keys  
These are all stuff to do in code, but this is what is planned

PCB  
---    

None of this is final, partly because I don't know if it's aligned correctly and if there is an egregious electrical error
[keyswitch.brd](https://github.com/karakot/keyswitch/blob/master/keyswitch.pdf)  |  [keyswitch.sch](https://github.com/karakot/keyswitch/blob/master/keyswitchsch.pdf)    
Basically I have no idea if the routes are "legal". I'm pretty sure that the schematic is correct though.  

---  

I may change the position of the feather but it will definitely have the usb port facing the outside edge as it serves as the charger for the battery that will be connected.  

[keyswitch_matrixOnly.brd](https://github.com/karakot/keyswitch/blob/master/keyswitch_matrixOnly.pdf) and [keyswitch_noRoutes.brd](https://github.com/karakot/keyswitch/blob/master/keyswitch_noRoutes.pdf) are checkpoint backups  
  
All of these are Eagle files, I am looking into converting the files for use in Kicad

# Thoughts

I didn't plan on Alps support since there isn't much keycap support for Alps, and I don't find contoured keycaps in the wrong rows attractive. I didn't find a component in the [clueboard eagle library](https://github.com/skullydazed/clueboard_eagle) with alps-mx mount that has a integrated diode footprint, but I may be able to put something together
