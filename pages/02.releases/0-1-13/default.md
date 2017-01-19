---
title: 0.1.13
---

#### Alpha release.
[https://github.com/Asnivor/MedLaunch/releases/tag/0.1.13](https://github.com/Asnivor/MedLaunch/releases/tag/0.1.13)

#### Notable Additions
* Added option to manually add disk-based games (context menu right-click on System filter in 'Games' tab.
* Implemented m3u auto-generation logic when adding multi-disk games 
* Enabled double-click to launch game in Games library
* Added 'Delete From Games Library' context menu option (removes from the database, not disk - roms will be re-added on next scan)

#### Current Issues
* The launcher currently only handles absolute paths correctly. Relative path handling may or may not work but this part of the code needs a proper overhaul
* It is recommended that you use a brand new Mednafen instance for the time being. You can download the latest version of Mednafen from the Mednafen website. If you do not do this you might experience issues with already existing system specific configuration files in the Mednafen folder. Specifically, these will override base settings in MedLaunch until said system configuration is enabled in the launcher. This will be addressed in future releases.

See [Changelog](http://medlaunch.asnitech.co.uk/changelog) for more information.