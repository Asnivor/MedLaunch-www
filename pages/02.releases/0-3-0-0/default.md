---
title: 0.3.0.0
---

#### Beta release
[https://github.com/Asnivor/MedLaunch/releases/tag/0.3.0.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.3.0.0)

#### Notable Additions
* Many bug fixes (see changelog for full details)
* Various UI style enhancements (more consistent controls and mouse cursor change over controls)
* Implemented games library datagrid sorting memory (per session only)
* Vastly improved 'Save Settings' execution speed
* Added ability to set custom fullscreen resolutions
* Details of unhandled exceptions (application crashes) are now written to 'Exceptions.log' in the root of the MedLaunch directory
* A merged 'DAT' file (json) has been created and will be shipped with each release. Using TOSEC, NOINTRO, TRURIP & REDUMP roms will be detected on import (and re-scan) based on MD5 checksum and game name, country, year and publisher will be populated in the games library grid (where information is available). Year and publisher will be overwritten when game data is scraped from online
* Added context menu option to re-scrape all game information for a system (rather than just trying to scrape for games that have no previously been scraped). This will download all content again

#### Important Release Notes
In this major release there have been many low-level changes to the way MedLaunch functions 'under the hood'. If you have any issues upgrading from an older version of MedLaunch it is recommended that you attempt a fresh install. I haven't however seen any upgrade issues during testing.

In order to populate the new grid fields in the games library you will have to rescan your existing ROMs. This will automatically attempt to match them using MD5 hash with the merged DAT that now ships with MedLaunch.

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