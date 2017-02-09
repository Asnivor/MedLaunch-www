---
title: 0.4.1.0
---

#### Beta release
[https://github.com/Asnivor/MedLaunch/releases/tag/0.4.1.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.4.1.0)

#### Important Release Notes
** This MedLaunch release is *ONLY* compatible with version 0.9.42.x of Mednafen (although you *may* get away with running 0.9.41.x as not much has changed between versions). Do *NOT* upgrade if you are not planning to update Mednafen also **

#### Notable Additions
* Added new config controls for mednafen 0.9.42 (snes_faust multitap and additional virtual controller selection)
* Fixed a few small UI bugs
* Modified the update checker to use github's API rather than individually generated json files

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