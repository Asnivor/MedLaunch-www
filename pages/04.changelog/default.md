---
title: Changelog
---

# Changelog
------------------------------------
#### Pre-Release Changes ([Master](https://github.com/Asnivor/MedLaunch) branch)
------------------------------------
* (Fixed) Fixed some spelling mistakes
* (Removal) Removed duplicate scanning commands from the top-left menu (still present in games library filter context menus)
* (Feature) Added option (under top-left menu 'Visual') to show/hide specific mednafen systems in the launcher
* (Feature) Added right-click context menu options to the 'favorites' filter to 'Scrape previously unscraped games' and 'Re-scrape all games'. This is a similar process to the other system filter scraping options
* (Feature) Enabled multi-select of games in the library along with additional context menu for multiple games (add/remove from favorites, auto-scrape and delete games)
* (Feature) Added option (to Settings>Emulator Engine) to automatically save and set the mednafen windows position on a per-system basis (disabled by default)
* Also added button to remove all saved mednafen window positions (in case of a screw up)
* (BugFix) Fixed missing snes.input.port3-8.gampad controls

##### [0.4.3.1](http://medlaunch.asnitech.co.uk/releases/0-4-3-1)
###### 2017-02-17
* ** Only compatible with version 0.9.42.x of Mednafen (although 0.9.41 will probably still launch games) **
* (Bugfix) Fixed exception(crash) caused by mednafen application not being properly initialised before importing configs into MedLaunch
* (Bugfix) Added null-check on netplay servers datagrid (mitigates application exception if the database didnt initialise correctly with the pre-defined servers)
* (Bugfix) Fixed localisation lookup issue when attempting to determine the mednafen version from the mednafen output log (stdout.txt)
* (Addition) Added another public netplay server to the list

##### [0.4.3.0](http://medlaunch.asnitech.co.uk/releases/0-4-3-0)
###### 2017-02-16
* ** Only compatible with version 0.9.42.x of Mednafen (although 0.9.41 will probably still launch games) **
* Implemented option to choose games library column visibility on a per-system basis (in top-left menu and settings page)
* Added new MedLaunch icon and 'Loading' splash-screen
* Fixed default system videoip and x/y scale values
* Changes made on 'Settings' tab are now automatically saved in realtime (and the 'Save Settings' button has been removed)
* Added a games library right-click option to view/edit the Mednafen launch string before the game runs
* Added (in top-left menu system) an option to Audit the Scraped Data Folder (so that you can determine which folder is for which game regardless of whether that data is currently liked to a game in the games library)
* Modified the 'Netplay Server Settings' module to be a datagrid, enabling as many custom servers as needed

##### [0.4.2.0](http://medlaunch.asnitech.co.uk/releases/0-4-2-0)
###### 2017-02-13
* ** Only compatible with version 0.9.42.x of Mednafen (although 0.9.41 will probably still launch games) **
* Fixed launcher crash when clicking the 'rescrape game' button if game has not been scraped before
* Changed 'Disks' to 'Discs' in games library menu
* Fixed arbitrary game launch when double-clicking on the games library scrollbars
* Implemented 7zip archive support for non-disc systems (roms are extracted to local cache folder before game launch) - one rom per archive file
* Added new setting to clear rom cache folder on application exit (enabled by default)
* Added an option to open the MedLaunch unhandled exception log (if one if present)
* Merged the 'top-right' title-bar buttons into a new (more standard) 'top-left' dropdown menu system
* Duplicated some of the ROM scanning functions in the top menu
* Added top-menu option to locate and launch a game through the filesystem (bypassing MedLaunch config database options meaning the game launches using the Mednafen config files on-disk)
* Moved hidden debug options to new hidden top-right debug menu (visible in Visual Studio debug-mode only)
* Fixed 'Unscraped Games' filter in games library
* Swapped text boxes that require decimal input for NumericUpDown controls (so that decimal and negative numbers can be entered by hand)

##### [0.4.1.0](http://medlaunch.asnitech.co.uk/releases/0-4-1-0)
###### 2017-02-09
* ** Only compatible with version 0.9.42.x of Mednafen (although 0.9.41 will probably still launch games) **
* Added new config controls for mednafen 0.9.42 (snes_faust multitap and additional virtual controller selection)
* Fixed a few small UI bugs
* Modified the update checker to use github's API rather than individually generated json files

##### [0.4.0.0](http://medlaunch.asnitech.co.uk/releases/0-4-0-0)
###### 2017-01-21
* ** Only compatible with version 0.9.41.x of Mednafen **
* Implemented config control changes for the latest Mednafen release
* Added a Mednafen version check on game launch (to avoid errors with wrong versions)
* Fixed some minor errors in the Mednafen config control names
* Added tooltips on config controls based on Mednafen documentation (can be turned off/on in settings)

##### [0.3.1.0](http://medlaunch.asnitech.co.uk/releases/0-3-1-0)
###### 2017-01-09
* Fixed 'Joystick Axis Threshold' config value not saving to database

##### [0.3.0.1](http://medlaunch.asnitech.co.uk/releases/0-3-0-1)
###### 2016-12-22
* Implemented color picker/canvas control for all Mednafen hex-color related options (lightgun crosshair colors etc..)
* Bugfix to stop application exception when trying to 'Browse Game Data Folder' when the game does not have a GDBID set in the database

##### [0.3.0.0](http://medlaunch.asnitech.co.uk/releases/0-3-0-0)
###### 2016-12-22
* Fixed netplay launch string issue affecting Windows 10 installs
* Fixed netplay nullable gamekey and password issue
* Various UI style enhancements (more consistent controls and mouse cursor change over controls)
* Implemented games library datagrid sorting memory (per session only)
* Vastly improved 'Save Settings' execution speed
* Added ability to set custom fullscreen resolutions
* Details of unhandled exceptions (application crashes) are now written to 'Exceptions.log' in the root of the MedLaunch directory
* A merged 'DAT' file (json) has been created and will be shipped with each release. Using TOSEC, NOINTRO, TRURIP & REDUMP roms will be detected on import (and re-scan) based on MD5 checksum and game name, country, year and publisher will be populated in the games library grid (where information is available). Year and publisher will be overwritten when game data is scraped from online
* Added context menu option to re-scrape all game information for a system (rather than just trying to scrape for games that have no previously been scraped). This will download all content again
* Added link to top bar that opens the Mednafen log file (stdout.txt) in the default text viewer

##### [0.2.20.0](http://medlaunch.asnitech.co.uk/releases/0-2-20-0)
###### 2016-11-22
* Fixed pce-cd games not being found when doing a batch scrape
* Added option (disabled by default) to always import Mednafen cfg files when MedLaunch starts
* Major performance gains on games library datagrid (dirty flag updates to in-memory data rather than individual database calls everywhere)
* Several secondary scraper edge-case bugfixes
* Added scraped data related columns to main games library datagrid

##### [0.2.15.0](http://medlaunch.asnitech.co.uk/releases/0-2-15-0)
###### 2016-11-17
* Fixed media content from downloading when option is de-selected in settings
* Fixed launch strings not being passed to mednafen for PCE CD games
* Fixed (unneeded) pcecd.cfg config being created in mednafen folder
* Fixed game scraping local match for PCD-CD games (games were not being found)
* Added option to set the size of the image tooltip popups (based on a percentage of the current MedLaunch window size)

##### [0.2.14.5](http://medlaunch.asnitech.co.uk/releases/0-2-14-5)
###### 2016-11-16
* Fixed control iteration bug where pce_fast (and possibly snes_faust) command line arguments were not being generated correctly
* Mednafen config backups are now stored in the MedLaunch folder (.\Data\MednafenCFGBackups\)
* Fixed some config controls not setting correctly
* Added messagebox on initial database creation - asking whether user wants to enable auto-check for updates on start

##### [0.2.14.2](http://medlaunch.asnitech.co.uk/releases/0-2-14-2)
###### 2016-11-16
* Fixed config import bug with non-valid values

##### [0.2.14.1](http://medlaunch.asnitech.co.uk/releases/0-2-14-1)
###### 2016-11-15
* Overhauled the database config tables (to more closely mirror Mednafen's config files)
* Implemented import-config-from-files functionality
* Fixed launch issue when using a fresh instance of MedLaunch 0.2.11.1
* Modified game launcher so that only system-specific command line arguments are used
* Added option (on by default) to backup Mednafen configuration on disk when MedLaunch first starts
* 'Base Configuration' config filter has been removed and the way MedLaunch handles Mednafen config arguments has been completely overhauled (if updating rather than new install of MedLaunch please ensure that you 'Import All Configs' once before launching a game
* Added option to automatically save system.cfg file in the Mednafen directory on game launch (enabled by default). It is recommended that you leave this on to avoid any inconsistencies when importing configs into MedLaunch. As above definitely do an 'Import All Configs' on first run and backup your pre-existing system.cfg files if you don't want them tampered with

##### [0.2.11.1](http://medlaunch.asnitech.co.uk/releases/0-2-11-1)
###### 2016-11-10
* Bufix to update checker

##### [0.2.11.0](http://medlaunch.asnitech.co.uk/releases/0-2-11-0)
###### 2016-11-10
* Fixed major issues with auto-game scraper (it actually works now and content is re-downloaded if it is already present)
* Added application colour theme picker
* Added option to check for MedLaunch updates on startup (but not auto-install) - disabled by default

##### [0.2.8.0](http://medlaunch.asnitech.co.uk/releases/0-2-8-0)
###### 2016-11-09
* Implemented manual 'check for updates' button - if a new update to MedLaunch is found you can choose to automatically download, extract and upgrade your current MedLaunch install
* Changed release zip file (from next release) so that there is no sub-folder inside (so the built-in updater works properly and folks can manually upgrade a little more easily)
* Game scraping has been completed overhauled - scraped data is now completely database independent (so images/manuals can be placed directory inside the game data folder and be picked up in the games library)
* Modified scraping module to include other sources
* Implemented game manual/instructions (PDF) scraping
* Added option to show ALL possible settings on the 'Base Configuration'. This is similar to how the actual Mednafen mednafen-09x.cfg file works and means that you don't have to use MedLaunch system-specific configurations to access system-specific settings (if you don't want to)
* Dev-only 'Release Generator' application for generation of release info json files
* Modifications to httprequest code to deal with random timeouts (although thegamesdb.net is still slow)
* Fixed db upgrade DateTime? exception on null value
* Fixed some of the database and application update checking logic

##### [0.2.3.1](http://medlaunch.asnitech.co.uk/releases/0-2-3-1)
###### 2016-10-24
* More UI threading fixes
* Implemented basic games library sidebar
* Added setting to always hide the sidebar
* Added .md as an allowed Megagrive ROM extension (so it will be picked up by the RomScanner)
* Implemented thegamesdb scraping code
* Added scraped data display in the sidebar
* Auto-save games library expander states on application close
* Implemented database update code (so application can be unzipped over a previous version's folder)
* Added 'Unscraped Games' filter to games library
* Simplified the GUI zoom code so (hopefully) there will be less edge-case crashes

##### [0.1.16.2](http://medlaunch.asnitech.co.uk/releases/0-1-16-2)
###### 2016-10-12
* Fixed vb config option that was causing games not to launch
* Fixed crash on double-click of empty games library
* Fixed all context menu exceptions (null errors) on Games Library
* Fixed a master system config option (so games now run)
* Added 'Minimise to taskbar on Game Launch' settings option (default is ON)
* Some UI speed optimisations

##### [0.1.15.7](http://medlaunch.asnitech.co.uk/releases/0-1-15-7)
###### 2016-10-11
* Added system specific debug config controls
* Added WonderSwan specific config controls
* Moved 'Enable Netplay' checkbox to Settings tab
* Changed netplay.password and netplay.gamekey so that they can be applied to static servers in the list
* Added startup check - if screen resolution is less than standard MedLaunch resolution - maximise the window to fit
* Moved snes_faust and pce_fast launch toggles to the settings page
* Added games library context menu option 'copy launch string to clipboard'
* Modified all panel heights so that they are viewable on lower resolutions
* Added a 'Set GUI Zoom' selector on the settings tab. Useful for people with tiny resolutions who cant see all content (and people with large resolutions who want the GUI content bigger)
* Added Mednafen directory selectors (cheats, snaps, sav etc)
* Better whitespace validation when building launch config (values with spaces are now encapsulated with quotation marks)
* Added System BIOS/Rom path controls

##### [0.1.14.6](http://medlaunch.asnitech.co.uk/releases/0-1-14-6)
###### 2016-10-10
* Added 32000Hz audio sample rate option
* Games library case-insensitive search
* Game path handling overhaul (fixed pce CD games not launching)
* Error handling and fixes to missing game or ROM folders (library games are marked as hidden until found again)
* Moved to semantic versioning
* Threaded game library import (so application doesnt appear to 'hang')
* Added context menu options in the games library for deleting all games in the database

##### [0.1.14](http://medlaunch.asnitech.co.uk/releases/0-1-14)
###### 2016-10-06
* Minor dialog box visual changes
* Hide unimplemented menu items
* Remove arbitary wait commands when launching games (so games launch as fast as GUI drawing allows)
* Implemented Saturn-specific configuration controls
* Implemented PSX-specific configuration controls
* Moved static game system information out of the database (where it had no business being)
* Unified 'Configs' tab so similar layout to 'Games' library tab
* Unified 'Settings' tab visual layout
* Fixed (force-ignore) JavaScript errors within the web browser control

##### [0.1.13](http://medlaunch.asnitech.co.uk/releases/0-1-13)
###### 2016-10-04
* Exception handling when corrupt Zip archive interogated
* Removed .smd as a supported Megadrive/Gensis ROM format (to re-implement once .smd to .bin conversion code is in place)
* Removed 'Rescan All Disks' option for the time being (as not yet implemented)
* Added option to manually add disk-based games (context menu right-click on System filter in 'Games' tab.
* Implemented m3u auto-generation logic when adding multi-disk games 
* Enabled double-click to launch game in Games library
* Added 'Delete From Games Library' context menu option (removes from the database, not disk - roms will be re-added on next scan)
* Modified games library refresh code so that data is updated after a change

##### [0.1.12](http://medlaunch.asnitech.co.uk/releases/0-1-12)
###### 2016-10-03
* Fixed broken URLs on 'help' tab
* Removed 'About' tab (as it is currently empty)

##### [0.1.11](http://medlaunch.asnitech.co.uk/releases/0-1-11)
###### 2016-10-03
* Updated first time initialisation routines
* Removed game info sidebar (to be re-added once scraping is implemented)
* Disabled disk-scanning function for the time being (until it is written properly)
* Implemented embedded browser control for 'Help' tab
* Modified WrapPanel and ScrollViewer code along with Expander controls so launcher can be used on smaller resolution systems


