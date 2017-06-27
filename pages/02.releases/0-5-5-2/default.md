---
title: 0.5.5.2
content:
    items: '@self.children'
    limit: '5'
    order:
        by: date
        dir: desc
    pagination: '1'
    url_taxonomy_filters: '1'
---

[https://github.com/Asnivor/MedLaunch/releases/tag/0.5.6.0](https://github.com/Asnivor/MedLaunch/releases/tag/0.5.6.0)

#### Important Release Notes

This release introduces a number of bugfixes, along with a games library context-menu option for multi-disc (m3u) games that allows you to pick the disc you want to launch mednafen with (implementing the mednafen '-which_medium' command).

Sub-categorisation of certain systems has also been implemented, meaning that you can easily tell apart and sort Gameboy/Gameboy Color, NGP/NGC, NES/FDS and WSWAN/WSWANC. Game scraping also now implements these sub-categories, along with a bunch of optimisations that should make the scraping more accurate.

The other major implementation is the ability to download and extract the latest compatible version of Mednafen (x64). This also ties into the first-time initialisation of MedLaunch, enabling you to select or create an empty directory (rather than just an existing mednafen directory) and have MedLaunch automatically download and extract Mednafen.

There is also (still) an official MedLaunch mednafen server running in the UK.  More details can be found here:
[http://node.asnitech.co.uk/](http://node.asnitech.co.uk/) and the server is automatically listed in the server browser within MedLaunch.

#### Notable Additions
* (Feature) For multi-disc games added a context menu launch option to choose the disc you wish to boot from initially
* (Feature) Added sub-categorisation to the games library view (based on ROM extension). Gameboy/Gameboy Color, WSWAN/WSWAN-Color etc..
* (Feature) Megadrive/Genesis games scraping updated to use detected region (based on DAT lookup). Manual scrape where region is not explitly US or EUR/JPN displays results from both sets. Auto scrape performs the same, except the 'prefer genesis' scraping option is used to determine which system to auto-scrape if region info is not found
* (BugFix) Improved auto-scraping accuracy (more accurate scrapes, less 'missed' games)
* (Feature) Implemented code to check for, and manually download the latest compatible mednafen version (x64 only) and extract into configured mednafen folder (resides under the 'updates' tab)
* (Feature) First time init now gives the option to choose/create a new directory (rather than just an existing mednafen directory) so that the latest compatible mednafen version can be downloaded and extracted (mednafen x64 only)
* **Some other bugfixes that can be found in the [CHANGELOG](http://medlaunch.asnitech.co.uk/changelog)**

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