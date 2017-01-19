---
title: 0.2.20.0
---

#### Beta release
[https://github.com/Asnivor/MedLaunch/releases/tag/0.2.20.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.2.20.0)

#### Notable Additions
* Fixed media content from downloading when option is de-selected in settings
* Fixed launch strings not being passed to mednafen for PCE CD games
* Fixed (unneeded) pcecd.cfg config being created in mednafen folder
* Fixed game scraping local match for PCD-CD games (games were not being found)
* Added option to set the size of the image tooltip popups (based on a percentage of the current MedLaunch window size)

#### Important Release Notes
This latest release completely overhauls much of the Games Library code, along with the underlying database structure. These changes should provide much better performance for large libraries (so far tested with approx 20,000 games in the library).

Because of the database changes, you will find that updating your current version of MedLaunch results in all the games in your library showing as not scraped. You will have to scrape them again - although if any media files have been previously downloaded these will be found once scraping has been completed.

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