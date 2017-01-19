---
title: 0.2.8.0
---

#### Alpha release.
[https://github.com/Asnivor/MedLaunch/releases/tag/0.2.8.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.2.8.0)

#### Notable Additions
* Implemented manual 'check for updates' button - if a new update to MedLaunch is found you can choose to automatically download, extract and upgrade your current MedLaunch install
* Changed release zip file (from next release) so that there is no sub-folder inside (so the built-in updater works properly and folks can manually upgrade a little more easily)
* Game scraping has been completed overhauled - scraped data is now completely database independent (so images/manuals can be placed directory inside the game data folder and be picked up in the games library)
* Modified scraping module to include other sources
* Implemented game manual/instructions (PDF) scraping
* Added option to show ALL possible settings on the 'Base Configuration'. This is similar to how the actual Mednafen mednafen-09x.cfg file works and means that you don't have to use MedLaunch system-specific configurations to access system-specific settings (if you don't want to)

#### Important Notes
The release format has been modified slightly from this version - as in the zip file contains the MedLaunch files in the root of the zip, rather than within a sub-folder of the zip. This makes it easier for the auto-update code to work through the application, or if you want to upgrade manually, you can just download the release zip to your current MedLaunch directory and 'Extract Here'.

This version of MedLaunch completely overhauls the game scraping module. Downloaded data is stored within a new folder structure that lives in a different location within your MedLaunch folder. Once a game has been scraped you will be able to directly access it's 'Game Data' folder through Windows Explorer using a button in the Games Library sidebar. You can place your own content (images, manuals etc..) in the correct folder and the Games Library will automatically pick these up. Scraped data now barely touches the database which makes for far better portability and maintainability (from a development point of view).

This does however mean that any data you have previously scraped is now redundant and you will need to match/scrape games again from the start.

#### New Install
* Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.39.x branch). 
* If you currently use system-specific config files with Mednafen it is recommended that you setup a new Mednafen folder (extract Mednafen to a new folder) to avoid issues.

#### Upgrade
* You can safely extract this new release over an existing Medlaunch folder (providing you do not have MedLaunch running at the time).
* Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.