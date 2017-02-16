---
title: 0.4.3.0
---

[https://github.com/Asnivor/MedLaunch/releases/tag/0.4.3.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.4.3.0)

#### Important Release Notes
** This MedLaunch release is *ONLY* compatible with version 0.9.42.x of Mednafen. Do *NOT* upgrade if you are not planning to update Mednafen also **

I thought it was about time I removed the 'beta' tag. There is still functionality to come, but unless I'm told otherwise many of the larger bugs have already been squashed.

#### Notable Additions
* Implemented option to choose games library column visibility on a per-system basis (in top-left menu and settings page)
* Added new MedLaunch icon and 'Loading' splash-screen
* Fixed default system videoip and x/y scale values
* Changes made on 'Settings' tab are now automatically saved in realtime (and the 'Save Settings' button has been removed)
* Added a games library right-click option to view/edit the Mednafen launch string before the game runs
* Added (in top-left menu system) an option to Audit the Scraped Data Folder (so that you can determine which folder is for which game regardless of whether that data is currently liked to a game in the games library)
* Modified the 'Netplay Server Settings' module to be a datagrid, enabling as many custom servers as needed

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