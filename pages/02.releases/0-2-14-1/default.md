---
title: 0.2.14.1
---

#### Alpha release.
[https://github.com/Asnivor/MedLaunch/releases/tag/0.2.14.1](https://github.com/Asnivor/MedLaunch/releases/tag/0.2.14.1)

#### Important Release Notes
This version implements some BIG changes in the way that MedLaunch handles configurations on disk. The 'Base Configuration' filter has been completed removed so that you just have a separate button for each system.

An option has been added to settings (on by default) that saves a system-specific cfg file to the root of the Mednafen directory whenever you launch a game. You can disable this in the settings but there is less chance of a screw-up if you don't. If you are precious about these cfg files (nes.cfg, psx.cfg etc.) then please back them up before you proceed.

You will also notice an amber button on the Configs page called 'IMPORT ALL CONFIGS FROM DISK'. When you click this the following happens:

* The contents of the main Mednafen configuration file are loaded into MedLaunch (mednafen-09x.cfg)
* All general (non-system-specific) options are applied to EVERY system configuration in MedLaunch
* Then every single system config file (snes.cfg, pce.cfg etc.) is loaded into MedLaunch and applied to the correct system

You are also asked if you want to import all configs every time you choose a new Mednafen directory within MedLaunch.

You can also right-click on a system filter in MedLaunch and choose to import just the system.cfg file from disk for this system (useful if you have made manual changes to a system.cfg file and want to import these changes into MedLaunch without having to import every config, and before it gets overwritten by running a game).

When you launch a game all config options for the selected system are still supplied via the command line (therefore the mednafen-09x.cfg file is updated automatically by Mednafen itself)

Please note: Netplay and Server settings are still independent of system configurations. You can set these up once in MedLaunch and not have to worry.

Finally there is another setting (also on by default) that creates a uniquely named backup of your existing Mednafen-09x.cfg file (in the root of the Mednafen directory) every time you start MedLaunch.

Hopefully these changes will mean that the way MedLaunch handles configurations is more intuitive to the average user, and more functional for those people who want to generate config files through a GUI for use in other Front-Ends/Launchers.

#### Notable Additions
* Overhauled the database config tables (to more closely mirror Mednafen's config files)
* Implemented import-config-from-files functionality
* Added option (on by default) to backup Mednafen configuration on disk when MedLaunch first starts
* 'Base Configuration' config filter has been removed and the way MedLaunch handles Mednafen config arguments has been completely overhauled (if updating rather than new install of MedLaunch please ensure that you 'Import All Configs' once before launching a game
* Added option to automatically save system.cfg file in the Mednafen directory on game launch (enabled by default). It is recommended that you leave this on to avoid any inconsistencies when importing configs into MedLaunch. As above definitely do an 'Import All Configs' on first run and backup your pre-existing system.cfg files if you don't want them tampered with

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