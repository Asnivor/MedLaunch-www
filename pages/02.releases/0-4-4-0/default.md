---
title: 0.4.4.0
---

[http://medlaunch.asnitech.co.uk/releases/0-4-4-0](http://medlaunch.asnitech.co.uk/releases/0-4-4-0)

#### Important Release Notes
** This MedLaunch release is *ONLY* compatible with version 0.9.43.x of Mednafen. Do *NOT* upgrade if you are not planning to update Mednafen also **

#### Notable Additions
** Only compatible with version 0.9.43.x of Mednafen (although 0.9.41 and up will probably still launch games) **
* Added SS additional (0.9.43) wheel/joystick options to config tab
* (Feature) Added option (under top-left menu 'Visual') to show/hide specific mednafen systems in the launcher
* (Feature) Added right-click context menu options to the 'favorites' filter to 'Scrape previously unscraped games' and 'Re-scrape all games'. This is a similar process to the other system filter scraping options
* (Feature) Enabled multi-select of games in the library along with additional context menu for multiple games (add/remove from favorites, auto-scrape and delete games)
* (Feature) Added option (to Settings>Emulator Engine) to automatically save and set the mednafen windows position on a per-system basis (disabled by default)

#### New Install
* Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.43.x branch - 64-bit version is required if you want to emulate Saturn games). 
* You are then prompted to choose whether to import all config settings from your Mednafen folder into the MedLaunch database (this is recommended).
* If you currently use system-specific config files with Mednafen the settings from these will be imported with the above process. However MedLaunch will write to these files when you launch a game - so back them up somewhere if you are not happy with this.

#### Upgrade
##### Preferred Method: 
* Automatically download and upgrade using the 'Updates' tab within MedLaunch itself.
* Ensure you have the correct version of Mednafen installed (v0.9.43.x)
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else

##### Manual Method: 
* You can safely extract this new release over an existing MedLaunch folder (providing you do not have MedLaunch running at the time) 
* Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.
* Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
* In settings change your mednafen directory if you installed the new version of mednafen somewhere else