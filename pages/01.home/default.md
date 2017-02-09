---
title: Home
---

# MedLaunch
## A Windows Front-End for Mednafen

**MedLaunch** is a .NET (Windows only) front-end for the excellent [Mednafen](http://mednafen.fobby.net/) multi-system emulator. It is developed in C# .NET using the Windows Presentation Foundation (WPF). 

! Please Note: You should consider this software beta at the moment.

### Features
* Responsive GUI that allows for a wide range of monitor resolutions
* No installation required
* Local (SQLite) auto-generated database where all settings are saved
* Built-in games library (with system filters and dynamic search)
* ROM scanner (for games library import)
* Game data (images, manuals etc) scraping
* Automatic ROM detection based on NOINTRO & TOSEC DAT releases (so the games library is auto-populated with year, publisher etc. without having to scrape from an external source)
* Manual import of disk-based games (both single and multiple disk games with auto-m3u playlist generation)
* (Nearly) All Mednafen command line parameters available and configurable
* So far uses only Mednafen command line options (and not local configuration files)
* Per-system configuration options
* Built-in browser control with links to Mednafen help pages
* Built-in static netplay server selection along with the ability to specify a custom Mednafen netplay server to connect to

### Broken Features
* The launcher currently only handles absolute paths correctly. This means that it is not truely portable. It however only use its own directory for storing any generated files

### To Do
* Implement scanning (and importing into the games library) of disk images (currently only manual import is available)
* SDL Joystick integration (so that controllers can be configured from within MedLaunch)

### Requirements
* [Microsoft .NET Framework 4.5.2](https://www.microsoft.com/en-gb/download/details.aspx?id=42643)
* At least [Mednafen version 0.9.42.x](http://mednafen.fobby.net/releases/) - x64 required for Saturn emulation
* Windows 7 and above (may work on Vista but has not been tested)
* x64 (has not been tested on x86 but should still work on it)

! You can download the latest version of Mednafen from the [**Mednafen website**](http://mednafen.fobby.net/releases/).

#### New Install
* Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.42.x branch and 64-bit version if you want to emulate Saturn games). 
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

### Download
Check out the [**Releases**](http://medlaunch.asnitech.co.uk/releases) page or the project on [**GitHub**](https://github.com/Asnivor/MedLaunch).


##### Donate
MedLaunch is an open-source project that will always be free. 
We will however accept donations in the following cryptocurrencies if you feel the need:
* BTC:    1G2c36qEjRjnEM8dEv7xf6AEL1VWLvqguK
* DOGE:   DSpFRXxNZkuCwsZDpPwj3BDgb8GYQaggy5

