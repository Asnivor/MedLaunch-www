---
title: 0.5.0.0
---

[https://github.com/Asnivor/MedLaunch/releases/tag/0.5.0.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.5.0.0)

#### Important Release Notes
This is a pretty large release with many core changes. Please report any bugs on the github issues page if you find them.

Scanning of Disc Games:  This is now implemented and working. However, games must be separated into sub-folders (one game disc or discs per folder) otherwise they will be ignored.

Archives with Multiple Roms: This is now handled correctly in MedLaunch, providing the archive is either zip or 7zip - with no sub-folders within the archives and no archives within archives.

Controller Configuration: This was a pain in the backside. It attempts to emulate the way mednafen configures controllers - so xinput controllers (xbox360, xbone) will be detected correctly and everything else will use directinput. All seems to be working so far with my limited test controllers. Keyboard mapping *should* work correctly. Any bug-spotting would be much appreciated.

#### Notable Additions
* (Feature) MedLaunch now supports mednafen versions 0.9.39.x through 0.9.43
* (Feature) Game controls can now be configured from within MedLaunch under the 'Controls' tab. This attempts to mirror the way mednafen configures devices (xinput for compatible devices, directinput for keyboard and other gamepads/joysticks). This is currently experimental and any bugs should be reported
* (Feature) Auto-scanning & import of disc games! (see release notes for caviats)
* (Feature) On launch, psx game serial numbers are extracted from disc image(s) and an SBI file offered (if one is needed and available)
* (Feature) MedLaunch can now import multiple ROMs per archive (zip/7z) file (see release notes for restrictions)
* (Feature) PSX and Saturn games now have library details automatically populated on scan (by serial number lookup)
* (Feature) Added country filter radiobuttons (ALL, USA, EUR, JPN) to the games library. These filters obviously only work if the 'Country' field has been populated (either by DAT lookup or scrape). There is also an option to hide these filters on the settings tab
* Numerous BugFixes - see the full [changelog](http://medlaunch.asnitech.co.uk/changelog) for more info.

#### New Install
- Extract this release to a folder, run the 'MedLaunch.exe' executable and choose your Mednafen directory (must be the Mednafen 0.9.39 - 0.9.43  - 64-bit version is required if you want to emulate Saturn games). 
- You are then prompted to choose whether to import all config settings from your Mednafen folder into the MedLaunch database (this is recommended).
- If you currently use system-specific config files with Mednafen the settings from these will be imported with the above process. However MedLaunch will write to these files when you launch a game - so back them up somewhere if you are not happy with this.

#### Upgrade

##### Preferred Method:
- Automatically download and upgrade using the 'Updates' tab within MedLaunch itself.
- Ensure you have the a supported version of Mednafen installed (v0.9.39.x - v0.9.43.x)
- Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
- In settings change your mednafen directory if you installed the new version of mednafen somewhere else

##### Manual Method:
- You can safely extract this new release over an existing MedLaunch folder (providing you do not have MedLaunch running at the time) 
- Once extracted run the MedLaunch.exe executable and your current database will be upgraded before the application starts proper.
- Once MedLaunch has upgraded, go to the 'Configs' tab and click the 'IMPORT ALL CONFIGS FROM DISK' button
- In settings change your mednafen directory if you installed the new version of mednafen somewhere else
