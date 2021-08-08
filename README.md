

##  Ender-3-Pro-Klipper with SKR 1.4 Turbo, BLTouch, Octoprint
 Author : Chandan M 
 email : tochandan@icloud.com

## Printer 
Ender 3 pro  
 --
   
    Options

    BLTOUCH 
    Octoprint
    Ditect Drive 3d printed 
    BTT SKR 1.4 Turbo TMC 2209
    Stock Ender 3 pro LCD


## Build status

In Progress 
Latest update 2.1.2, Please leave a comment if you need help


<b>Built with</b>
- [KLIPPER](https://github.com/KevinOConnor/klipper)
- [VS CODE ]()
- [OCTOPI KLIPPER]()
- [Rotation Distance Calculation](https://www.klipper3d.org/Rotation_Distance.html)
- [ Stock Ender 3 profile](https://github.com/KevinOConnor/klipper/blob/master/config/printer-creality-ender3-v2-2020.cfg)
- TBD
  - [DD with Bulleye](https://www.thingiverse.com/make:794919)
    - [Blog](https://all3dprint.blogspot.com/2020/09/ender3-pro-direct-drive-bullseye-mount.html)
  - [Klipper Tmc2209 calibration ](https://www.klipper3d.org/Config_Reference.html#tmc-stepper-driver-configuration)
  - [Blog calculation Rotation distance](https://3dprinting.stackexchange.com/questions/10986/how-to-calculate-the-proper-layer-height-multiples)
  - [To do links](https://www.reddit.com/r/klippers/comments/ew2xtp/ender_3_pro_skr13_tmc2209_config/)

## Features

## OCTOPRINT SETTINGS
-Octoklipper install and perform basic setup to talk to printer
-Configure printer 
-Klipper assisted bed leveling setting in octopi
- Probe height = 0.4 # unique number
- Add probe points
 ------------------------
    Left front = 60 , 60  
    Right front = 190, 60
    Left rear   = 60 , 190                
    Right rear  = 190 ,190
    -----------------------

### BED VISUALIZER plugin setting  

---------

    G28
    M115 S30
    M190 S60
    @BEDLEVELVISUALIZER
    G29 T
    BED_MESH_OUTPUT

--------
manualy type SAVE_CONFIG in terminal to save the measured setting ( see printer.cfg )



### Tests
-----------------------------------------------------------------------------------------
 Version 1.    : Octopi - Installed Klipper plugin and setup connection 
 Version 1.1   : Push to Raspberry test VS CODE 
 Version 1.1.3 : Reformat to basic settings
 Version 2     : Adjust bed size to accomodate 3d printed direct drive unit in x
 Version 2.1   : set and perform Assisted Bed leveling in Octo print using Klipper plugin
 Version 2.1.2 : update Github , and Raspberry with comments: BL-Touch Working
    
    Test Print confimation TBD

### How to use?
 
Please use this as reference , Not to be used directly and i am not responsible for your 3d printer catching fire  :P

### Credits
BLTOUCH and X gantry fix [Albertogg](https://github.com/albertogg/klipper-config/blob/97b36987ebfe697a084584e684897f2f1b13dea1/ender-3/printer.cfg#L194) and [blog](https://github.com/albertogg/albertogg.github.com) 

Direct Drive mount [Direct Drive 3d printed](https://www.youtube.com/watch?v=Zbk0viFC1ew&t=1s) File :[ DD Thingiverse](https://www.thingiverse.com/thing:3816051)

BL Touch without STOWing  [BL-Touch Video ](https://www.youtube.com/watch?v=JRvHT8X2vMw)

### License
 MIT
