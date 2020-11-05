# OnePlus Battery Saver for Magisk 20+

### What it is?
This small module is based on [this XDA thread](https://forum.xda-developers.com/oneplus-7/how-to/battery-savings-t3971507) and intended to change some properties to disable packages that are installed on the phone by default. They are:  
System tracing:
* com.android.traceur

OnePlus logging and bug reporting:
* net.oneplus.odm
* net.oneplus.odm.provider
* com.oneplus.opbugreportlite

Zen Mode:
* com.oneplus.brickmode

### Default values
To play safe, the default values in the opbs.prop file are "enabled".

### How to use?
1) run 'su'
2) run 'opbs'
3) navigate in the menu with the numbers, quit with q
4) if you changed something a new menu will be shown in the menu, save and quit  
It'll generate an opbatterysaver.sh file in the /data/adb/service.d/ directory, that will be executed at system start-up.

### Requirements
- a OnePlus phone with its original OS
- Magisk 20 or higher

### Tested and working on:
- OnePlus 7 pro with OOS 10.0.9

### Warning
It won't have any effect on other manufacturers' devices because the above mentioned packages are not installed on them.

# Changelog
## v1.0
	- Root permission checking
	- Menu system
	- 5 OnePlus packages to be disabled or enabled
	- Hiding "Save and quit" menu until you change something