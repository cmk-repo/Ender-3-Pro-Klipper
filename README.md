# Ender-3-Pro-Klipper
Ender 3 Pro SKR 1.4 Turbo With BLTouch
# Please use this as reference , Not to be used directly and i am not responsible for your 3d printer catching fire  :P
######################################################################
## Author : Chandan M 
## Printer configuration file of Klipper
## email : tochandan@icloud.com
 Ender 3 pro
        + BLTOUCH 
        + Octoprint
        + Ditect Drive 3d printed 
        + BTT SKR 1.4 Turbo TMC 2209
        + Stock Ender 3 pro LCD
###################################################################### 
Version 1.    ; Octopi - Installed Klipper plugin and setup connection 
Version 1.1   ; Push to Raspberry test VS CODE 
Version 1.1.3 : Reformat to basic settings
Version 2     : Adjust bed size to accomodate 3d printed direct drive unit in x
Version 2.1   : set and perform Assisted Bed leveling in Octo print using Klipper plugin
Version 2.1.2 : update Github , and Raspberry with comments


######################################################################
# OCTOPI SETTINGS
 Klipper assisted bed leveling setting in octopi
 probe points  : Left front = 60 , 60  
                 Right front = 190, 60
                 Left rear   = 60 , 190                
                 Right rear  = 190 ,190
                 Probe height = 0.4 # unique number

# BED visualiser plugin setting  : STRICTLY ON OCTOPI .
                ## G28
                ## M115 S30
                ## M190 S60
                ## @BEDLEVELVISUALIZER
                ## G29 T
                ## BED_MESH_OUTPUT

# type SAVE_CONFIG in terminal to save the measured setting ( scroll down to see my unique values )
######################################################################