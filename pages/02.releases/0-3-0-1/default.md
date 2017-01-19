---
title: 0.3.0.1
---

#### Beta release
[https://github.com/Asnivor/MedLaunch/releases/tag/0.3.0.1](https://github.com/Asnivor/MedLaunch/releases/tag/0.3.0.1)

#### Notable Additions
* Implemented color picker/canvas control for all Mednafen hex-color related options (lightgun crosshair colors etc..)
* Bugfix to stop application exception when trying to 'Browse Game Data Folder' when the game does not have a GDBID set in the database

#### Important Release Notes
This is a quick bugfix release that also bundles a Mednafen config colorpicker control.

#### New Install
* Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.39.x branch and 64-bit version if you want to emulate Saturn games). 
* You are then prompted to choose whether to import all config settings from your Mednafen folder into the MedLaunch database (this is recommended).
* If you currently use system-specific config files with Mednafen the settings from these will be imported with the above process. However MedLaunch will write to these files when you launch a game - so back them up somewhere if you are not happy with this.

#### Upgrade
##### Preferred Method: 
* Automatically download and upgrade using the 'Updates' tab within MedLaunch itself.
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button

##### Manual Method: 
* You can safely extract this new release over an existing MedLaunch folder (providing you do not have MedLaunch running at the time) 
* Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button