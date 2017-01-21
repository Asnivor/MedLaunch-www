---
title: 0.4.0.0
---

#### Beta release
[https://github.com/Asnivor/MedLaunch/releases/tag/0.4.0.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.4.0.0)

#### Notable Additions
* Implemented config control changes for the latest Mednafen release
* Added a Mednafen version check on game launch (to avoid errors with wrong versions)
* Fixed some minor errors in the Mednafen config control names
* Added tooltips on config controls based on Mednafen documentation (can be turned off/on in settings)

#### Important Release Notes
** This MedLaunch release is *ONLY* compatible with version 0.9.41.x of Mednafen. Do *NOT* upgrade if you are not planning to update Mednafen also **

#### New Install
* Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.41.x branch - 64-bit version is required if you want to emulate Saturn games). 
* You are then prompted to choose whether to import all config settings from your Mednafen folder into the MedLaunch database (this is recommended).
* If you currently use system-specific config files with Mednafen the settings from these will be imported with the above process. However MedLaunch will write to these files when you launch a game - so back them up somewhere if you are not happy with this.

#### Upgrade
##### Preferred Method: 
* Automatically download and upgrade using the 'Updates' tab within MedLaunch itself.
* Ensure you have the correct version of Mednafen installed (v0.9.41.x)
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else

##### Manual Method: 
* You can safely extract this new release over an existing MedLaunch folder (providing you do not have MedLaunch running at the time) 
* Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else