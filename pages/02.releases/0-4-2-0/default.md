---
title: 0.4.2.0
---

#### Beta release
[https://github.com/Asnivor/MedLaunch/releases/tag/0.4.2.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.4.2.0)

#### Important Release Notes
** This MedLaunch release is *ONLY* compatible with version 0.9.42.x of Mednafen. Do *NOT* upgrade if you are not planning to update Mednafen also **

#### Notable Additions
* Implemented 7zip archive support for non-disc systems (roms are extracted to local cache folder before game launch) - one rom per archive file
* Added new setting to clear rom cache folder on application exit (enabled by default)
* Added an option to open the MedLaunch unhandled exception log (if one if present)
* Swapped text boxes that require decimal input for NumericUpDown controls (so that decimal and negative numbers can be entered by hand)
* Merged the 'top-right' title-bar buttons into a new (more standard) 'top-left' dropdown menu system
* Added top-menu option to locate and launch a game through the filesystem (bypassing MedLaunch config database options meaning the game launches using the Mednafen config files on-disk)
* Other misc bugfixes (see full [Changelog](http://medlaunch.asnitech.co.uk/changelog) for more details)

#### New Install
* Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.42.x branch - 64-bit version is required if you want to emulate Saturn games). 
* You are then prompted to choose whether to import all config settings from your Mednafen folder into the MedLaunch database (this is recommended).
* If you currently use system-specific config files with Mednafen the settings from these will be imported with the above process. However MedLaunch will write to these files when you launch a game - so back them up somewhere if you are not happy with this.

#### Upgrade
##### Preferred Method: 
* Automatically download and upgrade using the 'Updates' tab within MedLaunch itself.
* Ensure you have the correct version of Mednafen installed (v0.9.42.x)
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else

##### Manual Method: 
* You can safely extract this new release over an existing MedLaunch folder (providing you do not have MedLaunch running at the time) 
* Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else