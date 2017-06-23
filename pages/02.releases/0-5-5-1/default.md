---
title: 0.5.5.1
---

[https://github.com/Asnivor/MedLaunch/releases/tag/0.5.5.1](https://github.com/Asnivor/MedLaunch/releases/tag/0.5.5.1)

##### Minor bugfix release to rectify the following issues with 0.5.5.0:
* WonderSwan games now launch
* 'Launch game and view/edit launch string' window text area is now properly visable on smaller resolutions


#### Important Release Notes
This release introduces support for the last two major Mednafen releases (0.9.44.x & 0.9.45.x) as well as a number of bugfixes and requested features implemented.

There has been also an almost complete re-write of the games library display code. This should improve performance, but also enables multi-column sorting (click one column to sort, then shift-click a second column for secondary sorting etc.). All column sorting and layout states are saved dynamically on a per-system filter basis.

There is still a fair amount of stuff to implement, so please check the github [issues](https://github.com/Asnivor/MedLaunch/issues) page to see where we are at currently.

There is also an official MedLaunch mednafen server running in the UK (this has been added to the server browser in MedLaunch as of this release). More details can be found here:
[http://node.asnitech.co.uk/](http://node.asnitech.co.uk/)

#### Notable Additions
* (Feature) Games library overhaul - implemented multi-tier sorting and library state saving (per system filter)
* (Feature) Migrated gamesdb and mobygames json lookup files into a more manageable SQLite database
* (Feature) Added compatibility with mednafen 0.9.44.1 (snes_faust aspect ratio commands, vb LED onstate option, Wonderswan config changes and new virtual gamepad device)
* (BugFix) Enabled lookup of Famicom Disk System games on thegamesdb.net (for scraping)
* (BugFix) Games library view now updates correctly when disc-based games are manually added
* (Feature) Added compatibility with mednafen 0.9.45.1 (ss lightgun selection and crosshair color for all virtual ports)
* (Feature) Added official MedLaunch netplay server into server list
* Numerous BugFixes - see the full [changelog](http://medlaunch.asnitech.co.uk/changelog) for more info.

#### New Install
- Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.39 - 0.9.45  - 64-bit version is required if you want to emulate Saturn games). 
- You are then prompted to choose whether to import all config settings from your Mednafen folder into the MedLaunch database (this is recommended).
- If you currently use system-specific config files with Mednafen the settings from these will be imported with the above process. However MedLaunch will write to these files when you launch a game - so back them up somewhere if you are not happy with this.

#### Upgrade

##### Preferred Method:
- Automatically download and upgrade using the 'Updates' tab within MedLaunch itself.
- Ensure you have the a supported version of Mednafen installed (v0.9.39.x - v0.9.45.x)
- Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
- In settings change your mednafen directory if you installed the new version of mednafen somewhere else

##### Manual Method:
- You can safely extract this new release over an existing MedLaunch folder (providing you do not have MedLaunch running at the time) 
- Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.
- Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
- In settings change your mednafen directory if you installed the new version of mednafen somewhere else
